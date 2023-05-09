# Comparing `tmp/grizzly-loadtester-2.6.4.tar.gz` & `tmp/grizzly-loadtester-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-2.6.4.tar", last modified: Thu May  4 07:58:47 2023, max compression
+gzip compressed data, was "grizzly-loadtester-2.6.5.tar", last modified: Tue May  9 06:55:55 2023, max compression
```

## Comparing `grizzly-loadtester-2.6.4.tar` & `grizzly-loadtester-2.6.5.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.946077 grizzly-loadtester-2.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.github/workflows/code-quality.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.pytest_tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.pytest_tmp/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/build.novella
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/docs/content/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/docs/content/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.962078 grizzly-loadtester-2.6.4/docs/content/assets/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   116365 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_1024.png
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_16.png
--rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_256.png
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_48.png
--rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_512.png
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_64.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.962078 grizzly-loadtester-2.6.4/docs/content/command-line-interface/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/licenses.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.962078 grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/metadata.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/editor-support/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/editor-support/editors/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/editors/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/editors/vscode.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/licenses.md
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/example.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/framework/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/licenses.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.946077 grizzly-loadtester-2.6.4/docs/content/framework/usage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/environment-configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/templating.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/mkdocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/environments/example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/features/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/example.feature
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.950078 grizzly-loadtester-2.6.4/example/features/requests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/features/requests/books/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/requests/books/books.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/features/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/steps/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/steps/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/auth/aad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/behave.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/listeners/appinsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/listeners/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26965 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/locust.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/scenarios/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.974078 grizzly-loadtester-2.6.4/grizzly/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.974078 grizzly-loadtester-2.6.4/grizzly/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/background/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/background/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.974078 grizzly-loadtester-2.6.4/grizzly/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    35217 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.978078 grizzly-loadtester-2.6.4/grizzly/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/async_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.982078 grizzly-loadtester-2.6.4/grizzly/tasks/clients/
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/set_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/task_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/until.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.982078 grizzly-loadtester-2.6.4/grizzly/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.986078 grizzly-loadtester-2.6.4/grizzly/testdata/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/integer_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.986078 grizzly-loadtester-2.6.4/grizzly/types/
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/types/behave.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/types/locust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.986078 grizzly-loadtester-2.6.4/grizzly/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly/users/base/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/grizzly_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/request_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/response_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly_extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly_extras/async_message/
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/
--rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/rfh2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26029 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/sb.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/dummy_pymqi.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/script/docs-generate-changelog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4893 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/script/docs-generate-licenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2855 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/script/docs-generate.bash
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/tests/e2e/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.998078 grizzly-loadtester-2.6.4/tests/e2e/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.998078 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    45278 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_iteration_pace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_until.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    38536 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.998078 grizzly-loadtester-2.6.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33819 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/test_aad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_appinsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/test_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.006078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34083 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21230 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test__helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.010078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.010078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    30575 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_async_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_set_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_task_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_until.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_behave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    32204 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_locust.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.010078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.014078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.014078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_grizzly_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_request_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    35818 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/
--rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_sb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.625021 grizzly-loadtester-2.6.5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.613021 grizzly-loadtester-2.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.625021 grizzly-loadtester-2.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.github/workflows/code-quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.629021 grizzly-loadtester-2.6.5/.pytest_tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.pytest_tmp/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.629021 grizzly-loadtester-2.6.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.629021 grizzly-loadtester-2.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/build.novella
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.629021 grizzly-loadtester-2.6.5/docs/content/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.629021 grizzly-loadtester-2.6.5/docs/content/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.633020 grizzly-loadtester-2.6.5/docs/content/assets/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   116365 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_1024.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_64.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.633020 grizzly-loadtester-2.6.5/docs/content/command-line-interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/command-line-interface/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/command-line-interface/licenses.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.633020 grizzly-loadtester-2.6.5/docs/content/command-line-interface/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/command-line-interface/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/command-line-interface/usage/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.633020 grizzly-loadtester-2.6.5/docs/content/editor-support/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/editor-support/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/docs/content/editor-support/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/editor-support/editors/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/editor-support/editors/vscode.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/editor-support/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/editor-support/language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/editor-support/licenses.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/example.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/docs/content/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/framework/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/framework/licenses.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.617020 grizzly-loadtester-2.6.5/docs/content/framework/usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/docs/content/framework/usage/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/framework/usage/variables/environment-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/framework/usage/variables/templating.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/content/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/docs/mkdocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/example/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/environments/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/example/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/features/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/features/example.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.617020 grizzly-loadtester-2.6.5/example/features/requests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/example/features/requests/books/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/features/requests/books/books.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.637020 grizzly-loadtester-2.6.5/example/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/features/steps/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/features/steps/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/example/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.641020 grizzly-loadtester-2.6.5/grizzly/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.641020 grizzly-loadtester-2.6.5/grizzly/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25996 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/auth/aad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.641020 grizzly-loadtester-2.6.5/grizzly/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/listeners/appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/listeners/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26965 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.641020 grizzly-loadtester-2.6.5/grizzly/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/scenarios/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.641020 grizzly-loadtester-2.6.5/grizzly/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.641020 grizzly-loadtester-2.6.5/grizzly/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/background/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/background/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.645020 grizzly-loadtester-2.6.5/grizzly/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/scenario/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/scenario/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/scenario/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35217 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/scenario/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/scenario/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/steps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.645020 grizzly-loadtester-2.6.5/grizzly/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/async_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.649021 grizzly-loadtester-2.6.5/grizzly/tasks/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/clients/blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/clients/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/clients/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/clients/servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/set_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/task_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/tasks/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.649021 grizzly-loadtester-2.6.5/grizzly/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.649021 grizzly-loadtester-2.6.5/grizzly/testdata/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/integer_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/testdata/variables/random_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.649021 grizzly-loadtester-2.6.5/grizzly/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/types/behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/types/locust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.653020 grizzly-loadtester-2.6.5/grizzly/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.653020 grizzly-loadtester-2.6.5/grizzly/users/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/base/grizzly_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/base/request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/base/response_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/base/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/users/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.653020 grizzly-loadtester-2.6.5/grizzly_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.657020 grizzly-loadtester-2.6.5/grizzly_extras/async_message/
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/async_message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/async_message/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.657020 grizzly-loadtester-2.6.5/grizzly_extras/async_message/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/async_message/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/async_message/mq/rfh2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/async_message/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/dummy_pymqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/grizzly_extras/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.657020 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 06:55:55.000000 grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.657020 grizzly-loadtester-2.6.5/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/script/docs-generate-changelog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4893 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/script/docs-generate-licenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2855 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/script/docs-generate.bash
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.657020 grizzly-loadtester-2.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.657020 grizzly-loadtester-2.6.5/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/e2e/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/e2e/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/background/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/background/test_shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45278 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/steps/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_iteration_pace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/e2e/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38536 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/auth/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33819 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/auth/test_aad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/test_appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/test_influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/scenarios/test_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.661020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/background/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/background/test_shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.665020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34083 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21230 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/test__helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.665020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.665020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30575 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_async_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_set_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_task_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32204 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.665020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22243 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_random_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_grizzly_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_response_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35818 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:55:55.669020 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/test_sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-09 06:55:01.000000 grizzly-loadtester-2.6.5/tests/webserver.py
```

### Comparing `grizzly-loadtester-2.6.4/.devcontainer/Dockerfile` & `grizzly-loadtester-2.6.5/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/.devcontainer/devcontainer.json` & `grizzly-loadtester-2.6.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/.github/workflows/code-quality.yaml` & `grizzly-loadtester-2.6.5/.github/workflows/code-quality.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/.github/workflows/release.yaml` & `grizzly-loadtester-2.6.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/.vscode/launch.json` & `grizzly-loadtester-2.6.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/LICENSE.md` & `grizzly-loadtester-2.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/PKG-INFO` & `grizzly-loadtester-2.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester
-Version: 2.6.4
+Version: 2.6.5
 Summary: Traffic generator based on locust and behave
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,load,loadtest,performance,traffic generator
```

### Comparing `grizzly-loadtester-2.6.4/README.md` & `grizzly-loadtester-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/build.novella` & `grizzly-loadtester-2.6.5/docs/build.novella`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/favicon.ico` & `grizzly-loadtester-2.6.5/docs/content/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown.svg` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange.svg` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo.svg` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_1024.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_1024.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_128.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_128.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_16.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_16.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_256.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_256.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_32.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_32.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_48.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_48.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_512.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_512.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_64.png` & `grizzly-loadtester-2.6.5/docs/content/assets/logo/grizzly_logo_64.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/metadata.md` & `grizzly-loadtester-2.6.5/docs/content/command-line-interface/usage/metadata.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/editor-support/index.md` & `grizzly-loadtester-2.6.5/docs/content/editor-support/index.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/example.md` & `grizzly-loadtester-2.6.5/docs/content/example.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/environment-configuration.md` & `grizzly-loadtester-2.6.5/docs/content/framework/usage/variables/environment-configuration.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/templating.md` & `grizzly-loadtester-2.6.5/docs/content/framework/usage/variables/templating.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/docs/mkdocs.yaml` & `grizzly-loadtester-2.6.5/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/example/features/environment.py` & `grizzly-loadtester-2.6.5/example/features/environment.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/example/features/example.feature` & `grizzly-loadtester-2.6.5/example/features/example.feature`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/example/features/steps/custom.py` & `grizzly-loadtester-2.6.5/example/features/steps/custom.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/example/features/steps/steps.py` & `grizzly-loadtester-2.6.5/example/features/steps/steps.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/auth/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/auth/aad.py` & `grizzly-loadtester-2.6.5/grizzly/auth/aad.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,25 +469,28 @@
                             return AuthType.COOKIE, f'{cookie.name}={cookie.value}'
 
                     raise RuntimeError('did not find AAD cookie in authorization flow response session')
         except Exception as e:
             exception = e
             logger.error(str(e), exc_info=True)
         finally:
-            name = client.__class__.__name__.rsplit('_', 1)[-1]
+            if client.parent is not None:
+                scenario_index = client.parent.user._scenario.identifier
+            else:
+                scenario_index = client.__class__.__name__.rsplit('_', 1)[-1]
 
             if is_token_v2_0 is None:
                 version = ''
             else:
                 version = 'v1.0' if not is_token_v2_0 else 'v2.0'
 
             request_meta = {
                 'request_type': 'AUTH',
                 'response_time': int((time_perf_counter() - start_time) * 1000),
-                'name': f'{name} {cls.__name__} OAuth2 user token {version}',
+                'name': f'{scenario_index} {cls.__name__} OAuth2 user token {version}',
                 'context': client._context,
                 'response': None,
                 'exception': exception,
                 'response_length': total_response_length,
             }
 
             client.environment.events.request.fire(**request_meta)
```

### Comparing `grizzly-loadtester-2.6.4/grizzly/behave.py` & `grizzly-loadtester-2.6.5/grizzly/behave.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/clients.py` & `grizzly-loadtester-2.6.5/grizzly/clients.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/context.py` & `grizzly-loadtester-2.6.5/grizzly/context.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/exceptions.py` & `grizzly-loadtester-2.6.5/grizzly/exceptions.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/listeners/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/listeners/appinsights.py` & `grizzly-loadtester-2.6.5/grizzly/listeners/appinsights.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/listeners/influxdb.py` & `grizzly-loadtester-2.6.5/grizzly/listeners/influxdb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/locust.py` & `grizzly-loadtester-2.6.5/grizzly/locust.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/scenarios/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/scenarios/iterator.py` & `grizzly-loadtester-2.6.5/grizzly/scenarios/iterator.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/_helpers.py` & `grizzly-loadtester-2.6.5/grizzly/steps/_helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/background/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/steps/background/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/background/setup.py` & `grizzly-loadtester-2.6.5/grizzly/steps/background/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/background/shapes.py` & `grizzly-loadtester-2.6.5/grizzly/steps/background/shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/scenario/response.py` & `grizzly-loadtester-2.6.5/grizzly/steps/scenario/response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/scenario/results.py` & `grizzly-loadtester-2.6.5/grizzly/steps/scenario/results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/scenario/setup.py` & `grizzly-loadtester-2.6.5/grizzly/steps/scenario/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/scenario/tasks.py` & `grizzly-loadtester-2.6.5/grizzly/steps/scenario/tasks.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/scenario/user.py` & `grizzly-loadtester-2.6.5/grizzly/steps/scenario/user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/steps/setup.py` & `grizzly-loadtester-2.6.5/grizzly/steps/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/async_group.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/async_group.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/clients/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/clients/blobstorage.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/clients/blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/clients/http.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/clients/http.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/clients/messagequeue.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/clients/messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/clients/servicebus.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/clients/servicebus.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,20 +59,21 @@
 
 * `<consume>` _bool_ - if messages should be consumed (removed from endpoint), or only peeked at (left on endpoint) (default: `True`)
 
 * `<wait>` _int_ - how many seconds to wait for a message to arrive on the endpoint (default: `∞`)
 
 * `<content type>` _str_ - content type of response payload, should be used in combination with `<expression>`
 """  # noqa: E501
-from typing import Optional, cast
+from typing import Optional, Dict, cast
 from urllib.parse import urlparse, parse_qs
 from platform import node as hostname
 from pathlib import Path
 from textwrap import dedent
 from json import dumps as jsondumps
+from dataclasses import dataclass, field
 
 import zmq.green as zmq
 
 from zmq.sugar.constants import REQ as ZMQ_REQ, LINGER as ZMQ_LINGER
 
 from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageRequest, AsyncMessageResponse
 from grizzly_extras.transformer import TransformerContentType
@@ -83,27 +84,47 @@
 from grizzly.scenarios import GrizzlyScenario
 from grizzly.tasks import template
 from grizzly.utils import async_message_request_wrapper
 
 from . import client, ClientTask, logger  # pylint: disable=unused-import
 
 
+@dataclass
+class State:
+    worker: Optional[str] = field(init=False, default=None)
+    parent: GrizzlyScenario
+    _first_response: Optional[AsyncMessageResponse] = field(init=False, default=None)
+    client: zmq.Socket
+    context: AsyncMessageContext
+
+    @property
+    def parent_id(self) -> int:
+        return id(self.parent.user)
+
+    @property
+    def first_response(self) -> Optional[AsyncMessageResponse]:
+        return self._first_response
+
+    @first_response.setter
+    def first_response(self, value: Optional[AsyncMessageResponse]) -> None:
+        self._first_response = value
+        if value is not None:
+            self.worker = value.get('worker', None)
+
+
 @template('context')
 @client('sb')
 class ServiceBusClientTask(ClientTask):
     __dependencies__ = set(['async-messaged'])
 
     _zmq_url = 'tcp://127.0.0.1:5554'
     _zmq_context: zmq.Context
 
-    _client: Optional[zmq.Socket] = None
-    worker_id: Optional[str]
+    _state: Dict[GrizzlyScenario, State]
     context: AsyncMessageContext
-    _parent: Optional[GrizzlyScenario]
-    _first_response: Optional[AsyncMessageResponse]
 
     def __init__(
         self,
         direction: RequestDirection,
         endpoint: str,
         name: Optional[str] = None,
         /,
@@ -127,16 +148,14 @@
         )
 
         url = self.endpoint.replace(';', '?', 1).replace(';', '&')
 
         parsed = urlparse(url)
 
         self.endpoint = f'{parsed.scheme}://{parsed.netloc}/;{parsed.query.replace("&", ";")}'
-        self._parent = None
-        self.worker_id = None
         self._zmq_context = zmq.Context()
 
         parameters = parse_qs(parsed.fragment)
 
         try:
             message_wait: Optional[int] = int(parameters.get('MessageWait', ['0'])[0])
             if message_wait is not None and message_wait < 1:
@@ -167,158 +186,147 @@
             'message_wait': message_wait,
             'consume': consume,
         }
 
         if content_type is not None:
             self.context.update({'content_type': content_type})
 
-        self._first_response = None
+        self._state = {}
 
-        # zmq connection to async-messaged must be done when creating the instance
-        self._client = cast(zmq.Socket, self._zmq_context.socket(ZMQ_REQ))
-        self.client.connect(self._zmq_url)
+    def get_state(self, parent: 'GrizzlyScenario') -> State:
+        state = self._state.get(parent, None)
 
-    @property
-    def parent(self) -> GrizzlyScenario:
-        if self._parent is None:
-            raise AttributeError('no parent set')
-
-        return self._parent
-
-    @parent.setter
-    def parent(self, value: GrizzlyScenario) -> None:
-        if self._parent is not None and value is not self._parent:
-            raise AttributeError('parent already set, why are a different parent being set?')
+        if state is None:
+            context = self.context.copy()
+            # add id of user as suffix to subscription name, to make it unique
+            endpoint_arguments = parse_arguments(context['endpoint'], separator=':')
 
-        self._parent = value
+            if 'subscription' in endpoint_arguments:
+                endpoint_arguments['subscription'] = f'{endpoint_arguments["subscription"]}_{id(parent.user)}'
+                context['endpoint'] = ', '.join([f'{key}:{value}' for key, value in endpoint_arguments.items()])
 
-    @property
-    def client(self) -> zmq.Socket:
-        if self._client is None:
-            raise ConnectionError('not connected to async-messaged')
+            state = State(
+                parent=parent,
+                client=cast(zmq.Socket, self._zmq_context.socket(ZMQ_REQ)),
+                context=context,
+            )
+            state.client.connect(self._zmq_url)
+            self._state.update({parent: state})
 
-        return self._client
+        return state
 
     @ClientTask.text.setter  # type: ignore
     def text(self, value: str) -> None:
         self._text = dedent(value).strip()
 
-    def connect(self) -> None:
-        if self.worker_id is not None:
-            logger.debug(f'{id(self.parent.user)}::sb already connected')
-            return
-
-        if self._first_response is not None:
-            self.worker_id = self._first_response.get('worker', None)
+    def connect(self, parent: GrizzlyScenario) -> None:
+        state = self.get_state(parent)
 
-        logger.debug(f'{id(self.parent.user)}::sb connecting, {self.worker_id=}')
+        logger.debug(f'{state.parent_id}::sb connecting, {state.worker=}')
 
         request: AsyncMessageRequest = {
-            'worker': self.worker_id,
+            'worker': state.worker,
             'action': RequestType.HELLO.name,
-            'context': self.context,
+            'context': state.context,
         }
 
-        response = async_message_request_wrapper(self.parent, self.client, request)
+        response = async_message_request_wrapper(parent, state.client, request)
+
+        if state.first_response is None:
+            state.first_response = response
 
-        if self._first_response is None:
-            self.worker_id = response['worker']
-            self._first_response = response
+        logger.debug(f'{state.parent_id}::sb connected to worker {state.worker} at {hostname()}')
 
-        logger.debug(f'{id(self.parent.user)}::sb connected to worker {self.worker_id} at {hostname()}')
+    def disconnect(self, parent: GrizzlyScenario) -> None:
+        state = self.get_state(parent)
 
-    def disconnect(self) -> None:
-        if self._client is None:
+        if state.worker is None:
             return
 
         request: AsyncMessageRequest = {
-            'worker': self.worker_id,
+            'worker': state.worker,
             'action': RequestType.DISCONNECT.name,
-            'context': self.context,
+            'context': state.context,
         }
 
-        async_message_request_wrapper(self.parent, self.client, request)
+        async_message_request_wrapper(parent, state.client, request)
+
+        state.client.setsockopt(ZMQ_LINGER, 0)
+        state.client.close()
+
+        del self._state[parent]
 
-        self.worker_id = None
-        self.client.setsockopt(ZMQ_LINGER, 0)
-        self.client.close()
-        self._client = None
+    def subscribe(self, parent: GrizzlyScenario) -> None:
+        state = self.get_state(parent)
 
-    def subscribe(self) -> None:
         request: AsyncMessageRequest = {
-            'worker': self.worker_id,
+            'worker': state.worker,
             'action': RequestType.SUBSCRIBE.name,
-            'context': self.context,
+            'context': state.context,
             'payload': self.text,
         }
 
-        response = async_message_request_wrapper(self.parent, self.client, request)
+        response = async_message_request_wrapper(parent, state.client, request)
         logger.info(response['message'])
 
-        self._first_response = response
+        state.first_response = response
+
+    def unsubscribe(self, parent: GrizzlyScenario) -> None:
+        state = self.get_state(parent)
 
-    def unsubscribe(self) -> None:
         request: AsyncMessageRequest = {
-            'worker': self.worker_id,
+            'worker': state.worker,
             'action': RequestType.UNSUBSCRIBE.name,
-            'context': self.context,
+            'context': state.context,
         }
 
-        response = async_message_request_wrapper(self.parent, self.client, request)
+        response = async_message_request_wrapper(parent, state.client, request)
         logger.info(response['message'])
 
     def on_start(self, parent: GrizzlyScenario) -> None:
-        self.parent = parent
-
         # create subscription before connecting to it
         if self.text is not None:
-            # add id of user as suffix to subscription name, to make it unique
-            endpoint_arguments = parse_arguments(self.context['endpoint'], separator=':')
+            self.subscribe(parent)
 
-            if 'subscription' in endpoint_arguments:
-                endpoint_arguments['subscription'] = f'{endpoint_arguments["subscription"]}_{id(self.parent)}'
-                self.context['endpoint'] = ', '.join([f'{key}:{value}' for key, value in endpoint_arguments.items()])
-
-            self.subscribe()
-
-        self.connect()
+        self.connect(parent)
 
     def on_stop(self, parent: GrizzlyScenario) -> None:
-        self.parent = parent
-
         if self.text is not None:
-            self.unsubscribe()
+            self.unsubscribe(parent)
 
-        self.disconnect()
+        self.disconnect(parent)
 
     def request(self, parent: GrizzlyScenario, request: AsyncMessageRequest) -> AsyncMessageResponse:
         response = None
+        state = self.get_state(parent)
 
         with self.action(parent) as meta:
             if request['context'].get('url', None) is None:
                 request['context'].update({'url': self.endpoint})
 
-            response = async_message_request_wrapper(parent, self.client, request)
+            response = async_message_request_wrapper(parent, state.client, request)
 
             response_length_source = ((response or {}).get('payload', None) or '').encode('utf-8')
 
             meta.update({
-                'action': self.context['endpoint'],
+                'action': state.context['endpoint'],
                 'request': request.copy(),
                 'response_length': len(response_length_source),
                 'response': response,
             })
 
         return response or {}
 
     def get(self, parent: GrizzlyScenario) -> GrizzlyResponse:
+        state = self.get_state(parent)
+
         request: AsyncMessageRequest = {
             'action': 'RECEIVE',
-            'worker': self.worker_id,
-            'context': self.context,
+            'worker': state.worker,
+            'context': state.context,
             'payload': None,
         }
 
         response = self.request(parent, request)
 
         metadata = response.get('metadata', None)
         payload = response.get('payload', None)
@@ -328,24 +336,26 @@
 
         if metadata is not None and self.metadata_variable is not None:
             parent.user._context['variables'][self.metadata_variable] = jsondumps(metadata)
 
         return metadata, payload
 
     def put(self, parent: GrizzlyScenario) -> GrizzlyResponse:
+        state = self.get_state(parent)
+
         source = parent.render(cast(str, self.source))
         source_file = Path(self._context_root) / 'requests' / source
 
         if source_file.exists():
             source = parent.render(source_file.read_text())
 
         request: AsyncMessageRequest = {
             'action': 'SEND',
-            'worker': self.worker_id,
-            'context': self.context,
+            'worker': state.worker,
+            'context': state.context,
             'payload': source,
         }
 
         response = self.request(parent, request)
 
         metadata = response.get('metadata', None)
         payload = response.get('payload', None)
```

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/conditional.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/conditional.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/date.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/log_message.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/log_message.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/loop.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/loop.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/request.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/request.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/set_variable.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/set_variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,11 +70,12 @@
             if self._variable_instance is None and self._variable_instance_type is not None:
                 self._variable_instance = cast(MutableMapping[str, Any], self._variable_instance_type.get())
 
             value = parent.render(self.value)
 
             if self._variable_instance is not None:
                 self._variable_instance[self._variable_key] = value
-            else:
-                parent.user._context['variables'][self.variable] = value
+
+            # always update user context with new value
+            parent.user._context['variables'][self.variable] = value
 
         return task
```

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/task_wait.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/task_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/timer.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/timer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/transformer.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/until.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/until.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/tasks/wait.py` & `grizzly-loadtester-2.6.5/grizzly/tasks/wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/ast.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/ast.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/communication.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/communication.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,18 @@
                                                         try:
                                                             loaded_variable_datatypes[testdata_type] = variable[variable_name]
                                                         except NotImplementedError:
                                                             continue
 
                                                     value = loaded_variable_datatypes[testdata_type][data_attribute]
                                                 else:
-                                                    value = variable[variable_name]
+                                                    try:
+                                                        value = variable[variable_name]
+                                                    except NotImplementedError:
+                                                        continue
                                             else:
                                                 value = variable
 
                                             if value is None and scenario_name not in self.scenarios_iteration:
                                                 message['action'] = 'stop'
                                                 self.logger.warning(f'{key} does not have a value and iterations is not set for {scenario_name}, stop test')
                                                 data = {}
```

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/utils.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_reader.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/csv_reader.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_writer.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/csv_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 @anchor pydoc:grizzly.testdata.variables.csv_writer CSV Writer
 This variable writes to a CSV file.
 
 The CSV files **must** have headers for each column, since these are used to reference the value.
 
-When all specified headers has been set, the row will be "flushed" and written to the specified destination file.
+When setting the value of the variable there must be one value per specified header.
 
 ## Format
 
 Value is the path, relative to `requests/`, of an file ending with `.csv`.
 
 ## Arguments
 
@@ -16,16 +16,15 @@
 * `overwrite` _bool_ (optional) - if destination file exists and should be overwritten (default: `False`)
 
 ## Example
 
 ``` gherkin
 And value for variable "AtomicCsvWriter.output" is "output.csv | headers='foo,bar'"
 ...
-And value for variable "AtomicCsvWriter.output.foo" is "{{ value }}"
-And value for variable "AtomicCsvWriter.output.bar" is "{{ value }}"
+And value for variable "AtomicCsvWriter.output" is "{{ foo_value }}, {{ bar_value }}"
 ```
 
 '''
 import os
 
 from typing import Dict, Any, Type, Optional, cast
 from csv import DictWriter
@@ -95,15 +94,14 @@
 
 class AtomicCsvWriter(AtomicVariable[str], AtomicVariableSettable):
     __base_type__ = atomiccsvwriter__base_type__
     __initialized: bool = False
     __message_handlers__ = {'atomiccsvwriter': atomiccsvwriter_message_handler}
 
     _settings: Dict[str, Dict[str, Any]]
-    _buffer: Dict[str, Dict[str, Any]]
     arguments: Dict[str, Any] = {'headers': list_type, 'overwrite': bool_type}
 
     def __init__(self, variable: str, value: str, outer_lock: bool = False) -> None:
         with self.semaphore(outer_lock):
             if variable.count('.') != 0:
                 raise ValueError(f'{self.__class__.__name__}.{variable} is not a valid CSV destination name, must be: {self.__class__.__name__}.<name>')
 
@@ -119,57 +117,57 @@
                     settings[argument] = caster(arguments[argument])
 
             super().__init__(variable, value, outer_lock=True)
 
             if self.__initialized:
                 if variable not in self._settings:
                     self._settings[variable] = settings
-                    self._buffer[variable] = {}
 
                 return
 
             self._settings = {variable: settings}
-            self._buffer = {variable: {}}
             self.__initialized = True
 
     @classmethod
     def clear(cls: Type['AtomicCsvWriter']) -> None:
         super().clear()
 
         instance = cast(AtomicCsvWriter, cls.get())
         variables = list(instance._settings.keys())
 
         for variable in variables:
             del instance._settings[variable]
-            del instance._buffer[variable]
 
     def __getitem__(self, variable: str) -> Optional[str]:
         raise NotImplementedError(f'{self.__class__.__name__} has not implemented "__getitem__"')  # pragma: no cover
 
     def __setitem__(self, variable: str, value: Optional[str]) -> None:
         if value is None or isinstance(self.grizzly.state.locust, MasterRunner):
             return
 
-        if variable.count('.') < 1:
+        if variable not in self._settings:
             raise ValueError(f'{self.__class__.__name__}.{variable} is not a valid reference')
 
-        variable, header = variable.split('.', 1)
+        values = [v.strip() for v in value.split(',')]
 
-        if header not in self._settings[variable].get('headers', []):
-            raise ValueError(f'{self.__class__.__name__}.{variable} has not specified header "{header}"')
+        headers = self._settings[variable].get('headers', [])
+        values_count = len(values)
+        header_count = len(headers)
+
+        if values_count != header_count:
+            delta = values_count - header_count
+            if delta < 0:
+                diff_text = 'less'
+            else:
+                diff_text = 'more'
 
-        buffer = self._buffer.get(variable, {})
+            raise ValueError(f'{self.__class__.__name__}.{variable}: {diff_text} values ({values_count}) than headers ({header_count})')
 
-        if header in buffer:
-            raise ValueError(f'{self.__class__.__name__}.{variable} has already set value for "{header}" in current row')
-
-        buffer.update({header: value})
+        buffer = {key: value for key, value in zip(headers, values)}
 
         # values for all headers set, flush to file
-        if list(buffer.keys()) == self._settings[variable].get('headers', []):
-            data = {
-                'destination': self._settings[variable]['destination'],
-                'row': buffer.copy(),
-            }
+        data = {
+            'destination': self._settings[variable]['destination'],
+            'row': buffer,
+        }
 
-            self.grizzly.state.locust.send_message('atomiccsvwriter', data)
-            self._buffer[variable].clear()
+        self.grizzly.state.locust.send_message('atomiccsvwriter', data)
```

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/date.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/directory_contents.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/directory_contents.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/integer_incrementer.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/integer_incrementer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_integer.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/random_integer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_string.py` & `grizzly-loadtester-2.6.5/grizzly/testdata/variables/random_string.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/types/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/types/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/types/locust.py` & `grizzly-loadtester-2.6.5/grizzly/types/locust.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/users/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/base/__init__.py` & `grizzly-loadtester-2.6.5/grizzly/users/base/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/base/grizzly_user.py` & `grizzly-loadtester-2.6.5/grizzly/users/base/grizzly_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/base/request_logger.py` & `grizzly-loadtester-2.6.5/grizzly/users/base/request_logger.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/base/response_event.py` & `grizzly-loadtester-2.6.5/grizzly/users/base/response_event.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/base/response_handler.py` & `grizzly-loadtester-2.6.5/grizzly/users/base/response_handler.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/blobstorage.py` & `grizzly-loadtester-2.6.5/grizzly/users/blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/dummy.py` & `grizzly-loadtester-2.6.5/grizzly/users/dummy.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/iothub.py` & `grizzly-loadtester-2.6.5/grizzly/users/iothub.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/messagequeue.py` & `grizzly-loadtester-2.6.5/grizzly/users/messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/restapi.py` & `grizzly-loadtester-2.6.5/grizzly/users/restapi.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/servicebus.py` & `grizzly-loadtester-2.6.5/grizzly/users/servicebus.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/users/sftp.py` & `grizzly-loadtester-2.6.5/grizzly/users/sftp.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly/utils.py` & `grizzly-loadtester-2.6.5/grizzly/utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/arguments.py` & `grizzly-loadtester-2.6.5/grizzly_extras/arguments.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/async_message/__init__.py` & `grizzly-loadtester-2.6.5/grizzly_extras/async_message/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     worker: str
     message_wait: Optional[int]
     logger: ThreadLogger
 
     def __init__(self, worker: str) -> None:
         self.worker = worker
         self.message_wait = None
-        self.logger = ThreadLogger(f'handler::{worker}')
+        self.logger = ThreadLogger(f'handler::{self.__class__.__name__}::{worker}')
 
         # silence uamqp loggers
         for uamqp_logger_name in ['uamqp', 'uamqp.c_uamqp']:
             logging.getLogger(uamqp_logger_name).setLevel(logging.ERROR)
 
     @abstractmethod
     def get_handler(self, action: str) -> Optional['AsyncMessageRequestHandler']:
```

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/async_message/daemon.py` & `grizzly-loadtester-2.6.5/grizzly_extras/async_message/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,17 +145,15 @@
                 worker_id = request_worker_id
 
                 if payload.get('worker', None) is None:
                     payload['worker'] = worker_id
 
             request = jsondumps(payload).encode()
             backend_request = [worker_id.encode(), SPLITTER_FRAME, request_id, SPLITTER_FRAME, request]
-            logger.debug(f'{backend_request=}')
             backend.send_multipart(backend_request)
-            logger.debug(f'forwarding frontend request to worker {request_worker_id}')
 
     logger.info('stopping')
     for worker_thread in worker_threads:
         logger.debug(f'waiting for {worker_thread.ident}')
         worker_thread.join()
 
     try:
```

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/__init__.py` & `grizzly-loadtester-2.6.5/grizzly_extras/async_message/mq/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/rfh2.py` & `grizzly-loadtester-2.6.5/grizzly_extras/async_message/mq/rfh2.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/async_message/sb.py` & `grizzly-loadtester-2.6.5/grizzly_extras/async_message/sb.py`

 * *Files 4% similar despite different names*

```diff
@@ -469,14 +469,15 @@
         cache_endpoint = ', '.join([f'{key}:{value}' for key, value in endpoint_arguments.items()])
 
         self.logger.info(f'handling request towards {cache_endpoint}')
 
         message: Optional[ServiceBusMessage] = None
         metadata: Optional[Dict[str, Any]] = None
         payload = request.get('payload', None)
+        client = request.get('client', -1)
 
         if instance_type not in ['receiver', 'sender']:
             raise AsyncMessageError(f'"{instance_type}" is not a valid value for context.connection')
 
         arguments = self._arguments.get(f'{instance_type}={cache_endpoint}', None)
 
         if arguments is None:
@@ -520,18 +521,18 @@
                             get_values = transform.parser(request_arguments['expression'])
                         except Exception as e:
                             raise AsyncMessageError(str(e)) from e
 
                     for received_message in receiver:
                         message = cast(ServiceBusReceivedMessage, received_message)
 
-                        self.logger.debug(f'got message id: {message.message_id}')
+                        self.logger.debug(f'{client}::{cache_endpoint}: got message id {message.message_id}')
 
                         if expression is None:
-                            self.logger.debug(f'completing message id: {message.message_id}')
+                            self.logger.debug(f'{client}::{cache_endpoint}: completing message id {message.message_id}')
                             receiver.complete_message(message)
                             break
 
                         had_error = True
                         try:
                             metadata, payload = self.from_message(message)
 
@@ -542,59 +543,62 @@
                                 transformed_payload = transform.transform(payload)
                             except TransformerError as e:
                                 self.logger.error(payload)
                                 raise AsyncMessageError(e.message)
 
                             values = get_values(transformed_payload)
 
-                            self.logger.debug(f'expression={request_arguments["expression"]}, matches={values}, payload={transformed_payload}')
+                            self.logger.debug(f'{client}::{cache_endpoint}: expression={request_arguments["expression"]}, matches={values}, payload={transformed_payload}')
 
                             if len(values) > 0:
-                                self.logger.debug(f'completing message id: {message.message_id}, with expression "{request_arguments["expression"]}"')
+                                self.logger.debug(f'{client}::{cache_endpoint}: completing message id {message.message_id}, with expression "{request_arguments["expression"]}"')
                                 receiver.complete_message(message)
                                 had_error = False
                                 break
                         except:
                             raise
                         finally:
                             if had_error:
                                 if message is not None:
                                     if not consume:
-                                        self.logger.debug(f'abandoning message id: {message.message_id}, {message._raw_amqp_message.header.delivery_count}')
+                                        self.logger.debug(
+                                            f'{client}::{cache_endpoint}: abandoning message id {message.message_id}, {message._raw_amqp_message.header.delivery_count}',
+                                        )
                                         receiver.abandon_message(message)
                                         message = None
                                     else:
-                                        self.logger.debug(f'consuming and ignoring message id: {message.message_id}')
+                                        self.logger.debug(f'{client}::{cache_endpoint}: consuming and ignoring message id {message.message_id}')
                                         receiver.complete_message(message)  # remove message from endpoint, but ignore contents
-                                        payload = metadata = None
+                                        message = payload = metadata = None
 
                                 if message_wait > 0 and (perf_counter() - wait_start) >= message_wait:
                                     raise StopIteration()
 
                                 sleep(0.2)
 
                     if message is None:
                         raise StopIteration()
 
                     break
                 except StopIteration:
-                    if message_wait > 0:
-                        receiver._handler._last_activity_timestamp = None
                     delta = perf_counter() - wait_start
 
                     if message_wait > 0:
                         if delta >= message_wait:
                             error_message = f'no messages on {endpoint}'
                             message = None
                             if message_wait > 0:
                                 error_message = f'{error_message} within {message_wait} seconds'
+                        elif consume and expression is not None:
+                            self.logger.debug(f'{client}::{cache_endpoint}: waiting for more messages')
+                            continue
                         else:
                             # ugly brute-force way of handling no messages on service bus
                             if retry < 3:
-                                self.logger.warning(f'receiver for {cache_endpoint} returned no message without trying, brute-force retry #{retry}')
+                                self.logger.warning(f'receiver for {client}::{cache_endpoint} returned no message without trying, brute-force retry #{retry}')
                                 # <!-- useful debugging information, actual message count on message entity
                                 if self.logger._logger.level == logging.DEBUG and self.mgmt_client is not None:
                                     if 'topic' in endpoint_arguments:
                                         topic_properties = self.mgmt_client.get_subscription_runtime_properties(
                                             topic_name=endpoint_arguments['topic'],
                                             subscription_name=endpoint_arguments['subscription']
                                         )
```

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/text.py` & `grizzly-loadtester-2.6.5/grizzly_extras/text.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_extras/transformer.py` & `grizzly-loadtester-2.6.5/grizzly_extras/transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/PKG-INFO` & `grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester
-Version: 2.6.4
+Version: 2.6.5
 Summary: Traffic generator based on locust and behave
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,load,loadtest,performance,traffic generator
```

### Comparing `grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/SOURCES.txt` & `grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/requires.txt` & `grizzly-loadtester-2.6.5/grizzly_loadtester.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/pyproject.toml` & `grizzly-loadtester-2.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/script/docs-generate-changelog.py` & `grizzly-loadtester-2.6.5/script/docs-generate-changelog.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/script/docs-generate-licenses.py` & `grizzly-loadtester-2.6.5/script/docs-generate-licenses.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/script/docs-generate.bash` & `grizzly-loadtester-2.6.5/script/docs-generate.bash`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/conftest.py` & `grizzly-loadtester-2.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_setup.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/background/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_shapes.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/background/test_shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_response.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_results.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_setup.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_tasks.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_tasks.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_user.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/scenario/test_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/test_setup.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/test_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,23 +41,22 @@
 
 
 def test_e2e_step_setup_variable_value(e2e_fixture: End2EndFixture) -> None:
     def validate_variables(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         assert grizzly.state.variables['AtomicCsvWriter.output'] == "output.csv | headers='foo, bar'"
-        assert len(grizzly.scenario.tasks()) == 3 + 1
+        assert len(grizzly.scenario.tasks()) == 2 + 1
 
     e2e_fixture.add_validator(validate_variables)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'And value for variable "AtomicCsvWriter.output" is "output.csv | headers=\'foo, bar\'"',
-            'And value for variable "AtomicCsvWriter.output.foo" is "bar"',
-            'And value for variable "AtomicCsvWriter.output.bar" is "foo"',
+            'And value for variable "AtomicCsvWriter.output" is "bar, foo"',
             'And value for variable "foobar" is "foobar"',
             'And value for variable "foobar" is "foobaz"',
         ]
     )
 
     assert e2e_fixture._root is not None
```

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/steps/test_utils.py` & `grizzly-loadtester-2.6.5/tests/e2e/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_auth.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_auth.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_example.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_example.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_failure.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_failure.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_iteration_pace.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_iteration_pace.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_persistence.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_persistence.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_until.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_until.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/e2e/test_variables.py` & `grizzly-loadtester-2.6.5/tests/e2e/test_variables.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/fixtures.py` & `grizzly-loadtester-2.6.5/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/helpers.py` & `grizzly-loadtester-2.6.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/auth/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/test_aad.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/auth/test_aad.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_appinsights.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/test_appinsights.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_influxdb.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/listeners/test_influxdb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/test_iterator.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/scenarios/test_iterator.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_setup.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/background/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_shapes.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/background/test_shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_response.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_results.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_setup.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_tasks.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_tasks.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_user.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/scenario/test_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test__helpers.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/test__helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test_setup.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/steps/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_http.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_http.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_servicebus.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/clients/test_servicebus.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Dict, Any
 from json import dumps as jsondumps
 
 import pytest
 
 from _pytest.logging import LogCaptureFixture
-from zmq.sugar.constants import LINGER as ZMQ_LINGER, REQ as ZMQ_REQ
+from zmq.sugar.constants import LINGER as ZMQ_LINGER
 from grizzly.tasks.clients import ServiceBusClientTask
 from grizzly.types import RequestDirection
 from grizzly_extras.async_message import AsyncMessageRequest
 
 from tests.fixtures import GrizzlyFixture, NoopZmqFixture, MockerFixture
 
 
@@ -24,20 +24,18 @@
         assert task.context == {
             'url': task.endpoint,
             'connection': 'receiver',
             'endpoint': '',
             'message_wait': None,
             'consume': False,
         }
-        assert task.worker_id is None
+        assert task._state == {}
         assert task.text is None
         assert task.get_templates() == []
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
-        context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
         context_mock.reset_mock()
 
         task = ServiceBusClientTask(
             RequestDirection.TO,
             'sb://my-sbns.servicebus.windows.net/queue:my-queue;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
             source='hello world!'
@@ -49,20 +47,18 @@
             'connection': 'sender',
             'endpoint': 'queue:my-queue',
             'message_wait': None,
             'consume': False,
         }
         assert task.text is None
         assert task.source == 'hello world!'
-        assert task.worker_id is None
+        assert task._state == {}
         assert task.__template_attributes__ == {'endpoint', 'destination', 'source', 'name', 'variable_template', 'context'}
         assert task.get_templates() == []
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
-        context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
         context_mock.reset_mock()
 
         grizzly = grizzly_fixture.grizzly
         grizzly.state.configuration.update({'sbns.host': 'sb.windows.net', 'sbns.key.name': 'KeyName', 'sbns.key.secret': 'SeCrEtKeY=='})
         grizzly.state.variables.update({'foobar': 'none'})
 
         task = ServiceBusClientTask(
@@ -85,19 +81,17 @@
             'message_wait': 300,
             'content_type': 'JSON'
         }
         assert task.text == 'foobar'
         assert task.payload_variable == 'foobar'
         assert task.metadata_variable is None
         assert task.source is None
-        assert task.worker_id is None
+        assert task._state == {}
         assert sorted(task.get_templates()) == sorted(['topic:my-topic, subscription:my-subscription-{{ id }}, expression:$.hello.world', '{{ foobar }}'])
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
-        context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
         context_mock.reset_mock()
 
         grizzly.state.variables.update({'barfoo': 'none'})
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             (
@@ -119,19 +113,17 @@
             'message_wait': 300,
             'content_type': 'JSON'
         }
         assert task.text == 'foobar'
         assert task.payload_variable == 'foobar'
         assert task.metadata_variable == 'barfoo'
         assert task.source is None
-        assert task.worker_id is None
+        assert task._state == {}
         assert sorted(task.get_templates()) == sorted(['topic:my-topic, subscription:my-subscription-{{ id }}, expression:$.hello.world', '{{ foobar }} {{ barfoo }}'])
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
-        context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
         context_mock.reset_mock()
 
         task = ServiceBusClientTask(
             RequestDirection.FROM, (
                 'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription'
                 ';SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=#MessageWait=120&ContentType=json'
             ),
@@ -143,51 +135,46 @@
             'url': task.endpoint,
             'connection': 'receiver',
             'endpoint': 'topic:my-topic, subscription:my-subscription',
             'message_wait': 120,
             'consume': False,
             'content_type': 'JSON',
         }
-        assert task.worker_id is None
+        assert task._state == {}
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
-        context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
         context_mock.reset_mock()
 
         with pytest.raises(ValueError) as ve:
             ServiceBusClientTask(
                 RequestDirection.FROM,
                 'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=#MessageWait=foo',
                 'test',
             )
         assert str(ve.value) == 'MessageWait parameter in endpoint fragment is not a valid integer'
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_not_called()
         context_mock.reset_mock()
 
         with pytest.raises(ValueError) as ve:
             ServiceBusClientTask(
                 RequestDirection.FROM,
                 'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=#Consume=foo',
                 'test',
             )
         assert str(ve.value) == 'Consume parameter in endpoint fragment is not a valid boolean'
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_not_called()
         context_mock.reset_mock()
 
         with pytest.raises(ValueError) as ve:
             ServiceBusClientTask(
                 RequestDirection.FROM,
                 'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=#ContentType=foo',
                 'test',
             )
         assert str(ve.value) == '"foo" is an unknown response content type'
         context_mock.assert_called_once_with()
-        context_mock.return_value.socket.assert_not_called()
         context_mock.reset_mock()
 
     def test_text(self, grizzly_fixture: GrizzlyFixture) -> None:
         task = ServiceBusClientTask(RequestDirection.FROM, 'sb://my-sbns.servicebus.windows.net/;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=', 'test')
 
         assert task.text is None
 
@@ -207,107 +194,107 @@
 
         noop_zmq('grizzly.tasks.clients.servicebus')
 
         async_message_request_mock = mocker.patch('grizzly.utils.async_message_request')
 
         grizzly_fixture.grizzly.state.configuration.update({'sbns.key.secret': 'fooBARfoo'})
 
-        task = ServiceBusClientTask(RequestDirection.FROM, 'sb://my-sbns.servicebus.windows.net/;SharedAccessKeyName=AccessKey;SharedAccessKey=$conf::sbns.key.secret$', 'test')
-
-        task._parent = scenario
-
-        # already connected
-        task.worker_id = 'foo-bar'
-
-        task.connect()
-
-        async_message_request_mock.assert_not_called()
+        task = ServiceBusClientTask(
+            RequestDirection.FROM,
+            'sb://my-sbns.servicebus.windows.net/queue:my-queue;SharedAccessKeyName=AccessKey;SharedAccessKey=$conf::sbns.key.secret$',
+            'test',
+        )
 
         # successfully connected
-        task.worker_id = None
+        assert task._state == {}
         async_message_request_mock.return_value = {'success': True, 'worker': 'foo-bar-baz-foo'}
 
-        task.connect()
+        task.connect(scenario)
+
+        state = task.get_state(scenario)
 
-        assert task.worker_id == 'foo-bar-baz-foo'
+        assert state.worker == 'foo-bar-baz-foo'
+        assert state.parent is scenario
         assert task.endpoint == 'sb://my-sbns.servicebus.windows.net/;SharedAccessKeyName=AccessKey;SharedAccessKey=fooBARfoo'
 
-        async_message_request_mock.assert_called_once_with(task.client, {
+        async_message_request_mock.assert_called_once_with(state.client, {
             'worker': None,
-            'client': id(scenario.user),
+            'client': state.parent_id,
             'action': 'HELLO',
-            'context': task.context,
+            'context': state.context,
         })
 
     def test_disconnect(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
         assert scenario is not None
 
         client_mock = mocker.MagicMock()
 
         async_message_request_mock = mocker.patch('grizzly.utils.async_message_request')
 
-        task = ServiceBusClientTask(RequestDirection.FROM, 'sb://my-sbns.servicebus.windows.net/;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=', 'test')
-        task._parent = scenario
+        task = ServiceBusClientTask(
+            RequestDirection.FROM,
+            'sb://my-sbns.servicebus.windows.net/queue:my-queue;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
+            'test',
+        )
 
         # not connected, don't do anything
-        task._client = None
-        task.disconnect()
+        task.disconnect(scenario)
 
-        client_mock.close.assert_not_called()
+        async_message_request_mock.assert_not_called()
 
         # connected
-        task._client = client_mock
-        task.worker_id = 'foo-bar-baz-foo'
+        state = task.get_state(scenario)
+        state.worker = 'foo-bar-baz-foo'
+        state.client = client_mock
 
-        task.disconnect()
+        task.disconnect(scenario)
 
         async_message_request_mock.assert_called_once_with(client_mock, {
             'worker': 'foo-bar-baz-foo',
-            'client': id(task.parent.user),
+            'client': state.parent_id,
             'action': 'DISCONNECT',
-            'context': task.context,
+            'context': state.context,
         })
         client_mock.setsockopt.assert_called_once_with(ZMQ_LINGER, 0)
         client_mock.close.assert_called_once_with()
 
-        assert getattr(task, 'worker_id', True) is None
-        assert task._client is None
+        assert task._state == {}
 
     def test_subscribe(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture, caplog: LogCaptureFixture) -> None:
         _, _, scenario = grizzly_fixture()
         assert scenario is not None
 
         client_mock = mocker.MagicMock()
 
         async_message_request_mock = mocker.patch('grizzly.utils.async_message_request', return_value={'message': 'foobar!'})
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
-            'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription-{{ id }};SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
+            'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:"my-subscription-{{ id }}";SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
 
-        task._parent = scenario
+        state = task.get_state(scenario)
 
-        task._client = client_mock
-        task.worker_id = 'foo-bar-baz'
+        state.worker = 'foo-bar-baz'
+        state.client = client_mock
         task._text = '1={{ condition }}'
 
         scenario.user._context['variables'].update({'id': 'baz-bar-foo', 'condition': '2'})
-        expected_context = task.context.copy()
+        expected_context = state.context.copy()
         expected_context['endpoint'] = expected_context['endpoint'].replace('{{ id }}', 'baz-bar-foo')
 
         with caplog.at_level(logging.INFO):
-            task.subscribe()
+            task.subscribe(scenario)
 
         assert caplog.messages == ['foobar!']
         async_message_request_mock.assert_called_once_with(client_mock, {
             'worker': 'foo-bar-baz',
-            'client': id(scenario.user),
+            'client': state.parent_id,
             'action': 'SUBSCRIBE',
             'context': expected_context,
             'payload': '1=2'
         })
 
     def test_unsubscribe(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture, caplog: LogCaptureFixture) -> None:
         _, _, scenario = grizzly_fixture()
@@ -319,29 +306,28 @@
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
 
-        task._parent = scenario
-
-        task._client = client_mock
-        task.worker_id = 'foo-bar-baz'
+        state = task.get_state(scenario)
+        state.client = client_mock
+        state.worker = 'foo-bar-baz'
 
         with caplog.at_level(logging.INFO):
-            task.unsubscribe()
+            task.unsubscribe(scenario)
 
         assert caplog.messages == ['hello world!']
 
         async_message_request_mock.assert_called_once_with(client_mock, {
             'worker': 'foo-bar-baz',
-            'client': id(task.parent.user),
+            'client': id(scenario.user),
             'action': 'UNSUBSCRIBE',
-            'context': task.context,
+            'context': state.context,
         })
 
     def test_on_start(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
 
         assert scenario is not None
 
@@ -350,34 +336,36 @@
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
 
         connect_mock = mocker.patch.object(task, 'connect', return_value=None)
         subscribe_mock = mocker.patch.object(task, 'subscribe', return_value=None)
 
+        state = task.get_state(scenario)
+
         # no text
         assert task._text is None
 
         task.on_start(scenario)
 
-        connect_mock.assert_called_once_with()
+        connect_mock.assert_called_once_with(scenario)
         subscribe_mock.assert_not_called()
         assert task.context.get('endpoint', None) == 'topic:my-topic, subscription:my-subscription'
 
         connect_mock.reset_mock()
         subscribe_mock.reset_mock()
 
         # text
         task._text = '1=1'
 
         task.on_start(scenario)
 
-        connect_mock.assert_called_once_with()
-        subscribe_mock.assert_called_once_with()
-        assert task.context.get('endpoint', None) == f'topic:my-topic, subscription:my-subscription_{id(scenario)}'
+        connect_mock.assert_called_once_with(scenario)
+        subscribe_mock.assert_called_once_with(scenario)
+        assert state.context.get('endpoint', None) == f'topic:my-topic, subscription:my-subscription_{id(scenario.user)}'
 
     def test_on_stop(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
 
         assert scenario is not None
 
         task = ServiceBusClientTask(
@@ -390,27 +378,27 @@
         unsubscribe_mock = mocker.patch.object(task, 'unsubscribe', return_value=None)
 
         # no text
         assert task._text is None
 
         task.on_stop(scenario)
 
-        disconnect_mock.assert_called_once_with()
+        disconnect_mock.assert_called_once_with(scenario)
         unsubscribe_mock.assert_not_called()
 
         disconnect_mock.reset_mock()
         unsubscribe_mock.reset_mock()
 
         # text
         task._text = '1=1'
 
         task.on_stop(scenario)
 
-        disconnect_mock.assert_called_once_with()
-        unsubscribe_mock.assert_called_once_with()
+        disconnect_mock.assert_called_once_with(scenario)
+        unsubscribe_mock.assert_called_once_with(scenario)
 
     def test_request(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
 
         assert scenario is not None
 
         client_mock = mocker.MagicMock()
@@ -418,55 +406,54 @@
         async_message_request_mock = mocker.patch('grizzly.utils.async_message_request', return_value={'message': 'foobar!'})
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
-        task._client = client_mock
-        task._parent = scenario
-
+        state = task.get_state(scenario)
+        state.client = client_mock
         action_mock = mocker.MagicMock()
         meta_mock: Dict[str, Any] = {}
         action_mock.__enter__.return_value = meta_mock
         context_mock = mocker.patch.object(task, 'action', return_value=action_mock)
 
         # got response, empty payload
         request: AsyncMessageRequest = {
             'context': task.context,
         }
 
-        assert task.request(task.parent, request) == {'message': 'foobar!'}
+        assert task.request(scenario, request) == {'message': 'foobar!'}
 
-        context_mock.assert_called_once_with(task.parent)
-        request.update({'client': id(task.parent.user)})
-        async_message_request_mock.assert_called_once_with(client_mock, request)
+        context_mock.assert_called_once_with(state.parent)
+        request.update({'client': state.parent_id})
+        async_message_request_mock.assert_called_once_with(state.client, request)
         del request['client']
 
         assert meta_mock == {
-            'action': 'topic:my-topic, subscription:my-subscription',
+            'action': state.context.get('endpoint', None),
             'request': request,
             'response_length': 0,
             'response': {'message': 'foobar!'}
         }
 
         context_mock.reset_mock()
         async_message_request_mock.reset_mock()
         meta_mock.clear()
 
         # got response, some payload
         del request['context']['url']
         async_message_request_mock = mocker.patch('grizzly.tasks.clients.servicebus.async_message_request_wrapper', return_value={'message': 'foobar!', 'payload': '1234567890'})
 
-        assert task.request(task.parent, request) == {'message': 'foobar!', 'payload': '1234567890'}
+        assert task.request(scenario, request) == {'message': 'foobar!', 'payload': '1234567890'}
 
-        context_mock.assert_called_once_with(task.parent)
-        async_message_request_mock.assert_called_once_with(task.parent, client_mock, request)
+        context_mock.assert_called_once_with(state.parent)
+        async_message_request_mock.assert_called_once_with(state.parent, state.client, request)
         assert meta_mock == {
-            'action': 'topic:my-topic, subscription:my-subscription',
+            'action': f'topic:my-topic, subscription:my-subscription_{state.parent_id}',
             'request': request,
             'response_length': 10,
             'response': {'message': 'foobar!', 'payload': '1234567890'}
         }
 
     def test_get(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
@@ -477,163 +464,136 @@
         scenario.user._context = {'variables': {}}
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
-        task._client = client_mock
-        task._parent = scenario
-        task.worker_id = 'foo-bar'
+        state = task.get_state(scenario)
+        state.client = client_mock
+        state.worker = 'foo-bar'
 
         request_mock = mocker.patch.object(task, 'request', return_value={'metadata': None, 'payload': 'foobar'})
 
         # no variables
         task.payload_variable = None
 
-        assert task.get(task.parent) == (None, 'foobar',)
+        assert task.get(scenario) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'RECEIVE',
             'worker': 'foo-bar',
-            'context': task.context,
+            'context': state.context,
             'payload': None,
         })
 
-        assert task.parent.user._context['variables'] == {}
+        assert scenario.user._context['variables'] == {}
 
         request_mock.reset_mock()
 
         # with payload variable
         task.payload_variable = 'foobaz'
 
-        assert task.get(task.parent) == (None, 'foobar',)
+        assert task.get(scenario) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'RECEIVE',
             'worker': 'foo-bar',
-            'context': task.context,
+            'context': state.context,
             'payload': None,
         })
 
-        assert task.parent.user._context['variables'] == {'foobaz': 'foobar'}
+        assert scenario.user._context['variables'] == {'foobaz': 'foobar'}
 
         # with payload and metadata variable
         task.payload_variable = 'foobaz'
         task.metadata_variable = 'bazfoo'
         request_mock = mocker.patch.object(task, 'request', return_value={'metadata': {'x-foo-bar': 'hello'}, 'payload': 'foobar'})
 
-        assert task.get(task.parent) == ({'x-foo-bar': 'hello'}, 'foobar',)
+        assert task.get(scenario) == ({'x-foo-bar': 'hello'}, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'RECEIVE',
             'worker': 'foo-bar',
-            'context': task.context,
+            'context': state.context,
             'payload': None,
         })
 
-        assert task.parent.user._context['variables'] == {'foobaz': 'foobar', 'bazfoo': jsondumps({'x-foo-bar': 'hello'})}
+        assert scenario.user._context['variables'] == {'foobaz': 'foobar', 'bazfoo': jsondumps({'x-foo-bar': 'hello'})}
 
     def test_put(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
         assert scenario is not None
 
         client_mock = mocker.MagicMock()
         scenario.user._context = {'variables': {}}
 
         task = ServiceBusClientTask(
             RequestDirection.TO,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
             source='hello world',
         )
-        task._client = client_mock
-        task._parent = scenario
-        task.worker_id = 'foo-baz'
+        state = task.get_state(scenario)
+        state.client = client_mock
+        state.worker = 'foo-baz'
 
         request_mock = mocker.patch.object(task, 'request', return_value={'metadata': None, 'payload': 'foobar'})
 
         # inline source, no file
-        assert task.put(task.parent) == (None, 'foobar',)
+        assert task.put(scenario) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
-            'context': task.context,
+            'context': state.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
 
         # inline source, template
         task.source = '{{ foobar }}'
         scenario.user._context['variables'].update({'foobar': 'hello world'})
 
-        assert task.put(task.parent) == (None, 'foobar',)
+        assert task.put(scenario) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
-            'context': task.context,
+            'context': state.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
         del scenario.user._context['variables']['foobar']
 
         # source file
         (grizzly_fixture.test_context / 'source.json').write_text('hello world')
         task.source = 'source.json'
 
-        assert task.put(task.parent) == (None, 'foobar',)
+        assert task.put(scenario) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
-            'context': task.context,
+            'context': state.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
 
         # source file, with template
         scenario.user._context['variables'].update({'foobar': 'hello world', 'filename': 'source.j2.json'})
         (grizzly_fixture.test_context / 'source.j2.json').write_text('{{ foobar }}')
         task.source = '{{ filename }}'
 
-        assert task.put(task.parent) == (None, 'foobar',)
+        assert task.put(scenario) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(task.parent, {
+        request_mock.assert_called_once_with(state.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
-            'context': task.context,
+            'context': state.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
-
-    def test_parent(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
-        _, _, scenario = grizzly_fixture()
-        assert scenario is not None
-
-        client_mock = mocker.MagicMock()
-
-        task = ServiceBusClientTask(
-            RequestDirection.TO,
-            'sb://my-sbns.servicebus.windows.net/topic:my-topic;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
-            'test',
-            source='hello world',
-        )
-
-        task._client = client_mock
-
-        with pytest.raises(AttributeError) as ae:
-            _ = task.parent
-        assert str(ae.value) == 'no parent set'
-
-        task.parent = mocker.MagicMock()
-
-        _ = task.parent
-
-        with pytest.raises(AttributeError) as ae:
-            task.parent = scenario
-        assert str(ae.value) == 'parent already set, why are a different parent being set?'
```

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_async_group.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_async_group.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_conditional.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_conditional.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_date.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_log_message.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_log_message.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_loop.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_loop.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_request.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_request.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_set_variable.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_set_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
             scenario.user._context['variables'].clear()
 
             # settable Atomic variable
             set_value_mock = mocker.patch('grizzly.testdata.variables.csv_writer.AtomicCsvWriter.__setitem__', return_value=None)
 
             grizzly_fixture.grizzly.state.variables.update({'AtomicCsvWriter.output': 'output.csv | headers="foo,bar"'})
             GrizzlyVariables.initialize_variable(grizzly_fixture.grizzly, 'AtomicCsvWriter.output')
-            task_factory_foo = SetVariableTask('AtomicCsvWriter.output.foo', '{{ value }}')
-            scenario.user._context['variables'].update({'value': 'hello world!'})
+            task_factory_foo = SetVariableTask('AtomicCsvWriter.output', '{{ value }}')
+            scenario.user._context['variables'].update({'value': 'hello, world!'})
 
             task = task_factory_foo()
             task(scenario)
 
-            set_value_mock.assert_called_once_with('output.foo', 'hello world!')
+            set_value_mock.assert_called_once_with('output', 'hello, world!')
             assert 'AtomicCsvWriter.output.foo' not in scenario.user._context['variables']
         finally:
             cleanup()
```

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_task_wait.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_task_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_timer.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_timer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_transformer.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_until.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_until.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_wait.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/tasks/test_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_behave.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_behave.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_clients.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_clients.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_context.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_context.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_locust.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_locust.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_types.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_types.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_utils.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_ast.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test_ast.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_communication.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test_communication.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from grizzly.types.locust import StopUser
 from grizzly.testdata.communication import TestdataConsumer, TestdataProducer
 from grizzly.testdata.utils import initialize_testdata, transform
 from grizzly.testdata.variables import AtomicIntegerIncrementer
 from grizzly.context import GrizzlyContext
 from grizzly.tasks import LogMessageTask
+from grizzly.testdata.variables.csv_writer import atomiccsvwriter_message_handler
 
 from tests.fixtures import AtomicVariableCleanupFixture, BehaveFixture, GrizzlyFixture, NoopZmqFixture
 
 
 class TestTestdataProducer:
     def test_run_with_behave(
         self,
@@ -69,18 +70,20 @@
             source['result']['IntWithStep'] = '{{ AtomicIntegerIncrementer.value }}'
             source['result']['UtcDate'] = '{{ AtomicDate.utc }}'
             source['result']['CustomVariable'] = '{{ tests.helpers.AtomicCustomVariable.foo }}'
 
             grizzly = cast(GrizzlyContext, behave_fixture.context.grizzly)
             grizzly.scenarios.clear()
             grizzly.scenarios.create(behave_fixture.create_scenario(scenario.__class__.__name__))
+            grizzly.scenario.orphan_templates.append('{{ AtomicCsvWriter.output }}')
             grizzly.state.variables['messageID'] = 123
             grizzly.state.variables['AtomicIntegerIncrementer.messageID'] = 456
             grizzly.state.variables['AtomicDirectoryContents.test'] = 'adirectory'
             grizzly.state.variables['AtomicCsvReader.test'] = 'test.csv'
+            grizzly.state.variables['AtomicCsvWriter.output'] = 'output.csv | headers="foo,bar"'
             grizzly.state.alias['AtomicCsvReader.test.header1'] = 'auth.user.username'
             grizzly.state.alias['AtomicCsvReader.test.header2'] = 'auth.user.password'
             grizzly.state.variables['AtomicIntegerIncrementer.value'] = '1 | step=5, persist=True'
             grizzly.state.variables['AtomicDate.utc'] = "now | format='%Y-%m-%dT%H:%M:%S.000Z', timezone=UTC"
             grizzly.state.variables['AtomicDate.now'] = 'now'
             grizzly.state.variables['tests.helpers.AtomicCustomVariable.foo'] = 'bar'
             grizzly.state.variables['world'] = 'hello!'
@@ -92,15 +95,15 @@
 
             grizzly.scenario.tasks.add(request)
             grizzly.scenario.tasks.add(LogMessageTask(message='hello {{ world }}'))
 
             testdata, external_dependencies, message_handlers = initialize_testdata(grizzly, grizzly.scenario.tasks())
 
             assert external_dependencies == set()
-            assert message_handlers == {}
+            assert message_handlers == {'atomiccsvwriter': atomiccsvwriter_message_handler}
 
             producer = TestdataProducer(
                 grizzly=grizzly,
                 address=address,
                 testdata=testdata,
             )
             producer_thread = gevent.spawn(producer.run)
@@ -123,14 +126,15 @@
                     return message
 
                 message: Dict[str, Any] = get_message_from_producer()
                 assert message['action'] == 'consume'
                 data = message['data']
                 assert 'variables' in data
                 variables = data['variables']
+                assert 'AtomicCsvWriter.output' not in variables
                 assert 'AtomicIntegerIncrementer.messageID' in variables
                 assert 'AtomicDate.now' in variables
                 assert 'messageID' in variables
                 assert 'AtomicDate.utc' in variables
                 assert variables['AtomicIntegerIncrementer.messageID'] == 456
                 assert variables['messageID'] == 123
                 assert variables['AtomicDirectoryContents.test'] == f'adirectory{sep}file1.txt'
```

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_utils.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,15 +77,14 @@
             with pytest.raises(ValueError) as ve:
                 AtomicCsvWriter('output.foo', 'foobar')
             assert str(ve.value) == 'AtomicCsvWriter.output.foo is not a valid CSV destination name, must be: AtomicCsvWriter.<name>'
 
             t = AtomicCsvWriter('output', 'foobar.csv | headers="foo,bar"')
 
             assert t._settings == {'output': {'headers': ['foo', 'bar'], 'destination': 'foobar.csv', 'overwrite': False}}
-            assert t._buffer == {'output': {}}
 
             u = AtomicCsvWriter('foobar', 'output.csv | headers="bar,foo", overwrite=True')
 
             assert u is t
 
             assert t._settings == {
                 'output': {
@@ -95,32 +94,28 @@
                 },
                 'foobar': {
                     'headers': ['bar', 'foo'],
                     'destination': 'output.csv',
                     'overwrite': True,
                 },
             }
-            assert t._buffer == {'output': {}, 'foobar': {}}
         finally:
             cleanup()
 
     def test_clear(self, cleanup: AtomicVariableCleanupFixture) -> None:
         try:
             u = AtomicCsvWriter('foobar', 'output.csv | headers="bar,foo", overwrite=True')
             assert len(u._settings) == 1
-            assert len(u._buffer) == 1
 
             t = AtomicCsvWriter('output', 'foobar.csv | headers="foo,bar"')
             assert len(t._settings) == 2
-            assert len(t._buffer) == 2
 
             AtomicCsvWriter.clear()
 
             assert len(t._settings) == 0
-            assert len(t._buffer) == 0
         finally:
             cleanup()
 
     def test___getitem__(self, cleanup: AtomicVariableCleanupFixture) -> None:
         try:
             u = AtomicCsvWriter('foobar', 'output.csv | headers="bar,foo", overwrite=True')
 
@@ -131,39 +126,34 @@
             cleanup()
 
     def test___setitem__(self, grizzly_fixture: GrizzlyFixture, cleanup: AtomicVariableCleanupFixture, mocker: MockerFixture) -> None:
         send_message_mock = mocker.patch.object(grizzly_fixture.grizzly.state.locust, 'send_message', return_value=None)
 
         t = AtomicCsvWriter('output', 'output.csv | headers="foo,bar"')
 
-        assert t._buffer == {'output': {}}
+        assert not hasattr(t, '_buffer')
 
         with pytest.raises(ValueError) as ve:
-            t['output'] = 'hello'
-        assert str(ve.value) == 'AtomicCsvWriter.output is not a valid reference'
+            t['world'] = 'hello'
+        assert str(ve.value) == 'AtomicCsvWriter.world is not a valid reference'
 
         with pytest.raises(ValueError) as ve:
-            t['output.baz'] = 'hello'
-        assert str(ve.value) == 'AtomicCsvWriter.output has not specified header "baz"'
-
-        t['output.foo'] = 'hello'
-
-        send_message_mock.assert_not_called()
-        assert t._buffer == {'output': {'foo': 'hello'}}
+            t['output'] = 'hello'
+        assert str(ve.value) == 'AtomicCsvWriter.output: less values (1) than headers (2)'
 
         with pytest.raises(ValueError) as ve:
-            t['output.foo'] = 'world'
-        assert str(ve.value) == 'AtomicCsvWriter.output has already set value for "foo" in current row'
+            t['output'] = 'hello,world,foo'
+        assert str(ve.value) == 'AtomicCsvWriter.output: more values (3) than headers (2)'
 
-        send_message_mock.assert_not_called()
-        assert t._buffer == {'output': {'foo': 'hello'}}
-
-        t['output.bar'] = 'world!'
+        t['output'] = 'hello, world'
 
         send_message_mock.assert_called_once_with('atomiccsvwriter', {
             'destination': 'output.csv',
-            'row': {'foo': 'hello', 'bar': 'world!'}
+            'row': {'foo': 'hello', 'bar': 'world'}
         })
-        assert t._buffer == {'output': {}}
+        send_message_mock.reset_mock()
+
+        with pytest.raises(ValueError) as ve:
+            t['output.foo'] = 'world'
+        assert str(ve.value) == 'AtomicCsvWriter.output.foo is not a valid reference'
 
-        # pass through
-        t['output'] = None
+        send_message_mock.assert_not_called()
```

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_date.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_integer.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_random_integer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_string.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/testdata/variables/test_random_string.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_grizzly_user.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_grizzly_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_request_logger.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_request_logger.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_event.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_response_event.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_handler.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/base/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_blobstorage.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_dummy.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_dummy.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_iothub.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_iothub.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_messagequeue.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_restapi.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_restapi.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_servicebus.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_servicebus.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_sftp.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly/users/test_sftp.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test___init__.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_daemon.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/test_daemon.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_sb.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/async_message/test_sb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_arguments.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/test_arguments.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_transformer.py` & `grizzly-loadtester-2.6.5/tests/unit/test_grizzly_extras/test_transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.4/tests/webserver.py` & `grizzly-loadtester-2.6.5/tests/webserver.py`

 * *Files identical despite different names*

