# Comparing `tmp/sageworks-0.1.4.3.tar.gz` & `tmp/sageworks-0.1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.1.4.3.tar", last modified: Tue May  2 13:29:22 2023, max compression
+gzip compressed data, was "sageworks-0.1.5.0.tar", last modified: Tue May  9 15:35:16 2023, max compression
```

## Comparing `sageworks-0.1.4.3.tar` & `sageworks-0.1.5.0.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.026030 sageworks-0.1.4.3/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.975436 sageworks-0.1.4.3/.github/
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.4.3/.github/dependabot.yml
--rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.4.3/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.4.3/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.4.3/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     5684 2023-05-02 13:29:22.026133 sageworks-0.1.4.3/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     4951 2023-05-01 19:54:07.000000 sageworks-0.1.4.3/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.4.3/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.969646 sageworks-0.1.4.3/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.975610 sageworks-0.1.4.3/applications/aws_dashboard/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.976095 sageworks-0.1.4.3/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12244 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.4.3/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     1066 2023-04-29 19:22:53.000000 sageworks-0.1.4.3/applications/aws_dashboard/aws_dashboard.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.977302 sageworks-0.1.4.3/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.977973 sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/
--rw-r--r--   0 briford    (501) staff       (20)     4046 2023-05-01 19:42:38.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      914 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      938 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     1786 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/main_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4722 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/models_callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.978443 sageworks-0.1.4.3/applications/aws_dashboard/pages/data/
--rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     2350 2023-05-02 13:17:43.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)     1423 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     1520 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/feature_sets.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.979686 sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/
--rw-r--r--   0 briford    (501) staff       (20)     1366 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/data_sources_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/endpoints_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/feature_sets_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/main_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2341 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/models_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2111 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/main.py
--rw-r--r--   0 briford    (501) staff       (20)     2535 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/aws_dashboard/pages/models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.980230 sageworks-0.1.4.3/applications/hello_world/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/applications/hello_world/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2158 2023-05-01 19:48:59.000000 sageworks-0.1.4.3/applications/hello_world/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/applications/hello_world/layout.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.980682 sageworks-0.1.4.3/applications/model_viewer/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/applications/model_viewer/callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.981147 sageworks-0.1.4.3/applications/model_viewer/data/
--rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.4.3/applications/model_viewer/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.4.3/applications/model_viewer/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/applications/model_viewer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2500 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/applications/model_viewer/model_viewer.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.981917 sageworks-0.1.4.3/applications/web_admin/
--rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/applications/web_admin/flask_test.py
--rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.4.3/applications/web_admin/hello-world-http-test.ini
--rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.4.3/applications/web_admin/hello-world.ini
--rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.4.3/applications/web_admin/hello-world.service
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.982151 sageworks-0.1.4.3/applications/web_admin/nginx_conf/
--rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.4.3/applications/web_admin/nginx_conf/nginx.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.982621 sageworks-0.1.4.3/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3315 2023-04-30 02:51:12.000000 sageworks-0.1.4.3/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     4010 2023-04-30 03:07:40.000000 sageworks-0.1.4.3/aws_setup/aws_account_check_deep.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.984186 sageworks-0.1.4.3/aws_setup/sageworks_cdk/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.984441 sageworks-0.1.4.3/aws_setup/sageworks_cdk/stacks/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/stacks/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2402 2023-04-30 18:00:46.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.984650 sageworks-0.1.4.3/aws_setup/sageworks_cdk/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.984819 sageworks-0.1.4.3/aws_setup/sageworks_cdk/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.4.3/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.985018 sageworks-0.1.4.3/config/
--rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.4.3/config/sageworks_config.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.986224 sageworks-0.1.4.3/data/
--rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.4.3/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)      613 2023-04-18 16:23:14.000000 sageworks-0.1.4.3/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.4.3/data/test_data.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.986896 sageworks-0.1.4.3/docs/
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.4.3/docs/admin_notes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.992688 sageworks-0.1.4.3/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.4.3/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.4.3/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.4.3/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.4.3/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.4.3/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.4.3/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.4.3/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.4.3/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.4.3/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.4.3/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.4.3/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.4.3/docs/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.4.3/docs/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.993487 sageworks-0.1.4.3/examples/
--rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/examples/data_to_data_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.993742 sageworks-0.1.4.3/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   236764 2023-04-20 18:57:28.000000 sageworks-0.1.4.3/notebooks/ML_Pipeline_with_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.998499 sageworks-0.1.4.3/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.4.3/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.4.3/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.4.3/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.4.3/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.4.3/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.4.3/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.4.3/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.002471 sageworks-0.1.4.3/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/scripts/data_source_tags.py
--rw-r--r--   0 briford    (501) staff       (20)     1716 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/scripts/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/scripts/list_data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-02 13:29:22.026433 sageworks-0.1.4.3/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1786 2023-05-02 13:29:00.000000 sageworks-0.1.4.3/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.970614 sageworks-0.1.4.3/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.002656 sageworks-0.1.4.3/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.4.3/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.003393 sageworks-0.1.4.3/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.970867 sageworks-0.1.4.3/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.003481 sageworks-0.1.4.3/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.4.3/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.003721 sageworks-0.1.4.3/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.4.3/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.971131 sageworks-0.1.4.3/src/sageworks/algorithms/table/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.003950 sageworks-0.1.4.3/src/sageworks/algorithms/table/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.4.3/src/sageworks/algorithms/table/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.005013 sageworks-0.1.4.3/src/sageworks/algorithms/table/light/
--rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.4.3/src/sageworks/algorithms/table/light/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.4.3/src/sageworks/algorithms/table/light/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/src/sageworks/algorithms/table/light/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/src/sageworks/algorithms/table/light/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.005683 sageworks-0.1.4.3/src/sageworks/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.4.3/src/sageworks/artifacts/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.4.3/src/sageworks/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4567 2023-04-30 15:25:18.000000 sageworks-0.1.4.3/src/sageworks/artifacts/artifact.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.006416 sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8473 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2534 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     1783 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/data_source_abstract.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.006687 sageworks-0.1.4.3/src/sageworks/artifacts/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/artifacts/endpoints/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9826 2023-04-19 16:14:58.000000 sageworks-0.1.4.3/src/sageworks/artifacts/endpoints/endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.007124 sageworks-0.1.4.3/src/sageworks/artifacts/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/artifacts/feature_sets/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    11500 2023-04-19 16:37:35.000000 sageworks-0.1.4.3/src/sageworks/artifacts/feature_sets/feature_set.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.007452 sageworks-0.1.4.3/src/sageworks/artifacts/models/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/artifacts/models/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4288 2023-04-19 16:37:35.000000 sageworks-0.1.4.3/src/sageworks/artifacts/models/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.007930 sageworks-0.1.4.3/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     7591 2023-04-30 17:35:38.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)     7426 2023-04-30 02:50:10.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.009771 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4187 2023-04-30 18:15:05.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
--rw-r--r--   0 briford    (501) staff       (20)     1512 2023-04-19 17:04:31.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     2589 2023-04-30 02:50:10.000000 sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.010370 sageworks-0.1.4.3/src/sageworks/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.4.3/src/sageworks/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.971802 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.010577 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)     5597 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.011317 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.011547 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.011638 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.011725 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.011984 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.012574 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2047 2023-04-19 22:49:17.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2346 2023-04-19 21:48:41.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.012746 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.012925 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5918 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.013170 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.013417 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.014043 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2585 2023-04-09 22:14:00.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     3000 2023-04-18 02:49:29.000000 sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.014267 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:21.972616 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.014359 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.014584 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.014836 sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7866 2023-04-19 18:49:44.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.015300 sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.015720 sageworks-0.1.4.3/src/sageworks/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.3/src/sageworks/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.4.3/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.017172 sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     7073 2023-04-19 22:49:17.000000 sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)     9472 2023-04-19 16:44:04.000000 sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-19 22:02:24.000000 sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5464 2023-04-30 02:50:10.000000 sageworks-0.1.4.3/src/sageworks/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.019069 sageworks-0.1.4.3/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.4.3/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.4.3/src/sageworks/utils/iso_8601.py
--rw-r--r--   0 briford    (501) staff       (20)     6563 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.4.3/src/sageworks/utils/sageworks_config.py
--rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.4.3/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.4.3/src/sageworks/utils/sageworks_sqs.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.020206 sageworks-0.1.4.3/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     9429 2023-05-02 13:13:09.000000 sageworks-0.1.4.3/src/sageworks/views/artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.4.3/src/sageworks/views/view.py
--rw-r--r--   0 briford    (501) staff       (20)    12557 2023-05-02 13:17:43.000000 sageworks-0.1.4.3/src/sageworks/views/web_artifacts_summary.py
--rw-r--r--   0 briford    (501) staff       (20)     5649 2023-05-01 19:53:31.000000 sageworks-0.1.4.3/src/sageworks/views/web_data_source_view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.022948 sageworks-0.1.4.3/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1335 2023-04-30 15:51:43.000000 sageworks-0.1.4.3/src/sageworks/web_components/box_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.4.3/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/src/sageworks/web_components/feature_details.py
--rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.4.3/src/sageworks/web_components/feature_importance.py
--rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.4.3/src/sageworks/web_components/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.4.3/src/sageworks/web_components/model_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.4.3/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.4.3/src/sageworks/web_components/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2116 2023-04-30 02:31:13.000000 sageworks-0.1.4.3/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     1920 2023-04-30 00:05:24.000000 sageworks-0.1.4.3/src/sageworks/web_components/violin_plot.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.003286 sageworks-0.1.4.3/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     5684 2023-05-02 13:29:21.000000 sageworks-0.1.4.3/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     8772 2023-05-02 13:29:21.000000 sageworks-0.1.4.3/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-02 13:29:21.000000 sageworks-0.1.4.3/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-02 13:29:21.000000 sageworks-0.1.4.3/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-02 13:29:21.000000 sageworks-0.1.4.3/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.023169 sageworks-0.1.4.3/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.024322 sageworks-0.1.4.3/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1169 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.4.3/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1095 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.024814 sageworks-0.1.4.3/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      347 2023-04-12 21:35:42.000000 sageworks-0.1.4.3/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      682 2023-04-02 18:05:33.000000 sageworks-0.1.4.3/tests/aws_account/aws_service_broker_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.4.3/tests/create_sageworks_objs_for_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:29:22.025891 sageworks-0.1.4.3/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.4.3/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.4.3/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.4.3/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.4.3/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.4.3/tests/transforms/pandas_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      729 2023-04-13 21:22:54.000000 sageworks-0.1.4.3/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.836481 sageworks-0.1.5.0/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.813758 sageworks-0.1.5.0/.github/
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.0/.github/dependabot.yml
+-rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.0/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.0/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.0/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-09 15:35:16.836568 sageworks-0.1.5.0/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     5231 2023-05-06 21:24:25.000000 sageworks-0.1.5.0/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.0/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.808909 sageworks-0.1.5.0/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.813867 sageworks-0.1.5.0/applications/aws_dashboard/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.814077 sageworks-0.1.5.0/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12244 2023-04-30 02:31:13.000000 sageworks-0.1.5.0/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.0/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     1081 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/aws_dashboard.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.814588 sageworks-0.1.5.0/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.815112 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/
+-rw-r--r--   0 briford    (501) staff       (20)     4530 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      937 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      984 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     1786 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/main_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4766 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/models_callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.815313 sageworks-0.1.5.0/applications/aws_dashboard/pages/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     2372 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)     1434 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     1535 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/feature_sets.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.815828 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/
+-rw-r--r--   0 briford    (501) staff       (20)     1458 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/data_sources_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/endpoints_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/feature_sets_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/main_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2436 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/models_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2124 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/main.py
+-rw-r--r--   0 briford    (501) staff       (20)     2556 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.816123 sageworks-0.1.5.0/applications/hello_world/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/hello_world/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2158 2023-05-01 19:48:59.000000 sageworks-0.1.5.0/applications/hello_world/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/hello_world/layout.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.816454 sageworks-0.1.5.0/applications/model_viewer/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/model_viewer/callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.816647 sageworks-0.1.5.0/applications/model_viewer/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.0/applications/model_viewer/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.0/applications/model_viewer/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/model_viewer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2525 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/model_viewer/model_viewer.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.817055 sageworks-0.1.5.0/applications/web_admin/
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/web_admin/flask_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.0/applications/web_admin/hello-world-http-test.ini
+-rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.0/applications/web_admin/hello-world.ini
+-rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.0/applications/web_admin/hello-world.service
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.817161 sageworks-0.1.5.0/applications/web_admin/nginx_conf/
+-rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.0/applications/web_admin/nginx_conf/nginx.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.817364 sageworks-0.1.5.0/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     4013 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818053 sageworks-0.1.5.0/aws_setup/sageworks_cdk/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818242 sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818339 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818500 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818615 sageworks-0.1.5.0/config/
+-rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.0/config/sageworks_config.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.819018 sageworks-0.1.5.0/data/
+-rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.0/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)      829 2023-05-02 22:39:27.000000 sageworks-0.1.5.0/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.0/data/test_data.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.819306 sageworks-0.1.5.0/docs/
+-rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.5.0/docs/admin_notes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.821205 sageworks-0.1.5.0/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.0/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.0/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.0/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.0/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.0/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.0/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.0/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.0/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.0/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.0/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.0/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.0/docs/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.0/docs/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.821506 sageworks-0.1.5.0/examples/
+-rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/examples/data_to_data_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.821605 sageworks-0.1.5.0/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.0/notebooks/ML_Pipeline_with_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.822904 sageworks-0.1.5.0/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.0/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.0/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.0/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.0/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.0/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.0/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.5.0/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.823290 sageworks-0.1.5.0/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/scripts/data_source_tags.py
+-rw-r--r--   0 briford    (501) staff       (20)     1717 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/scripts/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/scripts/list_data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-09 15:35:16.837009 sageworks-0.1.5.0/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1787 2023-05-09 15:35:04.000000 sageworks-0.1.5.0/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.809909 sageworks-0.1.5.0/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.823403 sageworks-0.1.5.0/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.0/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824047 sageworks-0.1.5.0/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.810141 sageworks-0.1.5.0/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824136 sageworks-0.1.5.0/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.0/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824238 sageworks-0.1.5.0/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.0/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.810304 sageworks-0.1.5.0/src/sageworks/algorithms/table/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824339 sageworks-0.1.5.0/src/sageworks/algorithms/table/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824752 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/
+-rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825051 sageworks-0.1.5.0/src/sageworks/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.0/src/sageworks/artifacts/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.0/src/sageworks/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5749 2023-05-05 18:17:33.000000 sageworks-0.1.5.0/src/sageworks/artifacts/artifact.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825459 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    12779 2023-05-07 17:34:22.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2943 2023-05-05 22:50:09.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2023-05-06 16:00:13.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source_abstract.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825675 sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9820 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825891 sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    12888 2023-05-07 17:34:22.000000 sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/feature_set.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.826112 sageworks-0.1.5.0/src/sageworks/artifacts/models/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/models/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4328 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/src/sageworks/artifacts/models/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.826350 sageworks-0.1.5.0/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     7633 2023-05-04 14:48:56.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)     7911 2023-05-07 17:26:56.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.827459 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4187 2023-04-30 18:15:05.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     1512 2023-04-19 17:04:31.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     2589 2023-04-30 02:50:10.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.827820 sageworks-0.1.5.0/src/sageworks/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.0/src/sageworks/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.810953 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.827955 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)     7367 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828348 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828475 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828581 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828695 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828825 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829126 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2047 2023-04-19 22:49:17.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2346 2023-04-19 21:48:41.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829256 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829447 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5843 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829554 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829659 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829968 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2591 2023-05-05 22:47:42.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     3000 2023-04-18 02:49:29.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830094 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.811754 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830200 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830308 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830497 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7866 2023-04-19 18:49:44.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830713 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830920 sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.831513 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     7029 2023-05-05 21:05:21.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    10898 2023-05-05 22:58:13.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-19 22:02:24.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6568 2023-05-07 17:39:34.000000 sageworks-0.1.5.0/src/sageworks/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.832765 sageworks-0.1.5.0/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.0/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.0/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.5.0/src/sageworks/utils/iso_8601.py
+-rw-r--r--   0 briford    (501) staff       (20)     6532 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_config.py
+-rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_sqs.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.833445 sageworks-0.1.5.0/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     9387 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/views/artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.0/src/sageworks/views/view.py
+-rw-r--r--   0 briford    (501) staff       (20)    12447 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/views/web_artifacts_summary.py
+-rw-r--r--   0 briford    (501) staff       (20)     7030 2023-05-06 16:08:21.000000 sageworks-0.1.5.0/src/sageworks/views/web_data_source_view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.834863 sageworks-0.1.5.0/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1304 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/web_components/box_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.5.0/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/web_components/feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/web_components/feature_importance.py
+-rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.0/src/sageworks/web_components/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.5.0/src/sageworks/web_components/model_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/web_components/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2023-05-07 21:37:50.000000 sageworks-0.1.5.0/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1944 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/web_components/violin_plot.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.823946 sageworks-0.1.5.0/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     8767 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.834985 sageworks-0.1.5.0/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.835492 sageworks-0.1.5.0/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1159 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.0/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1075 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.835753 sageworks-0.1.5.0/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.0/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.0/tests/aws_account/aws_service_broker_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.0/tests/create_sageworks_objs_for_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.836338 sageworks-0.1.5.0/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.5.0/tests/transforms/pandas_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.0/tox.ini
```

### Comparing `sageworks-0.1.4.3/.gitignore` & `sageworks-0.1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/LICENSE` & `sageworks-0.1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/Makefile` & `sageworks-0.1.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/PKG-INFO` & `sageworks-0.1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.4.3
+Version: 0.1.5.0
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
+<img height="360" align="left" src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png">
+<img height="360" aligh="right" src="https://user-images.githubusercontent.com/4806709/236641581-51777977-bca4-4af3-8bec-fb1758c964b8.png">
+
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
 <img src="docs/images/sageworks_concepts.png">
 
 ### Full SageWorks OverView
```

### Comparing `sageworks-0.1.4.3/Readme.md` & `sageworks-0.1.5.0/Readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
+<img height="360" align="left" src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png">
+<img height="360" aligh="right" src="https://user-images.githubusercontent.com/4806709/236641581-51777977-bca4-4af3-8bec-fb1758c964b8.png">
+
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
 <img src="docs/images/sageworks_concepts.png">
 
 ### Full SageWorks OverView
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/assets/custom.css` & `sageworks-0.1.5.0/applications/aws_dashboard/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/aws_dashboard.py` & `sageworks-0.1.5.0/applications/aws_dashboard/aws_dashboard.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 # Note: The 'app' and 'server' objects need to be at the top level since NGINX/uWSGI needs to
 #       import this file and use the server object as an ^entry-point^ into the Dash Application Code
 
 # Create our Dash Application
 # app = Dash(title='SageWorks: Artifacts', external_stylesheets=[dbc.themes.BOOTSTRAP], use_pages=True)
 # app = Dash(title="SageWorks: Artifacts", use_pages=True)
-app = Dash(title="SageWorks: Artifacts", external_stylesheets=[dbc.themes.DARKLY], use_pages=True)
+app = Dash(
+    title="SageWorks: Artifacts",
+    external_stylesheets=[dbc.themes.DARKLY],
+    use_pages=True,
+)
 server = app.server
 
 # For Multi-Page Applications, we need to create a 'page container' to hold all the pages
 app.layout = dash.page_container
 
 
 if __name__ == "__main__":
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 """FeatureSets Callbacks: Callback within the DataSources Web User Interface"""
 from datetime import datetime
 import dash
 from dash import Dash
-from dash.dependencies import Input, Output, State
+from dash.dependencies import Input, Output
 
 # SageWorks Imports
 from sageworks.views.web_data_source_view import WebDataSourceView
 from sageworks.web_components import violin_plot
 
+# Cheese Sauce
+data_source_rows = WebDataSourceView().data_sources_summary()
+data_source_rows["id"] = data_source_rows.index
 
-def update_last_updated(app: Dash):
+"""
+def refresh_timer(app: Dash):
     @app.callback(Output("last-updated-data-sources", "children"), Input("data-sources-updater", "n_intervals"))
-    def time_updated(n):
+    def time_updated(_n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
+"""
 
 
-def update_data_sources_summary(app: Dash, web_data_source_view: WebDataSourceView):
+def refresh_data_broker(app: Dash, data_source_broker: WebDataSourceView):
     @app.callback(
-        [Output("data_sources_summary", "data"), Output("data_sources_summary", "selected_rows")],
+        Output("last-updated-data-sources", "children"),
         Input("data-sources-updater", "n_intervals"),
-        State("data_sources_summary", "selected_rows")
     )
-    def data_sources_update(n, selected_rows):
-        print("Calling DataSources Summary Refresh...")
-        web_data_source_view.refresh()
-        data_sources = web_data_source_view.data_sources_summary()
-        return [data_sources.to_dict("records"), selected_rows]
+    def time_updated(_n):
+        global data_source_rows
+        data_source_broker.refresh()
+        data_source_rows = data_source_broker.data_sources_summary()
+        data_source_rows["id"] = data_source_rows.index
+        print(data_source_rows)
+        return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
+
+
+def update_data_sources_table(app: Dash):
+    @app.callback(
+        Output("data_sources_table", "data"),
+        Input("data-sources-updater", "n_intervals"),
+        prevent_initial_call=True,
+    )
+    def data_sources_update(_n):
+        """Return the table data as a dictionary"""
+        global data_source_rows
+        return data_source_rows.to_dict("records")
 
 
 # Highlights the selected row in the table
 def table_row_select(app: Dash, table_name: str):
     @app.callback(
         Output(table_name, "style_data_conditional"),
         Input(table_name, "derived_viewport_selected_row_ids"),
@@ -47,28 +65,30 @@
         ]
         return row_style
 
 
 def update_sample_rows_header(app: Dash):
     @app.callback(
         Output("sample_rows_header", "children"),
-        Input("data_sources_summary", "derived_viewport_selected_row_ids"),
-        prevent_initial_call=True
+        Input("data_sources_table", "derived_viewport_selected_row_ids"),
+        prevent_initial_call=True,
     )
     def update_sample_header(selected_rows):
         return "Sampled Rows: Updating..."
 
 
 def update_data_source_sample_rows(app: Dash, web_data_source_view: WebDataSourceView):
     @app.callback(
-        [Output("sample_rows_header", "children", allow_duplicate=True),
-         Output("data_source_sample_rows", "columns"),
-         Output("data_source_sample_rows", "data")],
-        Input("data_sources_summary", "derived_viewport_selected_row_ids"),
-        prevent_initial_call=True
+        [
+            Output("sample_rows_header", "children", allow_duplicate=True),
+            Output("data_source_sample_rows", "columns"),
+            Output("data_source_sample_rows", "data"),
+        ],
+        Input("data_sources_table", "derived_viewport_selected_row_ids"),
+        prevent_initial_call=True,
     )
     def sample_rows_update(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling DataSource Sample Rows Refresh...")
         sample_rows = web_data_source_view.data_source_sample(selected_rows[0])
@@ -82,19 +102,20 @@
 
         # Return the columns and the data
         return [header, column_setup, sample_rows.to_dict("records")]
 
 
 def update_violin_plots(app: Dash, web_data_source_view: WebDataSourceView):
     """Updates the Violin Plots when a new data source is selected"""
+
     @app.callback(
         Output("violin_plot", "figure"),
-        Input("data_sources_summary", "derived_viewport_selected_row_ids"),
-        prevent_initial_call=True
+        Input("data_sources_table", "derived_viewport_selected_row_ids"),
+        prevent_initial_call=True,
     )
     def generate_new_violin_plot(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling DataSource Sample Rows Refresh...")
-        sample_rows = web_data_source_view.data_source_sample(selected_rows[0])
-        return violin_plot.create_figure(sample_rows)
+        smart_sample_rows = web_data_source_view.data_source_smart_sample(selected_rows[0])
+        return violin_plot.create_figure(smart_sample_rows)
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
 from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 
 def update_last_updated(app: Dash):
-    @app.callback(Output("last-updated-endpoints", "children"), Input("endpoints-updater", "n_intervals"))
+    @app.callback(
+        Output("last-updated-endpoints", "children"),
+        Input("endpoints-updater", "n_intervals"),
+    )
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_endpoints_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
     @app.callback(Output("ENDPOINTS_DETAILS", "data"), Input("endpoints-updater", "n_intervals"))
     def data_sources_update(n):
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
 from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 
 def update_last_updated(app: Dash):
-    @app.callback(Output("last-updated-feature-sets", "children"), Input("feature-sets-updater", "n_intervals"))
+    @app.callback(
+        Output("last-updated-feature-sets", "children"),
+        Input("feature-sets-updater", "n_intervals"),
+    )
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_feature_sets_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
-    @app.callback(Output("FEATURE_SETS_DETAILS", "data"), Input("feature-sets-updater", "n_intervals"))
+    @app.callback(
+        Output("FEATURE_SETS_DETAILS", "data"),
+        Input("feature-sets-updater", "n_intervals"),
+    )
     def data_sources_update(n):
         print("Calling FeatureSets Refresh...")
         sageworks_artifacts.refresh()
         feature_sets = sageworks_artifacts.feature_sets_summary()
         return feature_sets.to_dict("records")
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/main_callbacks.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/main_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/callbacks/models_callbacks.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/models_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,28 @@
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 from datetime import datetime
 
 # SageWorks Imports
 from sageworks.web_components.model_data import ModelData
-from sageworks.web_components import feature_importance, confusion_matrix, model_details, feature_details
+from sageworks.web_components import (
+    feature_importance,
+    confusion_matrix,
+    model_details,
+    feature_details,
+)
 from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 
 def update_last_updated(app: Dash):
-    @app.callback(Output("last-updated-models", "children"), Input("models-updater", "n_intervals"))
+    @app.callback(
+        Output("last-updated-models", "children"),
+        Input("models-updater", "n_intervals"),
+    )
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_models_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
     @app.callback(Output("models_table", "data"), Input("models-updater", "n_intervals"))
     def data_sources_update(n):
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/data/toy_data.csv` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/data/toy_scores.json` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/data_sources.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/data_sources.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,56 +17,57 @@
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Put the components into 'dark' mode
 load_figure_template("darkly")
 
 # Grab a view that gives us a summary of the DataSources in SageWorks
-web_data_source_view = WebDataSourceView()
-summary_data = web_data_source_view.data_sources_summary()
+data_source_broker = WebDataSourceView()
+data_source_rows = data_source_broker.data_sources_summary()
 
 # Create a table to display the data sources
-data_sources_summary = table.create(
-    "data_sources_summary",
-    summary_data,
+data_sources_table = table.create(
+    "data_sources_table",
+    data_source_rows,
     header_color="rgb(100, 60, 60)",
     row_select="single",
     markdown_columns=["Name"],
 )
 
-# Grab the a sample of rows from the first data source
-sample_rows = web_data_source_view.data_source_sample(0)
+# Grab a sample of rows from the first data source
+sample_rows = data_source_broker.data_source_sample(0)
 data_source_sample_rows = table.create(
     "data_source_sample_rows",
     sample_rows,
     header_color="rgb(60, 60, 100)",
     max_height="200px",
-    fixed_headers=True
 )
 
 # Create a box plot of all the numeric columns in the sample rows
-# histo = histogram.create()
-violin = violin_plot.create(sample_rows)
+smart_sample_rows = data_source_broker.data_source_smart_sample(0)
+violin = violin_plot.create(smart_sample_rows)
 
 # Create our components
 components = {
-    "data_sources_summary": data_sources_summary,
+    "data_sources_table": data_sources_table,
     "data_source_sample_rows": data_source_sample_rows,
-    "violin_plot": violin
+    "violin_plot": violin,
 }
 
 # Setup our callbacks/connections
 app = dash.get_app()
-callbacks.update_last_updated(app)
+
+# Refresh our timer and data sources broker
+# callbacks.refresh_timer(app)
+callbacks.refresh_data_broker(app, data_source_broker)
 
 # Periodic update to the data sources summary
-# FIXME: This causes issues with the table selections
-# callbacks.update_data_sources_summary(app, web_data_source_view)
+callbacks.update_data_sources_table(app)
 
 # Callbacks for when a data source is selected
-callbacks.table_row_select(app, "data_sources_summary")
+callbacks.table_row_select(app, "data_sources_table")
 callbacks.update_sample_rows_header(app)
-callbacks.update_data_source_sample_rows(app, web_data_source_view)
-callbacks.update_violin_plots(app, web_data_source_view)
+callbacks.update_data_source_sample_rows(app, data_source_broker)
+callbacks.update_violin_plots(app, data_source_broker)
 
 # Set up our layout (Dash looks for a var called layout)
 layout = data_sources_layout(components)
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/endpoints.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
     markdown_columns=["Name"],
 )
 
 # Create a fake scatter plot
 endpoint_traffic = line_chart.create()
 
 # Create our components
-components = {"endpoints_details": endpoints_table, "endpoint_traffic": endpoint_traffic}
+components = {
+    "endpoints_details": endpoints_table,
+    "endpoint_traffic": endpoint_traffic,
+}
 
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_last_updated(app)
 callbacks.update_endpoints_table(app, sageworks_artifacts)
 
 # Set up our layout (Dash looks for a var called layout)
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/feature_sets.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/feature_sets.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,19 @@
 )
 
 # Create a fake scatter plot
 scatter1 = scatter_plot.create()
 scatter2 = scatter_plot.create(variant=2)
 
 # Create our components
-components = {"feature_sets_details": feature_sets_table, "scatter1": scatter1, "scatter2": scatter2}
+components = {
+    "feature_sets_details": feature_sets_table,
+    "scatter1": scatter1,
+    "scatter2": scatter2,
+}
 
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_last_updated(app)
 callbacks.update_feature_sets_table(app, sageworks_artifacts)
 
 # Set up our layout (Dash looks for a var called layout)
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/data_sources_layout.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/data_sources_layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,22 @@
                             "fontSize": 15,
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
-            dbc.Row(components["data_sources_summary"]),
-            dbc.Row(html.H3("Sampled Rows", id="sample_rows_header"), style={"padding": "30px 0px 10px 0px"}),
-            dbc.Row(components["data_source_sample_rows"], style={"padding": "0px 0px 30px 0px"}),
+            dbc.Row(components["data_sources_table"]),
+            dbc.Row(
+                html.H3("Sampled Rows", id="sample_rows_header"),
+                style={"padding": "30px 0px 10px 0px"},
+            ),
+            dbc.Row(
+                components["data_source_sample_rows"],
+                style={"padding": "0px 0px 30px 0px"},
+            ),
             dbc.Row(components["violin_plot"]),
             dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
         ],
         style={"margin": "30px"},
     )
     return layout
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/endpoints_layout.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/endpoints_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/feature_sets_layout.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/feature_sets_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/main_layout.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/main_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/layout/models_layout.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/models_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,18 @@
                             dbc.Row(components["feature_importance"]),
                             dbc.Row(
                                 html.H3(
                                     "Feature Details",
                                     style={"padding": "20px 0px 0px 20px"},
                                 )
                             ),
-                            dbc.Row(components["feature_details"], style={"padding": "0px 0px 0px 20px"}),
+                            dbc.Row(
+                                components["feature_details"],
+                                style={"padding": "0px 0px 0px 20px"},
+                            ),
                         ],
                         width=4,
                     ),
                 ]
             ),
             dcc.Interval(id="models-updater", interval=5000, n_intervals=0),
         ],
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/main.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 tables["MODELS"] = table.create(
     "MODELS",
     sageworks_artifacts["MODELS"],
     header_color="rgb(60, 100, 60)",
     markdown_columns=["Model Group"],
 )
 tables["ENDPOINTS"] = table.create(
-    "ENDPOINTS", sageworks_artifacts["ENDPOINTS"], header_color="rgb(100, 60, 100)", markdown_columns=["Name"]
+    "ENDPOINTS",
+    sageworks_artifacts["ENDPOINTS"],
+    header_color="rgb(100, 60, 100)",
+    markdown_columns=["Name"],
 )
 
 # Create our components
 components = {
     "incoming_data": tables["INCOMING_DATA"],
     "data_sources": tables["DATA_SOURCES"],
     "feature_sets": tables["FEATURE_SETS"],
```

### Comparing `sageworks-0.1.4.3/applications/aws_dashboard/pages/models.py` & `sageworks-0.1.5.0/applications/aws_dashboard/pages/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 import dash
 from dash_bootstrap_templates import load_figure_template
 
 
 # SageWorks Imports
 
 from sageworks.web_components import confusion_matrix, table, scatter_plot
-from sageworks.web_components import feature_importance, model_data, model_details, feature_details
+from sageworks.web_components import (
+    feature_importance,
+    model_data,
+    model_details,
+    feature_details,
+)
 from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 # Local Imports
 from pages.layout.models_layout import models_layout
 import pages.callbacks.models_callbacks as callbacks
 
 register_page(__name__, path="/models")
```

### Comparing `sageworks-0.1.4.3/applications/hello_world/callbacks.py` & `sageworks-0.1.5.0/applications/hello_world/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/hello_world/hello_world.py` & `sageworks-0.1.5.0/applications/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/hello_world/layout.py` & `sageworks-0.1.5.0/applications/hello_world/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/model_viewer/callbacks.py` & `sageworks-0.1.5.0/applications/model_viewer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/model_viewer/data/toy_data.csv` & `sageworks-0.1.5.0/applications/model_viewer/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/model_viewer/data/toy_scores.json` & `sageworks-0.1.5.0/applications/model_viewer/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/model_viewer/layout.py` & `sageworks-0.1.5.0/applications/model_viewer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/applications/model_viewer/model_viewer.py` & `sageworks-0.1.5.0/applications/model_viewer/model_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     # Read in our model data
     data_path = os.path.join(os.path.dirname(__file__), "data/toy_data.csv")
     model_info = model_data.ModelData(data_path)
 
     # Create our components
     model_df = model_info.get_model_df()
     model_table = table.create(
-        "model_table", model_df, show_columns=["model_name", "date_created", "f_scores"], row_select="single"
+        "model_table",
+        model_df,
+        show_columns=["model_name", "date_created", "f_scores"],
+        row_select="single",
     )
     details = model_details.create(model_info.get_model_details(0))
     c_matrix = confusion_matrix.create(model_info.get_model_confusion_matrix(0))
     scatter = scatter_plot.create(model_df)
     my_feature_importance = feature_importance.create(model_info.get_model_feature_importance(0))
     my_feature_details = feature_details.create(model_info.get_model_feature_importance(0))
     components = {
```

### Comparing `sageworks-0.1.4.3/aws_setup/aws_account_check.py` & `sageworks-0.1.5.0/aws_setup/aws_account_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,34 +30,34 @@
         self.log.info("*** AWS SageWorks Bucket Check ***")
         s3 = self.aws_clamp.boto_session().resource("s3")
         bucket_name = self.config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
         bucket = s3.Bucket(bucket_name)
 
         # Check if the bucket exists
         if bucket.creation_date is None:
-            self.log.critical(f'The {bucket_name} bucket does not exist')
+            self.log.critical(f"The {bucket_name} bucket does not exist")
             sys.exit(1)
         else:
-            self.log.info(f'The {bucket_name} bucket exists')
+            self.log.info(f"The {bucket_name} bucket exists")
 
         # Check if the sub-folders exists
         sub_folders = ["incoming-data", "data-sources", "feature-sets", "athena-queries"]
 
         # Get all object prefixes in the bucket
         prefixes = set()
         for obj in bucket.objects.all():
-            prefix = obj.key.split('/')[0]
+            prefix = obj.key.split("/")[0]
             prefixes.add(prefix)
 
         # Check for the existence of the sub-folders
         for folder in sub_folders:
             if folder in prefixes:
-                self.log.info(f'The {folder} prefix exists')
+                self.log.info(f"The {folder} prefix exists")
             else:
-                self.log.info(f'The {folder} prefix does not exist...which is fine...')
+                self.log.info(f"The {folder} prefix does not exist...which is fine...")
 
     def check(self):
         """Check if the AWS Account is Setup Correctly"""
         self.log.info("*** AWS Identity Check ***")
         self.aws_clamp.check_aws_identity()
         self.log.info("Identity Check Success...")
```

### Comparing `sageworks-0.1.4.3/aws_setup/aws_account_check_deep.py` & `sageworks-0.1.5.0/aws_setup/build_ml_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 def redis_check():
     """Check if the Redis Database is available"""
     print("*** Redis Database Check ***")
     try:
         from sageworks.utils.redis_cache import RedisCache
+
         RedisCache(prefix="test")
         print("Redis Database Check Success...")
     except RuntimeError as err:
         print(f"Redis Database Check Failed: {err} but this is fine.. Redis is optional")
 
 
 if __name__ == "__main__":
@@ -50,23 +51,23 @@
 
     # Create the test_data DataSource
     if not DataSource("test_data").check():
         my_loader = CSVToDataSource(test_data_path, "test_data")
         my_loader.set_output_tags("test:small")
         my_loader.transform()
         print("Waiting for the test_data to be created...")
-        time.sleep(5)
+        time.sleep(10)
 
     # Create the abalone_data DataSource
     if not DataSource("abalone_data").check():
         my_loader = CSVToDataSource(abalone_data_path, "abalone_data")
         my_loader.set_output_tags("abalone:public")
         my_loader.transform()
         print("Waiting for the abalone_data to be created...")
-        time.sleep(5)
+        time.sleep(10)
 
     # Create the test_feature_set FeatureSet
     if not FeatureSet("test_feature_set").check():
         data_to_features = DataToFeaturesLight("test_data", "test_feature_set")
         data_to_features.set_output_tags(["test", "small"])
         data_to_features.transform(id_column="id", event_time_column="date")
 
@@ -80,14 +81,14 @@
 
     # Create the abalone_regression Model
     if not Model("abalone-regression").check():
         features_to_model = FeaturesToModel("abalone_feature_set", "abalone-regression")
         features_to_model.set_output_tags(["abalone", "regression"])
         features_to_model.transform(target="class_number_of_rings", description="Abalone Regression Model")
         print("Waiting for the Model to be created...")
-        time.sleep(10)
+        time.sleep(30)
 
     # Create the abalone_regression Endpoint
     if not Endpoint("abalone-regression-end").check():
         model_to_endpoint = ModelToEndpoint("abalone-regression", "abalone-regression-end")
         model_to_endpoint.set_output_tags(["abalone", "regression"])
         model_to_endpoint.transform()
```

### Comparing `sageworks-0.1.4.3/aws_setup/sageworks_cdk/README.md` & `sageworks-0.1.5.0/aws_setup/sageworks_cdk/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/aws_setup/sageworks_cdk/app.py` & `sageworks-0.1.5.0/aws_setup/sageworks_cdk/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/aws_setup/sageworks_cdk/cdk.json` & `sageworks-0.1.5.0/aws_setup/sageworks_cdk/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/aws_setup/sageworks_cdk/stacks/sageworks_stack.py` & `sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/sageworks_stack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-from aws_cdk import (
-    Stack,
-    aws_iam as iam,
-    aws_s3 as s3,
-    aws_glue_alpha as glue
-)
+from aws_cdk import Stack, aws_iam as iam, aws_s3 as s3, aws_glue_alpha as glue
 from constructs import Construct
 
 
 class SageworksStack(Stack):
     def __init__(
         self,
         scope: Construct,
@@ -18,39 +13,37 @@
     ) -> None:
         super().__init__(scope, construct_id, **kwargs)
 
         # Create the SageWorks Artifact Bucket (must be created before Roles)
         self.artifact_bucket = self.add_artifact_bucket(s3_bucket_name)
 
         # Create our main SageWorks Execution Role and the Glue Service Role
-        self.sageworks_execution_role = self.create_execution_role(sageworks_role_name)
-        self.glue_service_role = self.create_execution_role("AWSGlueServiceRole-Sageworks")
+        self.sageworks_execution_role = self.create_execution_role(sageworks_role_name, iam.AnyPrincipal())
+        self.glue_service_role = self.create_execution_role(
+            "AWSGlueServiceRole-Sageworks", iam.ServicePrincipal("glue.amazonaws.com")
+        )
 
         # Create the SageWorks Data Catalog Databases
         self.create_data_catalog_databases()
 
     def add_artifact_bucket(self, bucket_name) -> s3.Bucket:
         return s3.Bucket(
             self,
             id=bucket_name,
             bucket_name=bucket_name,
         )
 
-    def create_execution_role(self, role_name) -> iam.Role:
+    def create_execution_role(self, role_name, assumed_by) -> iam.Role:
         execution_role = iam.Role(
             self,
             id=role_name,
-            assumed_by=iam.AnyPrincipal(),
+            assumed_by=assumed_by,
             managed_policies=[
-                iam.ManagedPolicy.from_aws_managed_policy_name(
-                    "service-role/AWSGlueServiceRole"
-                ),
-                iam.ManagedPolicy.from_aws_managed_policy_name(
-                    "AmazonSageMakerFullAccess"
-                ),
+                iam.ManagedPolicy.from_aws_managed_policy_name("service-role/AWSGlueServiceRole"),
+                iam.ManagedPolicy.from_aws_managed_policy_name("AmazonSageMakerFullAccess"),
             ],
             role_name=role_name,
         )
         execution_role.add_to_policy(
             iam.PolicyStatement(
                 actions=["s3:*", "s3-object-lambda:*"],
                 resources=[
@@ -59,17 +52,9 @@
                 ],
             )
         )
         return execution_role
 
     def create_data_catalog_databases(self) -> None:
         # Create two Data Catalog Databases (sageworks and sagemaker_featurestore)
-        glue.Database(
-            self,
-            id="sageworks_database",
-            database_name="sageworks"
-        )
-        glue.Database(
-            self,
-            id="sagemaker_featurestore_database",
-            database_name="sagemaker_featurestore"
-        )
+        glue.Database(self, id="sageworks_database", database_name="sageworks")
+        glue.Database(self, id="sagemaker_featurestore_database", database_name="sagemaker_featurestore")
```

### Comparing `sageworks-0.1.4.3/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/data/abalone.csv` & `sageworks-0.1.5.0/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/data/test_data.json` & `sageworks-0.1.5.0/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/admin_notes.md` & `sageworks-0.1.5.0/docs/admin_notes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/big_spider.png` & `sageworks-0.1.5.0/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/graph_representation.png` & `sageworks-0.1.5.0/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/powered_aws_dark_blue.png` & `sageworks-0.1.5.0/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/powered_aws_transparent.png` & `sageworks-0.1.5.0/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/powered_aws_white.png` & `sageworks-0.1.5.0/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.1.5.0/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/sageworks.png` & `sageworks-0.1.5.0/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/sageworks_concepts.png` & `sageworks-0.1.5.0/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/scp.png` & `sageworks-0.1.5.0/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/scp_labs.png` & `sageworks-0.1.5.0/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/images/small_spider.png` & `sageworks-0.1.5.0/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/sageworks_classes_concepts.md` & `sageworks-0.1.5.0/docs/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/docs/scp_consulting.md` & `sageworks-0.1.5.0/docs/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/examples/data_to_data_example.py` & `sageworks-0.1.5.0/examples/data_to_data_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.1.5.0/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999043924825175%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'<div style="float: right; padding: 20px"><img '*

 * *            'width="350" '*

 * *            'src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png"></div>\\n\')], '*

 * *            'delete: [0]}}, 35: {\'source\': {insert: [(2, \'<div style="float: right; padding: '*

 * *            '20px"><img width="350" '*

 * *            'src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "5aa74260",
             "metadata": {},
             "source": [
-                "<div style=\"float: right; padding: 20px\"><img src=\"images/scp_labs.png\" width=300px\"></div>\n",
+                "<div style=\"float: right; padding: 20px\"><img width=\"350\" src=\"https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png\"></div>\n",
                 "\n",
                 "# Building an AWS<sup>\u00ae</sup> ML Pipeline with SageWorks\n",
                 "\n",
                 "This notebook uses the SageWorks Science Workbench to quickly build an AWS\u00ae Machine Learning Pipeline with the AQSolDB public dataset. This dataset aggregates aqueous solubility data for a large set of compounds.\n",
                 "\n",
                 "We're going to set up a full AWS Machine Learning Pipeline from start to finish. Since the SageWorks Classes encapsulate, organize, and manage sets of AWS\u00ae Services, setting up our ML pipeline will be straight forward.\n",
                 "\n",
@@ -1210,15 +1210,15 @@
         {
             "cell_type": "markdown",
             "id": "2358b668",
             "metadata": {},
             "source": [
                 "# Wrap up: Building an AWS<sup>\u00ae</sup> ML Pipeline with SageWorks\n",
                 "\n",
-                "<div style=\"float: right; padding: 20px\"><img src=\"images/scp_labs.png\" width=300px\"></div>\n",
+                "<div style=\"float: right; padding: 20px\"><img width=\"350\" src=\"https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png\"></div>\n",
                 "\n",
                 "This notebook used the SageWorks Science Toolkit to quickly build an AWS\u00ae Machine Learning Pipeline with the AQSolDB public dataset. We built a full AWS Machine Learning Pipeline from start to finish. \n",
                 "\n",
                 "SageWorks made it easy:\n",
                 "- Visibility into AWS services for every step of the process.\n",
                 "- Managed the complexity of organizing the data and populating the AWS services.\n",
                 "- Provided an easy to use API to perform Transformations and inspect Artifacts.\n",
```

### Comparing `sageworks-0.1.4.3/notebooks/images/athena_query_aqsol.png` & `sageworks-0.1.5.0/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.1.5.0/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.1.5.0/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/notebooks/images/model_screenshot.png` & `sageworks-0.1.5.0/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/notebooks/images/sageworks_concepts.png` & `sageworks-0.1.5.0/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/notebooks/images/scp_labs.png` & `sageworks-0.1.5.0/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/scripts/data_source_tags.py` & `sageworks-0.1.5.0/scripts/data_source_tags.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/scripts/generate_jsonl_data.py` & `sageworks-0.1.5.0/scripts/generate_jsonl_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Define a function to generate random data
 def generate_data():
     return {
         "id": "".join(random.choices(string.ascii_letters + string.digits, k=8)),
         "name": "".join(random.choices(string.ascii_letters, k=10)),
         "age": random.randint(18, 65),
         "address": "".join(random.choices(string.ascii_letters + string.digits + ", .", k=20)),
-        "date": datetime_to_iso8601(datetime.now(timezone.utc))
+        "date": datetime_to_iso8601(datetime.now(timezone.utc)),
     }
 
 
 # Loop through and generate the files
 for i in range(num_files):
     # Set up the file name
     filename = f"data_{i}.jsonl"
```

### Comparing `sageworks-0.1.4.3/scripts/list_data_sources.py` & `sageworks-0.1.5.0/scripts/list_data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/setup.cfg` & `sageworks-0.1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/setup.py` & `sageworks-0.1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Simple directory walker"""
     return [(os.path.join(".", d), [os.path.join(d, f) for f in files]) for d, _, files in os.walk(dir_name)]
 
 
 setup(
     name="sageworks",
     # use_scm_version=True,
-    version="0.1.4.3",
+    version="0.1.5.0",
     description="SageWorks: A Python WorkBench for creating and deploying SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
     packages=find_packages("src"),
@@ -36,15 +36,15 @@
         "sagemaker >= 2.143",
         "pandas",
         "scikit-learn",
         "redis",
         "dash",
         "dash-bootstrap-components",
         "dash-bootstrap-templates",
-        "termcolor"
+        "termcolor",
     ],
     license="MIT",
     keywords="SageMaker, Machine Learning, AWS, Python, Utilities",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
```

### Comparing `sageworks-0.1.4.3/src/sageworks/__init__.py` & `sageworks-0.1.5.0/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/algorithms/table/light/data_source_eda.py` & `sageworks-0.1.5.0/src/sageworks/algorithms/table/light/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/algorithms/table/light/feature_spider.py` & `sageworks-0.1.5.0/src/sageworks/algorithms/table/light/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/algorithms/table/light/row_tagger.py` & `sageworks-0.1.5.0/src/sageworks/algorithms/table/light/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/Readme.md` & `sageworks-0.1.5.0/src/sageworks/artifacts/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/artifact.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/artifact.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Artifact: Abstract Base Class for all Artifact classes in SageWorks.
                 Artifacts simply reflect and aggregate one or more AWS Services"""
 from abc import ABC, abstractmethod
 from datetime import datetime
 import logging
+import json
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.aws_service_broker.aws_service_broker import AWSServiceBroker
 from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
@@ -75,44 +76,48 @@
 
     @abstractmethod
     def aws_url(self):
         """AWS console/web interface for this artifact"""
         pass
 
     @abstractmethod
-    def aws_meta(self):
+    def meta(self) -> dict:
         """Get the full AWS metadata for this artifact"""
         pass
 
     @abstractmethod
     def delete(self):
         """Delete this artifact including all related AWS objects"""
         pass
 
-    def set_tags(self, tag):
-        """Set the tags for this artifact"""
-        self.log.error("set_tags: functionality needs to be added!")
-
-    @staticmethod
-    def aws_tags_to_dict(aws_tags):
-        """AWS Tags are in an odd format, so convert to regular dictionary"""
-        return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
-
-    def sageworks_meta(self):
+    def sageworks_meta(self) -> dict:
         """Get the SageWorks specific metadata for this Artifact
         Note: This functionality will work for FeatureSets, Models, and Endpoints
-        but not for DataSources. DataSources need to overwrite this method
+              but not for DataSources. DataSources need to overwrite this method
         """
         aws_arn = self.arn()
         self.log.info(f"Retrieving SageWorks Metadata for Artifact: {aws_arn}...")
         aws_tags = self.sm_session.list_tags(aws_arn)
-        meta = self.aws_tags_to_dict(aws_tags)
+        meta = self._aws_tags_to_dict(aws_tags)
         return meta
 
-    def sageworks_tags(self):
+    def upsert_sageworks_meta(self, new_meta: dict):
+        """Add SageWorks specific metadata to this Artifact
+        Args:
+            new_meta (dict): Dictionary of new metadata to add
+        Note:
+            This functionality will work for FeatureSets, Models, and Endpoints
+            but not for DataSources. DataSources need to overwrite this method
+        """
+        aws_arn = self.arn()
+        self.log.info(f"Upserting SageWorks Metadata for Artifact: {aws_arn}...")
+        aws_tags = self._dict_to_aws_tags(new_meta)
+        self.sm_session.sagemaker_client.add_tags(ResourceArn=aws_arn, Tags=aws_tags)
+
+    def sageworks_tags(self) -> list:
         """Get the tags for this artifact"""
         combined_tags = self.sageworks_meta().get("sageworks_tags", "")
         tags = combined_tags.split(":")
         return tags
 
     def summary(self) -> dict:
         """This is generic summary information for all Artifacts. If you
@@ -124,7 +129,30 @@
             "aws_url": self.aws_url(),
             "size": self.size(),
             "created": self.created(),
             "modified": self.modified(),
             "sageworks_tags": self.sageworks_tags(),
             "sageworks_meta": self.sageworks_meta(),
         }
+
+    @staticmethod
+    def _aws_tags_to_dict(aws_tags) -> dict:
+        """Internal: AWS Tags are in an odd format, so convert to regular dictionary"""
+        return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
+
+    @staticmethod
+    def _dict_to_aws_tags(meta_data: dict) -> list:
+        """Internal: AWS Tags are in an odd format, so we need to dictionary
+        Args:
+            meta_data (dict): Dictionary of metadata to convert to AWS Tags
+        """
+
+        # First convert any non-string values to JSON strings
+        for key, value in meta_data.items():
+            if not isinstance(value, str):
+                meta_data[key] = json.dumps(value)
+
+        # Now convert to AWS Tags format
+        aws_tags = []
+        for key, value in meta_data.items():
+            aws_tags.append({"Key": key, "Value": value})
+        return aws_tags
```

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/athena_source.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/athena_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """AthenaSource: SageWorks Data Source accessible through Athena"""
 import pandas as pd
 import awswrangler as wr
 from datetime import datetime
+import json
 
 # SageWorks Imports
 from sageworks.artifacts.data_sources.data_source_abstract import DataSourceAbstract
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 
 
 class AthenaSource(DataSourceAbstract):
@@ -28,27 +29,34 @@
 
         # Call superclass init
         super().__init__(data_uuid)
 
         self.data_catalog_db = database
         self.table_name = data_uuid
 
-        # Grab an AWS Metadata Broker object and pull information for Data Sources
-        self.catalog_meta = self.aws_broker.get_metadata(ServiceCategory.DATA_CATALOG)[self.data_catalog_db].get(
-            self.table_name
-        )
+        # Refresh our internal catalog metadata
+        self.catalog_table_meta = None
+        self.refresh()
 
         # All done
         print(f"AthenaSource Initialized: {self.data_catalog_db}.{self.table_name}")
 
+    def refresh(self, force_fresh: bool = False):
+        """Refresh our internal catalog metadata
+        Args:
+            force_fresh (bool): Force a refresh of the metadata
+        """
+        _catalog_meta = self.aws_broker.get_metadata(ServiceCategory.DATA_CATALOG, force_fresh=force_fresh)
+        self.catalog_table_meta = _catalog_meta[self.data_catalog_db].get(self.table_name)
+
     def check(self) -> bool:
         """Validation Checks for this Data Source"""
 
         # We're we able to pull AWS Metadata for this table_name?"""
-        if self.catalog_meta is None:
+        if self.catalog_table_meta is None:
             self.log.info(f"AthenaSource.check() {self.table_name} not found in SageWorks Metadata...")
             return False
         return True
 
     def deep_check(self) -> bool:
         """These are more comprehensive checks for this Data Source (may take a LONG TIME)"""
 
@@ -66,96 +74,178 @@
         account_id = self.aws_account_clamp.account_id()
         region = self.aws_account_clamp.region()
         arn = f"arn:aws:glue:{region}:{account_id}:table/{self.data_catalog_db}/{self.table_name}"
         return arn
 
     def sageworks_meta(self):
         """Get the SageWorks specific metadata for this Artifact"""
-        params = self.catalog_meta.get("Parameters", {})
+        params = self.meta().get("Parameters", {})
         return {key: value for key, value in params.items() if "sageworks" in key}
 
+    def upsert_sageworks_meta(self, new_meta: dict):
+        """Add SageWorks specific metadata to this Artifact
+        Args:
+            new_meta (dict): Dictionary of new metadata to add
+        """
+        # Grab our existing metadata
+        meta = self.sageworks_meta()
+
+        # Make sure the new data has keys that are valid
+        for key in new_meta.keys():
+            if not key.startswith("sageworks_"):
+                new_meta[f"sageworks_{key}"] = new_meta.pop(key)
+
+        # Now convert any non-string values to JSON strings
+        for key, value in new_meta.items():
+            if not isinstance(value, str):
+                new_meta[key] = json.dumps(value)
+
+        # Update our existing metadata with the new metadata
+        meta.update(new_meta)
+
+        # Store our updated metadata
+        wr.catalog.upsert_table_parameters(
+            parameters=meta,
+            database=self.data_catalog_db,
+            table=self.table_name,
+            boto3_session=self.boto_session,
+        )
+
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         size_in_bytes = sum(wr.s3.size_objects(self.s3_storage_location(), boto3_session=self.boto_session).values())
         size_in_mb = size_in_bytes / 1_000_000
         return size_in_mb
 
-    def aws_meta(self):
-        """Get the full AWS metadata for this artifact"""
-        return self.catalog_meta
+    def meta(self) -> dict:
+        """Get the FULL AWS metadata for this artifact"""
+        return self.catalog_table_meta
 
     def aws_url(self):
         """The AWS URL for looking at/querying this data source"""
         return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
 
     def created(self) -> datetime:
         """Return the datetime when this artifact was created"""
-        return self.catalog_meta["CreateTime"]
+        return self.catalog_table_meta["CreateTime"]
 
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
-        return self.catalog_meta["UpdateTime"]
+        return self.catalog_table_meta["UpdateTime"]
 
     def num_rows(self) -> int:
         """Return the number of rows for this Data Source"""
         count_df = self.query(f'select count(*) AS count from "{self.data_catalog_db}"."{self.table_name}"')
         return count_df["count"][0]
 
     def num_columns(self) -> int:
         """Return the number of columns for this Data Source"""
         return len(self.column_names())
 
     def column_names(self) -> list[str]:
         """Return the column names for this Athena Table"""
-        return [item["Name"] for item in self.catalog_meta["StorageDescriptor"]["Columns"]]
+        return [item["Name"] for item in self.catalog_table_meta["StorageDescriptor"]["Columns"]]
 
     def column_types(self) -> list[str]:
         """Return the column types of the internal AthenaSource"""
-        return [item["Type"] for item in self.catalog_meta["StorageDescriptor"]["Columns"]]
+        return [item["Type"] for item in self.catalog_table_meta["StorageDescriptor"]["Columns"]]
 
     def query(self, query: str) -> pd.DataFrame:
         """Query the AthenaSource"""
         df = wr.athena.read_sql_query(sql=query, database=self.data_catalog_db, boto3_session=self.boto_session)
         scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
         self.log.info(f"Athena Query successful (scanned bytes: {scanned_bytes})")
         return df
 
     def s3_storage_location(self) -> str:
         """Get the S3 Storage Location for this Data Source"""
-        return self.catalog_meta["StorageDescriptor"]["Location"]
+        return self.catalog_table_meta["StorageDescriptor"]["Location"]
 
     def athena_test_query(self):
         """Validate that Athena Queries are working"""
         query = f"select count(*) as count from {self.table_name}"
         df = wr.athena.read_sql_query(sql=query, database=self.data_catalog_db, boto3_session=self.boto_session)
         scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
         self.log.info(f"Athena TEST Query successful (scanned bytes: {scanned_bytes})")
 
-    def sample_df(self, max_rows: int = 1000) -> pd.DataFrame:
+    def sample_df(self, recompute: bool = False) -> pd.DataFrame:
         """Pull a sample of rows from the DataSource
         Args:
-            max_rows (int): Maximum number of rows to pull
+            recompute(bool): Recompute the sample (default: False)
+        Returns:
+            pd.DataFrame: A sample DataFrame from this DataSource
         """
+
+        # First check if we have already computed the quartiles
+        if self.sageworks_meta().get("sageworks_sample_rows") and not recompute:
+            return pd.read_json(self.sageworks_meta()["sageworks_sample_rows"], orient="records", lines=True)
+
+        # Note: Hardcoded to 100 rows so that metadata storage is consistent
+        sample_rows = 100
         num_rows = self.num_rows()
-        if num_rows > max_rows:
-            # With Bernoulli Sampling it can give you 0 rows on small samples
-            # so we need to make sure we have at least 100 rows for the sample
-            # and then we can limit the output to max_rows
-            sample_rows = max(max_rows, 100)
-            percentage = min(100, round(sample_rows * 100.0 / num_rows))
-            self.log.warning(f"DataSource has {num_rows} rows.. sampling down to {max_rows}...")
+        if num_rows > sample_rows:
+            # Bernoulli Sampling has reasonable variance so we're going to +1 the
+            # sample percentage and then simply clamp it to 100 rows
+            percentage = round(sample_rows * 100.0 / num_rows) + 1
+            self.log.warning(f"DataSource has {num_rows} rows.. sampling down to {sample_rows}...")
             query = f"SELECT * FROM {self.table_name} TABLESAMPLE BERNOULLI({percentage})"
         else:
             query = f"SELECT * FROM {self.table_name}"
-        return self.query(query).head(max_rows)
+        sample_df = self.query(query).head(sample_rows)
+
+        # Store the sample_df in our SageWorks metadata
+        rows_json = sample_df.to_json(orient="records", lines=True)
+        self.upsert_sageworks_meta({"sageworks_sample_rows": rows_json})
+
+        # Return the sample_df
+        return sample_df
+
+    def quartiles(self, recompute=False) -> dict[dict]:
+        """Compute Quartiles for all the numeric columns in a DataSource
+        Args:
+            recompute: Recompute the quartiles (default: False)
+        Returns:
+            dict(dict): A dictionary of quartiles for each column in the form
+                 {'col1': {'min': 0, 'q1': 1, 'median': 2, 'q3': 3, 'max': 4},
+                  'col2': ...}
+        """
+
+        # First check if we have already computed the quartiles
+        if self.sageworks_meta().get("sageworks_quartiles") and not recompute:
+            return json.loads(self.sageworks_meta()["sageworks_quartiles"])
+
+        # For every column in the table that is numeric, get the quartiles
+        self.log.info("Computing Quartiles for all numeric columns (this may take a while)...")
+        quartile_data = []
+        for column, data_type in zip(self.column_names(), self.column_types()):
+            print(column, data_type)
+            if data_type in ["bigint", "double", "int", "smallint", "tinyint"]:
+                query = (
+                    f"SELECT MIN({column}) AS min, "
+                    f"approx_percentile({column}, 0.25) AS q1, "
+                    f"approx_percentile({column}, 0.5) AS median, "
+                    f"approx_percentile({column}, 0.75) AS q3, "
+                    f"MAX({column}) AS max FROM {self.table_name}"
+                )
+                result_df = self.query(query)
+                result_df["column_name"] = column
+                quartile_data.append(result_df)
+        quartile_data = pd.concat(quartile_data).set_index("column_name").to_dict(orient="index")
+
+        # Push the quartile data into our DataSource Metadata
+        self.upsert_sageworks_meta({"sageworks_quartiles": quartile_data})
+
+        # Return the quartile data
+        return quartile_data
 
     def details(self) -> dict:
         """Additional Details about this AthenaSource Artifact"""
         details = super().details()
         details["s3_storage_location"] = self.s3_storage_location()
+        details.update(self.meta())
         return details
 
     def delete(self):
         """Delete the AWS Data Catalog Table and S3 Storage Objects"""
 
         # Make sure the Feature Group exists
         if not self.check():
@@ -168,14 +258,15 @@
         # Delete S3 Storage Objects
         self.log.info(f"Deleting S3 Storage Object: {self.s3_storage_location()}...")
         wr.s3.delete_objects(self.s3_storage_location(), boto3_session=self.boto_session)
 
 
 if __name__ == "__main__":
     """Exercise the AthenaSource Class"""
+    from pprint import pprint
 
     # Retrieve a Data Source
     my_data = AthenaSource("abalone_data")
 
     # Verify that the Athena Data Source exists
     assert my_data.check()
 
@@ -197,18 +288,33 @@
     print(f"Modified: {my_data.modified()}")
 
     # Column Names and Types
     print(f"Column Names: {my_data.column_names()}")
     print(f"Column Types: {my_data.column_types()}")
 
     # Get Metadata and tags associated with this Artifact
-    print(f"Meta: {my_data.sageworks_meta()}")
+    print(f"Meta: {my_data.meta()}")
     print(f"Tags: {my_data.sageworks_tags()}")
 
     # Get a sample of the data
-    df = my_data.sample_df(10)
+    df = my_data.sample_df()
     print(f"Sample Data: {df.shape}")
     print(df)
 
+    # Get the SageWorks Metadata for this Data Source
+    meta = my_data.sageworks_meta()
+    print("SageWorks Meta")
+    pprint(meta)
+
+    # Add some SageWorks Metadata to this Data Source
+    my_data.upsert_sageworks_meta({"sageworks_tags": "abalone:public"})
+    print("SageWorks Meta NEW")
+    pprint(my_data.sageworks_meta())
+
+    # Get quartiles for all the columns
+    quartile_info = my_data.quartiles()
+    print("Quartiles")
+    pprint(quartile_info)
+
     # Now delete the AWS artifacts associated with this DataSource
     # print('Deleting SageWorks Data Source...')
     # my_data.delete()
```

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/data_source.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,16 +16,21 @@
     Methods: (implemented by subclasses)
         num_rows(): Return the number of rows for this DataSource
         num_columns(): Return the number of columns
         column_names(): Return the column names
         column_types(): Return the column types
         column_details(): Return the column details
         query(query: str): Returns a pd.DataFrame with the query results
-        sample_df(max_rows: int=1000): Returns a SAMPLED pd.DataFrame from this DataSource
+        sample_df(): Returns a SAMPLED pd.DataFrame from this DataSource
+        summary(): Returns a summary of this DataSource
         details(): Returns additional details about this DataSource
+        quartiles(): Returns the quartiles for each numeric column in this DataSource
+        meta(): Returns ALL AWS Metadata for this DataSource
+        sageworks_meta(): Returns the SageWorks Metadata for this DataSource
+        sageworks_tags(): Returns the SageWorks Tags for this DataSource
     """
 
     def __new__(cls, uuid, data_source_type: str = "athena"):
         """DataSource: A Factory for DataSources (Athena, RDS, etc)
         Args:
             uuid: The UUID of the DataSource
             data_source_type: The type of DataSource (athena, rds, etc)
@@ -38,15 +43,15 @@
             raise NotImplementedError(f"DataSource type {data_source_type} not implemented")
 
 
 if __name__ == "__main__":
     """Exercise the DataSource Factory Class"""
 
     # Retrieve a DataSource
-    my_data = DataSource("test_data")
+    my_data = DataSource("abalone_data")
 
     # Verify that the Athena DataSource exists
     assert my_data.check()
 
     # What's my SageWorks UUID
     print(f"UUID: {my_data.uuid}")
 
@@ -65,9 +70,12 @@
     print(f"Modified: {my_data.modified()}")
 
     # Column Names and Types
     print(f"Column Names: {my_data.column_names()}")
     print(f"Column Types: {my_data.column_types()}")
 
     # Get Metadata and tags associated with this Artifact
-    print(f"Meta: {my_data.sageworks_meta()}")
+    print(f"Meta: {my_data.meta()}")
     print(f"Tags: {my_data.sageworks_tags()}")
+
+    # Get a SAMPLE of the data
+    print(f"Sample Data: {my_data.sample_df()}")
```

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/data_sources/data_source_abstract.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source_abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,18 +39,36 @@
 
     @abstractmethod
     def query(self, query: str) -> pd.DataFrame:
         """Query the DataSourceAbstract"""
         pass
 
     @abstractmethod
-    def sample_df(self, max_rows: int = 1000) -> pd.DataFrame:
-        """Return a sample DataFrame from this DataSource"""
+    def sample_df(self, recompute: bool = False) -> pd.DataFrame:
+        """Return a sample DataFrame from this DataSource
+        Args:
+            recompute(bool): Recompute the sample (default: False)
+        Returns:
+            pd.DataFrame: A sample DataFrame from this DataSource
+        """
+        pass
+
+    @abstractmethod
+    def quartiles(self, recompute: bool = False) -> dict[dict]:
+        """Compute Quartiles for all the numeric columns in a DataSource
+        Args:
+            recompute(bool): Recompute the quartiles (default: False)
+        Returns:
+            dict(dict): A dictionary of quartiles for each column in the form
+                 {'col1': {'min': 0, 'q1': 1, 'median': 2, 'q3': 3, 'max': 4},
+                  'col2': ...}
+        """
         pass
 
     def details(self) -> dict:
         """Additional Details about this DataSourceAbstract Artifact"""
         details = self.summary()
         details["num_rows"] = self.num_rows()
         details["num_columns"] = self.num_columns()
         details["column_details"] = self.column_details()
+        details.update(self.meta())
         return details
```

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/endpoints/endpoint.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             error_df[column] = df[column].values
         return error_df
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def aws_meta(self):
+    def meta(self) -> dict:
         """Get the metadata for this artifact"""
         return self.endpoint_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.endpoint_meta["EndpointArn"]
 
@@ -179,15 +179,15 @@
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
         return self.endpoint_meta["LastModifiedTime"]
 
     def details(self) -> dict:
         """Additional Details about this Endpoint"""
         details = self.summary()
-        # Fill in more details here if needed
+        details.update(self.meta())
         return details
 
     def performance_metrics(self, target: str, prediction_df: pd.DataFrame) -> dict:
         """Compute the performance metrics for this Endpoint"""
 
         # Compute the metrics
         metrics = {
```

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/feature_sets/feature_set.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/feature_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,45 +32,57 @@
             feature_uuid (str): Name of Feature Set in SageWorks Metadata.
         """
         # Call superclass init
         super().__init__(feature_uuid)
 
         # Grab an AWS Metadata Broker object and pull information for Feature Sets
         self.feature_set_name = feature_uuid
-        self.feature_meta = self.aws_broker.get_metadata(ServiceCategory.FEATURE_STORE).get(self.feature_set_name)
+        self.feature_meta = None
+        self.data_source = None
+        self.refresh()
         if self.feature_meta is None:
             self.log.info(f"Could not find feature set {self.feature_set_name} within current visibility scope")
             self.data_source = None
             return
         else:
             self.record_id = self.feature_meta["RecordIdentifierFeatureName"]
             self.event_time = self.feature_meta["EventTimeFeatureName"]
 
             # Pull Athena and S3 Storage information from metadata
             self.athena_database = self.feature_meta["sageworks"].get("athena_database")
             self.athena_table = self.feature_meta["sageworks"].get("athena_table")
             self.s3_storage = self.feature_meta["sageworks"].get("s3_storage")
 
-            # Creat our internal DataSource (hardcoded to Athena for now)
+            # Create our internal DataSource (hardcoded to Athena for now)
             self.data_source = AthenaSource(self.athena_table, self.athena_database)
 
         # Spin up our Feature Store
         self.feature_store = FeatureStore(self.sm_session)
 
         # All done
         self.log.info(f"FeatureSet Initialized: {self.feature_set_name}")
 
+    def refresh(self, force_fresh: bool = False):
+        """Refresh our internal AWS Feature Store metadata
+        Args:
+            force_fresh (bool, optional): Force a refresh of the metadata. Defaults to False.
+        """
+        _catalog_meta = self.aws_broker.get_metadata(ServiceCategory.FEATURE_STORE, force_fresh=force_fresh)
+        self.feature_meta = _catalog_meta.get(self.feature_set_name)
+        if self.data_source is not None:
+            self.data_source.refresh(force_fresh=force_fresh)
+
     def check(self) -> bool:
         """Does the feature_set_name exist in the AWS Metadata?"""
         if self.feature_meta is None:
             self.log.info(f"FeatureSet.check() {self.feature_set_name} not found in AWS Metadata!")
             return False
         return True
 
-    def aws_meta(self) -> dict:
+    def meta(self) -> dict:
         """Get the full AWS metadata for this artifact"""
         return self.feature_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.feature_meta["FeatureGroupArn"]
 
@@ -199,14 +211,17 @@
         # Column Details
         fs_details["column_details"] = self.column_details()
 
         # Underlying Storage Details
         fs_details["storage_type"] = "athena"  # TODO: Add RDS support
         fs_details["storage_uuid"] = self.data_source.uuid
 
+        # Full Metadata from AWS
+        fs_details.update(self.meta())
+
         # Return the details
         return fs_details
 
     def delete(self):
         """Delete the Feature Set: Feature Group, Catalog Table, and S3 Storage Objects"""
 
         # Delete the Feature Group and ensure that it gets deleted
@@ -233,21 +248,37 @@
                 if error.response["Error"]["Code"] == "ResourceNotFound":
                     break
                 else:
                     raise error
             time.sleep(1)
         self.log.info(f"FeatureSet {feature_group.name} successfully deleted")
 
+    def quartiles(self) -> dict:
+        """Get the quartiles for all numeric columns of the underlying DataSource
+        Returns:
+            dict: A dictionary of quartiles for all numeric columns
+        """
+        return self.data_source.quartiles()
+
+    def sample_df(self) -> pd.DataFrame:
+        """Get a sample of the data from the underlying DataSource"""
+        return self.data_source.sample_df()
+
 
 if __name__ == "__main__":
     """Exercise for FeatureSet Class"""
     from pprint import pprint
 
+    # Setup Pandas output options
+    pd.set_option("display.max_colwidth", 50)
+    pd.set_option("display.max_columns", 15)
+    pd.set_option("display.width", 1000)
+
     # Grab a FeatureSet object and pull some information from it
-    my_features = FeatureSet("test_feature_set")
+    my_features = FeatureSet("abalone_feature_set")
 
     # Call the various methods
     # What's my AWS ARN and URL
     print(f"AWS ARN: {my_features.arn()}")
     print(f"AWS URL: {my_features.aws_url()}")
 
     # Let's do a check/validation of the feature set
@@ -277,10 +308,20 @@
 
     # Now do deep dive on storage
     if details["storage_type"] == "athena":
         storage = my_features.get_data_source()
         print("\nStorage Details:")
         pprint(storage.details())
 
+    # Get a sample of the data
+    df = my_features.sample_df()
+    print(f"Sample Data: {df.shape}")
+    print(df)
+
+    # Get quartiles for all the columns
+    quartile_info = my_features.quartiles()
+    print("Quartiles")
+    pprint(quartile_info)
+
     # Now delete the AWS artifacts associated with this Feature Set
     # print('Deleting SageWorks Feature Set...')
     # my_features.delete()
```

### Comparing `sageworks-0.1.4.3/src/sageworks/artifacts/models/model.py` & `sageworks-0.1.5.0/src/sageworks/artifacts/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             return False
         return True
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def aws_meta(self):
+    def meta(self) -> dict:
         """Get the metadata for this artifact"""
         return self.latest_model
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for the Model Package Group"""
         return self.group_arn()
 
@@ -77,14 +77,15 @@
         return self.latest_model["CreationTime"]
 
     def details(self) -> dict:
         """Additional Details about this Endpoint"""
         details = self.summary()
         details["model_package_group_arn"] = self.group_arn()
         details["model_package_arn"] = self.model_arn()
+        details.update(self.meta())
         return details
 
     def delete(self):
         """Delete the Model Packages and the Model Group"""
 
         # If we don't have meta then the model probably doesn't exist
         if self.model_meta is None:
```

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """AWSAccountClamp provides logic/functionality over a set of AWS IAM Services"""
 import sys
 import boto3
-from botocore.exceptions import ClientError, UnauthorizedSSOTokenError
+from botocore.exceptions import ClientError, UnauthorizedSSOTokenError, TokenRetrievalError
 from botocore.credentials import RefreshableCredentials
 from botocore.session import get_session
 from sagemaker.session import Session as SageSession
 from datetime import timedelta
 import logging
 
 # SageWorks Imports
@@ -67,15 +67,15 @@
 
     def is_sageworks_role(self) -> bool:
         """Check if the current AWS Identity is the SageWorks Role"""
         sts = boto3.client("sts")
         try:
             if self.role_name in sts.get_caller_identity()["Arn"]:
                 return True
-        except (ClientError, UnauthorizedSSOTokenError) as exc:
+        except (ClientError, UnauthorizedSSOTokenError, TokenRetrievalError) as exc:
             self.log.critical("SageWorks Role Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
             self.log.critical(exc)
             sys.exit(1)  # FIXME: Longer term we probably want to raise exc and have caller catch it
 
     def sageworks_execution_role_arn(self):
         """Get the SageWorks Execution Role"""
         iam = boto3.client("iam")
```

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,33 +104,34 @@
         """
         # Refresh the connection for the given category and pull new data
         cls.connection_map[category].refresh()
         cls.meta_cache.set(category, cls.connection_map[category].metadata())
         cls.fresh_cache.set(category, True)
 
     @classmethod
-    def get_metadata(cls, category: ServiceCategory) -> dict:
+    def get_metadata(cls, category: ServiceCategory, force_fresh=False) -> dict:
         """Pull Metadata for the given Service Category
 
         Args:
             category (ServiceCategory): The Service Category to pull metadata from
+            force_fresh (bool, optional): Force a refresh of the metadata. Defaults to False.
 
         Returns:
             dict: The Metadata for the Requested Service Category
         """
         # Logic:
         # - NO metadata in the cache, we need to BLOCK and get it
         # - Metadata is in the cache but is stale, launch a thread to refresh, return stale data
         # - Metadata is in the cache and is fresh, so we just return it
 
         # Do we have the metadata in the cache?
         meta_data = cls.meta_cache.get(category)
 
         # If we don't have the metadata in the cache, we need to BLOCK and get it
-        if meta_data is None:
+        if meta_data is None or force_fresh:
             cls.log.info(f"Blocking: Getting metadata for {category}...")
             cls.refresh_meta(category)
             return cls.meta_cache.get(category)
 
         # Is the metadata stale?
         if cls.fresh_cache.get(category) is None:
             cls.log.info(f"Async: Metadata for {category} is stale, launching refresh thread...")
@@ -140,19 +141,23 @@
             return cls.meta_cache.get(category)
 
         # If the metadata is fresh, just return it
         cls.log.info(f"Metadata for {category} is fresh!")
         return cls.meta_cache.get(category)
 
     @classmethod
-    def get_all_metadata(cls, warn=True) -> dict:
-        """Pull the metadata for ALL the Service Categories"""
-        if warn:
-            cls.log.warning("Getting ALL AWS Metadata: You should call get_metadata() with specific categories")
-        return {_category: cls.get_metadata(_category) for _category in ServiceCategory}
+    def get_all_metadata(cls, force_fresh=False) -> dict:
+        """Pull the metadata for ALL the Service Categories
+        Args:
+            force_fresh (bool, optional): Force a refresh of the metadata. Defaults to False.
+        Returns:
+            dict: The Metadata for ALL the Service Categories
+        """
+        cls.log.warning("Getting ALL AWS Metadata: You should call get_metadata() with specific categories")
+        return {_category: cls.get_metadata(_category, force_fresh) for _category in ServiceCategory}
 
     @classmethod
     def wait_for_refreshes(cls) -> None:
         """Wait for any open threads to finish"""
         for thread in cls.open_threads:
             thread.join()
 
@@ -179,13 +184,17 @@
         print(f"{my_category}:")
         pprint(aws_broker.get_metadata(my_category))
 
     # Get the Metadata for ALL the categories
     # NOTE: There should be NO Refreshes in the logs
     pprint(aws_broker.get_all_metadata())
 
+    # Get the Metadata for ALL the categories
+    # NOTE: This should force a refresh of the metadata
+    pprint(aws_broker.get_all_metadata(force_fresh=True))
+
     # Get S3 object sizes
     incoming_data_size = aws_broker.artifact_info.s3_object_sizes(aws_broker.incoming_data.bucket)
     print(f"Incoming Data Size: {incoming_data_size} MB")
 
     # Wait for any open threads to finish
     aws_broker.wait_for_refreshes()
```

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/Readme.md` & `sageworks-0.1.5.0/src/sageworks/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from botocore.exceptions import ClientError
 
 # Import all the AWS Glue Python Libraries
 from awsglue.utils import getResolvedOptions
 from awsglue.context import GlueContext
 from awsglue.job import Job
 from pyspark.context import SparkContext
+from awsglue.dynamicframe import DynamicFrame
+from awsglue.transforms import ApplyMapping
 
 
 class S3HeavyToDataSource:
     def __init__(self, glue_context: GlueContext, input_uuid: str, output_uuid: str):
         """S3HeavyToDataSource: Class to move HEAVY S3 Files into a SageWorks DataSource
         Args:
             glue_context: GlueContext, AWS Glue Specific wrapper around SparkContext
@@ -26,14 +28,40 @@
         self.output_meta = {"sageworks_input": self.input_uuid}
         sageworks_bucket = "s3://scp-sageworks-artifacts"
         self.data_source_s3_path = sageworks_bucket + "/data-sources"
 
         # Our Spark Context
         self.glue_context = glue_context
 
+    @staticmethod
+    def column_type_conversion(input_dyf: DynamicFrame) -> DynamicFrame:
+        """Convert the column types from the input data (Spark) to the output data (Athena/Parquet)"""
+        # Define the mapping from Spark data types to Athena data types
+        type_mapping = {"struct": "string", "choice": "long"}
+
+        # Get the column names and types from the input data
+        column_names_types = [(col.name, col.dataType.typeName()) for col in input_dyf.schema().fields]
+        input_dyf.printSchema()
+
+        # Define the mapping from input column names/types (Spark) to output
+        # column names and types that are compatible with Athena/Parquet.
+        mapping = []
+        for name, col_type in column_names_types:
+            output_type = type_mapping.get(col_type, col_type)
+            if col_type == "timestamp":
+                # Apply to_timestamp transformation for timestamp columns
+                output_type = f"to_timestamp({name})"
+            mapping.append((name, col_type, name, output_type))
+        print(mapping)
+
+        # Apply the mapping and convert data types
+        output_dyf = ApplyMapping.apply(frame=input_dyf, mappings=mapping, transformation_ctx="applymapping")
+        output_dyf.printSchema()
+        return output_dyf
+
     def transform(self, input_type: str = "json", overwrite: bool = True):
         """Convert the CSV or JSON data into Parquet Format in the SageWorks S3 Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database"""
 
         # Add some tags here
         tags = ["heavy"]
 
@@ -47,47 +75,57 @@
             connection_options={
                 "paths": [self.input_uuid],
                 "recurse": True,
                 "gzip": True,
             },
             format=input_type,
             # format_options={'jsonPath': 'auto'}, Look into this later
-            transformation_ctx="apply_mapping",
         )
         self.log.info("Incoming DataFrame...")
         input_dyf.show(5)
 
+        # Convert the columns types from Spark types to Athena/Parquet types
+        output_dyf = self.column_type_conversion(input_dyf)
+
         # Write Parquet files to S3
         self.log.info(f"Writing Parquet files to {s3_storage_path}...")
         self.glue_context.purge_s3_path(s3_storage_path, {"retentionPeriod": 0})
         self.glue_context.write_dynamic_frame.from_options(
-            frame=input_dyf,
+            frame=output_dyf,
             connection_type="s3",
             connection_options={
                 "path": s3_storage_path
                 # "partitionKeys": ["year", "month", "day"],
             },
-            format="parquet"
+            format="parquet",
         )
 
         # Set up our SageWorks metadata (description, tags, etc)
         description = f"SageWorks data source: {self.output_uuid}"
         sageworks_meta = {"sageworks_tags": ":".join(tags)}
         for key, value in self.output_meta.items():
             sageworks_meta[key] = value
 
         # Create a new table in the AWS Data Catalog
         self.log.info(f"Creating Data Catalog Table: {self.output_uuid}...")
+
+        # Converting the Spark Types to Athena Types
+        def to_athena_type(col):
+            athena_type_map = {"long": "bigint", "struct": "string"}
+            spark_type = col.dataType.typeName()
+            return athena_type_map.get(spark_type, spark_type)
+
+        column_name_types = [{"Name": col.name, "Type": to_athena_type(col)} for col in output_dyf.schema().fields]
         table_input = {
             "Name": self.output_uuid,
             "Description": description,
             "Parameters": sageworks_meta,
             "TableType": "EXTERNAL_TABLE",
             "StorageDescriptor": {
-                "Columns": [{"Name": col.name, "Type": col.dataType.typeName()} for col in input_dyf.schema().fields],
+                "Columns": column_name_types,
                 "Location": s3_storage_path,
                 "InputFormat": "org.apache.hadoop.mapred.TextInputFormat",
                 "OutputFormat": "org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
                 "Compressed": True,
                 "NumberOfBuckets": -1,
                 "SerdeInfo": {
                     "SerializationLibrary": "org.apache.hadoop.hive.ql.io.parquet.serde.ParquetHiveSerDe",
@@ -123,16 +161,16 @@
     # These are all AWS Glue Job specific
     sc = SparkContext()
     glueContext = GlueContext(sc)
     job = Job(glueContext)
     job.init(args["JOB_NAME"], args)
 
     # Test the Heavy Data Loader
-    input_path = "s3://scp-sageworks-artifacts/incoming-data/jsonl-data/"
-    data_output_uuid = "heavy_data_test"
+    input_path = "s3://scp-sageworks-artifacts/incoming-data/dns/"
+    data_output_uuid = "heavy_dns"
     my_loader = S3HeavyToDataSource(glueContext, input_path, data_output_uuid)
 
     # Store this data as a SageWorks DataSource
     my_loader.transform()
 
     # Commit the Glue Job
     job.commit()
```

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/light/clean_data.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             df[column] = df[column].astype("int32")
         for column in list(df.select_dtypes(include=[pd.Int64Dtype]).columns):
             df[column] = df[column].astype("int64")
         for column in list(df.select_dtypes(include=[pd.Float64Dtype]).columns):
             df[column] = df[column].astype("float64")
         return df
 
-    def transform_impl(self, id_column: str, event_time_column: str = None, delete_existing: bool = True):
+    def transform_impl(self, query, id_column: str, event_time_column: str = None, delete_existing: bool = True):
         """Convert the Data Source into a Feature Set, also storing the information
         about the data to the AWS Data Catalog sageworks database and create S3 Objects"""
 
         # Do we want to delete the existing FeatureSet?
         if delete_existing:
             try:
                 delete_fs = FeatureSet(self.output_uuid)
@@ -65,25 +65,24 @@
         self.id_column = id_column
         self.event_time_column = event_time_column
 
         # Create the Output Parquet file S3 Storage Path for this Feature Set
         s3_storage_path = f"{self.feature_sets_s3_path}"
 
         # Now we'll make a Query of the Data Source to create a FeatureSet
-        query = f"SELECT * FROM {self.input_data_source.table_name}"
         self.log.info(f"Creating FeatureSet Data with Query: {query}")
         info = wr.athena.create_ctas_table(
             sql=query,
             database=self.input_data_source.data_catalog_db,
             ctas_table=self.output_uuid,
             ctas_database=self.output_database,
             s3_output=s3_storage_path,
             write_compression="snappy",
             boto3_session=self.boto_session,
-            wait=True
+            wait=True,
         )
         self.log.info(f"FeatureSet Data Created: {info}")
 
         # Convert Int32, Int64 and Float64 types (see: https://github.com/aws/sagemaker-python-sdk/pull/3740)
         self.input_sample_df = self.convert_nullable_types(self.input_sample_df)
 
         # Create a Feature Group and load our Feature Definitions
@@ -91,28 +90,28 @@
         my_feature_group = FeatureGroup(name=self.output_uuid, sagemaker_session=self.sm_session)
         my_feature_group.load_feature_definitions(data_frame=self.input_sample_df)
 
         # Get the metadata/tags to push into AWS
         aws_tags = self.get_aws_tags()
 
         # Data Catalog Config
-        my_config = DataCatalogConfig(table_name=self.output_uuid,
-                                      catalog='AwsDataCatalog',
-                                      database=self.output_database)
+        my_config = DataCatalogConfig(
+            table_name=self.output_uuid, catalog="AwsDataCatalog", database=self.output_database
+        )
 
         # Write out the DataFrame to Parquet/FeatureSet/Athena
         my_feature_group.create(
             s3_uri=s3_storage_path,
             record_identifier_name=self.id_column,
             event_time_feature_name=self.event_time_column,
             role_arn=self.sageworks_role_arn,
             enable_online_store=True,
             tags=aws_tags,
             data_catalog_config=my_config,
-            disable_glue_table_creation=True
+            disable_glue_table_creation=True,
         )
 
         # Ensure/wait for the feature group to be created
         self.ensure_feature_group_created(my_feature_group)
 
     def ensure_feature_group_created(self, feature_group):
         status = feature_group.describe().get("FeatureGroupStatus")
@@ -127,8 +126,8 @@
     """Exercise the DataToFeaturesHeavy Class"""
 
     # Create my DF to Feature Set Transform
     data_to_features_heavy = DataToFeaturesHeavy("heavy_data_test", "heavy_data_test_features")
     data_to_features_heavy.set_output_tags(["test", "heavy"])
 
     # Store this dataframe as a SageWorks Feature Set
-    data_to_features_heavy.transform(id_column="id", event_time_column="date")
+    data_to_features_heavy.transform(query="SELECT * FROM heavy_data_test", id_column="id", event_time_column="date")
```

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/data_to_features_light.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,13 +47,13 @@
         output_features.transform(delete_existing=delete_existing)
 
 
 if __name__ == "__main__":
     """Exercise the DataToFeaturesLight Class"""
 
     # Create the class with inputs and outputs and invoke the transform
-    input_uuid = "aqsol_data"
-    output_uuid = "aqsol_feature_set"
+    input_uuid = "abalone_data"
+    output_uuid = "abalone_feature_set"
     data_to_features = DataToFeaturesLight(input_uuid, output_uuid)
-    data_to_features.set_output_tags(["aqsol", "public"])
+    data_to_features.set_output_tags(["abalone", "public"])
     # data_to_features.transform(id_column="id", event_time_column="date")
     data_to_features.transform(id_column="id")
```

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py` & `sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/features_to_model.py` & `sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,15 @@
 
         Args:
             overwrite (bool): Overwrite the existing data in the SageWorks S3 Bucket
         """
 
         # Set up our metadata storage
         sageworks_meta = {"sageworks_tags": self.output_tags}
-        for key, value in self.output_meta.items():
-            sageworks_meta[key] = value
+        sageworks_meta.update(self.output_meta)
 
         # Create the Output Parquet file S3 Storage Path
         s3_storage_path = f"{self.data_source_s3_path}/{self.output_uuid}"
 
         # Convert Object Columns to Datetime or String
         self.output_df = self.convert_object_columns(self.output_df)
```

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_features.py`

 * *Files 18% similar despite different names*

```diff
@@ -158,25 +158,59 @@
             # data_catalog_config=my_config,
             # disable_glue_table_creation=True
         )
 
         # Ensure/wait for the feature group to be created
         self.ensure_feature_group_created(my_feature_group)
 
+        # Add the parameters to the FeatureSet DataCatalog Table
+        feature_info = my_feature_group.describe()
+        self.add_parameters_to_table(feature_info["OfflineStoreConfig"]["DataCatalogConfig"]["TableName"])
+
         # Now we actually push the data into the Feature Group
         my_feature_group.ingest(self.output_df, max_processes=4)
 
     def ensure_feature_group_created(self, feature_group):
         status = feature_group.describe().get("FeatureGroupStatus")
         while status == "Creating":
             self.log.info("FeatureSet being Created...")
             time.sleep(5)
             status = feature_group.describe().get("FeatureGroupStatus")
         self.log.info(f"FeatureSet {feature_group.name} successfully created")
 
+    def add_parameters_to_table(self, table_name):
+        """Add the parameters to the FeatureSet DataCatalog Table
+        Note: Stupid hack because the Feature Group create() method doesn't create
+              a Parameters section when it makes the AWS Glue Catalog Table
+        """
+        glue_client = self.boto_session.client("glue")
+
+        # Get the current table parameters
+        catalog_db = "sagemaker_featurestore"
+        table_info = glue_client.get_table(DatabaseName=catalog_db, Name=table_name)["Table"]
+
+        # These keys are automatically generated by AWS and the update_table call doesn't
+        # like them as input so we need to remove them from the update dictionary
+        auto_keys = [
+            "DatabaseName",
+            "CreateTime",
+            "UpdateTime",
+            "CreatedBy",
+            "IsRegisteredWithLakeFormation",
+            "CatalogId",
+            "VersionId",
+        ]
+        table_input = {k: v for k, v in table_info.items() if k not in auto_keys}
+
+        # Add the Parameters section
+        table_input["Parameters"] = {}
+
+        # Update the Table
+        glue_client.update_table(DatabaseName=catalog_db, TableInput=table_input)
+
 
 if __name__ == "__main__":
     """Exercise the PandasToFeatures Class"""
 
     # Setup Pandas output options
     pd.set_option("display.max_colwidth", 15)
     pd.set_option("display.max_columns", 15)
```

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/pandas_transforms/pandas_utils.py` & `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/transforms/transform.py` & `sageworks-0.1.5.0/src/sageworks/transforms/transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Transform: Base Class for all transforms within SageWorks
               Inherited Classes must implement the abstract transform_impl() method"""
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import final
 import logging
 import awswrangler as wr
+from time import sleep
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
+from sageworks.artifacts.data_sources.data_source import DataSource
+from sageworks.artifacts.feature_sets.feature_set import FeatureSet
 
 # Setup Logging
 logging_setup()
 
 
 class TransformInput(Enum):
     """Enumerated Types for SageWorks Transform Inputs"""
@@ -79,15 +82,36 @@
 
     def pre_transform(self, **kwargs):
         """Perform any Pre-Transform operations"""
         self.log.debug("Pre-Transform...")
 
     def post_transform(self, **kwargs):
         """Perform any Post-Transform operations"""
-        self.log.debug("Post-Transform...")
+        self.log.info("Post-Transform...")
+
+        # For DataSource and FeatureSet outputs we'll compute sample rows and quartiles
+        if self.output_type == TransformOutput.DATA_SOURCE:
+            self.log.info("Computing Sample Rows and Quartiles...")
+            while not DataSource(self.output_uuid).check():
+                self.log.info("Waiting for DataSource to be created...")
+                sleep(1)
+            ds = DataSource(self.output_uuid)
+            ds.sample_df()
+            ds.quartiles()
+            ds.refresh(force_fresh=True)
+
+        elif self.output_type == TransformOutput.FEATURE_SET:
+            self.log.info("Computing Sample Rows and Quartiles...")
+            while not FeatureSet(self.output_uuid).check():
+                self.log.info("Waiting for FeatureSet to be created...")
+                sleep(1)
+            fs = FeatureSet(self.output_uuid)
+            fs.sample_df()
+            fs.quartiles()
+            fs.refresh(force_fresh=True)
 
     def set_output_tags(self, tags: list | str):
         """Set the tags that will be associated with the output object
         Args:
             tags (list | str): The list of tags or a ':' separated string of tags"""
         if isinstance(tags, list):
             self.output_tags = ":".join(tags)
```

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/cache.py` & `sageworks-0.1.5.0/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.1.5.0/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/iso_8601.py` & `sageworks-0.1.5.0/src/sageworks/utils/iso_8601.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/redis_cache.py` & `sageworks-0.1.5.0/src/sageworks/utils/redis_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     redis_db = None
     try:
         # Create a temporary connection to test the connection
         _redis_db = redis.Redis(host, port=port, password=password, socket_timeout=1)
         _redis_db.ping()
 
         # Now create the actual connection
-        redis_db = redis.Redis(host, port=port, password=password, charset="utf-8",
-                               decode_responses=True, db=0)
+        redis_db = redis.Redis(host, port=port, password=password, charset="utf-8", decode_responses=True, db=0)
         log.info(f"Redis connection success: {host}:{port}...")
     except (redis.exceptions.ConnectionError, redis.exceptions.TimeoutError):
         msg = f"Could not connect to Redis Database: {host}:{port}..."
         log.warning(msg)
 
     @classmethod
     def check(cls):
```

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/sageworks_config.py` & `sageworks-0.1.5.0/src/sageworks/utils/sageworks_config.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.1.5.0/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.1.5.0/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.1.5.0/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/views/artifacts.py` & `sageworks-0.1.5.0/src/sageworks/views/artifacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,21 @@
             "MODELS": self.models_summary(),
             "ENDPOINTS": self.endpoints_summary(),
         }
         return summary_data
 
     def header_text(self, header_text: str) -> str:
         """Colorize text for the terminal"""
-        color_map = { "INCOMING_DATA": "cyan",
-                      "DATA_SOURCES": "red",
-                      "FEATURE_SETS": "yellow",
-                      "MODELS": "green",
-                      "ENDPOINTS": "magenta"}
+        color_map = {
+            "INCOMING_DATA": "cyan",
+            "DATA_SOURCES": "red",
+            "FEATURE_SETS": "yellow",
+            "MODELS": "green",
+            "ENDPOINTS": "magenta",
+        }
         header = f"\n{'='*111}\n{header_text}\n{'='*111}"
         return colored(header, color_map[header_text])
 
     def dump(self) -> None:
         """Dump all the data to stdout"""
         for name, df in self.view_data().items():
             print(self.header_text(name))
@@ -149,20 +151,20 @@
 
             # Get Summary information for each model in the model_list
             for model in model_list:
                 # Get the tags for this Model Group
                 model_group_arn = model["ModelPackageGroupArn"]
                 sageworks_meta = self.artifact_info.get_sagemaker_obj_info(model_group_arn)
                 summary = {
-                        "Model Group": model["ModelPackageGroupName"],
-                        "Description": model["ModelPackageDescription"],
-                        "Created": self.datetime_string(model.get("CreationTime")),
-                        "Tags": sageworks_meta.get("sageworks_tags", "-"),
-                        "Input": sageworks_meta.get("sageworks_input", "-"),
-                    }
+                    "Model Group": model["ModelPackageGroupName"],
+                    "Description": model["ModelPackageDescription"],
+                    "Created": self.datetime_string(model.get("CreationTime")),
+                    "Tags": sageworks_meta.get("sageworks_tags", "-"),
+                    "Input": sageworks_meta.get("sageworks_input", "-"),
+                }
                 model_summary.append(summary)
         return pd.DataFrame(model_summary)
 
     def endpoints_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks Endpoints"""
         data = self.aws_artifact_data[ServiceCategory.ENDPOINTS]
         data_summary = []
```

### Comparing `sageworks-0.1.4.3/src/sageworks/views/view.py` & `sageworks-0.1.5.0/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/views/web_artifacts_summary.py` & `sageworks-0.1.5.0/src/sageworks/views/web_artifacts_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,22 +69,15 @@
             }
             data_summary.append(summary)
 
         # Make sure we have data else return just the column names
         if data_summary:
             return pd.DataFrame(data_summary)
         else:
-            columns = [
-                "Name",
-                "Size(MB)",
-                "Modified",
-                "ContentType",
-                "ServerSideEncryption",
-                "Tags"
-            ]
+            columns = ["Name", "Size(MB)", "Modified", "ContentType", "ServerSideEncryption", "Tags"]
             return pd.DataFrame(columns=columns)
 
     def data_sources_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks DataSources"""
         data = self.aws_artifact_data[ServiceCategory.DATA_CATALOG]
         data_summary = []
```

### Comparing `sageworks-0.1.4.3/src/sageworks/views/web_data_source_view.py` & `sageworks-0.1.5.0/src/sageworks/views/web_data_source_view.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from sageworks.views.view import View
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 from sageworks.artifacts.data_sources.data_source import DataSource
 
 
 class WebDataSourceView(View):
     def __init__(self):
-        """WebDataSourceView pulls DataSource metadata from the AWS Service Broker with Details Panels on each DataSource"""
+        """WebDataSourceView pulls DataSource metadata from the AWS Service
+        Broker with Details Panels on each DataSource"""
         # Call SuperClass Initialization
         super().__init__()
 
         # Get AWS Service information for the Data Catalog (DataSources)
         self.data_sources_meta = {}
         self.refresh()
 
@@ -81,24 +82,55 @@
 
     def hyperlinks(self, name, detail_type):
         athena_url = f"https://{self.aws_account_clamp.region()}.console.aws.amazon.com/athena/home"
         link = f"<a href='{detail_type}' target='_blank'>{name}</a>"
         link += f" [<a href='{athena_url}' target='_blank'>query</a>]"
         return link
 
-    def data_source_sample(self, data_source_index: int, max_rows=100) -> pd.DataFrame:
+    def data_source_sample(self, data_source_index: int) -> pd.DataFrame:
         """Get a sample dataframe for the given DataSource Index"""
         # Grab the a sample of N rows of the data source
         if self.data_sources_meta and data_source_index < len(self.data_sources_meta):
             data_uuid = list(self.data_sources_meta.keys())[data_source_index]
-            sample_rows = DataSource(data_uuid).sample_df(max_rows=max_rows).head(max_rows)
+            sample_rows = DataSource(data_uuid).sample_df()
         else:
             sample_rows = pd.DataFrame()
         return sample_rows
 
+    def data_source_quartiles(self, data_source_index: int) -> (dict, None):
+        """Get all columns quartiles for the given DataSource Index"""
+        if self.data_sources_meta and data_source_index < len(self.data_sources_meta):
+            data_uuid = list(self.data_sources_meta.keys())[data_source_index]
+            quartiles_data = DataSource(data_uuid).quartiles()
+            print(quartiles_data)
+            return quartiles_data
+        else:
+            return None
+
+    def data_source_smart_sample(self, data_source_index: int) -> pd.DataFrame:
+        """Get a SMART sample dataframe for the given DataSource Index
+        Note:
+            SMART here means a sample data + quartiles for each column"""
+        # Sample DataFrame
+        sample_rows = self.data_source_sample(data_source_index)
+
+        # Quartiles Data
+        quartiles_data = self.data_source_quartiles(data_source_index)
+        if quartiles_data is None:
+            return sample_rows
+
+        # Convert the Quartiles Data into a DataFrame
+        quartiles_dict_list = dict()
+        for col_name, quartiles in quartiles_data.items():
+            quartiles_dict_list[col_name] = quartiles.values()
+        quartiles_df = pd.DataFrame(quartiles_dict_list)
+
+        # Combine the sample rows with the quartiles data
+        return pd.concat([sample_rows, quartiles_df]).reset_index(drop=True)
+
     def data_source_name(self, data_source_index: int) -> str:
         """Helper method for getting the data source name for the given DataSource Index"""
         if self.data_sources_meta and data_source_index < len(self.data_sources_meta):
             data_uuid = list(self.data_sources_meta.keys())[data_source_index]
             return data_uuid
         else:
             return "Unknown"
@@ -135,9 +167,10 @@
 
     # List the DataSources
     print("DataSourcesSummary:")
     summary = data_view.view_data()["DATA_SOURCES"]
     print(summary.head())
 
     # Get a sample dataframe for the given DataSources
-    sample_df = data_view.data_source_sample(0)
+    sample_df = data_view.data_source_smart_sample(0)
+    print(sample_df.shape)
     print(sample_df.head())
```

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/box_plot.py` & `sageworks-0.1.5.0/src/sageworks/web_components/box_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,21 @@
 import plotly.graph_objects as go
 
 
 # For colormaps see (https://plotly.com/python/discrete-color/#color-sequences-in-plotly-express)
 def create_figure(df: pd.DataFrame) -> plotly.graph_objects.Figure:
     """Create a set of Box Plots for the numeric columns in the dataframe"""
 
-    numeric_columns = list(df.select_dtypes('number').columns)[:10]  # Max 10 columns
+    numeric_columns = list(df.select_dtypes("number").columns)[:10]  # Max 10 columns
     numeric_columns = [col for col in numeric_columns if len(df[col].unique()) > 1]  # Only columns > 1 unique value
-    numeric_columns = [col for col in numeric_columns if col not in ['id', 'Id', 'ID', 'Id_']]  # Remove id columns
+    numeric_columns = [col for col in numeric_columns if col not in ["id", "Id", "ID", "Id_"]]  # Remove id columns
     fig = make_subplots(rows=1, cols=len(numeric_columns))
     for i, col in enumerate(numeric_columns):
-        fig.add_trace(
-            go.Box(y=df[col], name=col, notched=True, showlegend=False),
-            row=1, col=i+1
-        )
-    fig.update_traces(boxpoints='all', jitter=.2)
+        fig.add_trace(go.Box(y=df[col], name=col, notched=True, showlegend=False), row=1, col=i + 1)
+    fig.update_traces(boxpoints="all", jitter=0.2)
     fig.update_layout(margin=dict(l=20, r=20, t=20, b=20))
     return dcc.Graph(id="box_plot", figure=fig)
 
 
 def create(df: pd.DataFrame) -> dcc.Graph:
     """Create a Violin Plot Graph Component"""
```

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.1.5.0/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/feature_details.py` & `sageworks-0.1.5.0/src/sageworks/web_components/feature_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/feature_importance.py` & `sageworks-0.1.5.0/src/sageworks/web_components/feature_importance.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/histogram.py` & `sageworks-0.1.5.0/src/sageworks/web_components/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/line_chart.py` & `sageworks-0.1.5.0/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/model_data.py` & `sageworks-0.1.5.0/src/sageworks/web_components/model_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/model_details.py` & `sageworks-0.1.5.0/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/scatter_plot.py` & `sageworks-0.1.5.0/src/sageworks/web_components/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/table.py` & `sageworks-0.1.5.0/src/sageworks/web_components/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,32 +38,32 @@
         id=table_id,
         data=df.to_dict("records"),
         columns=column_setup,
         sort_action="native",
         row_selectable=row_select,
         cell_selectable=False,
         selected_rows=[0],
-        fixed_rows={'headers': fixed_headers},
+        fixed_rows={"headers": fixed_headers},
         style_table={"maxHeight": max_height, "overflowX": "auto", "overflowY": "auto"},
         style_as_list_view=True,
         style_cell={
             "font-family": "HelveticaNeue",
             "padding": "5px",
             "overflow": "hidden",
             "textOverflow": "ellipsis",
-            "maxWidth": 250
+            "maxWidth": 250,
         },
         style_header={
             "textAlign": "left",
             "fontSize": 16,
             "backgroundColor": header_color,
-            "color": "rgb(200, 200, 200)"
+            "color": "rgb(200, 200, 200)",
         },
         style_data={
             "fontSize": 14,
             "backgroundColor": "rgb(60, 60, 60)",
             "color": "rgb(200, 200, 200)",
-            "border": "0px"
+            "border": "0px",
         },
         markdown_options={"html": True},
     )
     return table
```

### Comparing `sageworks-0.1.4.3/src/sageworks/web_components/violin_plot.py` & `sageworks-0.1.5.0/src/sageworks/web_components/violin_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,37 +6,38 @@
 import plotly.graph_objects as go
 
 
 def compute_rows_columns(num_plots):
     """Errr... I think this works but happy to be improved"""
     max_columns = 8
     overflow = 1 if num_plots % max_columns != 0 else 0
-    num_rows = num_plots//max_columns + overflow
-    num_columns = round(num_plots/num_rows + .1)
+    num_rows = num_plots // max_columns + overflow
+    num_columns = round(num_plots / num_rows + 0.1)
     return num_rows, num_columns
 
 
 # For colormaps see (https://plotly.com/python/discrete-color/#color-sequences-in-plotly-express)
 def create_figure(df: pd.DataFrame) -> plotly.graph_objs.Figure:
     """Create a set of Violin Plots for the numeric columns in the dataframe"""
 
-    numeric_columns = list(df.select_dtypes('number').columns)
+    numeric_columns = list(df.select_dtypes("number").columns)
     numeric_columns = [col for col in numeric_columns if len(df[col].unique()) > 1]  # Only columns > 1 unique value
-    numeric_columns = [col for col in numeric_columns if col not in ['id', 'Id', 'ID', 'Id_']]  # Remove id columns
+    numeric_columns = [col for col in numeric_columns if col not in ["id", "Id", "ID", "Id_"]]  # Remove id columns
     numeric_columns = numeric_columns[:24]  # Max 24 plots
 
     # Compute the number of rows and columns
     num_plots = len(numeric_columns)
     num_rows, num_columns = compute_rows_columns(num_plots)
     print(f"Creating {num_plots} violin plots in {num_rows} rows and {num_columns} columns")
     fig = make_subplots(rows=num_rows, cols=num_columns)
     for i, var in enumerate(numeric_columns):
         fig.add_trace(
             go.Violin(y=df[var], name=var, box_visible=True, meanline_visible=True, showlegend=False, points="all"),
-            row=i//num_columns+1, col=i % num_columns+1
+            row=i // num_columns + 1,
+            col=i % num_columns + 1,
         )
     fig.update_layout(margin=dict(l=20, r=20, t=20, b=20))
     return fig
 
 
 def create(df: pd.DataFrame) -> dcc.Graph:
     """Create a Violin Plot Graph Component"""
```

### Comparing `sageworks-0.1.4.3/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.1.5.0/src/sageworks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.4.3
+Version: 0.1.5.0
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
+<img height="360" align="left" src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png">
+<img height="360" aligh="right" src="https://user-images.githubusercontent.com/4806709/236641581-51777977-bca4-4af3-8bec-fb1758c964b8.png">
+
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
 <img src="docs/images/sageworks_concepts.png">
 
 ### Full SageWorks OverView
```

### Comparing `sageworks-0.1.4.3/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.1.5.0/src/sageworks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 applications/model_viewer/data/toy_scores.json
 applications/web_admin/flask_test.py
 applications/web_admin/hello-world-http-test.ini
 applications/web_admin/hello-world.ini
 applications/web_admin/hello-world.service
 applications/web_admin/nginx_conf/nginx.conf
 aws_setup/aws_account_check.py
-aws_setup/aws_account_check_deep.py
+aws_setup/build_ml_pipeline.py
 aws_setup/sageworks_cdk/.gitignore
 aws_setup/sageworks_cdk/README.md
 aws_setup/sageworks_cdk/app.py
 aws_setup/sageworks_cdk/cdk.json
 aws_setup/sageworks_cdk/requirements-dev.txt
 aws_setup/sageworks_cdk/requirements.txt
 aws_setup/sageworks_cdk/source.bat
```

### Comparing `sageworks-0.1.4.3/tests/artifacts/data_source_tests.py` & `sageworks-0.1.5.0/tests/artifacts/data_source_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     print(f"Size of Data (MB): {my_data.size()}")
 
     # When was it created and last modified?
     print(f"Created: {my_data.created()}")
     print(f"Modified: {my_data.modified()}")
 
     # Get Metadata and tags associated with this Artifact
-    print(f"Meta: {my_data.sageworks_meta()}")
+    print(f"Meta: {my_data.meta()}")
     print(f"Tags: {my_data.sageworks_tags()}")
 
     # Now delete the AWS artifacts associated with this DataSource
     # print('Deleting SageWorks Data Source...')
     # my_data.delete()
```

### Comparing `sageworks-0.1.4.3/tests/artifacts/endpoint_tests.py` & `sageworks-0.1.5.0/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/artifacts/feature_set_tests.py` & `sageworks-0.1.5.0/tests/artifacts/feature_set_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     print(f"Rows: {num_rows} Columns: {num_columns}")
 
     # What are the column names?
     columns = my_features.column_names()
     print(columns)
 
     # Get the metadata and tags associated with this feature set
-    print(f"SageWorks Meta: {my_features.sageworks_meta()}")
+    print(f"Meta: {my_features.meta()}")
     print(f"SageWorks Tags: {my_features.sageworks_tags()}")
 
     # Now delete the AWS artifacts associated with this Feature Set
     # print('Deleting SageWorks Feature Set...')
     # my_features.delete()
```

### Comparing `sageworks-0.1.4.3/tests/artifacts/model_tests.py` & `sageworks-0.1.5.0/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.1.5.0/tests/aws_account/aws_service_broker_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,7 @@
     for my_category in ServiceCategory:
         print(f"{my_category}:")
         pprint(aws_broker.get_metadata(my_category))
 
     # Get the Metadata for ALL the categories
     # NOTE: There should be NO Refreshes in the logs
     pprint(aws_broker.get_all_metadata())
-
-
-if __name__ == "__main__":
-    test()
```

### Comparing `sageworks-0.1.4.3/tests/create_sageworks_objs_for_tests.py` & `sageworks-0.1.5.0/tests/create_sageworks_objs_for_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/transforms/data_to_data_tests.py` & `sageworks-0.1.5.0/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/transforms/data_to_features_tests.py` & `sageworks-0.1.5.0/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/transforms/features_to_model_tests.py` & `sageworks-0.1.5.0/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.1.5.0/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.1.5.0/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.3/tox.ini` & `sageworks-0.1.5.0/tox.ini`

 * *Files identical despite different names*

