# Comparing `tmp/danling-0.2.5.tar.gz` & `tmp/danling-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.2.5.tar", last modified: Wed Apr 26 10:03:19 2023, max compression
+gzip compressed data, was "danling-0.2.6.tar", last modified: Tue May  9 09:27:35 2023, max compression
```

## Comparing `danling-0.2.5.tar` & `danling-0.2.6.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.615284 danling-0.2.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 10:03:10.000000 danling-0.2.5/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.615284 danling-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 10:03:10.000000 danling-0.2.5/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-26 10:03:10.000000 danling-0.2.5/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-26 10:03:10.000000 danling-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.619284 danling-0.2.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 10:03:10.000000 danling-0.2.5/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-26 10:03:19.643284 danling-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 10:03:10.000000 danling-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-26 10:03:10.000000 danling-0.2.5/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.619284 danling-0.2.5/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 10:03:10.000000 danling-0.2.5/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 10:03:18.000000 danling-0.2.5/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 10:03:10.000000 danling-0.2.5/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-26 10:03:10.000000 danling-0.2.5/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-26 10:03:10.000000 danling-0.2.5/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-26 10:03:10.000000 danling-0.2.5/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 10:03:10.000000 danling-0.2.5/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.627284 danling-0.2.5/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 10:03:10.000000 danling-0.2.5/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-26 10:03:10.000000 danling-0.2.5/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-26 10:03:10.000000 danling-0.2.5/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/runner_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 10:03:10.000000 danling-0.2.5/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 10:03:10.000000 danling-0.2.5/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-26 10:03:10.000000 danling-0.2.5/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-26 10:03:10.000000 danling-0.2.5/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 10:03:10.000000 danling-0.2.5/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-26 10:03:10.000000 danling-0.2.5/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.623284 danling-0.2.5/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 10:03:19.000000 danling-0.2.5/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 10:03:10.000000 danling-0.2.5/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 10:03:10.000000 danling-0.2.5/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 10:03:10.000000 danling-0.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 10:03:10.000000 danling-0.2.5/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 10:03:10.000000 danling-0.2.5/docs/metrics/average_meter.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 10:03:10.000000 danling-0.2.5/docs/optim/lr_scheduler.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 10:03:10.000000 danling-0.2.5/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 10:03:10.000000 danling-0.2.5/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/runner_base.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 10:03:10.000000 danling-0.2.5/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 10:03:10.000000 danling-0.2.5/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 10:03:10.000000 danling-0.2.5/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 10:03:10.000000 danling-0.2.5/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 10:03:10.000000 danling-0.2.5/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 10:03:10.000000 danling-0.2.5/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 10:03:10.000000 danling-0.2.5/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-26 10:03:10.000000 danling-0.2.5/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.615284 danling-0.2.5/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.631284 danling-0.2.5/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 10:03:10.000000 danling-0.2.5/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 10:03:10.000000 danling-0.2.5/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-26 10:03:10.000000 danling-0.2.5/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-26 10:03:11.000000 danling-0.2.5/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 10:03:11.000000 danling-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-26 10:03:11.000000 danling-0.2.5/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 10:03:11.000000 danling-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:03:19.643284 danling-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:03:11.000000 danling-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:03:19.643284 danling-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-26 10:03:11.000000 danling-0.2.5/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-26 10:03:11.000000 danling-0.2.5/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.140900 danling-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-09 09:27:28.000000 danling-0.2.6/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-09 09:27:28.000000 danling-0.2.6/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-09 09:27:28.000000 danling-0.2.6/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-09 09:27:28.000000 danling-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-09 09:27:28.000000 danling-0.2.6/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 09:27:35.140900 danling-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 09:27:28.000000 danling-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-09 09:27:28.000000 danling-0.2.6/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-09 09:27:28.000000 danling-0.2.6/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 09:27:34.000000 danling-0.2.6/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 09:27:28.000000 danling-0.2.6/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-09 09:27:28.000000 danling-0.2.6/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-09 09:27:28.000000 danling-0.2.6/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-09 09:27:28.000000 danling-0.2.6/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-09 09:27:28.000000 danling-0.2.6/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-09 09:27:28.000000 danling-0.2.6/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-09 09:27:28.000000 danling-0.2.6/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-09 09:27:28.000000 danling-0.2.6/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-09 09:27:28.000000 danling-0.2.6/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 09:27:28.000000 danling-0.2.6/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-05-09 09:27:28.000000 danling-0.2.6/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 09:27:28.000000 danling-0.2.6/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 09:27:28.000000 danling-0.2.6/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-09 09:27:28.000000 danling-0.2.6/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-09 09:27:28.000000 danling-0.2.6/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-09 09:27:28.000000 danling-0.2.6/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-09 09:27:28.000000 danling-0.2.6/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.124900 danling-0.2.6/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 09:27:35.000000 danling-0.2.6/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-09 09:27:35.000000 danling-0.2.6/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:27:35.000000 danling-0.2.6/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 09:27:35.000000 danling-0.2.6/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 09:27:35.000000 danling-0.2.6/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 09:27:28.000000 danling-0.2.6/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 09:27:28.000000 danling-0.2.6/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 09:27:28.000000 danling-0.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 09:27:28.000000 danling-0.2.6/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 09:27:28.000000 danling-0.2.6/docs/metrics/average_meter.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 09:27:28.000000 danling-0.2.6/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 09:27:28.000000 danling-0.2.6/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 09:27:28.000000 danling-0.2.6/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 09:27:28.000000 danling-0.2.6/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 09:27:28.000000 danling-0.2.6/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 09:27:28.000000 danling-0.2.6/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 09:27:28.000000 danling-0.2.6/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 09:27:28.000000 danling-0.2.6/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 09:27:28.000000 danling-0.2.6/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 09:27:28.000000 danling-0.2.6/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 09:27:28.000000 danling-0.2.6/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 09:27:28.000000 danling-0.2.6/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 09:27:28.000000 danling-0.2.6/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 09:27:28.000000 danling-0.2.6/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-09 09:27:28.000000 danling-0.2.6/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-09 09:27:28.000000 danling-0.2.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.120900 danling-0.2.6/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.128900 danling-0.2.6/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.136900 danling-0.2.6/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.136900 danling-0.2.6/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.140900 danling-0.2.6/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-09 09:27:28.000000 danling-0.2.6/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 09:27:28.000000 danling-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-09 09:27:28.000000 danling-0.2.6/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 09:27:28.000000 danling-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:27:35.140900 danling-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:27:28.000000 danling-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:27:35.140900 danling-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-09 09:27:28.000000 danling-0.2.6/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-09 09:27:28.000000 danling-0.2.6/tests/test_runner.py
```

### Comparing `danling-0.2.5/.github/workflows/docs.yaml` & `danling-0.2.6/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/.github/workflows/push.yaml` & `danling-0.2.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/.gitignore` & `danling-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.Apache2` & `danling-0.2.6/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.BSD2` & `danling-0.2.6/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.BSD3` & `danling-0.2.6/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.BSD4` & `danling-0.2.6/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.GPL2` & `danling-0.2.6/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.GPL3` & `danling-0.2.6/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.MIT` & `danling-0.2.6/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/LICENSES/LICENSE.Unlicense` & `danling-0.2.6/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/PKG-INFO` & `danling-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.5
+Version: 0.2.6
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.5/README.md` & `danling-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/anaconda-project.yml` & `danling-0.2.6/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/__init__.py` & `danling-0.2.6/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/metrics/average_meter.py` & `danling-0.2.6/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/metrics/average_meters.py` & `danling-0.2.6/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/__init__.py` & `danling-0.2.6/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/mlp/dense.py` & `danling-0.2.6/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/mlp/mlp.py` & `danling-0.2.6/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/__init__.py` & `danling-0.2.6/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.6/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.6/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/decoder.py` & `danling-0.2.6/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/encoder.py` & `danling-0.2.6/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.6/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.6/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.2.6/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,15 @@
         elif cooldown_steps < 0:
             raise ValueError(f"Cooldown steps must be positive, but got {cooldown_steps}")
         if final_lr_ratio < 0:
             raise ValueError(f"`final_lr_ratio` must be positive, but got {final_lr_ratio}")
         if min_lr < 0:
             raise ValueError(f"`min_lr` must be positive, but got {min_lr}")
         self.strategies = {
-            k: v
-            for k, v in self.__class__.__dict__.items()
-            if callable(v) and (not k.startswith("_") or k in "get_lr")
+            k: v for k, v in self.__class__.__dict__.items() if callable(v) and (not k.startswith("_") or k in "get_lr")
         }
         if strategy not in self.strategies:
             raise ValueError(f"Scaling strategy must be one of {self.strategies.keys()}, but got {strategy}")
         self.steps = steps
         if final_lr is not None:
             warn("Argument `final_lr` is deprecated, use `final_lr_ratio` instead", DeprecationWarning)
         self.final_lr = final_lr
@@ -153,10 +151,12 @@
     def cosine(self, progress: float) -> float:  # pylint: disable=C0116
         return 1 - ((1 + np.cos(np.pi * progress)) / 2)
 
     def constant(self, progress: float) -> float:  # pylint: disable=W0613, C0116
         return 0.0
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.strategy}, method={self.method}, " \
-                f"final_lr_ratio={self.final_lr_ratio}, steps={self.steps}, " \
-                f"warmup_steps={self.warmup_steps}, cooldown_steps={self.cooldown_steps})"
+        return (
+            f"{self.__class__.__name__}({self.strategy}, method={self.method}, "
+            f"final_lr_ratio={self.final_lr_ratio}, steps={self.steps}, "
+            f"warmup_steps={self.warmup_steps}, cooldown_steps={self.cooldown_steps})"
+        )
```

### Comparing `danling-0.2.5/danling/registry.py` & `danling-0.2.6/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/runner/README.md` & `danling-0.2.6/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/runner/base_runner.py` & `danling-0.2.6/danling/runner/base_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,23 +237,24 @@
             save_path = os.path.join(self.checkpoint_dir, f"epoch-{self.state.epochs}.pth")
             shutil.copy(latest_path, save_path)
         if self.is_best:
             best_path = os.path.join(self.checkpoint_dir, "best.pth")
             shutil.copy(latest_path, best_path)
 
     def load_checkpoint(  # pylint: disable=W1113
-        self, checkpoint: Optional[Union[Mapping, str]] = None, override_config: bool = True, *args, **kwargs
+        self, checkpoint: Optional[Union[Mapping, str]] = None, override_state: bool = False, *args, **kwargs
     ) -> None:
         """
         Load info from checkpoint.
 
         Args:
             checkpoint: Checkpoint (or its path) to load.
                 Defaults to `self.checkpoint_dir/latest.pth`.
-            override_config: If True, override runner config with checkpoint config.
+            override_state: If True, override runner state with checkpoint state.
+                Defaults to `False`.
             *args: Additional arguments to pass to `self.load`.
             **kwargs: Additional keyword arguments to pass to `self.load`.
 
         Raises:
             FileNotFoundError: If `checkpoint` does not exists.
 
         See Also:
@@ -266,18 +267,19 @@
         # TODO: Support loading checkpoints in other format
         if isinstance(checkpoint, str):
             if not os.path.exists(checkpoint):
                 raise FileNotFoundError(f"checkpoint is set to {checkpoint} but does not exist.")
             self.checkpoint = checkpoint  # pylint: disable=W0201
             checkpoint: Mapping = self.load(checkpoint, *args, **kwargs)  # type: ignore
         # TODO: Wrap state_dict in a dataclass
-        if override_config:
+        if override_state:
             self.__dict__.update(NestedDict(**checkpoint["runner"]))  # type: ignore
         if self.model is not None and "model" in checkpoint:
-            self.model.load_state_dict(checkpoint["model"])  # type: ignore
+            model = self.unwrap_model(self.model)
+            model.load_state_dict(checkpoint["model"])  # type: ignore
         if self.optimizer is not None and "optimizer" in checkpoint:
             self.optimizer.load_state_dict(checkpoint["optimizer"])  # type: ignore
         if self.scheduler is not None and "scheduler" in checkpoint:
             self.scheduler.load_state_dict(checkpoint["scheduler"])  # type: ignore
 
     def load_pretrained(self, checkpoint: Union[Mapping, str], *args, **kwargs) -> None:
         """
@@ -320,15 +322,15 @@
         Returns:
             (BaseRunner):
         """
 
         if isinstance(checkpoint, str):
             checkpoint = cls.load(checkpoint, *args, **kwargs)
         runner = cls(**checkpoint["runner"])  # type: ignore
-        runner.load_checkpoint(checkpoint, override_config=False)
+        runner.load_checkpoint(checkpoint, override_state=False)
         return runner
 
     def append_result(self, result) -> None:
         r"""
         Append result to `self.state.results`.
 
         Warnings:
```

### Comparing `danling-0.2.5/danling/runner/runner_base.py` & `danling-0.2.6/danling/runner/runner_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import logging.config
 import os
 from typing import IO, Any, Callable, List, Mapping, Optional, Union
 
 from chanfig import Config, FlatDict, NestedDict, Variable
 
+from danling.metrics import AverageMeters
 from danling.utils import catch, ensure_dir, load, save
 
 from .runner_state import RunnerState
 
 PathStr = Union[os.PathLike, str, bytes]
 File = Union[PathStr, IO]
 
@@ -101,20 +102,22 @@
     optimizer: Optional[Any] = None
     scheduler: Optional[Any] = None
 
     datasets: FlatDict
     datasamplers: FlatDict
     dataloaders: FlatDict
 
+    meters: Optional[AverageMeters] = None
     logger: Optional[logging.Logger] = None
     writer: Optional[Any] = None
 
     def __init__(self, *args, **kwargs):
         super().__init__()
         self.state = RunnerState(*args, **kwargs)
+        self.meters = AverageMeters()
         self.datasets = FlatDict()
         self.datasamplers = FlatDict()
         self.dataloaders = FlatDict()
 
     @property
     def batch_size(self) -> int:
         r"""
```

### Comparing `danling-0.2.5/danling/runner/runner_state.py` & `danling-0.2.6/danling/runner/runner_state.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/runner/torch_runner.py` & `danling-0.2.6/danling/runner/torch_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/runner/utils.py` & `danling-0.2.6/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/tensors/nested_tensor.py` & `danling-0.2.6/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/tensors/torch_func_registry.py` & `danling-0.2.6/danling/tensors/torch_func_registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/utils/basex.py` & `danling-0.2.6/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/utils/decorators.py` & `danling-0.2.6/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling/utils/io.py` & `danling-0.2.6/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/danling.egg-info/PKG-INFO` & `danling-0.2.6/danling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.5
+Version: 0.2.6
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.5/danling.egg-info/SOURCES.txt` & `danling-0.2.6/danling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/mkdocs.yml` & `danling-0.2.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.6/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.6/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.6/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.6/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/assets/images/favicon.ico` & `danling-0.2.6/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/assets/images/logo.png` & `danling-0.2.6/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/overrides/main.html` & `danling-0.2.6/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/pyproject.toml` & `danling-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/tests/test_lr_scheduler.py` & `danling-0.2.6/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.5/tests/test_runner.py` & `danling-0.2.6/tests/test_runner.py`

 * *Files identical despite different names*

