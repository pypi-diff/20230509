# Comparing `tmp/aedttest-0.0.1.dev9.tar.gz` & `tmp/aedttest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aedttest-0.0.1.dev9.tar", last modified: Thu Sep  1 11:41:04 2022, max compression
+gzip compressed data, was "aedttest-0.0.2.tar", last modified: Tue May  9 12:44:47 2023, max compression
```

## Comparing `aedttest-0.0.1.dev9.tar` & `aedttest-0.0.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0      550 2022-09-01 11:40:26.929861 aedttest-0.0.1.dev9/.github/workflows/ci-sim-data.yml
--rw-r--r--   0        0        0      586 2022-09-01 11:40:26.929861 aedttest-0.0.1.dev9/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1169 2022-09-01 11:40:26.929861 aedttest-0.0.1.dev9/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      202 2022-09-01 11:40:26.929861 aedttest-0.0.1.dev9/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     5084 2022-09-01 11:40:26.929861 aedttest-0.0.1.dev9/.gitignore
--rw-r--r--   0        0        0     1251 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1099 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/LICENSE
--rw-r--r--   0        0        0     4052 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/README.md
--rw-r--r--   0        0        0        0 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/__init__.py
--rw-r--r--   0        0        0    42374 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/aedt_test_runner.py
--rw-r--r--   0        0        0        0 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/clusters/__init__.py
--rw-r--r--   0        0        0     8640 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/clusters/job_hosts.py
--rw-r--r--   0        0        0      607 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/clusters/job_hosts.pyi
--rw-r--r--   0        0        0     1559 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/logger.py
--rw-r--r--   0        0        0      257 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/logger.pyi
--rw-r--r--   0        0        0        0 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/py.typed
--rw-r--r--   0        0        0    14811 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/simulation_data.py
--rw-r--r--   0        0        0     1260 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/simulation_data.pyi
--rw-r--r--   0        0        0    11167 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/css/css-lib/bootstrap-slider.css
--rw-r--r--   0        0        0   161409 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/css/css-lib/bootstrap.min.css
--rw-r--r--   0        0        0    16199 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/css/css-lib/jquery-ui.min.css
--rw-r--r--   0        0        0     8495 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/css/style.css
--rw-r--r--   0        0        0     2297 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/js/chartjs-init.js
--rw-r--r--   0        0        0      727 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/js/common.js
--rw-r--r--   0        0        0   188368 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/js/js-lib/Chart.bundle.js
--rw-r--r--   0        0        0    38829 2022-09-01 11:40:26.933861 aedttest-0.0.1.dev9/aedttest/static/js/js-lib/bootstrap-slider.min.js
--rw-r--r--   0        0        0    69782 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/js/js-lib/bootstrap.min.js
--rw-r--r--   0        0        0    97362 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/js/js-lib/jquery.min.js
--rw-r--r--   0        0        0    12394 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/js/js-lib/jquery.nanoscroller.min.js
--rw-r--r--   0        0        0      792 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/js/main.js
--rw-r--r--   0        0        0      319 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/js/project.js
--rw-r--r--   0        0        0     6119 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/templates/main.html
--rw-r--r--   0        0        0     8800 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/aedttest/static/templates/project-report.html
--rw-r--r--   0        0        0      461 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/docs/CONTRIBUTE.md
--rw-r--r--   0        0        0      114 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/examples/configs/config_19.toml
--rw-r--r--   0        0        0      131 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/examples/configs/config_expression.toml
--rw-r--r--   0        0        0     1410 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/examples/configs/config_with_comments.toml
--rw-r--r--   0        0        0      220 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/examples/configs/config_without_comments.toml
--rw-r--r--   0        0        0      581 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/mypy.ini
--rw-r--r--   0        0        0     1445 2022-09-01 11:41:04.490201 aedttest-0.0.1.dev9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/__init__.py
--rw-r--r--   0        0        0     5543 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/2020R2_profile.prof
--rw-r--r--   0        0        0     4338 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/2021R2_profile.prof
--rw-r--r--   0        0        0     2558 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/R2019R1_profile.prof
--rw-r--r--   0        0        0     1151 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/allocator_config.json
--rw-r--r--   0        0        0      120 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/config_simple/config_just_winding.toml
--rw-r--r--   0        0        0      115 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/configs/config_19.toml
--rw-r--r--   0        0        0      122 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/configs/config_2019R1.toml
--rw-r--r--   0        0        0      132 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/configs/config_expression.toml
--rw-r--r--   0        0        0      221 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/configs/config_just_winding.toml
--rw-r--r--   0        0        0      261 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/configs/config_voltage.toml
--rw-r--r--   0        0        0     2904 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/icepak.prof
--rw-r--r--   0        0        0     2144 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/icepak_231.prof
--rw-r--r--   0        0        0      894 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/mesh.mstat
--rw-r--r--   0        0        0      180 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/no_mesh.mstat
--rw-r--r--   0        0        0     8093 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/prof_test_mixed_case.prof
--rw-r--r--   0        0        0      589 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/input/reference_simple/ref_sample.json
--rw-r--r--   0        0        0       87 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/reqs_test_sim_data_py27.txt
--rw-r--r--   0        0        0        0 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/unittests/__init__.py
--rw-r--r--   0        0        0    19670 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/unittests/test_aedt_test_runner.py
--rw-r--r--   0        0        0     4001 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/unittests/test_clusters.py
--rw-r--r--   0        0        0    10358 2022-09-01 11:40:26.937861 aedttest-0.0.1.dev9/tests/unittests/test_simulation_data.py
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 aedttest-0.0.1.dev9/setup.py
--rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 aedttest-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-05-09 12:44:32.931816 aedttest-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1169 2023-05-09 12:44:32.931816 aedttest-0.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      324 2023-05-09 12:44:32.931816 aedttest-0.0.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     5084 2023-05-09 12:44:32.931816 aedttest-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1536 2023-05-09 12:44:32.931816 aedttest-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1099 2023-05-09 12:44:32.931816 aedttest-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4056 2023-05-09 12:44:32.931816 aedttest-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/__init__.py
+-rw-r--r--   0        0        0    44775 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/aedt_test_runner.py
+-rw-r--r--   0        0        0        0 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/clusters/__init__.py
+-rw-r--r--   0        0        0     8640 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/clusters/job_hosts.py
+-rw-r--r--   0        0        0      607 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/clusters/job_hosts.pyi
+-rw-r--r--   0        0        0     1559 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/logger.py
+-rw-r--r--   0        0        0      257 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/logger.pyi
+-rw-r--r--   0        0        0        0 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/py.typed
+-rw-r--r--   0        0        0    15962 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/simulation_data.py
+-rw-r--r--   0        0        0     1295 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/simulation_data.pyi
+-rw-r--r--   0        0        0    11167 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/static/css/css-lib/bootstrap-slider.css
+-rw-r--r--   0        0        0   161409 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/static/css/css-lib/bootstrap.min.css
+-rw-r--r--   0        0        0    16199 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/static/css/css-lib/jquery-ui.min.css
+-rw-r--r--   0        0        0     8495 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/static/css/style.css
+-rw-r--r--   0        0        0     2297 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/static/js/chartjs-init.js
+-rw-r--r--   0        0        0      727 2023-05-09 12:44:32.931816 aedttest-0.0.2/aedttest/static/js/common.js
+-rw-r--r--   0        0        0   188368 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/js-lib/Chart.bundle.js
+-rw-r--r--   0        0        0    38829 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/js-lib/bootstrap-slider.min.js
+-rw-r--r--   0        0        0    69782 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/js-lib/bootstrap.min.js
+-rw-r--r--   0        0        0    97362 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/js-lib/jquery.min.js
+-rw-r--r--   0        0        0    12394 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/js-lib/jquery.nanoscroller.min.js
+-rw-r--r--   0        0        0      792 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/main.js
+-rw-r--r--   0        0        0      319 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/js/project.js
+-rw-r--r--   0        0        0     6119 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/templates/main.html
+-rw-r--r--   0        0        0     9810 2023-05-09 12:44:32.935816 aedttest-0.0.2/aedttest/static/templates/project-report.html
+-rw-r--r--   0        0        0      595 2023-05-09 12:44:32.935816 aedttest-0.0.2/docs/CONTRIBUTE.md
+-rw-r--r--   0        0        0      114 2023-05-09 12:44:32.935816 aedttest-0.0.2/examples/configs/config_19.toml
+-rw-r--r--   0        0        0      131 2023-05-09 12:44:32.935816 aedttest-0.0.2/examples/configs/config_expression.toml
+-rw-r--r--   0        0        0     1410 2023-05-09 12:44:32.935816 aedttest-0.0.2/examples/configs/config_with_comments.toml
+-rw-r--r--   0        0        0      220 2023-05-09 12:44:32.935816 aedttest-0.0.2/examples/configs/config_without_comments.toml
+-rw-r--r--   0        0        0      581 2023-05-09 12:44:32.935816 aedttest-0.0.2/mypy.ini
+-rw-r--r--   0        0        0     1547 2023-05-09 12:44:47.264040 aedttest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     5543 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/2020R2_profile.prof
+-rw-r--r--   0        0        0     4338 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/2021R2_profile.prof
+-rw-r--r--   0        0        0     2558 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/R2019R1_profile.prof
+-rw-r--r--   0        0        0     1151 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/allocator_config.json
+-rw-r--r--   0        0        0      120 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/config_simple/config_just_winding.toml
+-rw-r--r--   0        0        0      115 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/configs/config_19.toml
+-rw-r--r--   0        0        0      122 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/configs/config_2019R1.toml
+-rw-r--r--   0        0        0      132 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/configs/config_expression.toml
+-rw-r--r--   0        0        0      221 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/configs/config_just_winding.toml
+-rw-r--r--   0        0        0      261 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/configs/config_voltage.toml
+-rw-r--r--   0        0        0     2904 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/icepak.prof
+-rw-r--r--   0        0        0     2144 2023-05-09 12:44:32.935816 aedttest-0.0.2/tests/input/icepak_231.prof
+-rw-r--r--   0        0        0      894 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/input/mesh.mstat
+-rw-r--r--   0        0        0      180 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/input/no_mesh.mstat
+-rw-r--r--   0        0        0     8093 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/input/prof_test_mixed_case.prof
+-rw-r--r--   0        0        0     3128 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/input/project_report.json
+-rw-r--r--   0        0        0      589 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/input/reference_simple/ref_sample.json
+-rw-r--r--   0        0        0        0 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/unittests/__init__.py
+-rw-r--r--   0        0        0    19767 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/unittests/test_aedt_test_runner.py
+-rw-r--r--   0        0        0     4001 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/unittests/test_clusters.py
+-rw-r--r--   0        0        0    12274 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/unittests/test_simulation_data.py
+-rw-r--r--   0        0        0     4801 2023-05-09 12:44:32.939816 aedttest-0.0.2/tests/unittests/test_web_pages.py
+-rw-r--r--   0        0        0      467 2023-05-09 12:44:32.939816 aedttest-0.0.2/tox.ini
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 aedttest-0.0.2/setup.py
+-rw-r--r--   0        0        0     5415 1970-01-01 00:00:00.000000 aedttest-0.0.2/PKG-INFO
```

### Comparing `aedttest-0.0.1.dev9/.github/workflows/ci-sim-data.yml` & `aedttest-0.0.2/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 name: CI
 
 on:
   pull_request:
 
 jobs:
-  sim-data-tests:
-    runs-on: windows-latest
+  tests:
+    runs-on: ubuntu-latest
     strategy:
       fail-fast: false
 
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v2
       with:
         fetch-depth: 1
 
     - uses: actions/setup-python@v2
       with:
-        python-version: 2.7
+        python-version: 3.7
 
     - name: Install dependencies
       run: |
-        python -m pip install -r tests/reqs_test_sim_data_py27.txt
+        python -m pip install --upgrade pip
+        python -m pip install .[test]
         
     - name: Unittests
       run: |
-        pytest -v tests/unittests/test_simulation_data.py --disable-pytest-warnings --cov-report term-missing --cov
+        pytest -v tests/unittests --cov-report term-missing --cov
+
+    - name: MyPy
+      run: |
+        mypy --config-file=./mypy.ini -p aedttest
```

### Comparing `aedttest-0.0.1.dev9/.github/workflows/deploy.yml` & `aedttest-0.0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/.gitignore` & `aedttest-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/.pre-commit-config.yaml` & `aedttest-0.0.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -12,29 +12,40 @@
         args: ["-l", "120"]
   - repo: https://github.com/asottile/blacken-docs
     rev: v1.12.1
     hooks:
       - id: blacken-docs
         additional_dependencies: [black]
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
         name: isort (python)
         args: ["-sl", "--profile", "black"]
       - id: isort
         name: isort (pyi)
         types: [pyi]
         args: ["-sl", "--profile", "black"]
 
   - repo: https://github.com/pycqa/flake8
-    rev: 3.9.2
+    rev: 5.0.4
     hooks:
       - id: flake8
+        name: flake8-py3
         args: ["--max-line-length", "120", "--max-doc-length", "120"]
+
+  - repo: https://github.com/pycqa/flake8
+    rev: 3.9.2
+    hooks:
+      - id: flake8
+        name: flake8-py27
+        language_version: python2.7
+        files: "simulation_data.py$"
+        args: [ "--max-line-length", "120", "--max-doc-length", "120" ]
+
   - repo: https://github.com/Lucas-C/pre-commit-hooks-nodejs
     rev: v1.1.2
     hooks:
       - id: markdown-toc
         name: Table of Contents
 
   - repo: https://github.com/pre-commit/mirrors-prettier
```

### Comparing `aedttest-0.0.1.dev9/LICENSE` & `aedttest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/README.md` & `aedttest-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 ##### Generate only reference results
 ```bash
 aedt_test_runner --config-folder=examples/configs --aedt-version=193 --only-reference
 ```
 
 ##### Run comparison between versions
 ```bash
-aedt_test_runner --config-folder=examples/configs --aedt-version=222 --reference-file=reference_folder
+aedt_test_runner --config-folder=examples/configs --aedt-version=231 --reference-folder=reference_folder
 ```
 
 #### Slurm
 ##### Generate only reference results
 ```bash
 sbatch \
   --job-name aedttest \
@@ -99,15 +99,15 @@
 ##### Run comparison between versions
 ```bash
 sbatch \
   --job-name aedttest \
   --partition ottc01 \
   --export "ALL,ANSYSEM_ROOT222=/ott/apps/software/ANSYS_EM_2022R2_211129/v222/Linux64,ANS_NODEPCHECK=1" \
   --nodes 2-2 --ntasks 56 \
-  --wrap "aedt_test_runner --config-folder=examples/configs --aedt-version=222 --reference-file=~/reference_folder"
+  --wrap "aedt_test_runner --config-folder=examples/configs --aedt-version=222 --reference-folder=~/reference_folder"
 ```
 
 ## Limitations
 Currently, project does not support or partially supports following features:
 * Automatic results creation is possible only for versions 2019R1+
 * LS-DSO is not supported
```

### Comparing `aedttest-0.0.1.dev9/aedttest/aedt_test_runner.py` & `aedttest-0.0.2/aedttest/aedt_test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         self.only_reference = only_reference
         self.reference_data = {}
         if not only_reference and reference_folder is not None:
             for ref in reference_folder.rglob("*.json"):
                 with open(ref) as file:
                     data = json.load(file)
                 self.reference_data[data["name"]] = data
+                self.reference_data[data["name"]]["filepath"] = reference_folder
 
         self.script = str(MODULE_DIR / "simulation_data.py")
 
         # logfile path will be appended dynamically later
         self.script_args = f"\"--pyaedt-path='{Path(_py_aedt_path).parent.parent}' --logfile-path='{{}}'\""
 
         if debug:
@@ -230,32 +231,40 @@
 
         """
         if self.results_path.exists():
             remove_tree(str(self.results_path))
         copy_path_to(str(MODULE_DIR / "static" / "css"), str(self.results_path))
         copy_path_to(str(MODULE_DIR / "static" / "js"), str(self.results_path))
         self.reference_folder.mkdir()
-
+        if self.only_reference:
+            for project_name in self.project_tests_config:
+                Path(self.reference_folder, project_name, "prof").mkdir(parents=True, exist_ok=True)
         self.report_data["all_delta"] = 1 if not self.only_reference else None
         self.report_data["projects"] = {}
 
-        for project_name, project_config in self.project_tests_config.items():
+        for project_name in sorted(self.project_tests_config):
             self.report_data["projects"][project_name] = {
-                "cores": project_config["distribution"]["cores"],
+                "cores": self.project_tests_config[project_name]["distribution"]["cores"],
                 "status": "queued",
                 "link": None,
                 "delta": None,
                 "avg": None,
                 "time": time_now(),
             }
 
             if not self.only_reference:
                 # initialize integer for proper rendering
                 self.report_data["projects"][project_name]["delta"] = 0
                 self.report_data["projects"][project_name]["avg"] = 0
+                if project_name in self.reference_data:
+                    reference_path = Path(self.reference_data[project_name]["filepath"], project_name)
+                    copy_path_to(
+                        reference_path.resolve(),
+                        self.reference_folder,
+                    )
 
         self.render_main_html()
 
     def render_main_html(self, finished: bool = False) -> None:
         """Renders main report page.
 
         Using ``self.report_data`` updates django template with the data.
@@ -338,14 +347,16 @@
                 script_args=self.script_args.format(log_file),
                 project_path=project_path,
             )
             logger.debug(f"Project {project_name} analyses finished. Prepare report.")
 
         except OSError as exc:
             errors = str(exc)
+        except subprocess.CalledProcessError as exc:
+            errors = f"Electronics Desktop crashed. Most probably design is not valid. Log: {exc}"
         finally:
             # return cores back
             for machine in allocated_machines:
                 self.machines_dict[machine] += allocated_machines[machine]["cores"]
 
         project_report = self.prepare_project_report(project_name, project_path)
         if errors:
@@ -391,16 +402,14 @@
             "simulation_time": [],
             "slider_limit": 0,
             "max_avg": 0,
         }
         project_data = self.check_all_results_present(project_report["error_exception"], report_file, project_name)
         project_data["aedt_version"] = self.version
         project_data["name"] = project_name
-        with open(self.reference_folder / f"ref_{project_name}.json", "w") as file:
-            json.dump(project_data, file, indent=4)
 
         keys_missing = bool(project_report["error_exception"])
 
         try:
             project_report["error_exception"] += project_data["error_exception"]
 
             if keys_missing:
@@ -412,14 +421,18 @@
                 self.extract_mesh_or_time_data("mesh", design_data, design_name, project_name, project_report)
                 # get simulation time
                 self.extract_mesh_or_time_data(
                     "simulation_time", design_data, design_name, project_name, project_report
                 )
                 # extract XY curve data
                 self.extract_curve_data(design_data, design_name, project_name, project_report)
+
+            with open(self.reference_folder / f"ref_{project_name}.json", "w") as file:
+                json.dump(project_data, file, indent=4)
+
         except Exception as exc:
             project_report["error_exception"].append(str(exc))
 
         return project_report
 
     def check_all_results_present(
         self, project_exceptions: List[str], report_file: Path, project_name: str
@@ -441,15 +454,15 @@
 
         Returns
         -------
         project_data : dict
             Dictionary loaded from .json file.
 
         """
-        project_data: Dict[str, Any] = {}
+        project_data: Dict[str, Any] = {"error_exception": []}
         if not report_file.exists():
             project_exceptions.append(f"Project report for {project_name} does not exist")
             return project_data
 
         with open(report_file) as file:
             project_data = json.load(file)
 
@@ -493,14 +506,18 @@
             Name of the project.
         project_report : dict
             Project report dictionary that is required by 'render_project_html()'.
 
         """
         for report_name, report_data in design_data["report"].items():
             for trace_name, trace_data in report_data.items():
+                if not trace_data["curves"]:
+                    msg = f"{design_name}:{report_name}:{trace_name} is empty"
+                    project_report["error_exception"].append(msg)
+                    continue
                 for curve_name, curve_data in trace_data["curves"].items():
                     plot_data = {
                         "name": f"{design_name}:{report_name}:{trace_name}:{curve_name}",
                         "id": unique_id(),
                         "x_label": f'"{trace_data["x_name"]} [{trace_data["x_unit"]}]"',
                         "y_label": f'"[{trace_data["y_unit"]}]"',
                         "x_axis": curve_data["x_data"],
@@ -526,19 +543,20 @@
                             project_report["error_exception"].append(msg)
                             continue
 
                         max_delta = 0
                         difference = []
                         for ref, actual in zip(y_ref_data, curve_data["y_data"]):
                             difference.append(ref - actual)
-                            if actual != 0:
-                                # if 0, just skip, no sense for 'infinite' delta
-                                max_delta = max(max_delta, abs(1 - ref / actual))
+                            # avoid division by zero by using small tolerance of 1e-20
+                            max_delta = max(max_delta, abs(1 - ref / (actual or 1e-20)))
+
                         max_delta_perc = round(max_delta * 100, 3)
-                        avg_perc = round(abs(1 - mean(y_ref_data) / mean(curve_data["y_data"])), 3)
+                        mean_curve_data = mean(curve_data["y_data"])
+                        avg_perc = round(abs(1 - mean(y_ref_data) / (mean_curve_data or 1e-20)), 3)
 
                         # take always integer since ticks are integers, and +1 to allow to slide
                         project_report["slider_limit"] = max(project_report["slider_limit"], int(max_delta_perc) + 1)
                         project_report["max_avg"] = max(project_report["max_avg"], int(avg_perc))
                         plot_data.update(
                             {
                                 "version_ref": self.reference_data[project_name]["aedt_version"],
@@ -575,27 +593,44 @@
             Name of the project.
         project_report : dict
             Project report dictionary that is required by ``render_project_html()``.
 
         """
         for variation_name, variation_data in design_data[key_name].items():
             for setup_name, current_stat in variation_data.items():
+                extract = "mesh_name" if key_name == "mesh" else "profile_name"
+                absolute_path = design_data[extract][variation_name][setup_name]
+
+                # Check if profile exists already to avoid duplicates
+                cont = 1
+                filepath = new_absolute_path = Path(absolute_path)
+                reference_profiles = Path(self.reference_folder, project_name, "prof")
+                while (reference_profiles / new_absolute_path.name).exists():
+                    new_absolute_path = filepath.parent / f"{filepath.stem}{cont}{filepath.suffix}"
+                    cont += 1
+                filepath.rename(new_absolute_path)
+
+                new_path = str(copy_path_to(new_absolute_path, reference_profiles))
+                new_path_relative = str(Path(new_path).relative_to(self.proj_dir)).replace("\\", "/")
+                design_data[extract][variation_name][setup_name] = new_path_relative
                 stat_dict = {
                     "name": f"{design_name}:{setup_name}:{variation_name}",
                     "current": current_stat,
+                    "link": new_path_relative,
                 }
                 if not self.only_reference:
-                    reference_dict = self.reference_data[project_name]["designs"][design_name][key_name]
-                    if variation_name not in reference_dict:
+                    reference_dict = self.reference_data[project_name]["designs"][design_name]
+                    if variation_name not in reference_dict[key_name]:
                         project_report["error_exception"].append(
                             f"Variation ({variation_name}) wasn't found in reference results for design: {design_name}"
                         )
                         continue
 
-                    stat_dict["ref"] = reference_dict[variation_name][setup_name]
+                    stat_dict["ref"] = reference_dict[key_name][variation_name][setup_name]
+                    stat_dict["ref_link"] = reference_dict[extract][variation_name][setup_name]
 
                 project_report[key_name].append(stat_dict)
 
     def allocator(self) -> Iterable[Tuple[str, Dict[str, Dict[str, int]]]]:
         """Generator that yields resources.
 
         Waits until resources are available.
@@ -763,14 +798,17 @@
     Returns
     -------
     path : str
         Location where it was copied.
 
     """
     src = project_config["path"]
+    src_aedb = src.replace(".aedt", ".aedb")
+    if Path(src_aedb).exists():
+        copy_path_to(src_aedb, dst)
     return copy_path_to(src, dst)
 
 
 def copy_dependencies(project_config: Dict[str, Any], dst: str) -> None:
     """Copies project dependencies to run location.
 
     Parameters
@@ -786,54 +824,58 @@
     if isinstance(deps, list):
         for dep in deps:
             copy_path_to(dep, dst)
     elif isinstance(deps, str):
         copy_path_to(deps, dst)
 
 
-def copy_path_to(src: str, dst: str) -> Union[str, List[str]]:
+def copy_path_to(src: Union[str, Path], dst: Union[str, Path]) -> Union[str, List[str]]:
     """Copy path from src to dst.
 
     If ``src`` is a relative path, preserves relative folder tree.
 
     Parameters
     ----------
-    src : str
+    src : str or Path
         Path with copy target, relative or absolute.
-    dst : str
+    dst : str or Path
         Path where to copy.
 
     Returns
     -------
     path: str or list
         Path to copied file or list with paths if folder is copied.
 
     """
-    src_path = Path(src.replace("\\", "/"))
-    if not src_path.is_absolute() and len(src_path.parents) > 1:
-        unpack_dst = Path(dst) / src_path.parents[0]
-        if not src_path.is_file():
-            unpack_dst /= src_path.name
-    elif not src_path.is_file():
-        unpack_dst = Path(dst) / src_path.name
+    if isinstance(src, str):
+        src = Path(src.replace("\\", "/"))
+    if isinstance(dst, str):
+        dst = Path(dst.replace("\\", "/"))
+
+    if not src.is_absolute() and len(src.parents) > 1:
+        unpack_dst = dst / src.parents[0]
+        if not src.is_file():
+            unpack_dst /= src.name
+    elif not src.is_file():
+        unpack_dst = dst / src.name
     else:
-        unpack_dst = Path(dst)
+        unpack_dst = dst
 
-    src_path = src_path.expanduser().resolve()
-    if not src_path.exists():
-        raise FileExistsError(f"File {src_path} doesn't exist")
+    src = src.expanduser().resolve()
+    if not src.exists():
+        raise FileExistsError(f"File {src} doesn't exist")
 
     dst = str(unpack_dst)
     mkpath(dst)
 
-    if src_path.is_file():
-        file_path = copy_file(str(src_path), dst)
+    if src.is_file():
+        file_path = copy_file(str(src), dst)
         return file_path[0]
     else:
-        return copy_tree(str(src_path), dst)
+        return copy_tree(str(src), dst)
 
 
 def mkdtemp_persistent(*args: Any, persistent: bool = True, **kwargs: Any) -> Any:
     """Provides a context manager to create a temporary/permanent directory depending on 'persistent' argument
 
     Parameters
     ----------
@@ -909,14 +951,17 @@
     project_path : str, optional
         Path to the project.
 
     """
     aedt_path = get_aedt_executable_path(version)
     command = [aedt_path]
 
+    if int(version) >= 231:
+        os.environ["ANSYSEM_GEOM_KERN_FORCE_OVERWRITE_ORIG_PROJECT"] = "1"
+
     if distribution_config["auto"]:
         # for auto number of tasks on host must be "-1"
         aedt_format_machines = ",".join([f"{name}:-1:{conf['cores']}:90%" for name, conf in machines.items()])
         command += ["-auto", f"NumDistributedVariations={distribution_config['parametric_tasks']}"]
     else:
         aedt_format_machines = ",".join(
             [f"{name}:{conf['tasks']}:{conf['cores']}:90%" for name, conf in machines.items()]
```

### Comparing `aedttest-0.0.1.dev9/aedttest/clusters/job_hosts.py` & `aedttest-0.0.2/aedttest/clusters/job_hosts.py`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/clusters/job_hosts.pyi` & `aedttest-0.0.2/aedttest/clusters/job_hosts.pyi`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/logger.py` & `aedttest-0.0.2/aedttest/logger.py`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/simulation_data.py` & `aedttest-0.0.2/aedttest/simulation_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,43 @@
 sys.path.append(MODULE_DIR_PARENT)
 
 from aedttest.logger import logger  # noqa: E402
 from aedttest.logger import set_logger  # noqa: E402
 
 
 def parse_args():
+    """Parse arguments that were provided to the script when executed with RunScriptAndExit."""
     arg_string = ScriptArgument.replace('"', "")  # noqa: F821
     parser = argparse.ArgumentParser()
     parser.add_argument("--pyaedt-path")
     parser.add_argument("--logfile-path")
     parser.add_argument("--debug", action="store_true")
     args = parser.parse_args(shlex.split(arg_string))
     return args.pyaedt_path, args.logfile_path, args.debug
 
 
+def parse_args_debug():
+    """Parse arguments that were provided to the script when the script is executed directly."""
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--desktop-version", default="2022.1")
+    args = parser.parse_args()
+
+    return args.desktop_version
+
+
 log_level = logging.DEBUG
 if not DEBUG:
     pyaedt_path, logfile_path, debug = parse_args()
     sys.path.insert(0, pyaedt_path)
     specified_version = None
 
     if not debug:
         log_level = logging.INFO
 else:
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--desktop-version", default="2022.1")
-    args = parser.parse_args()
-    specified_version = args.desktop_version
+    specified_version = parse_args_debug()
     logfile_path = os.path.join(MODULE_DIR_PARENT, "aedt_test_framework.log")
 
 try:
     import pyaedt  # noqa: E402
     from pyaedt import get_pyaedt_app  # noqa: E402
     from pyaedt.desktop import Desktop  # noqa: E402
     from pyaedt.generic.general_methods import generate_unique_name  # noqa: E402
@@ -174,15 +181,15 @@
 
 
 def extract_data(desktop, project_dir, project_name, design_names):
     """Extract designs' data for a project.
 
     Parameters
     ----------
-    desktop : object
+    desktop : pyaedt.desktop.Desktop
         ``pyaedt`` ``Desktop`` object.
     project_dir : str
         Path to the project.
     project_name : str
         Name of the project
     design_names : list
         List of design names.
@@ -191,18 +198,19 @@
     -------
     designs_dict : dict
         Dictionary includes data of all listed designs.
 
     """
 
     designs_dict = {}
-    oDesktop = desktop._main.oDesktop
 
     for design_name in design_names:
-        design_dict = {design_name: {"mesh": {}, "simulation_time": {}, "report": {}}}
+        design_dict = {
+            design_name: {"mesh": {}, "simulation_time": {}, "report": {}, "profile_name": {}, "mesh_name": {}}
+        }
         app = get_pyaedt_app(design_name=design_name)
         setups_names = app.setup_names
         if not setups_names:
             PROJECT_DICT["error_exception"].append("Design {} has no setups".format(design_name))
             designs_dict.update(design_dict)
             continue
 
@@ -214,22 +222,20 @@
                     setup_dict[setups] = sweep
                     break
 
         analyze_success = desktop.analyze_all(design=design_name)
 
         if not analyze_success:
             logger.error("design {} 'analyze_all' failed".format(design_name))
-
-            error_messages = oDesktop.GetMessages(project_name, design_name, 1)
-            message = str(error_messages).replace("[error]", "")
-            message = "{}: {}".format(design_name, message)
-            logger.error(message)
-            PROJECT_DICT["error_exception"].append(message)
-
-            continue
+            error_messages = app.logger.get_messages(project_name, design_name, level=1, aedt_messages=True)
+            messages = error_messages.design_level + error_messages.project_level + error_messages.global_level
+            for message in messages:
+                log_message = "{}: {}".format(design_name, message)
+                logger.error(log_message)
+                PROJECT_DICT["error_exception"].append(log_message)
         else:
             logger.info("design {} 'analyze_all' success".format(design_name))
 
         design_dict = extract_design_data(
             app=app,
             design_name=design_name,
             setup_dict=setup_dict,
@@ -250,15 +256,15 @@
 
 
 def extract_design_data(app, design_name, setup_dict, project_dir, design_dict):
     """Extract single design data.
 
     Parameters
     ----------
-    app : object
+    app : pyaedt.application.AedtObjects
         ``pyaedt`` Electronics Desktop application object.
     design_name : str
         Name of the design
     setup_dict : dict
         Dictionary of the setups. key: setup name, value: sweeps.
     project_dir : str
         Path to the project folder
@@ -269,38 +275,49 @@
     -------
     design_dict : dict
         Dictionary with values of mesh elements, simulation_time and report data.
 
     """
 
     for setup, sweep in setup_dict.items():
-        variation_strings = app.available_variations.get_variation_strings(sweep)
+        if app.design_type == "HFSS 3D Layout Design":
+            variation_strings = app.list_of_variations(setup, sweep.lstrip(setup + " : "))
+        else:
+            variation_strings = app.available_variations.get_variation_strings(sweep)
         if not variation_strings:
             continue
         for variation_string in variation_strings:
             variation_name = "nominal" if not variation_string else compose_variation_string(variation_string)
 
             if variation_name not in design_dict[design_name]["mesh"]:
                 design_dict[design_name]["mesh"][variation_name] = {}
             if variation_name not in design_dict[design_name]["simulation_time"]:
                 design_dict[design_name]["simulation_time"][variation_name] = {}
+            if variation_name not in design_dict[design_name]["profile_name"]:
+                design_dict[design_name]["profile_name"][variation_name] = {}
+            if variation_name not in design_dict[design_name]["mesh_name"]:
+                design_dict[design_name]["mesh_name"][variation_name] = {}
 
             profile_file = generate_unique_file_path(project_dir, ".prof")
             profile_file = app.export_profile(setup, variation_string, profile_file)
             simulation_time, cell_number = parse_profile_file(profile_file, design_name, variation_name, setup)
             design_dict[design_name]["simulation_time"][variation_name][setup] = simulation_time
 
             if app.design_type == "Icepak":
                 design_dict[design_name]["mesh"][variation_name][setup] = cell_number
+                mesh_stats_file = profile_file
             else:
                 mesh_stats_file = generate_unique_file_path(project_dir, ".mstat")
                 app.export_mesh_stats(setup, variation_string, mesh_stats_file)
                 mesh_data = parse_mesh_stats(mesh_stats_file, design_name, variation_name, setup)
                 design_dict[design_name]["mesh"][variation_name][setup] = mesh_data
 
+            design_dict[design_name]["profile_name"][variation_name][setup] = profile_file
+            design_dict[design_name]["mesh_name"][variation_name][setup] = mesh_stats_file
+
     return design_dict
 
 
 def compose_variation_string(variation_string):
     """Format the variation string.
 
     Parameters
@@ -330,15 +347,15 @@
 
 
 def extract_reports_data(app, design_name, project_dir, report_names):
     """Get the report data form .rdat file.
 
     Parameters
     ----------
-    app : object
+    app : pyaedt.application.AedtObjects
         Any ``pyaedt`` Electronics Desktop application object.
     design_name : str
         Name of the design.
     project_dir : str
         Path to the project.
     report_names : list
         List of report names.
```

### Comparing `aedttest-0.0.1.dev9/aedttest/simulation_data.pyi` & `aedttest-0.0.2/aedttest/simulation_data.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 DEBUG: bool
 
 def parse_args() -> str: ...
+def parse_args_debug() -> str: ...
 
 pyaedt_path: str
 specified_version: Optional[str]
 parser: Any
 args: Any
 PROJECT_DICT: Dict[str, Any]
```

### Comparing `aedttest-0.0.1.dev9/aedttest/static/css/css-lib/bootstrap-slider.css` & `aedttest-0.0.2/aedttest/static/css/css-lib/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/css/css-lib/bootstrap.min.css` & `aedttest-0.0.2/aedttest/static/css/css-lib/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/css/css-lib/jquery-ui.min.css` & `aedttest-0.0.2/aedttest/static/css/css-lib/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/css/style.css` & `aedttest-0.0.2/aedttest/static/css/style.css`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/chartjs-init.js` & `aedttest-0.0.2/aedttest/static/js/chartjs-init.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/common.js` & `aedttest-0.0.2/aedttest/static/js/common.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/js-lib/Chart.bundle.js` & `aedttest-0.0.2/aedttest/static/js/js-lib/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/js-lib/bootstrap-slider.min.js` & `aedttest-0.0.2/aedttest/static/js/js-lib/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/js-lib/bootstrap.min.js` & `aedttest-0.0.2/aedttest/static/js/js-lib/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/js-lib/jquery.min.js` & `aedttest-0.0.2/aedttest/static/js/js-lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/js-lib/jquery.nanoscroller.min.js` & `aedttest-0.0.2/aedttest/static/js/js-lib/jquery.nanoscroller.min.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/js/main.js` & `aedttest-0.0.2/aedttest/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/templates/main.html` & `aedttest-0.0.2/aedttest/static/templates/main.html`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/aedttest/static/templates/project-report.html` & `aedttest-0.0.2/aedttest/static/templates/project-report.html`

 * *Files 4% similar despite different names*

```diff
@@ -102,17 +102,25 @@
                           </tr>
                         </thead>
                         <tbody>
                           {% for time in sim_time %}
                           <tr>
                             <td>{{ time.name }}</td>
                             {% if has_reference %}
-                            <td>{{ time.ref }}</td>
+                            <td>
+                              {% if time.ref_link %}
+                              <a href="{{ time.ref_link }}">{{ time.ref }}</a>
+                              {% else %} {{ time.ref }} {% endif %}
+                            </td>
                             {% endif %}
-                            <td>{{ time.current }}</td>
+                            <td>
+                              {% if time.link %}
+                              <a href="{{ time.link }}">{{ time.current }}</a>
+                              {% else %} {{ time.current }} {% endif %}
+                            </td>
                           </tr>
                           {% endfor %}
                         </tbody>
                       </table>
                     </div>
                   </div>
                 </div>
@@ -140,17 +148,29 @@
                           </tr>
                         </thead>
                         <tbody>
                           {% for mesh_data in mesh %}
                           <tr>
                             <td>{{ mesh_data.name }}</td>
                             {% if has_reference %}
-                            <td>{{ mesh_data.ref }}</td>
+                            <td>
+                              {% if mesh_data.ref_link %}
+                              <a href="{{ mesh_data.ref_link }}"
+                                >{{ mesh_data.ref }}</a
+                              >
+                              {% else %} {{ mesh_data.ref }} {% endif %}
+                            </td>
                             {% endif %}
-                            <td>{{ mesh_data.current }}</td>
+                            <td>
+                              {% if mesh_data.link %}
+                              <a href="{{ mesh_data.link }}"
+                                >{{ mesh_data.current }}</a
+                              >
+                              {% else %} {{ mesh_data.current }} {% endif %}
+                            </td>
                           </tr>
                           {% endfor %}
                         </tbody>
                       </table>
                     </div>
                   </div>
                 </div>
```

#### html2text {}

```diff
@@ -10,19 +10,24 @@
 *** Difference Threshold [%] ***
 [                    ]
  {% endif %} {% if errors %}
 *** Error Messages ***
 {{ error }}
  {% endif %} {% if sim_time %}
 *** Simulation Time ***
-Source          Reference Time Current Time
-{{ time.name }} {{ time.ref }} {{ time.current }}
+Source          Reference Time             Current Time
+                {% if time.ref_link %} {   {% if time.link %} {{_time.current
+{{ time.name }} {_time.ref_}} {% else %} { }} {% else %} {{ time.current }}
+                { time.ref }} {% endif %}  {% endif %}
  {% endif %} {% if mesh %}
 *** Mesh Statistics ***
-Source               Reference Elements Count Current Elements Count
-{{ mesh_data.name }} {{ mesh_data.ref }}      {{ mesh_data.current }}
+Source               Reference Elements Count      Current Elements Count
+                     {% if mesh_data.ref_link %} { {% if mesh_data.link %} {
+{{ mesh_data.name }} {_mesh_data.ref_}} {% else %} {_mesh_data.current_}} {%
+                     {{ mesh_data.ref }} {% endif  else %} {{ mesh_data.current
+                     %}                            }} {% endif %}
  {% endif %} {% for plot in plots %}
   {% if has_reference %} {{ plot.name }} [maxΔ{{ plot.delta }}%] [avgΔ {
 { plot.avg }}%] {% else %} {{ plot.name }} {% endif %}
 {% endfor %}
 2021 &#xa9; Ansys Inc - ansys.com
```

### Comparing `aedttest-0.0.1.dev9/examples/configs/config_with_comments.toml` & `aedttest-0.0.2/examples/configs/config_with_comments.toml`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/mypy.ini` & `aedttest-0.0.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/pyproject.toml` & `aedttest-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,51 +4,54 @@
     "flit_core >=3.2,<4",
 ]
 build-backend = "flit_core.buildapi"
 
 # description of current module
 [project]
 name = "aedttest"
-version = "0.0.1.dev9"
+version = "0.0.2"
 
 description = """
 Ansys Electronics Desktop Testing Framework.
 Current module allows to setup and run automated tests and validate results across multiple versions of
 Ansys Electronics Desktop products, eg HFSS, Maxwell, Icepak, Q3D, etc
 """
 
 authors = [
     {name = "Maksim Beliaev", email = "maksim.beliaev@ansys.com"},
     {name = "Bo Yang", email = "bo.yang@ansys.com"},
+    {name = "Samuel Lopez", email = "samuel.lopez@ansys.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
-    "pyaedt==0.4.86",
-    "Django==3.2.8",
+    "pyaedt==0.6.57",
+    "Django==3.2.18",
     "tomli>=2.0.0",
 ]
 
 # development dependencies
 [project.optional-dependencies]
 test = [
     "pre-commit==2.15.0",
     "mypy==0.960",
     "pytest==6.2.5",
     "pytest-cov==3.0.0",
+    "webdriver-manager",
+    "selenium>4",
 ]
 
 deploy = [
     "flit==3.4.0",
 ]
 
 [project.urls]
```

### Comparing `aedttest-0.0.1.dev9/tests/input/2020R2_profile.prof` & `aedttest-0.0.2/tests/input/2020R2_profile.prof`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/2021R2_profile.prof` & `aedttest-0.0.2/tests/input/2021R2_profile.prof`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/R2019R1_profile.prof` & `aedttest-0.0.2/tests/input/R2019R1_profile.prof`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/allocator_config.json` & `aedttest-0.0.2/tests/input/allocator_config.json`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/icepak.prof` & `aedttest-0.0.2/tests/input/icepak.prof`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/icepak_231.prof` & `aedttest-0.0.2/tests/input/icepak_231.prof`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/mesh.mstat` & `aedttest-0.0.2/tests/input/mesh.mstat`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/prof_test_mixed_case.prof` & `aedttest-0.0.2/tests/input/prof_test_mixed_case.prof`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/input/reference_simple/ref_sample.json` & `aedttest-0.0.2/tests/input/reference_simple/ref_sample.json`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/unittests/test_aedt_test_runner.py` & `aedttest-0.0.2/tests/unittests/test_aedt_test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,15 @@
         assert "just_winding requires 2 cores. Not enough resources to run" in str(exc.value)
 
     @mock.patch("aedttest.aedt_test_runner.time_now", wraps=lambda *a, **kw: "2021-12-31 20:16:04")
     def test_initialize_results(self, time_mock):
         with TemporaryDirectory() as tmp_dir:
             self.aedt_tester.results_path = Path(tmp_dir)
             self.aedt_tester.reference_folder = Path(tmp_dir) / "1"
+            self.aedt_tester.reference_profiles = self.aedt_tester.reference_folder / "profiles"
             self.aedt_tester.initialize_results()
 
             assert self.aedt_tester.report_data == {
                 "all_delta": 1,
                 "projects": {
                     "just_winding": {
                         "avg": 0,
```

### Comparing `aedttest-0.0.1.dev9/tests/unittests/test_clusters.py` & `aedttest-0.0.2/tests/unittests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `aedttest-0.0.1.dev9/tests/unittests/test_simulation_data.py` & `aedttest-0.0.2/tests/unittests/test_simulation_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,22 +54,56 @@
         mock_pyaedt_app.export_profile.return_value = None
 
         result_dict = simulation_data.extract_design_data(
             app=mock_pyaedt_app,
             design_name="only_winding2",
             setup_dict={"Setup1": "Setup1 : LastAdaptive"},
             project_dir="/tmp",
-            design_dict={"only_winding2": {"mesh": {}, "simulation_time": {}, "report": {}}},
+            design_dict={
+                "only_winding2": {"mesh": {}, "simulation_time": {}, "report": {}, "profile_name": {}, "mesh_name": {}}
+            },
         )
+        mesh1 = result_dict["only_winding2"]["mesh_name"]["Ia=30A"]["Setup1"]
+        mesh2 = result_dict["only_winding2"]["mesh_name"]["Ia=20A"]["Setup1"]
+        assert result_dict == {
+            "only_winding2": {
+                "mesh": {"Ia=30A": {"Setup1": 100}, "Ia=20A": {"Setup1": 100}},
+                "simulation_time": {"Ia=30A": {"Setup1": "10:00:00"}, "Ia=20A": {"Setup1": "10:00:00"}},
+                "report": {},
+                "profile_name": {"Ia=30A": {"Setup1": None}, "Ia=20A": {"Setup1": None}},
+                "mesh_name": {"Ia=30A": {"Setup1": mesh1}, "Ia=20A": {"Setup1": mesh2}},
+            }
+        }
 
+    @mock.patch("aedttest.simulation_data.parse_profile_file", return_value=["10:00:00", 100])
+    def test_extract_design_data_icepak(self, mock_parse_profile_file):
+        mock_pyaedt_app = mock.Mock()
+        mock_pyaedt_app.available_variations.get_variation_strings.return_value = ["Ia='30'A", "Ia='20'A"]
+        mock_pyaedt_app.export_mesh_stats.return_value = None
+        mock_pyaedt_app.export_profile.return_value = None
+        mock_pyaedt_app.design_type = "Icepak"
+
+        result_dict = simulation_data.extract_design_data(
+            app=mock_pyaedt_app,
+            design_name="only_winding2",
+            setup_dict={"Setup1": "Setup1 : LastAdaptive"},
+            project_dir="/tmp",
+            design_dict={
+                "only_winding2": {"mesh": {}, "simulation_time": {}, "report": {}, "profile_name": {}, "mesh_name": {}}
+            },
+        )
+        mesh1 = result_dict["only_winding2"]["mesh_name"]["Ia=30A"]["Setup1"]
+        mesh2 = result_dict["only_winding2"]["mesh_name"]["Ia=20A"]["Setup1"]
         assert result_dict == {
             "only_winding2": {
                 "mesh": {"Ia=30A": {"Setup1": 100}, "Ia=20A": {"Setup1": 100}},
                 "simulation_time": {"Ia=30A": {"Setup1": "10:00:00"}, "Ia=20A": {"Setup1": "10:00:00"}},
                 "report": {},
+                "profile_name": {"Ia=30A": {"Setup1": None}, "Ia=20A": {"Setup1": None}},
+                "mesh_name": {"Ia=30A": {"Setup1": mesh1}, "Ia=20A": {"Setup1": mesh2}},
             }
         }
 
     def test_parse_profile_2020r2(self):
 
         result, _ = simulation_data.parse_profile_file(
             profile_file=os.path.join(TESTS_DIR, "input", "2020R2_profile.prof"),
```

### Comparing `aedttest-0.0.1.dev9/setup.py` & `aedttest-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,31 +12,33 @@
               'static/css/*',
               'static/css/css-lib/*',
               'static/js/*',
               'static/js/js-lib/*',
               'static/templates/*']}
 
 install_requires = \
-['pyaedt==0.4.86', 'Django==3.2.8', 'tomli>=2.0.0']
+['pyaedt==0.6.57', 'Django==3.2.18', 'tomli>=2.0.0']
 
 extras_require = \
 {'deploy': ['flit==3.4.0'],
  'test': ['pre-commit==2.15.0',
           'mypy==0.960',
           'pytest==6.2.5',
-          'pytest-cov==3.0.0']}
+          'pytest-cov==3.0.0',
+          'webdriver-manager',
+          'selenium>4']}
 
 entry_points = \
 {'console_scripts': ['aedt_test_runner = aedttest.aedt_test_runner:main']}
 
 setup(name='aedttest',
-      version='0.0.1.dev9',
+      version='0.0.2',
       description='Ansys Electronics Desktop Testing Framework.\nCurrent module allows to setup and run automated tests and validate results across multiple versions of\nAnsys Electronics Desktop products, eg HFSS, Maxwell, Icepak, Q3D, etc\n',
       author=None,
-      author_email='Maksim Beliaev <maksim.beliaev@ansys.com>, Bo Yang <bo.yang@ansys.com>',
+      author_email='Maksim Beliaev <maksim.beliaev@ansys.com>, Bo Yang <bo.yang@ansys.com>, Samuel Lopez <samuel.lopez@ansys.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
       extras_require=extras_require,
       entry_points=entry_points,
       python_requires='>=3.7',
```

### Comparing `aedttest-0.0.1.dev9/PKG-INFO` & `aedttest-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: aedttest
-Version: 0.0.1.dev9
+Version: 0.0.2
 Summary: Ansys Electronics Desktop Testing Framework.
         Current module allows to setup and run automated tests and validate results across multiple versions of
         Ansys Electronics Desktop products, eg HFSS, Maxwell, Icepak, Q3D, etc
-Author-email: Maksim Beliaev <maksim.beliaev@ansys.com>, Bo Yang <bo.yang@ansys.com>
+Author-email: Maksim Beliaev <maksim.beliaev@ansys.com>, Bo Yang <bo.yang@ansys.com>, Samuel Lopez <samuel.lopez@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pyaedt==0.4.86
-Requires-Dist: Django==3.2.8
+Requires-Dist: pyaedt==0.6.57
+Requires-Dist: Django==3.2.18
 Requires-Dist: tomli>=2.0.0
 Requires-Dist: flit==3.4.0 ; extra == "deploy"
 Requires-Dist: pre-commit==2.15.0 ; extra == "test"
 Requires-Dist: mypy==0.960 ; extra == "test"
 Requires-Dist: pytest==6.2.5 ; extra == "test"
 Requires-Dist: pytest-cov==3.0.0 ; extra == "test"
+Requires-Dist: webdriver-manager ; extra == "test"
+Requires-Dist: selenium>4 ; extra == "test"
 Project-URL: Home, https://github.com/ansys/aedt-testing
 Provides-Extra: deploy
 Provides-Extra: test
 
 [![](https://img.shields.io/pypi/v/aedttest.svg)](https://pypi.python.org/pypi/aedttest/)
 [![](https://img.shields.io/pypi/pyversions/aedttest.svg)](https://pypi.python.org/pypi/aedttest/)
 
@@ -106,15 +108,15 @@
 ##### Generate only reference results
 ```bash
 aedt_test_runner --config-folder=examples/configs --aedt-version=193 --only-reference
 ```
 
 ##### Run comparison between versions
 ```bash
-aedt_test_runner --config-folder=examples/configs --aedt-version=222 --reference-file=reference_folder
+aedt_test_runner --config-folder=examples/configs --aedt-version=231 --reference-folder=reference_folder
 ```
 
 #### Slurm
 ##### Generate only reference results
 ```bash
 sbatch \
   --job-name aedttest \
@@ -127,15 +129,15 @@
 ##### Run comparison between versions
 ```bash
 sbatch \
   --job-name aedttest \
   --partition ottc01 \
   --export "ALL,ANSYSEM_ROOT222=/ott/apps/software/ANSYS_EM_2022R2_211129/v222/Linux64,ANS_NODEPCHECK=1" \
   --nodes 2-2 --ntasks 56 \
-  --wrap "aedt_test_runner --config-folder=examples/configs --aedt-version=222 --reference-file=~/reference_folder"
+  --wrap "aedt_test_runner --config-folder=examples/configs --aedt-version=222 --reference-folder=~/reference_folder"
 ```
 
 ## Limitations
 Currently, project does not support or partially supports following features:
 * Automatic results creation is possible only for versions 2019R1+
 * LS-DSO is not supported
```

