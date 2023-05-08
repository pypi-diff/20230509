# Comparing `tmp/render_engine-2023.4.2a1.tar.gz` & `tmp/render_engine-2023.5.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.4.2a1.tar", last modified: Sun Apr 16 16:25:51 2023, max compression
+gzip compressed data, was "render_engine-2023.5.1a1.tar", last modified: Mon May  8 22:49:52 2023, max compression
```

## Comparing `render_engine-2023.4.2a1.tar` & `render_engine-2023.5.1a1.tar`

### file list

```diff
@@ -1,119 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/create-app.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/create_app_check_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.508106 render_engine-2023.5.1a1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.512106 render_engine-2023.5.1a1/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.512106 render_engine-2023.5.1a1/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.512106 render_engine-2023.5.1a1/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.512106 render_engine-2023.5.1a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.512106 render_engine-2023.5.1a1/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-08 22:49:52.000000 render_engine-2023.5.1a1/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-08 22:49:52.000000 render_engine-2023.5.1a1/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:49:52.000000 render_engine-2023.5.1a1/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 22:49:52.000000 render_engine-2023.5.1a1/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-08 22:49:52.000000 render_engine-2023.5.1a1/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 22:49:52.000000 render_engine-2023.5.1a1/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:52.516106 render_engine-2023.5.1a1/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-08 22:49:37.000000 render_engine-2023.5.1a1/tests/test_site.py
```

### Comparing `render_engine-2023.4.2a1/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.5.1a1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.devcontainer/devcontainer.json` & `render_engine-2023.5.1a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.5.1a1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.github/CONTRIBUTION.md` & `render_engine-2023.5.1a1/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.github/FUNDING.yml` & `render_engine-2023.5.1a1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.github/LICENSE` & `render_engine-2023.5.1a1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.github/dependabot.yml` & `render_engine-2023.5.1a1/.github/dependabot.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     directory: "/"
     ignore:
       - dependency-name: "Markdown"
       # For Markdown, ignore all updates for version 3.4.X
         versions: ["3.4.x"]
     # Check the pypi registry for updates every day (weekdays)
     schedule:
-      interval: "daily"
+      interval: "weekly"
 
   - package-ecosystem: "github-actions"
     # Workflow files stored in the
     # default location of `.github/workflows`
     directory: "/"
     schedule:
       interval: "weekly"
```

### Comparing `render_engine-2023.4.2a1/.github/workflows/publish.yml` & `render_engine-2023.5.1a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/.gitignore` & `render_engine-2023.5.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/PKG-INFO` & `render_engine-2023.5.1a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.4.2a1
+Version: 2023.5.1a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 > ***Warning***
-> Render Engine 2022.12.3 introduced a change to the schema where now the following commands were changed. I apologize for any inconvenience.
-> - `render_page` is just `page`
-> - `render_collection` is just `collection`
-> - You will need to now add `site.render()` where `site` is your `Site` instance
+> 
+> **BREAKING CHANGE**
+> As of 2023.4.2a1 Render Engine no longer uses the `date_published` or `date_modified` attributes for `Blog` objects. Please instead use `date`.
+>
+> **BREAKING CHANGE**
+> As of 2023.4.2a1 Render Engine enforces that the `Blog.date` attribute is a `datetime` object. If using frontmatter please use [iso8601](https://en.wikipedia.org/wiki/ISO_8601) format for the date attribute.
 
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](.github/render_engine/page.html)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](.github/render_engine/collection.html)** - A group of webpages built from the same template, organized in a single directory
 * **[Site](.github/render_engine/site.html)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
@@ -31,15 +33,15 @@
 Render Engine is available in PyPI and can be installed using pip:
 
 ```bash
 pip install render-engine
 ```
 
 ## Getting Started
-Check out the [Getting Started](https://render-engine.readthedocs.io/en/latest/page.md) Section in the [Documentation](https://render-engine.readthedocs.io)
+Check out the [Getting Started](https://render-engine.readthedocs.io/en/latest/page/) Section in the [Documentation](https://render-engine.readthedocs.io)
 
 ## Sponsors
 This and much of the work that I do is made possible by those that sponsor me
 on github.
 
 ### Sponsors at the $20/month and higher Level
 - [Brian Douglas](https://github.com/bdougie)
```

### Comparing `render_engine-2023.4.2a1/README.md` & `render_engine-2023.5.1a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 > ***Warning***
-> Render Engine 2022.12.3 introduced a change to the schema where now the following commands were changed. I apologize for any inconvenience.
-> - `render_page` is just `page`
-> - `render_collection` is just `collection`
-> - You will need to now add `site.render()` where `site` is your `Site` instance
+> 
+> **BREAKING CHANGE**
+> As of 2023.4.2a1 Render Engine no longer uses the `date_published` or `date_modified` attributes for `Blog` objects. Please instead use `date`.
+>
+> **BREAKING CHANGE**
+> As of 2023.4.2a1 Render Engine enforces that the `Blog.date` attribute is a `datetime` object. If using frontmatter please use [iso8601](https://en.wikipedia.org/wiki/ISO_8601) format for the date attribute.
 
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](.github/render_engine/page.html)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](.github/render_engine/collection.html)** - A group of webpages built from the same template, organized in a single directory
 * **[Site](.github/render_engine/site.html)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
@@ -21,15 +23,15 @@
 Render Engine is available in PyPI and can be installed using pip:
 
 ```bash
 pip install render-engine
 ```
 
 ## Getting Started
-Check out the [Getting Started](https://render-engine.readthedocs.io/en/latest/page.md) Section in the [Documentation](https://render-engine.readthedocs.io)
+Check out the [Getting Started](https://render-engine.readthedocs.io/en/latest/page/) Section in the [Documentation](https://render-engine.readthedocs.io)
 
 ## Sponsors
 This and much of the work that I do is made possible by those that sponsor me
 on github.
 
 ### Sponsors at the $20/month and higher Level
 - [Brian Douglas](https://github.com/bdougie)
```

### Comparing `render_engine-2023.4.2a1/docs/docs/archive.md` & `render_engine-2023.5.1a1/docs/docs/archive.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Archive
+
+Archives are a [`BasePage`][src.render_engine.page.BasePage] object used to display a list of [`Page`][src.render_engine.page.Page] objects in a [`Collection`][src.render_engine.collection.Collection].
+
+Archive objects create a customizeable page that can be controlled via its parent Collction.
+
 ::: src.render_engine.archive.Archive
 
 Collection.archives yields a generator of Archive objects. Each Archive object will have a `pages` attribute that is a list of Page objects referenced in that Archive Page. The number of pages is determined by the `Collection.items_per_page` attribute.
 
 The slug of the Archive Page is determined by whether the Archive is paginated.
 
 If there is more than one archive page, the Archive.archive_index will be appended to the Archive.slug . For example, if the Archive.slug is `archive` and the Archive.archive_index is `2`, the Archive Page will have a slug of `archive2`.
```

### Comparing `render_engine-2023.4.2a1/docs/docs/assets/create-app-help.png` & `render_engine-2023.5.1a1/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/docs/docs/assets/render-engine-init.png` & `render_engine-2023.5.1a1/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/docs/docs/contributing/pages.md` & `render_engine-2023.5.1a1/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/docs/docs/custom_collections.md` & `render_engine-2023.5.1a1/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/docs/docs/getting-started/create-app.md` & `render_engine-2023.5.1a1/docs/docs/cli.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-## Build your site with `create-app`
+# Render Engine CLI
 
-You can get started quickly using the `create_app` command.
+Render Engine comes with a CLI that can be used to create, build, and serve your site.
 
-```bash
-$ create-app
-```
+## creating your app with `render-engine init`
 
-or
-
-```bash
-$ python -m render_engine.create_app
-```
-
-!!! Warning
-    This is a work in progress. It is not ready for production. The callable `create_app` may be changed to a different name.
-
-### Available Options
-
-`create-app` has a few options that you can use to customize your site. While you must provide a `site_title` and `site_url`, other values are optional.
-
-You can view the options using the `--help` flag.
-
-![create-app --help](../assets/create-app-help.png)
+::: src.render_engine.cli.init
 
 #### `collection-path` (`Path`: default=`"pages"`)
 
 The path to the folder that will contain your [collections](../collection). This is where you will put your data files to be processed.
 
 #### `force` (`bool`: default=`False` as `no-force`)
 
@@ -58,7 +41,17 @@
 #### `skip-static` - (`bool`: default: `False` as `no-skip-static`)
 
 If `True`, will not create the [`static`](../../site#static_path) folder. This is where you will put your static files (images, css, js, etc).
 
 #### `templates-path` (`Path`: default=`"templates"`)
 
 The path to the folder that will contain your [`templates`](../templates). This is where you will put your Jinja2 templates.
+
+## Building your site with `render-engine build`
+
+::: src.render_engine.cli.build
+
+`build` takes the `site_module` parameter in the format of `module:site`. `module` is the name of the python file that contains the `site` variable you've initialized. If the site `site` variable is in the `app.py` file, then the `site_module` parameter would be `app:site`.
+
+## Serving your site (locally) with `render-engine serve`
+
+:::src.render_engine.cli.serve
```

### Comparing `render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.5.1a1/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.5.1a1/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/docs/docs/getting-started/installation.md` & `render_engine-2023.5.1a1/docs/docs/getting-started/installation.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# Getting Started
-This document will walk you through the basics of Render Engine.
-
-## Installing Render Engine
+# Installing Render Engine
 
 In order to use render engine, you must have python 3.9+ installed. You can download python from [python.org](https://python.org).
 
 - Linux/MacOS: [python.org](https://python.org)
 - Windows: [Microsoft Store](https://apps.microsoft.com/store/detail/python-311/9NRWMJP3717K)
 
 Render Engine is available in PyPI and can be installed using pip:
```

### Comparing `render_engine-2023.4.2a1/docs/docs/getting-started/layout.md` & `render_engine-2023.5.1a1/docs/docs/getting-started/layout.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Simple Site Layout
+# Simple Site Layout
 Render Engine has a very simple site layout. You can see the example site layout below.
 
 ```bash
 .
 ├── app.py # Logic/Configuration for building your site
 ├── content
 │  ├── pages # collection of files to build similarly styled pages
@@ -143,17 +143,7 @@
 # app.py
 
 @mysite.render_collection()
 class Blog(Blog):
   template="blog.html"
   content_path="content/blog"
 ```
-
-### Generating your site
-
-Once you have your site's build file (in our case app.py), you can generate the site by running the `generate` method on your site object.
-
-```bash
-python app.py
-```
-
-Your site will be generated in the `output` folder. You can change the output folder by passing in the `output_path` attribute to the `Site` class.
```

### Comparing `render_engine-2023.4.2a1/docs/docs/index.md` & `render_engine-2023.5.1a1/docs/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](page.md)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](collection.md)** - A group of webpages built from the same template, organized in a single directory
-* **[Site](site.md)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
+* **[Site](site.md)** - The container that helps to render all Pages and Collections in with uniform settings and variables
 
 ## Installing Render Engine
 
 In order to use render engine, you must have python 3.9+ installed. You can download python from [python.org](https://python.org).
 
 - Linux/MacOS: [python.org](https://python.org)
 - Windows: [Microsoft Store](https://apps.microsoft.com/store/detail/python-311/9NRWMJP3717K)
```

### Comparing `render_engine-2023.4.2a1/docs/mkdocs.yml` & `render_engine-2023.5.1a1/docs/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 site_url: https://render-engine.readthedocs.io
 theme:
   name: material
 nav:
   - Home: index.md
   - Getting Started:
     - getting-started/installation.md
-    - getting-started/create-app.md
-    - getting-started/layout.md
+    - getting-started/creating-your-app.md
     - getting-started/creating-a-page.md
     - getting-started/creating-a-collection.md
+    - getting-started/layout.md
+    - getting-started/building-your-site.md
   - Components:
-    - Page: page.md
+    - Page Objects: page.md
     - Collection:
       - Collection: collection.md
       - Archive: archive.md
       - RSS Feed: feeds.md
     - Site:
       - Site: site.md
       - Plugins: hookspecs.md
   - Extending Render Engine:
     - Built-in Plugins: plugins.md
     - Plugins: plugins.md
+  - Parsers: parsers.md
+  - CLI: cli.md
+  - Templates: templates.md
 markdown_extensions:
   - toc
   - codehilite:
       guess_lang: false
   - admonition
   - pymdownx.details
   - pymdownx.superfences
   - attr_list
-
 watch:
   - ../src/render_engine
 plugins:
 - search
 - autorefs
 - mkdocstrings:
     handlers:
```

### Comparing `render_engine-2023.4.2a1/pyproject.toml` & `render_engine-2023.5.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/requirements.txt` & `render_engine-2023.5.1a1/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements.txt pyproject.toml
 #
-attrs==22.2.0
+attrs==23.1.0
     # via pytest
 black==23.3.0
     # via render-engine (pyproject.toml)
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
@@ -23,15 +23,15 @@
     # via render-engine (pyproject.toml)
 ghp-import==2.1.0
     # via mkdocs
 gitdb==4.0.10
     # via gitpython
 gitpython==3.1.31
     # via render-engine (pyproject.toml)
-griffe==0.27.0
+griffe==0.27.1
     # via mkdocstrings-python
 idna==3.4
     # via requests
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
@@ -54,15 +54,15 @@
     # via
     #   jinja2
     #   mkdocstrings
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.2
+mkdocs==1.4.3
     # via
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   render-engine (pyproject.toml)
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
@@ -83,25 +83,25 @@
 packaging==23.1
     # via
     #   black
     #   mkdocs
     #   pytest
 pathspec==0.11.1
     # via black
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via black
 pluggy==1.0.0
     # via
     #   pytest
     #   render-engine (pyproject.toml)
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==9.10
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
     #   render-engine (pyproject.toml)
 pytest==7.3.1
     # via
     #   pytest-mock
@@ -124,25 +124,25 @@
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 regex==2023.3.23
     # via mkdocs-material
 requests==2.28.2
     # via mkdocs-material
-rich==13.3.4
+rich==13.3.5
     # via render-engine (pyproject.toml)
-ruff==0.0.261
+ruff==0.0.265
     # via render-engine (pyproject.toml)
 six==1.16.0
     # via python-dateutil
 smmap==5.0.0
     # via gitdb
 text-unidecode==1.3
     # via python-slugify
 typer==0.7.0
     # via
     #   dtyper
     #   render-engine (pyproject.toml)
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 watchdog==3.0.0
     # via mkdocs
```

### Comparing `render_engine-2023.4.2a1/src/.DS_Store` & `render_engine-2023.5.1a1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/.DS_Store` & `render_engine-2023.5.1a1/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/_base_object.py` & `render_engine-2023.5.1a1/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/archive.py` & `render_engine-2023.5.1a1/src/render_engine/archive.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-"""
-The Archive is the Page object used by the collection that focuses on presenting Page objects.
-"""
 import pathlib
 
 import jinja2
 
 from .page import BasePage
 
 
 class Archive(BasePage):
     """
-    ???+ Warning "Not Directly Used"
-        The Archive object is not meant to be used directly. 
-        It is used by the [Collection][src.render_engine.Collection] object. 
-        Attributes can be used to customize the 
-        [archive_template][src.render_engine.collection.Collection].
-
-    Custom [`Page`][src.render_engine.page.Page] used to show the pages in a [Collection][src.render_engine.Collection].
+    The Archive is a [Page][src.render_engine.page.Page] object used by the collection that focuses on presenting the Collection's pages.
 
     Parameters:
         pages: The list of pages to include in the archive
         title: The title of the archive
         template: The template to use for the archive
         routes: The routes for where the archive page should be generated
         archive_index: The index of the page in the series of archive pages
         num_of_pages: The total number of pages in the series of archive pages
+
+    !!! Warning "Not Directly Used"
+        The Archive object is not meant to be used directly. 
+        It is used by the [Collection][src.render_engine.Collection] object. 
+        Attributes can be used to customize.
     """
 
     def __init__(
         self,
         title: str,
         pages: list[BasePage],
         template: str | jinja2.Template,
@@ -36,11 +32,12 @@
         archive_index: int = 0,
         num_archive_pages: int = 1,
     ) -> None:
         super().__init__()
         self.pages = pages
         self.template = template
         self.routes = routes
+        self.archive_index = archive_index
         self.title = title
 
-        if num_archive_pages > 1:
+        if archive_index:
             self.slug = f"{self._slug}{archive_index}"
```

### Comparing `render_engine-2023.4.2a1/src/render_engine/blog.py` & `render_engine-2023.5.1a1/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/cli.py` & `render_engine-2023.5.1a1/src/render_engine/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # noqa: UP007
 
 import importlib
 import pathlib
 import sys
-import typing
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 
 import dtyper
 import typer
 from rich.console import Console
 from rich.progress import Progress
 
@@ -98,33 +97,33 @@
         rich_help_panel="Path Attributes",
     ),
     project_folder: pathlib.Path = typer.Option(
         pathlib.Path("./"),
         help="path to create the project in",
         rich_help_panel="Path Attributes",
     ),
-    site_author: typing.Optional[str] = typer.Option(
+    site_author: str | None = typer.Option(
         None,
         help="(Optional): Author of the site",
         rich_help_panel="Site Vars",
     ),
-    site_description: typing.Optional[str] = typer.Option(
+    site_description: str | None = typer.Option(
         None,
         help="(Optional): Site Description",
         rich_help_panel="Site Vars",
     ),
-    site_title: typing.Optional[str] = typer.Option(
+    site_title: str | None = typer.Option(
         None,
         "--title",
         "-t",
         help="title of the site",
         rich_help_panel="Site Vars",
         show_default=False,
     ),
-    site_url: typing.Optional[str] = typer.Option(
+    site_url: str | None = typer.Option(
         None,
         "--url",
         "-u",
         help="URL for the site",
         rich_help_panel="Site Vars",
         show_default=False,
     ),
@@ -149,16 +148,32 @@
     ),
     templates_path: pathlib.Path = typer.Option(
         pathlib.Path("templates"),
         "--templates-path",
         help="custom templates folder",
     ),
 ):
-    """CLI for creating a new site"""
-
+    """
+    CLI for creating a new site configuration.
+    
+    Params:
+        collection_path: create your content folder in a custom location
+        force: Force overwrite of existing files
+        output_path: custom output folder location
+        project_path_name: name of render_engine app name
+        project_folder: path to create the project
+        site_author:  Author of the site
+        site_description: Site Description
+        site_title: title of the site
+        site_url: URL for the site
+        skip_collection: Skip creating the content folder and a collection
+        skip_static: Skip copying static files
+        static_path: custom static folder
+        templates_path: custom templates folder
+    """
     # creating the site object and site_vars
 
     project_folder_path = pathlib.Path(project_folder)
     with Progress() as progress:
         progress.console.rule("[green][bold]Creating Project")
         task_project = progress.add_task("Creating Site", total=5)
         site = _create_site_with_vars(
@@ -191,16 +206,19 @@
         project_config_path = (
             pathlib.Path(project_folder).joinpath(project_path_name).with_suffix(".py")
         )
         task_generate_project_path = progress.add_task(
             f"Generating App File: [blue]{project_config_path}", total=1
         )
 
+        has_attrs = any((site_title, site_url, site_description, site_author))
+
         project_config_path.write_text(
             CREATE_APP_PY_TEMPLATE.render(
+                has_attrs=has_attrs,
                 site_title=site_title,
                 site_url=site_url,
                 site_description=site_description,
                 site_author=site_author,
                 output_path=output_path,
                 static_path=static_path,
                 collection_path=collection_path,
@@ -237,77 +255,71 @@
 
             progress.update(task_create_collection, advance=1)
         progress.update(task_project, advance=1)
 
 
 @app.command()
 def build(site_module: str):
-    """CLI for creating a new site"""
+    """
+    CLI for creating a new site
+
+    Params:
+        site_module: module and class name of the site
+    
+    """
     app = get_app(site_module)
     app.render()
 
 
 @app.command()
 def serve(
-    module_site: str,
+    module_site: str | None = None,
     build: bool = False,
-    directory: typing.Optional[str] = typer.Option(
+    directory: str | None = typer.Option(
         None,
         "--directory",
         "-d",
         help="Directory to serve",
         show_default=False,
     ),
     port: int = typer.Option(
         8000,
         "--port",
         "-p",
         help="Port to serve on",
         show_default=False,
     ),
-    attempts: int = typer.Option(
-        10,
-        "--attempts",
-        help="Attempt to bind to port.",
-        show_default=True,
-    ),
-    attempts_wait_time: int = typer.Option(
-        60,
-        "--attempts-timeout",
-        help="Time to wait between attempts to bind to port.",
-        show_default=True,
-    ),
 ):
-    """CLI for creating a new site"""
+    """
+    Create an HTTP server to serve the site at `localhost`.
+
+    !!! warning
+        this is only for development purposes and should not be used in production.
+
+    Params:
+        module_site: Python module and initialize Site class
+        build: flag to build the site prior to serving the app
+        directory: Directory to serve. If `module_site` is provided, this will be the `output_path` of the site.
+        port: Port to serve on
+    """
+
     app = get_app(module_site)
 
     if build:
         app.render()
 
     if not directory:
         directory = app.output_path
 
     class server(SimpleHTTPRequestHandler):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, directory=directory, **kwargs)
 
     server_address = ("localhost", port)
     console = Console()
-    while attempts:
-        try:
-            httpd = HTTPServer(server_address, server)
-        except OSError as e:
-            if 'Address already in use' in str(e):
-                import time
-                attempts -= 1
-                if attempts:
-                    console.print(f"Unable to list to http://{server_address[0]}:{server_address[1]}.")
-                    console.print(f"Address is already in use, sleeping 60 sec. Attempts left {attempts}")
-                    time.sleep(attempts_wait_time)
-        else:
-           console.print(f"Serving [blue]{directory} on http://{server_address[0]}:{server_address[1]}")
-           console.print(f"Press [bold red]CTRL+C[/bold red] to stop serving")
-           return httpd.serve_forever()
+    console.print(f"Serving [blue]{directory} on http://{server_address[0]}:{server_address[1]}")
+    console.print(f"Press [bold red]CTRL+C[/bold red] to stop serving")
+    return httpd.serve_forever()
 
 
 def cli():
     app()
```

### Comparing `render_engine-2023.4.2a1/src/render_engine/collection.py` & `render_engine-2023.5.1a1/src/render_engine/collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 
     site = Site()
 
     @site.collection
     class BasicCollection(Collection):
         content_path = "content/pages"
     ```
-    Currently, collection pages **MUST** come from a `content_path` and all be the same
-    content type.
+
+    Collection pages **MUST** come from a `content_path` and all be the same
+    content type.  `content_path` can be a string representing a path or URL, depending on the [parser][src.render_engine.parsers.base_parsers] used.
 
     Attributes:
 
         archive_template: The template to use for the [`Archive`][src.render_engine.archive.Archive] pages.
         content_path: The path to iterate over to generate pages.
         content_type: Type[Page] = Page
         Feed: Type[RSSFeed]
@@ -136,28 +137,31 @@
             key=lambda page: getattr(page, self.sort_by, self._title),
             reverse=self.sort_reverse,
         )
 
     @property
     def archives(self) -> typing.Generator[Archive, None, None]:
         """
-        Returns a [Archive][src.render_engine.archive] objects containing the pages from the `content_path` .
+        Returns a [Archive][src.render_engine.archive.Archive] objects containing the pages from the `content_path` .
 
         Archives are an iterable and the individual pages are built shortly after the collection pages are built. This happens when [Site.render][render_engine.Site.render] is called.
         """
 
         if not self.has_archive:
             yield from ()
 
         sorted_pages = list(self.sorted_pages)
         items_per_page = getattr(self, "items_per_page", len(sorted_pages))
-        archives = list(batched(sorted_pages, items_per_page))
+        archives = [sorted_pages]
+
+        if items_per_page != len(sorted_pages):
+            archives.extend(list(batched(sorted_pages, items_per_page)))
         num_archive_pages = len(archives)
 
-        for index, pages in enumerate(archives, start=1):
+        for index, pages in enumerate(archives):
             yield Archive(
                 pages=pages,
                 template=getattr(self, "archive_template", None),
                 title=self._title,
                 routes=self.routes,
                 archive_index=index,
                 num_archive_pages=num_archive_pages,
```

### Comparing `render_engine-2023.4.2a1/src/render_engine/feeds.py` & `render_engine-2023.5.1a1/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/hookspecs.py` & `render_engine-2023.5.1a1/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/links.py` & `render_engine-2023.5.1a1/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/page.py` & `render_engine-2023.5.1a1/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/parsers/.DS_Store` & `render_engine-2023.5.1a1/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.5.1a1/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.5.1a1/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/plugins.py` & `render_engine-2023.5.1a1/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.5.1a1/tests/create_app_check_file.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 """
 This is a simple app setup script created with `render-engine init`
 """
 
 from render_engine import Site, Page, Collection
 
 app = Site()
-app.output_path = "{{output_path}}"
-app.static_path = "{{static_path}}"
+app.output_path = "output"
+app.static_path = "static"
 
 # Your site_vars will be used throughout your site
 app.site_vars.update(
-    SITE_TITLE="{{site_title}}",
-    SITE_URL="{{site_url}}",
-    {% if site_description %}
-    SITE_DESCRIPTION="{{site_description}}",
-    {% endif %}
-    {% if site_author %}
-    SITE_AUTHOR="{{site_author}}",
-    {% endif %}
+    SITE_TITLE="title",
+    SITE_URL="url",
+    SITE_DESCRIPTION="description",
+    SITE_AUTHOR="author",
     )
 
 @app.page
 class Index(Page):
     template = "index.html"
 
-{% if not skip_collection %}
 @app.collection
 class Pages(Collection):
-    content_path = "{{collection_path}}" # path to content files
-{% endif %}
+    content_path = "pages" # path to content files
 
 if __name__ == "__main__":
     app.render()
```

### Comparing `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.5.1a1/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.5.1a1/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.5.1a1/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/src/render_engine/site.py` & `render_engine-2023.5.1a1/src/render_engine/site.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,220 @@
 import logging
 import pathlib
 import shutil
 from collections import defaultdict
-from functools import partial
-from typing import Type
+
 from jinja2 import Environment
 from rich.progress import Progress
 
 from .collection import Collection
-from .engine import engine, url_for
+from .engine import engine
 from .hookspecs import register_plugins
 from .page import Page
-from datetime import datetime
 
 
 class Site:
     """
     The site stores your pages and collections to be rendered.
 
     Attributes:
-        output_path: str to write rendered content. **Default**: `output`
-        static: Output str Path for the static folder. This will get copied to the output folder. **Default**: `static`
-        site_vars: Vars that will be passed into the render functions
-
-            Default `site_vars`:
-
-            - SITE_TITLE: "Untitled Site"
-            - SITE_URL: "http://example.com"
+        engine: Jinja2 Environment used to render pages
+        output_path: 
+            path to write rendered content
+        partial: 
+            if True, only render pages that have been modified. Uses gitPython to check for changes.
+        plugins: 
+            list of plugins that will be loaded and passed into each object
+        static: 
+            path for the static folder. This will get copied to the output folder.
+        site_vars: 
+            dictionary that will be passed into page template
+        site_settings:
+            settings that will be passed into pages and collections but not into templates
     """
 
     output_path: str = "output"
     static_path: str = "static"
     partial: bool = False
-
+    site_settings: dict = {
+        "plugins": {}
+    }
     site_vars: dict = {
         "SITE_TITLE": "Untitled Site",
         "SITE_URL": "http://localhost:8000/",
         "DATETIME_FORMAT": "%d %b %Y %H:%M %Z"
     }
     plugins: list
-
+    engine: Environment = engine
 
 
     def __init__(
         self,
         plugins: list[str] = [],
     ) -> None:
-        self.route_list = dict()
+        self._route_list = dict()
         self.subcollections = defaultdict(lambda: {"pages": []})
-        self.engine.filters["url_for"] = partial(url_for, site=self)
+        self.engine.globals.update(self.site_vars)
         self.plugins = [*plugins, *getattr(self, "plugins", [])]
         self._pm = register_plugins(plugins=self.plugins)
 
-    @property
-    def engine(self) -> Environment:
-        env = engine
-        env.globals.update(self.site_vars)
-        return env
-
-    def add_to_route_list(self, page: Page) -> None:
-        """Add a page to the route list"""
-        self.route_list[getattr(page, page._reference)] = page
+    def collection(self, Collection: type[Collection]) -> Collection:
+        """
+        Add the collection to the route list to be rendered later.
+
+        This is the primary way to add a collection to the site and 
+        can either be called on an uninstantiated class or on the class definition as a decorator.
+
+        In most cases. You should use the decorator method.
+
+        ```python
+        from render_engine import Site, Collection
+
+        site = Site()
+
+        @site.collection # works
+        class Pages(Collection):
+            pass
+
+
+        class Posts(Collection):
+            pass
 
-    def collection(self, Collection: Type[Collection]) -> Collection:
-        """Create the pages in the collection including the archive"""
+        site.collection(Posts) # also works
+        ```
+        """
         _Collection = Collection(plugins=self.plugins)
         self._pm.hook.pre_build_collection(collection=_Collection) #type: ignore
-        self.route_list[_Collection._slug] = _Collection
+        self._route_list[_Collection._slug] = _Collection
         return _Collection
 
-    def page(self, Page: type[Page]) -> Page:
-        """Create a Page object and add it to self.routes"""
-        page = Page(plugins=self.plugins)
+    def page(self, Page: Page) -> Page:
+        """
+        Add the page to the route list to be rendered later.
+        Also remaps `title` in case the user wants to use it in the template rendering.
+
+        This is the primary way to add a page to the site and can either be called
+        on an uninstantiated class or on the class definition as a decorator.
+
+        In most cases. You should use the decorator method.
+
+        ```python
+
+        from render_engine import Site, Page
+
+        site = Site()
 
-        # Expose _title to the user through `title`
-        page.title = page._title
-        logging.info("Running Post Build Page")
-        self.add_to_route_list(page)
+        @site.page # works
+        class Home(Page):
+            pass
+
+        class About(Page):
+            pass
+
+        site.page(About) # also works
+        ```
+        """
+        page = Page(plugins=self.plugins)
+        page.title = page._title # Expose _title to the user through `title`
+        self._route_list[getattr(page, page._reference)] = page
         return page
 
-    def render_static(self) -> None:
+    def _render_static(self) -> None:
         """Copies a Static Directory to the output folder"""
         shutil.copytree(
             self.static_path,
             pathlib.Path(self.output_path) / pathlib.Path(self.static_path).name,
             dirs_exist_ok=True
         )
 
-    def render_output(self, route: str, page: Type[Page]):
+    def _render_output(self, route: str, page: type[Page]):
         """writes the page object to disk"""
         path = (
             pathlib.Path(self.output_path)
             / pathlib.Path(route)
             / pathlib.Path(page.path_name)
         )
         path.parent.mkdir(parents=True, exist_ok=True)
         return path.write_text(
             page._render_content(engine=self.engine)
         )
 
-    def render_partial_collection(self, collection: Collection) -> None:
+    def _render_partial_collection(self, collection: Collection) -> None:
         """Iterate through the Changed Pages and Check for Collections and Feeds"""
         for entry in collection._generate_content_from_modified_pages():
             for route in collection.routes:
-                self.render_output(route, entry)
+                self._render_output(route, entry)
 
         if collection.has_archive:
             for archive in collection.archives:
                 logging.debug("Adding Archive: %s", archive.__class__.__name__)
 
-                self.render_output(collection.routes[0], archive)
+                self._render_output(collection.routes[0], archive)
 
         if hasattr(collection, "Feed"):
-            self.render_output("./", collection._feed)
+            self._render_output("./", collection._feed)
 
-    def render_full_collection(self, collection: Collection) -> None:
+    def _render_full_collection(self, collection: Collection) -> None:
         """Iterate through Pages and Check for Collections and Feeds"""
 
         for entry in collection:
             for route in collection.routes:
-                self.render_output(route, entry)
+                self._render_output(route, entry)
 
         if collection.has_archive:
             for archive in collection.archives:
                 logging.debug("Adding Archive: %s", archive.__class__.__name__)
 
                 for route in collection.routes:
-                    self.render_output(collection.routes[0], archive)
+                    self._render_output(collection.routes[0], archive)
 
         if hasattr(collection, "Feed"):
-            self.render_output("./", collection._feed)
+            self._render_output("./", collection._feed)
 
     def render(self) -> None:
-        """Render all pages and collections"""
+        """
+        Render all pages and collections.
+
+        These are pages and collections that have been added to the site using 
+        the [`Site.page`][src.render_engine.Site.page] 
+        and [`Site.collection`][src.render_engine.Site.collection] methods.
+
+        Render should be called after all pages and collections have been added to the site.
+
+        You can choose to call it manually in your file or use the CLI command [`render-engine build`][src.render_engine.cli.build]
+        """
 
         with Progress() as progress:
 
             pre_build_task = progress.add_task("Loading Pre-Build Plugins", total=1)
             self._pm.hook.pre_build_site(site=self)
 
             # Parse Route List
             task_add_route = progress.add_task(
-                "[blue]Adding Routes", total=len(self.route_list)
+                "[blue]Adding Routes", total=len(self._route_list)
             )
 
             if pathlib.Path(self.static_path).exists():
-                self.render_static()
-            engine.globals["site"] = self
+                self._render_static()
+            self.engine.globals["site"] = self
+            self.engine.globals["routes"] = self._route_list
 
-            for slug, entry in self.route_list.items():
+            for slug, entry in self._route_list.items():
                 progress.update(
                     task_add_route, description=f"[blue]Adding[gold]Route: [blue]{slug}"
                 )
                 if isinstance(entry, Page):
                     for route in entry.routes:
                         progress.update(
                             task_add_route,
                             description=f"[blue]Adding[gold]Route: [blue]{entry._slug}",
                         )
-                        self.render_output(route, entry)
+                        self._render_output(route, entry)
 
                 if isinstance(entry, Collection):
                     if self.partial:
-                        self.render_partial_collection(entry)
+                        self._render_partial_collection(entry)
                     else:
-                        self.render_full_collection(entry)
-            post_build_task = progress.add_task("Loading Post-Build Plugins", total=1)
+                        self._render_full_collection(entry)
+            progress.add_task("Loading Post-Build Plugins", total=1)
             self._pm.hook.post_build_site(site=self)
             progress.update(pre_build_task, advance=1)
```

### Comparing `render_engine-2023.4.2a1/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.5.1a1/src/render_engine.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.4.2a1
+Version: 2023.5.1a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 > ***Warning***
-> Render Engine 2022.12.3 introduced a change to the schema where now the following commands were changed. I apologize for any inconvenience.
-> - `render_page` is just `page`
-> - `render_collection` is just `collection`
-> - You will need to now add `site.render()` where `site` is your `Site` instance
+> 
+> **BREAKING CHANGE**
+> As of 2023.4.2a1 Render Engine no longer uses the `date_published` or `date_modified` attributes for `Blog` objects. Please instead use `date`.
+>
+> **BREAKING CHANGE**
+> As of 2023.4.2a1 Render Engine enforces that the `Blog.date` attribute is a `datetime` object. If using frontmatter please use [iso8601](https://en.wikipedia.org/wiki/ISO_8601) format for the date attribute.
 
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](.github/render_engine/page.html)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](.github/render_engine/collection.html)** - A group of webpages built from the same template, organized in a single directory
 * **[Site](.github/render_engine/site.html)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
@@ -31,15 +33,15 @@
 Render Engine is available in PyPI and can be installed using pip:
 
 ```bash
 pip install render-engine
 ```
 
 ## Getting Started
-Check out the [Getting Started](https://render-engine.readthedocs.io/en/latest/page.md) Section in the [Documentation](https://render-engine.readthedocs.io)
+Check out the [Getting Started](https://render-engine.readthedocs.io/en/latest/page/) Section in the [Documentation](https://render-engine.readthedocs.io)
 
 ## Sponsors
 This and much of the work that I do is made possible by those that sponsor me
 on github.
 
 ### Sponsors at the $20/month and higher Level
 - [Brian Douglas](https://github.com/bdougie)
```

### Comparing `render_engine-2023.4.2a1/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.5.1a1/src/render_engine.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,33 @@
 .github/PULL_REQUEST_TEMPLATE/pull_request_template.md
 .github/workflows/publish.yml
 .github/workflows/test.yml
 .vscode/tasks.json
 docs/mkdocs.yml
 docs/requirements.txt
 docs/docs/archive.md
+docs/docs/cli.md
 docs/docs/collection.md
 docs/docs/custom_collections.md
 docs/docs/feeds.md
 docs/docs/hookspecs.md
 docs/docs/index.md
 docs/docs/page.md
+docs/docs/parsers.md
 docs/docs/plugins.md
 docs/docs/site.md
+docs/docs/templates.md
 docs/docs/assets/create-app-help.png
+docs/docs/assets/render-engine-init-help.png
 docs/docs/assets/render-engine-init.png
 docs/docs/contributing/pages.md
-docs/docs/getting-started/create-app.md
+docs/docs/getting-started/building-your-site.md
 docs/docs/getting-started/creating-a-collection.md
 docs/docs/getting-started/creating-a-page.md
+docs/docs/getting-started/creating-your-app.md
 docs/docs/getting-started/installation.md
 docs/docs/getting-started/layout.md
 src/.DS_Store
 src/render_engine/.DS_Store
 src/render_engine/.gitignore
 src/render_engine/__init__.py
 src/render_engine/__main__.py
@@ -76,14 +81,15 @@
 src/render_engine/render_engine_templates/index.html
 src/render_engine/render_engine_templates/rss2.0.xml
 src/render_engine/render_engine_templates/rss2.0_items.xml
 src/render_engine/render_engine_templates/sitemap.xml
 src/render_engine/render_engine_templates/sitemap_item.xml
 tests/conftest.py
 tests/create_app_check_file.txt
+tests/create_app_check_file_no_site_vars.txt
 tests/test_archive.py
 tests/test_base_object.py
 tests/test_base_parser.py
 tests/test_blog.py
 tests/test_collections.py
 tests/test_create_app.py
 tests/test_feeds.py
```

### Comparing `render_engine-2023.4.2a1/tests/test_base_object.py` & `render_engine-2023.5.1a1/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/tests/test_base_parser.py` & `render_engine-2023.5.1a1/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/tests/test_collections.py` & `render_engine-2023.5.1a1/tests/test_collections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import pathlib
+
 import pluggy
+import pytest
 
 from render_engine.collection import Collection
 from render_engine.page import Page
 from render_engine.parsers import BasePageParser
 
 pm = pluggy.PluginManager("fake_test")
 
@@ -21,15 +24,15 @@
 
     collection = BasicCollection()
     page = collection.get_page()
 
     assert page.Parser == SimpleBasePageParser
 
 
-def test_pages_generate_from_collection_content_path(tmp_path):
+def test_pages_generate_from_collection_content_path(tmp_path: pathlib.Path):
     """
     Tests that pages are generated from a collection
     """
 
     dir = tmp_path / "content"
     dir.mkdir()
 
@@ -44,15 +47,15 @@
     assert len([page for page in collection]) == len(content)
 
     for page in collection:
         # Order is not guaranteed
         assert page.content in content
 
 
-def test_collection_archive_no_items_per_page(tmp_path):
+def test_collection_archive_no_items_per_page(tmp_path: pathlib.Path):
     """
     Tests that archive generates a single page if items_per_page is not set
     """
 
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
     file = tmp_dir / "test.md"
@@ -62,15 +65,15 @@
         content_path = tmp_dir.absolute()
         archive_template = None
 
     collection = BasicCollection()
     assert len(list(collection.archives)) == 1
 
 
-def test_collection_vars(tmp_path):
+def test_collection_vars(tmp_path: pathlib.Path):
     """
     Tests that collection_vars are passed to the page objects
     """
 
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
     file = tmp_dir / "test.md"
@@ -82,15 +85,15 @@
 
     collection = BasicCollection()
 
     for page in collection:
         assert page.collection_vars["title"] == collection._title
 
 
-def test_collection_archives_has_title_of_collection(tmp_path):
+def test_collection_archives_has_title_of_collection(tmp_path: pathlib.Path):
     """
     Tests that the title of the Archive Collection is the same as the parent Collection.
 
     This should be the case with all archive pages generated
 
     Issue #105
     """
@@ -104,23 +107,48 @@
     file2.write_text("test")
 
     class BasicCollection(Collection):
         content_path = tmp_dir.absolute()
         items_per_page = 1
 
     collection = BasicCollection()
-    assert len(list(collection.archives)) == 2
+    assert len(list(collection.archives)) == 3
     for archive in collection.archives:
         assert archive._title == collection._title
 
 
-def test_collection_paginated_archives_start_at_1(tmp_path):
+def test_collection_paginated_archives_start_at_1(tmp_path: pathlib.Path):
     """Tests that the first archive page is page 1 and not page 0"""
 
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
 
     file1 = tmp_dir / "test.md"
     file1.write_text("test1")
 
     file2 = tmp_dir / "test2.md"
     file2.write_text("test")
+
+
+@pytest.mark.parametrize(
+        "attr,attrval",
+        [
+            ("template", "test.html"),
+            ("routes", ["/test/long/route"]),
+        ]
+)
+def test_collection_attrs_pass_to_page(attr: str, attrval: str | list[str]):
+    """Tests that the template attribute for the collection is passed to the page"""
+
+    class SimpleBasePageParser(BasePageParser):
+        pass
+
+    class BasicCollection(Collection):
+        PageParser = SimpleBasePageParser
+        content_type = Page
+        
+    setattr(BasicCollection, attr, attrval)
+
+    collection = BasicCollection()
+    page = collection.get_page()
+
+    assert getattr(page, attr) == attrval
```

### Comparing `render_engine-2023.4.2a1/tests/test_create_app.py` & `render_engine-2023.5.1a1/tests/test_create_app.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import pathlib
 
-import pytest
-
 import render_engine.cli as cli
-from render_engine.site import Site
 
 
 def test_create_site_with_vars():
     """Tests the site can be built with optional attributes""" ""
     site = cli._create_site_with_vars(
         site_title="title",
         site_url="url",
@@ -51,7 +48,20 @@
         project_folder=d,
     )
 
     assert (
         d.joinpath("app.py").read_text().strip()
         == pathlib.Path("tests/create_app_check_file.txt").read_text().strip()
     )
+
+def test_create_app_no_vars(tmp_path):
+    """Tests app.py is created with no update to vars"""
+    d = tmp_path
+
+    cli.init(
+        project_folder=d,
+    )
+
+    assert (
+        d.joinpath("app.py").read_text().strip()
+        == pathlib.Path("tests/create_app_check_file_no_site_vars.txt").read_text().strip()
+    )
```

### Comparing `render_engine-2023.4.2a1/tests/test_feeds.py` & `render_engine-2023.5.1a1/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.2a1/tests/test_page.py` & `render_engine-2023.5.1a1/tests/test_page.py`

 * *Files identical despite different names*

