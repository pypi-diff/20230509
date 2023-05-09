# Comparing `tmp/fractal_server-1.2.5a0.tar.gz` & `tmp/fractal_server-1.2.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.5a0.tar", max compression
+gzip compressed data, was "fractal_server-1.2.5a1.tar", max compression
```

## Comparing `fractal_server-1.2.5a0.tar` & `fractal_server-1.2.5a1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.5a0/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.5a0/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.5a0/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-05-09 07:16:49.151528 fractal_server-1.2.5a0/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.2.5a0/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.5a0/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.5a0/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.5a0/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.5a0/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2783 2023-05-08 11:38:10.463640 fractal_server-1.2.5a0/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    22641 2023-05-08 13:16:58.240665 fractal_server-1.2.5a0/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    12686 2023-05-09 07:14:02.421392 fractal_server-1.2.5a0/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11503 2023-05-08 13:16:58.240665 fractal_server-1.2.5a0/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-08 13:22:04.417311 fractal_server-1.2.5a0/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.5a0/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3175 2023-05-08 11:17:37.139725 fractal_server-1.2.5a0/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2529 2023-05-08 13:16:58.240665 fractal_server-1.2.5a0/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-05-08 13:16:58.244665 fractal_server-1.2.5a0/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.5a0/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.5a0/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.5a0/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.5a0/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8991 2023-04-28 14:21:32.268370 fractal_server-1.2.5a0/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19294 2023-04-17 13:34:24.748408 fractal_server-1.2.5a0/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5460 2023-04-17 13:34:24.748408 fractal_server-1.2.5a0/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.2.5a0/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.2.5a0/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.2.5a0/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3835 2023-04-21 11:00:14.178698 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-21 08:35:50.575851 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-04-21 11:00:14.178698 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    40272 2023-04-21 08:35:50.575851 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9749 2023-05-03 13:37:16.597419 fractal_server-1.2.5a0/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7400 2023-05-08 13:16:58.244665 fractal_server-1.2.5a0/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.5a0/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.5a0/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.5a0/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.5a0/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.5a0/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.5a0/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.5a0/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-05-08 12:02:12.593892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     4943 2023-05-08 12:02:12.605892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-05-08 12:02:12.609892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-05-08 12:02:12.613892 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-05-08 12:02:02.886003 fractal_server-1.2.5a0/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.5a0/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4323 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-05-08 12:02:02.886003 fractal_server-1.2.5a0/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-05-08 12:02:12.985888 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3046 2023-05-08 12:02:13.017887 fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-05-08 12:02:02.886003 fractal_server-1.2.5a0/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.2.5a0/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-05-08 12:02:02.886003 fractal_server-1.2.5a0/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12171 2023-05-08 06:31:53.082555 fractal_server-1.2.5a0/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.5a0/fractal_server/logger.py
--rw-r--r--   0        0        0     5805 2023-04-28 06:28:20.387228 fractal_server-1.2.5a0/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.5a0/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.5a0/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.5a0/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-05-08 13:16:58.244665 fractal_server-1.2.5a0/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-05-08 13:16:58.244665 fractal_server-1.2.5a0/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-05-08 13:16:58.244665 fractal_server-1.2.5a0/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.5a0/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.5a0/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.5a0/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12869 2023-05-09 07:14:02.421392 fractal_server-1.2.5a0/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.2.5a0/fractal_server/utils.py
--rw-r--r--   0        0        0     2629 2023-05-09 07:16:49.151528 fractal_server-1.2.5a0/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.5a0/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.5a1/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.5a1/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.5a1/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-05-09 10:12:29.466654 fractal_server-1.2.5a1/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.2.5a1/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.5a1/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.5a1/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-09 10:07:31.178019 fractal_server-1.2.5a1/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.5a1/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2783 2023-05-09 10:07:31.178019 fractal_server-1.2.5a1/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    22641 2023-05-09 10:07:31.178019 fractal_server-1.2.5a1/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    12643 2023-05-09 10:11:31.343338 fractal_server-1.2.5a1/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11503 2023-05-09 10:07:31.182019 fractal_server-1.2.5a1/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-08 13:22:04.417311 fractal_server-1.2.5a1/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.5a1/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3175 2023-05-08 11:17:37.139725 fractal_server-1.2.5a1/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2529 2023-05-08 13:16:58.240665 fractal_server-1.2.5a1/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-05-08 13:16:58.244665 fractal_server-1.2.5a1/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.5a1/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.5a1/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.5a1/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.5a1/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8991 2023-04-28 14:21:32.268370 fractal_server-1.2.5a1/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19294 2023-04-17 13:34:24.748408 fractal_server-1.2.5a1/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5460 2023-04-17 13:34:24.748408 fractal_server-1.2.5a1/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.2.5a1/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.2.5a1/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.2.5a1/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3835 2023-04-21 11:00:14.178698 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-21 08:35:50.575851 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19861 2023-04-21 11:00:14.178698 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    40272 2023-04-21 08:35:50.575851 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9749 2023-05-03 13:37:16.597419 fractal_server-1.2.5a1/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7400 2023-05-08 13:16:58.244665 fractal_server-1.2.5a1/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.5a1/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.5a1/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.5a1/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.5a1/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.5a1/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.5a1/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.5a1/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-05-09 10:11:26.675393 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-05-09 10:11:26.687393 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-05-08 12:02:12.609892 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-05-09 10:11:26.695393 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-05-09 10:08:09.097598 fractal_server-1.2.5a1/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.5a1/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-05-09 10:08:09.097598 fractal_server-1.2.5a1/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-05-09 10:08:09.097598 fractal_server-1.2.5a1/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-05-09 10:11:27.087389 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3046 2023-05-09 10:11:27.115388 fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-05-09 10:08:09.097598 fractal_server-1.2.5a1/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.2.5a1/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-05-09 10:08:09.097598 fractal_server-1.2.5a1/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12171 2023-05-08 06:31:53.082555 fractal_server-1.2.5a1/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.5a1/fractal_server/logger.py
+-rw-r--r--   0        0        0     5805 2023-04-28 06:28:20.387228 fractal_server-1.2.5a1/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.5a1/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.5a1/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.5a1/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-05-08 13:16:58.244665 fractal_server-1.2.5a1/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-05-08 13:16:58.244665 fractal_server-1.2.5a1/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-05-08 13:16:58.244665 fractal_server-1.2.5a1/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.5a1/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.5a1/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.5a1/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12869 2023-05-09 10:07:31.182019 fractal_server-1.2.5a1/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.2.5a1/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-05-09 10:12:29.466654 fractal_server-1.2.5a1/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.5a1/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.5a1/PKG-INFO
```

### Comparing `fractal_server-1.2.5a0/LICENSE` & `fractal_server-1.2.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/README.md` & `fractal_server-1.2.5a1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/__main__.py` & `fractal_server-1.2.5a1/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/alembic.ini` & `fractal_server-1.2.5a1/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/api/__init__.py` & `fractal_server-1.2.5a1/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.5a1/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.5a1/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.5a1/fractal_server/app/api/v1/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 from ....tasks.collection import download_package
 from ....tasks.collection import get_collection_data
 from ....tasks.collection import get_collection_log
 from ....tasks.collection import get_collection_path
 from ....tasks.collection import get_log_path
 from ....tasks.collection import inspect_package
 from ...db import AsyncSession
+from ...db import DBSyncSession
 from ...db import get_db
+from ...db import get_sync_db
 from ...models import State
 from ...models import Task
 from ...security import current_active_superuser
 from ...security import current_active_user
 from ...security import User
 
 router = APIRouter()
@@ -57,17 +59,17 @@
     Install a python package and collect the tasks it provides according to
     the manifest.
 
     In case of error, copy the log into the state and delete the package
     directory.
     """
 
-    async for db in get_db():
+    with get_sync_db() as db:
 
-        state: State = await db.get(State, state_id)
+        state: State = db.get(State, state_id)
 
         logger_name = task_pkg.package.replace("/", "_")
         logger = set_logger(
             logger_name=logger_name,
             log_file_path=get_log_path(venv_path),
         )
 
@@ -77,82 +79,83 @@
 
         try:
             # install
             logger.debug("Task-collection status: installing")
             data.status = "installing"
 
             state.data = data.sanitised_dict()
-            await db.merge(state)
-            await db.commit()
-            task_list = await create_package_environment_pip(
+            db.merge(state)
+            db.commit()
+            task_list = create_package_environment_pip(
                 venv_path=venv_path,
                 task_pkg=task_pkg,
                 logger_name=logger_name,
             )
 
             # collect
             logger.debug("Task-collection status: collecting")
             data.status = "collecting"
             state.data = data.sanitised_dict()
-            await db.merge(state)
-            await db.commit()
-            tasks = await _insert_tasks(task_list=task_list, db=db)
+            db.merge(state)
+            db.commit()
+            tasks = _insert_tasks(task_list=task_list, db=db)
 
             # finalise
             logger.debug("Task-collection status: finalising")
             collection_path = get_collection_path(venv_path)
             data.task_list = tasks
             with collection_path.open("w") as f:
                 json.dump(data.sanitised_dict(), f)
 
             # Update DB
             data.status = "OK"
             data.log = get_collection_log(venv_path)
             state.data = data.sanitised_dict()
             db.add(state)
-            await db.merge(state)
-            await db.commit()
+            db.merge(state)
+            db.commit()
 
             # Write last logs to file
             logger.debug("Task-collection status: OK")
             logger.info("Background task collection completed successfully")
             close_logger(logger)
-            await db.close()
+            db.close()
 
         except Exception as e:
             # Write last logs to file
             logger.debug("Task-collection status: fail")
             logger.info(f"Background collection failed. Original error: {e}")
             close_logger(logger)
 
             # Update db
             data.status = "fail"
             data.info = f"Original error: {e}"
             data.log = get_collection_log(venv_path)
             state.data = data.sanitised_dict()
-            await db.merge(state)
-            await db.commit()
-            await db.close()
+            db.merge(state)
+            db.commit()
+            db.close()
 
             # Delete corrupted package dir
             shell_rmtree(venv_path)
 
 
 async def _insert_tasks(
     task_list: list[TaskCreate],
-    db: AsyncSession,
+    db: DBSyncSession,
 ) -> list[Task]:
     """
     Insert tasks into database
     """
     task_db_list = [Task.from_orm(t) for t in task_list]
     db.add_all(task_db_list)
-    await db.commit()
-    await asyncio.gather(*[db.refresh(t) for t in task_db_list])
-    await db.close()
+    db.commit()
+    for t in task_db_list:
+        db.refresh(t)
+    db.close()
     return task_db_list
 
 
 @router.post(
     "/collect/pip/",
     response_model=StateRead,
     responses={
```

### Comparing `fractal_server-1.2.5a0/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.5a1/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/db/__init__.py` & `fractal_server-1.2.5a1/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/models/job.py` & `fractal_server-1.2.5a1/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/models/project.py` & `fractal_server-1.2.5a1/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/models/security.py` & `fractal_server-1.2.5a1/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/models/state.py` & `fractal_server-1.2.5a1/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/models/task.py` & `fractal_server-1.2.5a1/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/models/workflow.py` & `fractal_server-1.2.5a1/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_common.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/runner/common.py` & `fractal_server-1.2.5a1/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/app/security/__init__.py` & `fractal_server-1.2.5a1/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.5a1/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.5a1/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/README.md` & `fractal_server-1.2.5a1/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:02:02 2023 UTC, .py size: 1716 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 bae4 5864 b406 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 891b 5a64 b406 0000  o.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c06 6d07 5a07 0100 6406 6407 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6406 6408 6c08 6d0a 5a0a  m.Z...d.d.l.m.Z.
```

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 4323 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 e310 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 891b 5a64 8411 0000  o.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -216,94 +216,99 @@
 00000d70: 5442 440a 2020 2020 2020 2020 7061 636b  TBD.        pack
 00000d80: 6167 655f 6578 7472 6173 3a20 5442 440a  age_extras: TBD.
 00000d90: 2020 2020 da07 7061 636b 6167 65da 0776      ..package..v
 00000da0: 6572 7369 6f6e 4eda 0e70 7974 686f 6e5f  ersionN..python_
 00000db0: 7665 7273 696f 6eda 0e70 6163 6b61 6765  version..package
 00000dc0: 5f65 7874 7261 7363 0200 0000 0000 0000  _extrasc........
 00000dd0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00000de0: 732a 0000 0064 017c 0176 0072 1374 007c  s*...d.|.v.r.t.|
+00000de0: 7340 0000 0064 017c 0176 0072 1e74 007c  s@...d.|.v.r.t.|
 00000df0: 0183 017d 027c 02a0 01a1 0073 1374 0264  ...}.|.....s.t.d
-00000e00: 027c 029b 009d 0283 0182 017c 0153 0029  .|.........|.S.)
-00000e10: 034e fa01 2f7a 1f50 6163 6b61 6765 2070  .N../z.Package p
-00000e20: 6174 6820 6d75 7374 2062 6520 6162 736f  ath must be abso
-00000e30: 6c75 7465 3a20 2903 7202 0000 00da 0b69  lute: ).r......i
-00000e40: 735f 6162 736f 6c75 7465 da0a 5661 6c75  s_absolute..Valu
-00000e50: 6545 7272 6f72 2903 da03 636c 73da 0576  eError)...cls..v
-00000e60: 616c 7565 da0c 7061 636b 6167 655f 7061  alue..package_pa
-00000e70: 7468 721e 0000 0072 1e00 0000 721f 0000  thr....r....r...
-00000e80: 00da 1570 6163 6b61 6765 5f70 6174 685f  ...package_path_
-00000e90: 6162 736f 6c75 7465 8400 0000 730e 0000  absolute....s...
-00000ea0: 0008 0208 0108 0102 0108 0104 ff04 037a  ...............z
-00000eb0: 2454 6173 6b43 6f6c 6c65 6374 5069 702e  $TaskCollectPip.
+00000e00: 027c 029b 009d 0283 0182 017c 02a0 03a1  .|.........|....
+00000e10: 0073 1e74 0264 037c 029b 009d 0283 0182  .s.t.d.|........
+00000e20: 017c 0153 0029 044e fa01 2f7a 1f50 6163  .|.S.).N../z.Pac
+00000e30: 6b61 6765 2070 6174 6820 6d75 7374 2062  kage path must b
+00000e40: 6520 6162 736f 6c75 7465 3a20 7a1d 5061  e absolute: z.Pa
+00000e50: 636b 6167 6520 6669 6c65 2064 6f65 7320  ckage file does 
+00000e60: 6e6f 7420 6578 6973 743a 2029 0472 0200  not exist: ).r..
+00000e70: 0000 da0b 6973 5f61 6273 6f6c 7574 65da  ....is_absolute.
+00000e80: 0a56 616c 7565 4572 726f 72da 0665 7869  .ValueError..exi
+00000e90: 7374 7329 03da 0363 6c73 da05 7661 6c75  sts)...cls..valu
+00000ea0: 65da 0c70 6163 6b61 6765 5f70 6174 6872  e..package_pathr
+00000eb0: 1e00 0000 721e 0000 0072 1f00 0000 da15  ....r....r......
 00000ec0: 7061 636b 6167 655f 7061 7468 5f61 6273  package_path_abs
-00000ed0: 6f6c 7574 6529 0a72 1800 0000 7219 0000  olute).r....r...
-00000ee0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000ef0: 721d 0000 0072 0700 0000 7236 0000 0072  r....r....r6...r
-00000f00: 0900 0000 723e 0000 0072 1e00 0000 721e  ....r>...r....r.
-00000f10: 0000 0072 1e00 0000 721f 0000 0072 1300  ...r....r....r..
-00000f20: 0000 7400 0000 7310 0000 000a 0004 0108  ..t...s.........
-00000f30: 0a0c 0110 010c 0106 020e 0172 1300 0000  ...........r....
-00000f40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000f50: 0003 0000 0040 0000 0073 6800 0000 6500  .....@...sh...e.
-00000f60: 5a01 6400 5a02 5500 6401 5a03 6504 6402  Z.d.Z.U.d.Z.e.d.
-00000f70: 1900 6505 6403 3c00 6506 6505 6404 3c00  ..e.d.<.e.e.d.<.
-00000f80: 6507 6505 6405 3c00 6508 6700 6406 8d01  e.e.d.<.e.g.d...
-00000f90: 5a09 650a 650b 650c 1900 1900 6505 6407  Z.e.e.e.....e.d.
-00000fa0: 3c00 650a 6506 1900 6505 6408 3c00 650a  <.e.e...e.d.<.e.
-00000fb0: 6506 1900 6505 6409 3c00 640a 640b 8400  e...e.d.<.d.d...
-00000fc0: 5a0d 640c 5300 290d 7214 0000 007a ac0a  Z.d.S.).r....z..
-00000fd0: 2020 2020 5461 736b 436f 6c6c 6563 7453      TaskCollectS
-00000fe0: 7461 7475 7320 636c 6173 730a 0a20 2020  tatus class..   
-00000ff0: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-00001000: 2020 2020 2073 7461 7475 733a 2054 4244       status: TBD
-00001010: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
-00001020: 3a20 5442 440a 2020 2020 2020 2020 7665  : TBD.        ve
-00001030: 6e76 5f70 6174 683a 2054 4244 0a20 2020  nv_path: TBD.   
-00001040: 2020 2020 2074 6173 6b5f 6c69 7374 3a20       task_list: 
-00001050: 5442 440a 2020 2020 2020 2020 6c6f 673a  TBD.        log:
-00001060: 2054 4244 0a20 2020 2020 2020 2069 6e66   TBD.        inf
-00001070: 6f3a 2054 4244 0a20 2020 2029 05da 0770  o: TBD.    )...p
-00001080: 656e 6469 6e67 da0a 696e 7374 616c 6c69  ending..installi
-00001090: 6e67 da0a 636f 6c6c 6563 7469 6e67 da04  ng..collecting..
-000010a0: 6661 696c da02 4f4b da06 7374 6174 7573  fail..OK..status
-000010b0: 7234 0000 00da 0976 656e 765f 7061 7468  r4.....venv_path
-000010c0: 7230 0000 00da 0974 6173 6b5f 6c69 7374  r0.....task_list
-000010d0: da03 6c6f 67da 0469 6e66 6f63 0100 0000  ..log..infoc....
-000010e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000010f0: 4300 0000 731a 0000 007c 00a0 00a1 007d  C...s....|.....}
-00001100: 0174 017c 006a 0283 017c 0164 013c 007c  .t.|.j...|.d.<.|
-00001110: 0153 0029 027a 510a 2020 2020 2020 2020  .S.).zQ.        
-00001120: 5265 7475 726e 2060 7365 6c66 2e64 6963  Return `self.dic
-00001130: 7428 2960 2061 6674 6572 2063 6173 7469  t()` after casti
-00001140: 6e67 2060 7365 6c66 2e76 656e 765f 7061  ng `self.venv_pa
-00001150: 7468 6020 746f 2061 2073 7472 696e 670a  th` to a string.
-00001160: 2020 2020 2020 2020 7245 0000 0029 03da          rE...)..
-00001170: 0464 6963 7472 1c00 0000 7245 0000 0029  .dictr....rE...)
-00001180: 02da 0473 656c 66da 0164 721e 0000 0072  ...self..dr....r
-00001190: 1e00 0000 721f 0000 00da 0e73 616e 6974  ....r......sanit
-000011a0: 6973 6564 5f64 6963 74a3 0000 0073 0600  ised_dict....s..
-000011b0: 0000 0804 0e01 0401 7a20 5461 736b 436f  ........z TaskCo
-000011c0: 6c6c 6563 7453 7461 7475 732e 7361 6e69  llectStatus.sani
-000011d0: 7469 7365 645f 6469 6374 4e29 0e72 1800  tised_dictN).r..
-000011e0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-000011f0: 0072 0600 0000 721d 0000 0072 1c00 0000  .r....r....r....
-00001200: 7202 0000 0072 0a00 0000 7246 0000 0072  r....r....rF...r
-00001210: 0700 0000 7205 0000 0072 1000 0000 724c  ....r....r....rL
-00001220: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
-00001230: 0000 721f 0000 0072 1400 0000 8f00 0000  ..r....r........
-00001240: 7312 0000 000a 0004 010c 0c08 0108 011a  s...............
-00001250: 010c 010c 010c 0272 1400 0000 4e29 1ada  .......r....N)..
-00001260: 0770 6174 686c 6962 7202 0000 00da 0674  .pathlibr......t
-00001270: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
-00001280: 0500 0000 7206 0000 0072 0700 0000 da08  ....r....r......
-00001290: 7079 6461 6e74 6963 7208 0000 0072 0900  pydanticr....r..
-000012a0: 0000 da08 7371 6c6d 6f64 656c 720a 0000  ....sqlmodelr...
-000012b0: 0072 0b00 0000 da0b 5f76 616c 6964 6174  .r......_validat
-000012c0: 6f72 7372 0d00 0000 da07 5f5f 616c 6c5f  orsr......__all_
-000012d0: 5f72 1500 0000 720f 0000 0072 1100 0000  _r....r....r....
-000012e0: 7212 0000 0072 1000 0000 720e 0000 0072  r....r....r....r
-000012f0: 3300 0000 7213 0000 0072 1400 0000 721e  3...r....r....r.
-00001300: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-00001310: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001320: 732a 0000 000c 000c 010c 010c 010c 010c  s*..............
-00001330: 010c 020c 010c 010c 010c 0204 0210 0b10  ................
-00001340: 1c10 1510 0510 0410 0910 1310 0414 1b    ...............
+00000ed0: 6f6c 7574 6584 0000 0073 1600 0000 0802  olute....s......
+00000ee0: 0801 0801 0201 0801 04ff 0803 0201 0801  ................
+00000ef0: 04ff 0403 7a24 5461 736b 436f 6c6c 6563  ....z$TaskCollec
+00000f00: 7450 6970 2e70 6163 6b61 6765 5f70 6174  tPip.package_pat
+00000f10: 685f 6162 736f 6c75 7465 290a 7218 0000  h_absolute).r...
+00000f20: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000f30: 721c 0000 0072 1d00 0000 7207 0000 0072  r....r....r....r
+00000f40: 3600 0000 7209 0000 0072 3f00 0000 721e  6...r....r?...r.
+00000f50: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000f60: 0000 7213 0000 0074 0000 0073 1000 0000  ..r....t...s....
+00000f70: 0a00 0401 080a 0c01 1001 0c01 0602 0e01  ................
+00000f80: 7213 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000f90: 0000 0000 0000 0300 0000 4000 0000 7368  ..........@...sh
+00000fa0: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00000fb0: 0365 0464 0219 0065 0564 033c 0065 0665  .e.d...e.d.<.e.e
+00000fc0: 0564 043c 0065 0765 0564 053c 0065 0867  .d.<.e.e.d.<.e.g
+00000fd0: 0064 068d 015a 0965 0a65 0b65 0c19 0019  .d...Z.e.e.e....
+00000fe0: 0065 0564 073c 0065 0a65 0619 0065 0564  .e.d.<.e.e...e.d
+00000ff0: 083c 0065 0a65 0619 0065 0564 093c 0064  .<.e.e...e.d.<.d
+00001000: 0a64 0b84 005a 0d64 0c53 0029 0d72 1400  .d...Z.d.S.).r..
+00001010: 0000 7aac 0a20 2020 2054 6173 6b43 6f6c  ..z..    TaskCol
+00001020: 6c65 6374 5374 6174 7573 2063 6c61 7373  lectStatus class
+00001030: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00001040: 3a0a 2020 2020 2020 2020 7374 6174 7573  :.        status
+00001050: 3a20 5442 440a 2020 2020 2020 2020 7061  : TBD.        pa
+00001060: 636b 6167 653a 2054 4244 0a20 2020 2020  ckage: TBD.     
+00001070: 2020 2076 656e 765f 7061 7468 3a20 5442     venv_path: TB
+00001080: 440a 2020 2020 2020 2020 7461 736b 5f6c  D.        task_l
+00001090: 6973 743a 2054 4244 0a20 2020 2020 2020  ist: TBD.       
+000010a0: 206c 6f67 3a20 5442 440a 2020 2020 2020   log: TBD.      
+000010b0: 2020 696e 666f 3a20 5442 440a 2020 2020    info: TBD.    
+000010c0: 2905 da07 7065 6e64 696e 67da 0a69 6e73  )...pending..ins
+000010d0: 7461 6c6c 696e 67da 0a63 6f6c 6c65 6374  talling..collect
+000010e0: 696e 67da 0466 6169 6cda 024f 4bda 0673  ing..fail..OK..s
+000010f0: 7461 7475 7372 3400 0000 da09 7665 6e76  tatusr4.....venv
+00001100: 5f70 6174 6872 3000 0000 da09 7461 736b  _pathr0.....task
+00001110: 5f6c 6973 74da 036c 6f67 da04 696e 666f  _list..log..info
+00001120: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001130: 0003 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
+00001140: a000 a100 7d01 7401 7c00 6a02 8301 7c01  ....}.t.|.j...|.
+00001150: 6401 3c00 7c01 5300 2902 7a51 0a20 2020  d.<.|.S.).zQ.   
+00001160: 2020 2020 2052 6574 7572 6e20 6073 656c       Return `sel
+00001170: 662e 6469 6374 2829 6020 6166 7465 7220  f.dict()` after 
+00001180: 6361 7374 696e 6720 6073 656c 662e 7665  casting `self.ve
+00001190: 6e76 5f70 6174 6860 2074 6f20 6120 7374  nv_path` to a st
+000011a0: 7269 6e67 0a20 2020 2020 2020 2072 4600  ring.        rF.
+000011b0: 0000 2903 da04 6469 6374 721c 0000 0072  ..)...dictr....r
+000011c0: 4600 0000 2902 da04 7365 6c66 da01 6472  F...)...self..dr
+000011d0: 1e00 0000 721e 0000 0072 1f00 0000 da0e  ....r....r......
+000011e0: 7361 6e69 7469 7365 645f 6469 6374 a700  sanitised_dict..
+000011f0: 0000 7306 0000 0008 040e 0104 017a 2054  ..s..........z T
+00001200: 6173 6b43 6f6c 6c65 6374 5374 6174 7573  askCollectStatus
+00001210: 2e73 616e 6974 6973 6564 5f64 6963 744e  .sanitised_dictN
+00001220: 290e 7218 0000 0072 1900 0000 721a 0000  ).r....r....r...
+00001230: 0072 1b00 0000 7206 0000 0072 1d00 0000  .r....r....r....
+00001240: 721c 0000 0072 0200 0000 720a 0000 0072  r....r....r....r
+00001250: 4700 0000 7207 0000 0072 0500 0000 7210  G...r....r....r.
+00001260: 0000 0072 4d00 0000 721e 0000 0072 1e00  ...rM...r....r..
+00001270: 0000 721e 0000 0072 1f00 0000 7214 0000  ..r....r....r...
+00001280: 0093 0000 0073 1200 0000 0a00 0401 0c0c  .....s..........
+00001290: 0801 0801 1a01 0c01 0c01 0c02 7214 0000  ............r...
+000012a0: 004e 291a da07 7061 7468 6c69 6272 0200  .N)...pathlibr..
+000012b0: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
+000012c0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+000012d0: 0000 00da 0870 7964 616e 7469 6372 0800  .....pydanticr..
+000012e0: 0000 7209 0000 00da 0873 716c 6d6f 6465  ..r......sqlmode
+000012f0: 6c72 0a00 0000 720b 0000 00da 0b5f 7661  lr....r......_va
+00001300: 6c69 6461 746f 7273 720d 0000 00da 075f  lidatorsr......_
+00001310: 5f61 6c6c 5f5f 7215 0000 0072 0f00 0000  _all__r....r....
+00001320: 7211 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
+00001330: 0e00 0000 7233 0000 0072 1300 0000 7214  ....r3...r....r.
+00001340: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
+00001350: 0000 721f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00001360: 3e01 0000 0073 2a00 0000 0c00 0c01 0c01  >....s*.........
+00001370: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c02  ................
+00001380: 0402 100b 101c 1015 1005 1004 1009 1013  ................
+00001390: 1004 141f                                ....
```

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:02:02 2023 UTC, .py size: 2709 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 bae4 5864 950a 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 891b 5a64 950a 0000  o.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
```

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.5a1/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/project.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/state.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/task.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,14 +133,18 @@
     def package_path_absolute(cls, value):
         if "/" in value:
             package_path = Path(value)
             if not package_path.is_absolute():
                 raise ValueError(
                     f"Package path must be absolute: {package_path}"
                 )
+            if not package_path.exists():
+                raise ValueError(
+                    f"Package file does not exist: {package_path}"
+                )
         return value
 
 
 class TaskCollectStatus(_TaskCollectBase):
     """
     TaskCollectStatus class
```

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/user.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.5a1/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:02:02 2023 UTC, .py size: 1065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 bae4 5864 2904 0000  o.........Xd)...
+00000000: 6f0d 0d0a 0000 0000 891b 5a64 2904 0000  o.........Zd)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
```

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.2.5a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:02:02 2023 UTC, .py size: 2838 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 bae4 5864 160b 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 891b 5a64 160b 0000  o.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
```

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.5a1/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/config.py` & `fractal_server-1.2.5a1/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/logger.py` & `fractal_server-1.2.5a1/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/main.py` & `fractal_server-1.2.5a1/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/migrations/env.py` & `fractal_server-1.2.5a1/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.5a1/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.5a1/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.5a1/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.5a1/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/syringe.py` & `fractal_server-1.2.5a1/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/tasks/collection.py` & `fractal_server-1.2.5a1/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/fractal_server/utils.py` & `fractal_server-1.2.5a1/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.5a0/pyproject.toml` & `fractal_server-1.2.5a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.5a0"
+version = "1.2.5a1"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -71,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.5a0"
+current_version = "1.2.5a1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.5a0/setup.py` & `fractal_server-1.2.5a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.5a0',
+    'version': '1.2.5a1',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.5a0/PKG-INFO` & `fractal_server-1.2.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.5a0
+Version: 1.2.5a1
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

