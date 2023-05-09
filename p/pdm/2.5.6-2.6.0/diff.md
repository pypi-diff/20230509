# Comparing `tmp/pdm-2.5.6.tar.gz` & `tmp/pdm-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.5.6.tar", last modified: Sun May  7 09:40:45 2023, max compression
+gzip compressed data, was "pdm-2.6.0.tar", last modified: Tue May  9 08:43:55 2023, max compression
```

## Comparing `pdm-2.5.6.tar` & `pdm-2.6.0.tar`

### file list

```diff
@@ -1,270 +1,272 @@
--rw-r--r--   0        0        0   116715 2023-05-07 09:40:35.574249 pdm-2.5.6/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-05-07 09:40:35.574249 pdm-2.5.6/LICENSE
--rw-r--r--   0        0        0     1075 2023-05-07 09:40:35.574249 pdm-2.5.6/LICENSE
--rw-r--r--   0        0        0     7986 2023-05-07 09:40:35.574249 pdm-2.5.6/README.md
--rw-r--r--   0        0        0     7986 2023-05-07 09:40:35.574249 pdm-2.5.6/README.md
--rw-r--r--   0        0        0     4423 2023-05-07 09:40:45.522359 pdm-2.5.6/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/__version__.py
--rw-r--r--   0        0        0     2432 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11738 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    33652 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     2404 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2255 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     2380 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6529 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     6102 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     2948 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     1071 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     2318 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     5979 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     2263 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15743 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     1912 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6161 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     7904 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     4644 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     1672 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    14018 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9364 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     2392 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     1318 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1848 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2416 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6171 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      809 2023-05-07 09:40:35.578250 pdm-2.5.6/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1276 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     3027 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5025 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    37102 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18492 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    24792 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3553 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10328 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/options.py
--rw-r--r--   0        0        0    24464 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2409 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/compat.py
--rw-r--r--   0        0        0     9245 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/core.py
--rw-r--r--   0        0        0      904 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8889 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/environments/local.py
--rw-r--r--   0        0        0      808 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/environments/prefix.py
--rw-r--r--   0        0        0     1614 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1377 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1086 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5741 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2349 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7289 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7131 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2271 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1853 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10908 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    17107 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10903 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4394 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/backends.py
--rw-r--r--   0        0        0     9886 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/caches.py
--rw-r--r--   0        0        0    24220 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1714 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6182 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2120 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    20760 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    17969 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/search.py
--rw-r--r--   0        0        0     2414 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     5899 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2721 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16212 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/project/config.py
--rw-r--r--   0        0        0    26927 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/project/core.py
--rw-r--r--   0        0        0     1320 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3046 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/py.typed
--rw-r--r--   0        0        0    19636 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    12796 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-05-07 09:40:35.582249 pdm-2.5.6/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-05-07 09:40:35.586249 pdm-2.5.6/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-05-07 09:40:35.586249 pdm-2.5.6/src/pdm/signals.py
--rw-r--r--   0        0        0     7966 2023-05-07 09:40:35.586249 pdm-2.5.6/src/pdm/termui.py
--rw-r--r--   0        0        0    13510 2023-05-07 09:40:35.586249 pdm-2.5.6/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/__init__.py
--rw-r--r--   0        0        0     2631 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/conftest.py
--rw-r--r--   0        0        0    12370 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_add.py
--rw-r--r--   0        0        0     5811 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_build.py
--rw-r--r--   0        0        0     5277 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_cache.py
--rw-r--r--   0        0        0     7603 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10432 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4505 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_list.py
--rw-r--r--   0        0        0     4675 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7187 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_others.py
--rw-r--r--   0        0        0     5740 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3872 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_remove.py
--rw-r--r--   0        0        0    26440 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_run.py
--rw-r--r--   0        0        0     3641 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8888 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_update.py
--rw-r--r--   0        0        0     2960 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_use.py
--rw-r--r--   0        0        0    10565 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3172 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-05-07 09:40:35.586249 pdm-2.5.6/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0   305481 2023-05-07 09:40:35.590250 pdm-2.5.6/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-05-07 09:40:35.594250 pdm-2.5.6/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-07 09:40:35.598250 pdm-2.5.6/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1329 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/__init__.py
--rw-r--r--   0        0        0     3820 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_backends.py
--rw-r--r--   0        0        0    12991 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2526 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7187 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_formats.py
--rw-r--r--   0        0        0     7240 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_installer.py
--rw-r--r--   0        0        0     1862 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_integration.py
--rw-r--r--   0        0        0     2859 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_plugin.py
--rw-r--r--   0        0        0    11182 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_project.py
--rw-r--r--   0        0        0     1109 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_signals.py
--rw-r--r--   0        0        0     4364 2023-05-07 09:40:35.602250 pdm-2.5.6/tests/test_utils.py
--rw-r--r--   0        0        0     9669 1970-01-01 00:00:00.000000 pdm-2.5.6/PKG-INFO
+-rw-r--r--   0        0        0   118952 2023-05-09 08:43:40.952031 pdm-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-05-09 08:43:40.952031 pdm-2.6.0/LICENSE
+-rw-r--r--   0        0        0     1075 2023-05-09 08:43:40.952031 pdm-2.6.0/LICENSE
+-rw-r--r--   0        0        0     7986 2023-05-09 08:43:40.952031 pdm-2.6.0/README.md
+-rw-r--r--   0        0        0     7986 2023-05-09 08:43:40.952031 pdm-2.6.0/README.md
+-rw-r--r--   0        0        0     4448 2023-05-09 08:43:55.469098 pdm-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/__version__.py
+-rw-r--r--   0        0        0     2432 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11738 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    33958 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2404 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2174 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     2380 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6529 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     6186 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     2948 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     1071 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     5860 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3500 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15743 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6161 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     7904 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6424 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     1672 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15360 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9364 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     2392 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     1318 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1683 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6171 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5069 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    37780 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18548 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25037 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-05-09 08:43:40.956031 pdm-2.6.0/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10339 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    24638 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2409 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/compat.py
+-rw-r--r--   0        0        0     9744 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8780 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1365 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1086 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5741 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2349 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7289 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7131 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2271 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1320 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10908 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18026 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10903 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4394 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    10872 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    24340 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1714 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6182 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2111 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    20893 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    17998 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/search.py
+-rw-r--r--   0        0        0     2414 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5899 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2721 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    15969 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26706 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/py.typed
+-rw-r--r--   0        0        0    19689 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-05-09 08:43:40.960031 pdm-2.6.0/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13119 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/signals.py
+-rw-r--r--   0        0        0     7966 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/termui.py
+-rw-r--r--   0        0        0    13744 2023-05-09 08:43:40.964032 pdm-2.6.0/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     2631 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12370 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5784 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     7489 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4454 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7748 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_others.py
+-rw-r--r--   0        0        0     5722 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3872 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8888 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2942 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10430 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-05-09 08:43:40.964032 pdm-2.6.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-05-09 08:43:40.968032 pdm-2.6.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-05-09 08:43:40.972032 pdm-2.6.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-05-09 08:43:40.976033 pdm-2.6.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-05-09 08:43:40.980033 pdm-2.6.0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1329 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13285 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2526 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7187 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_integration.py
+-rw-r--r--   0        0        0     3361 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_plugin.py
+-rw-r--r--   0        0        0    11478 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_signals.py
+-rw-r--r--   0        0        0     4364 2023-05-09 08:43:40.984033 pdm-2.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     9669 1970-01-01 00:00:00.000000 pdm-2.6.0/PKG-INFO
```

### Comparing `pdm-2.5.6/CHANGELOG.md` & `pdm-2.6.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Release v2.6.0 (2023-05-09)
+---------------------------
+
+### Features & Improvements
+
+- Install project-level plugins from project config, with `tool.pdm.plugins` setting. [#1461](https://github.com/pdm-project/pdm/issues/1461)
+- Added a `--json` flag to both `run` and `info` command allowing to dump scripts and infos as JSON. [#1854](https://github.com/pdm-project/pdm/issues/1854)
+- Consider tasks with a name starting by an underscore (`_`) as internal tasks and hide them from the listing. [#1855](https://github.com/pdm-project/pdm/issues/1855)
+- When running `pdm init -n`(non-interactive mode), a venv will be created by default. Previously, the selected Python will be used under PEP 582 mode. [#1862](https://github.com/pdm-project/pdm/issues/1862)
+- Support [Trusted Publisher](https://docs.pypi.org/trusted-publishers/). [#1868](https://github.com/pdm-project/pdm/issues/1868)
+- Add an ephemeral wheel cache in process for wheels built from non-static revision sources. [#1885](https://github.com/pdm-project/pdm/issues/1885)
+- Allow self-referencing groups in dev-dependencies. [#1890](https://github.com/pdm-project/pdm/issues/1890)
+- Add an option `--no-cross-platform` to `pdm lock` to create a non-cross-platform lockfile. [#1898](https://github.com/pdm-project/pdm/issues/1898)
+
+### Bug Fixes
+
+- Fix brackets in `--venv` option descriptions in zsh completion script. [#1847](https://github.com/pdm-project/pdm/issues/1847)
+- The resolver doesn't take into account of the requirements for both bare `package` and `package[extra]`. [#1851](https://github.com/pdm-project/pdm/issues/1851)
+- Default pypi source does not use configured pypi.password, but "<hidden>" instead. [#1856](https://github.com/pdm-project/pdm/issues/1856)
+- Detect Python interpreters under the root of virtual environments. [#1866](https://github.com/pdm-project/pdm/issues/1866)
+- Fix a race condition when the builder is creating a new build directory. [#1869](https://github.com/pdm-project/pdm/issues/1869)
+- Raise `FileNotFoundError` if the requirement path is not found. [#1875](https://github.com/pdm-project/pdm/issues/1875)
+- Fix a bug that the self package isn't uninstallable. [#1901](https://github.com/pdm-project/pdm/issues/1901)
+
+
 Release v2.5.6 (2023-05-07)
 ---------------------------
 
 ### Bug Fixes
 
 - Fix a double reading issue due to cachecontrol not compatible with urllib3 2.0. [#1894](https://github.com/pdm-project/pdm/issues/1894)
```

### Comparing `pdm-2.5.6/LICENSE` & `pdm-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/README.md` & `pdm-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/pyproject.toml` & `pdm-2.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.5.6"
+version = "2.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
@@ -99,14 +99,15 @@
 
 [tool.pdm.dev-dependencies]
 test = [
     "pdm[pytest]",
     "pytest-cov",
     "pytest-xdist>=1.31.0",
     "pytest-rerunfailures>=10.2",
+    "pytest-httpserver>=1.0.6",
 ]
 tox = [
     "tox",
     "tox-pdm>=0.5",
 ]
 doc = [
     "mkdocs>=1.1",
@@ -148,15 +149,15 @@
 extend-ignore = [
     "B018",
     "B019",
 ]
 src = [
     "src",
 ]
-extend-exclude = [
+exclude = [
     "tests/fixtures",
 ]
 target-version = "py37"
 
 [tool.ruff.mccabe]
 max-complexity = 10
```

### Comparing `pdm-2.5.6/src/pdm/_types.py` & `pdm-2.6.0/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/builders/base.py` & `pdm-2.6.0/src/pdm/builders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from logging import Logger
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Mapping, cast
 
 from pyproject_hooks import BuildBackendHookCaller
 
 from pdm.compat import tomllib
-from pdm.environments import PrefixEnvironment
+from pdm.environments import PythonEnvironment
 from pdm.exceptions import BuildError
 from pdm.models.in_process import get_sys_config_paths
 from pdm.models.requirements import Requirement, parse_requirement
 from pdm.models.working_set import WorkingSet
 from pdm.termui import logger
 from pdm.utils import create_tracked_tempdir
 
@@ -286,15 +286,15 @@
     def install(self, requirements: Iterable[str], shared: bool = False) -> None:
         from pdm.installers.core import install_requirements
 
         missing = list(self.check_requirements(requirements))
         if not missing:
             return
         path = self._prefix.shared if shared else self._prefix.overlay
-        env = PrefixEnvironment(self._env.project, prefix=path)
+        env = PythonEnvironment(self._env.project, prefix=path)
         install_requirements(missing, env)
 
         if shared:
             # The shared env is prepared and is safe to be cached now. This is to make
             # sure no broken env is returned early when run in parallel mode.
             key = hash(frozenset(requirements))
             if key not in self._shared_envs:
```

### Comparing `pdm-2.5.6/src/pdm/builders/editable.py` & `pdm-2.6.0/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/builders/sdist.py` & `pdm-2.6.0/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/builders/wheel.py` & `pdm-2.6.0/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/actions.py` & `pdm-2.6.0/src/pdm/cli/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     project: Project,
     strategy: str = "all",
     tracked_names: Iterable[str] | None = None,
     requirements: list[Requirement] | None = None,
     dry_run: bool = False,
     refresh: bool = False,
     groups: list[str] | None = None,
+    cross_platform: bool | None = None,
     hooks: HookManager | None = None,
 ) -> dict[str, Candidate]:
     """Performs the locking process and update lockfile."""
     hooks = hooks or HookManager(project)
     check_project_file(project)
     if refresh:
         locked_repo = project.locked_repository
@@ -76,19 +77,24 @@
                 dependencies[candidate.dep_key] = list(map(parse_requirement, reqs))
             with project.core.ui.logging("lock"):
                 fetch_hashes(repo, mapping)
             lockfile = format_lockfile(project, mapping, dependencies)
         project.write_lockfile(lockfile, groups=groups)
         return mapping
     # TODO: multiple dependency definitions for the same package.
-    provider = project.get_provider(strategy, tracked_names)
+    if cross_platform is None:
+        cross_platform = project.lockfile.cross_platform
+    provider = project.get_provider(strategy, tracked_names, ignore_compatibility=cross_platform)
     if not requirements:
         requirements = [
             r for g, deps in project.all_dependencies.items() if groups is None or g in groups for r in deps.values()
         ]
+    if not cross_platform:
+        this_env = project.environment.marker_environment
+        requirements = [req for req in requirements if not req.marker or req.marker.evaluate(this_env)]
     resolve_max_rounds = int(project.config["strategy.resolve_max_rounds"])
     ui = project.core.ui
     with ui.logging("lock"):
         # The context managers are nested to ensure the spinner is stopped before
         # any message is thrown to the output.
         try:
             with ui.open_spinner(title="Resolving dependencies") as spin:
@@ -116,15 +122,15 @@
         except ResolutionImpossible as err:
             ui.echo(f"{termui.Emoji.LOCK} Lock failed", err=True)
             ui.echo(format_resolution_impossible(err), err=True)
             raise ResolutionImpossible("Unable to find a resolution") from None
         else:
             data = format_lockfile(project, mapping, dependencies)
             ui.echo(f"{termui.Emoji.LOCK} Lock successful")
-            project.write_lockfile(data, write=not dry_run, groups=groups)
+            project.write_lockfile(data, write=not dry_run, groups=groups, cross_platform=cross_platform)
             hooks.try_emit("post_lock", resolution=mapping, dry_run=dry_run)
 
     return mapping
 
 
 def resolve_candidates_from_lockfile(project: Project, requirements: Iterable[Requirement]) -> dict[str, Candidate]:
     ui = project.core.ui
@@ -151,15 +157,15 @@
 def check_lockfile(project: Project, raise_not_exist: bool = True) -> str | None:
     """Check if the lock file exists and is up to date. Return the update strategy."""
     if not project.lockfile.exists():
         if raise_not_exist:
             raise ProjectError("Lock file does not exist, nothing to install")
         project.core.ui.echo("Lock file does not exist", style="warning", err=True)
         return "all"
-    elif not project.is_lockfile_compatible():
+    elif not project.lockfile.is_compatible():
         project.core.ui.echo(
             "Lock file version is not compatible with PDM, installation may fail",
             style="warning",
             err=True,
         )
         return "reuse"  # try to reuse the lockfile if possible
     elif not project.is_lockfile_hash_match():
@@ -200,15 +206,14 @@
     synchronizer = project.core.synchronizer_class(
         candidates,
         project.environment,
         clean=clean,
         dry_run=dry_run,
         no_editable=no_editable,
         install_self=not no_self and "default" in selection and bool(project.name),
-        use_install_cache=project.config["install.cache"],
         reinstall=reinstall,
         only_keep=only_keep,
         fail_fast=fail_fast,
     )
     with project.core.ui.logging("install"):
         hooks.try_emit("pre_install", candidates=candidates, dry_run=dry_run)
         synchronizer.synchronize()
@@ -572,27 +577,27 @@
     save: bool = True,
     venv: str | None = None,
     hooks: HookManager | None = None,
 ) -> PythonInfo:
     """Use the specified python version and save in project config.
     The python can be a version string or interpreter path.
     """
-    from pdm.cli.commands.venv.utils import get_venv_python, get_venv_with_name
+    from pdm.cli.commands.venv.utils import get_venv_with_name
 
     def version_matcher(py_version: PythonInfo) -> bool:
         return py_version.valid and (
             ignore_requires_python or project.python_requires.contains(str(py_version.version), True)
         )
 
     hooks = hooks or HookManager(project)
 
     selected_python: PythonInfo | None = None
     if venv:
-        venv_path = get_venv_with_name(project, venv)
-        selected_python = PythonInfo.from_path(get_venv_python(venv_path))
+        virtualenv = get_venv_with_name(project, venv)
+        selected_python = PythonInfo.from_path(virtualenv.interpreter)
 
     if not project.cache_dir.exists():
         project.cache_dir.mkdir(parents=True)
     use_cache: JSONFileCache[str, str] = JSONFileCache(project.cache_dir / "use_cache.json")
     if python:
         python = python.strip()
     if selected_python is None and python and not ignore_remembered:
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/add.py` & `pdm-2.6.0/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/base.py` & `pdm-2.6.0/src/pdm/cli/commands/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import argparse
 from argparse import _SubParsersAction
 from typing import Any
 
 from pdm.cli.options import Option, global_option, project_option, verbose_option
-from pdm.cli.utils import PdmFormatter
 from pdm.project import Project
 
 
 class BaseCommand:
     """A CLI subcommand"""
 
     # The subcommand's name
@@ -36,15 +35,14 @@
         subparsers._name_parser_map.pop(name, None)
         subactions = subparsers._get_subactions()
         subactions[:] = [action for action in subactions if action.dest != name]
         parser = subparsers.add_parser(
             name,
             description=help_text,
             help=help_text,
-            formatter_class=PdmFormatter,
             **kwargs,
         )
         command = cls(parser)
         command.name = name
         # Store the command instance in the parsed args. See pdm/core.py for more details
         parser.set_defaults(command=command)
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/build.py` & `pdm-2.6.0/src/pdm/cli/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             help="Do not clean the target directory",
         )
         parser.add_argument(
             "--config-setting",
             "-C",
             action="append",
             help="Pass options to the backend. options with a value must be "
-            'specified after "=": "--config-setting=--opt(=value)" '
-            'or "-C--opt(=value)"',
+            'specified after "=": `--config-setting=--opt(=value)` '
+            "or `-C--opt(=value)`",
         )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         config_settings = None
         if options.config_setting:
             config_settings = {}
             for item in options.config_setting:
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/cache.py` & `pdm-2.6.0/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/completion.py` & `pdm-2.6.0/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/config.py` & `pdm-2.6.0/src/pdm/cli/commands/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
                 err=True,
             )
             options.key = project.project_config.deprecated[options.key]
         try:
             value = project.project_config[options.key]
         except KeyError:
             value = project.global_config[options.key]
+        if options.key.endswith(".password"):
+            value = "[i]<hidden>[/i]"
         project.core.ui.echo(value)
 
     def _set_config(self, project: Project, options: argparse.Namespace) -> None:
         config = project.project_config if options.local else project.global_config
         if options.key in config.deprecated:  # pragma: no cover
             project.core.ui.echo(
                 f"DEPRECATED: the config has been renamed to {config.deprecated[options.key]}",
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/export.py` & `pdm-2.6.0/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.6.0/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.6.0/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/import_cmd.py` & `pdm-2.6.0/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/info.py` & `pdm-2.6.0/src/pdm/cli/commands/info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
 import json
 
+from rich import print_json
+
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.options import ArgumentGroup, venv_option
 from pdm.cli.utils import check_project_file
 from pdm.project import Project
 
 
 class Command(BaseCommand):
@@ -18,14 +20,15 @@
             "--where",
             dest="where",
             action="store_true",
             help="Show the project root path",
         )
         group.add_argument("--packages", action="store_true", help="Show the local packages root")
         group.add_argument("--env", action="store_true", help="Show PEP 508 environment markers")
+        group.add_argument("--json", action="store_true", help="Dump the information in JSON")
         group.add_to_parser(parser)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         check_project_file(project)
         interpreter = project.environment.interpreter
         packages_path = ""
         if project.environment.is_local:
@@ -34,14 +37,29 @@
             project.core.ui.echo(str(interpreter.executable))
         elif options.where:
             project.core.ui.echo(str(project.root))
         elif options.packages:
             project.core.ui.echo(str(packages_path))
         elif options.env:
             project.core.ui.echo(json.dumps(project.environment.marker_environment, indent=2))
+        elif options.json:
+            print_json(
+                data={
+                    "pdm": {"version": project.core.version},
+                    "python": {
+                        "interpreter": str(interpreter.executable),
+                        "version": interpreter.identifier,
+                        "markers": project.environment.marker_environment,
+                    },
+                    "project": {
+                        "root": str(project.root),
+                        "pypackages": str(packages_path),
+                    },
+                }
+            )
         else:
             for name, value in zip(
                 [
                     f"[primary]{key}[/]:"
                     for key in [
                         "PDM version",
                         "Python Interpreter",
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/init.py` & `pdm-2.6.0/src/pdm/cli/commands/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from pdm import termui
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import skip_option
 from pdm.models.backends import _BACKENDS, DEFAULT_BACKEND, BuildBackend, get_backend
 from pdm.models.python import PythonInfo
+from pdm.models.venv import get_venv_python
 from pdm.project import Project
-from pdm.utils import get_user_email_from_git, get_venv_like_prefix
+from pdm.utils import get_user_email_from_git
 
 
 class Command(BaseCommand):
     """Initialize a pyproject.toml for PDM"""
 
     def __init__(self, parser: argparse.ArgumentParser) -> None:
         super().__init__(parser)
@@ -38,16 +39,14 @@
         )
         parser.add_argument("--python", help="Specify the Python version/path to use")
         parser.add_argument("--backend", choices=list(_BACKENDS), help="Specify the build backend")
         parser.add_argument("--lib", action="store_true", help="Create a library project")
         parser.set_defaults(search_parent=False)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        from pdm.cli.commands.venv.utils import get_venv_python
-
         hooks = HookManager(project, options.skip)
         if project.pyproject.exists():
             project.core.ui.echo("pyproject.toml already exists, update it now.", style="primary")
         else:
             project.core.ui.echo("Creating a pyproject.toml for PDM...", style="primary")
         self.set_interactive(not options.non_interactive)
 
@@ -56,39 +55,39 @@
                 project,
                 options.python or "",
                 first=bool(options.python),
                 ignore_remembered=True,
                 ignore_requires_python=True,
                 hooks=hooks,
             )
-            if project.config["python.use_venv"] and get_venv_like_prefix(python.executable) is None:
-                if termui.confirm(
-                    f"Would you like to create a virtualenv with [success]{python.executable}[/]?",
-                    default=True,
-                ):
-                    try:
-                        path = project._create_virtualenv()
-                        python = project.python = PythonInfo.from_path(get_venv_python(path))
-                    except Exception as e:  # pragma: no cover
-                        project.core.ui.echo(
-                            f"Error occurred when creating virtualenv: {e}\nPlease fix it and create later.",
-                            style="error",
-                            err=True,
-                        )
         else:
             python = actions.do_use(
                 project,
                 options.python or "3",
                 first=True,
                 ignore_remembered=True,
                 ignore_requires_python=True,
                 save=False,
                 hooks=hooks,
             )
-        if get_venv_like_prefix(python.executable) is None:
+        if project.config["python.use_venv"] and python.get_venv() is None:
+            if not self.interactive or termui.confirm(
+                f"Would you like to create a virtualenv with [success]{python.executable}[/]?",
+                default=True,
+            ):
+                try:
+                    path = project._create_virtualenv()
+                    python = project.python = PythonInfo.from_path(get_venv_python(path))
+                except Exception as e:  # pragma: no cover
+                    project.core.ui.echo(
+                        f"Error occurred when creating virtualenv: {e}\nPlease fix it and create later.",
+                        style="error",
+                        err=True,
+                    )
+        if python.get_venv() is None:
             project.core.ui.echo(
                 "You are using the PEP 582 mode, no virtualenv is created.\n"
                 "For more info, please visit https://peps.python.org/pep-0582/",
                 style="success",
             )
         is_library = options.lib
         if not is_library and self.interactive:
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/list.py` & `pdm-2.6.0/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/lock.py` & `pdm-2.6.0/src/pdm/cli/commands/lock.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,21 @@
         )
 
         parser.add_argument(
             "--check",
             action="store_true",
             help="Check if the lock file is up to date and quit",
         )
+        parser.add_argument(
+            "--no-cross-platform",
+            action="store_false",
+            default=True,
+            dest="cross_platform",
+            help="Only lock packages for the current platform",
+        )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if options.check:
             strategy = actions.check_lockfile(project, False)
             if strategy:
                 project.core.ui.echo(
                     f"[error]{termui.Emoji.FAIL}[/] Lockfile is [error]out of date[/].",
@@ -51,9 +58,10 @@
                 )
                 sys.exit(0)
         selection = GroupSelection.from_options(project, options)
         actions.do_lock(
             project,
             refresh=options.refresh,
             groups=selection.all(),
+            cross_platform=options.cross_platform,
             hooks=HookManager(project, options.skip),
         )
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.6.0/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/publish/package.py` & `pdm-2.6.0/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/remove.py` & `pdm-2.6.0/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/run.py` & `pdm-2.6.0/src/pdm/cli/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import shlex
 import signal
 import subprocess
 import sys
 from types import FrameType
 from typing import Any, Callable, Iterator, Mapping, NamedTuple, Sequence, cast
 
+from rich import print_json
+
 from pdm import termui
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import skip_option, venv_option
 from pdm.cli.utils import check_project_file, get_pep582_path
 from pdm.compat import TypedDict
 from pdm.exceptions import PdmUsageError
@@ -283,60 +285,97 @@
 
     def show_list(self) -> None:
         if not self.project.scripts:
             return
         columns = ["Name", "Type", "Description"]
         result = []
         for name in sorted(self.project.scripts):
-            if name == "_":
+            if name.startswith("_"):
                 continue
             task = self.get_task(name)
             assert task is not None
             result.append(
                 (
                     f"[success]{name}[/]",
                     task.kind,
                     task.short_description,
                 )
             )
         self.project.core.ui.display_columns(result, columns)
 
+    def as_json(self) -> dict[str, Any]:
+        out = {}
+        for name in sorted(self.project.scripts):
+            if name == "_":
+                data = out["_"] = dict(name="_", kind="shared", help="Shared options", **self.global_options)
+                _fix_env_file(data)
+                continue
+            task = self.get_task(name)
+            assert task is not None
+            data = out[name] = {
+                "name": name,
+                "kind": task.kind,
+                "help": task.short_description,
+                "args": task.args,  # type: ignore[dict-item]
+            }
+            data.update(**task.options)
+            _fix_env_file(data)
+        return out
+
+
+def _fix_env_file(data: dict[str, Any]) -> dict[str, Any]:
+    env_file = data.get("env_file")
+    if isinstance(env_file, dict):
+        del data["env_file"]
+        data["env_file.override"] = env_file.get("override")
+    return data
+
 
 class Command(BaseCommand):
     """Run commands or scripts with local packages loaded"""
 
     runner_cls: type[TaskRunner] = TaskRunner
     arguments = [*BaseCommand.arguments, skip_option, venv_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument(
+        action = parser.add_mutually_exclusive_group()
+        action.add_argument(
             "-l",
             "--list",
             action="store_true",
             help="Show all available scripts defined in pyproject.toml",
         )
-        parser.add_argument(
+        action.add_argument(
+            "-j",
+            "--json",
+            action="store_true",
+            help="Output all scripts infos in JSON",
+        )
+        exec = action.add_argument_group("execution", "Execution parameters")
+        exec.add_argument(
             "-s",
             "--site-packages",
             action="store_true",
             help="Load site-packages from the selected interpreter",
         )
-        parser.add_argument("script", nargs="?", help="The command to run")
-        parser.add_argument(
+        exec.add_argument("script", nargs="?", help="The command to run")
+        exec.add_argument(
             "args",
             nargs=argparse.REMAINDER,
             help="Arguments that will be passed to the command",
         )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         check_project_file(project)
         hooks = HookManager(project, options.skip)
         runner = self.runner_cls(project, hooks=hooks)
         if options.list:
             return runner.show_list()
+        if options.json:
+            return print_json(data=runner.as_json())
         if options.site_packages:
             runner.global_options.update({"site_packages": options.site_packages})
         if not options.script:
             project.core.ui.echo(
                 "No command is given, default to the Python REPL.",
                 style="warning",
                 err=True,
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/search.py` & `pdm-2.6.0/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/self_cmd.py` & `pdm-2.6.0/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/show.py` & `pdm-2.6.0/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/sync.py` & `pdm-2.6.0/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/update.py` & `pdm-2.6.0/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/use.py` & `pdm-2.6.0/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 from __future__ import annotations
 
 import argparse
-from pathlib import Path
-from pdm.cli.commands.venv.utils import get_venv_with_name, iter_venvs, get_venv_python
 
-from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.commands.venv.activate import ActivateCommand
 from pdm.cli.commands.venv.create import CreateCommand
 from pdm.cli.commands.venv.list import ListCommand
 from pdm.cli.commands.venv.purge import PurgeCommand
 from pdm.cli.commands.venv.remove import RemoveCommand
+from pdm.cli.commands.venv.utils import get_venv_with_name
 from pdm.cli.options import Option
 
 
 class Command(BaseCommand):
     """Virtualenv management"""
 
     name = "venv"
     arguments: list[Option] = []
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("--path", help="Show the path to the given virtualenv")
-        parser.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
+        group = parser.add_mutually_exclusive_group()
+        group.add_argument("--path", help="Show the path to the given virtualenv")
+        group.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
         subparser = parser.add_subparsers()
         CreateCommand.register_to(subparser, "create")
         ListCommand.register_to(subparser, "list")
         RemoveCommand.register_to(subparser, "remove")
         ActivateCommand.register_to(subparser, "activate")
         PurgeCommand.register_to(subparser, "purge")
         self.parser = parser
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        if options.path and options.python:
-            raise PdmUsageError("--path and --python are mutually exclusive")
         if options.path:
             venv = get_venv_with_name(project, options.path)
-            project.core.ui.echo(str(venv))
+            project.core.ui.echo(str(venv.root))
         elif options.python:
             venv = get_venv_with_name(project, options.python)
-            project.core.ui.echo(str(get_venv_python(venv)))
+            project.core.ui.echo(str(venv.interpreter))
         else:
             self.parser.print_help()
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/activate.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/activate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 import shlex
 from pathlib import Path
 
 import shellingham
 
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.commands.venv.utils import BIN_DIR, iter_venvs, get_venv_with_name
+from pdm.cli.commands.venv.utils import get_venv_with_name
 from pdm.cli.options import verbose_option
+from pdm.models.venv import VirtualEnv
 from pdm.project import Project
-from pdm.utils import get_venv_like_prefix
 
 
 class ActivateCommand(BaseCommand):
     """Activate the virtualenv with the given name"""
 
     arguments = [verbose_option]
 
@@ -28,34 +28,34 @@
             if not interpreter:
                 project.core.ui.echo(
                     "The project doesn't have a saved python.path. Run [success]pdm use[/] to pick one.",
                     style="warning",
                     err=True,
                 )
                 raise SystemExit(1)
-            venv_like = get_venv_like_prefix(interpreter)
+            venv_like = VirtualEnv.from_interpreter(Path(interpreter))
             if venv_like is None:
                 project.core.ui.echo(
                     f"Can't activate a non-venv Python [success]{interpreter}[/], "
                     "you can specify one with [success]pdm venv activate <env_name>[/]",
                     style="warning",
                     err=True,
                 )
                 raise SystemExit(1)
             venv = venv_like
         project.core.ui.echo(self.get_activate_command(venv))
 
-    def get_activate_command(self, venv: Path) -> str:  # pragma: no cover
+    def get_activate_command(self, venv: VirtualEnv) -> str:  # pragma: no cover
         shell, _ = shellingham.detect_shell()
         if shell == "fish":
             command, filename = "source", "activate.fish"
         elif shell == "csh":
             command, filename = "source", "activate.csh"
         elif shell in ["powershell", "pwsh"]:
             command, filename = ".", "Activate.ps1"
         else:
             command, filename = "source", "activate"
-        activate_script = venv / BIN_DIR / filename
+        activate_script = venv.interpreter.with_name(filename)
         if activate_script.exists():
             return f"{command} {shlex.quote(str(activate_script))}"
         # Conda backed virtualenvs don't have activate scripts
-        return f"conda activate {shlex.quote(str(venv))}"
+        return f"conda activate {shlex.quote(str(venv.root))}"
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/backends.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/create.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/list.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
     arguments = [verbose_option]
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         project.core.ui.echo("Virtualenvs created with this project:\n")
         for ident, venv in iter_venvs(project):
             saved_python = project._saved_python
-            if saved_python and Path(saved_python).parent.parent == venv:
+            if saved_python and Path(saved_python).parent.parent == venv.root:
                 mark = "*"
             else:
                 mark = "-"
-            project.core.ui.echo(f"{mark}  [success]{ident}[/]: {venv}")
+            project.core.ui.echo(f"{mark}  [success]{ident}[/]: {venv.root}")
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/purge.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/remove.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import shutil
 from pathlib import Path
 
 from pdm import termui
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.commands.venv.utils import get_venv_with_name, iter_venvs
+from pdm.cli.commands.venv.utils import get_venv_with_name
 from pdm.cli.options import verbose_option
 from pdm.project import Project
 
 
 class RemoveCommand(BaseCommand):
     """Remove the virtualenv with the given name"""
 
@@ -22,13 +22,13 @@
             help="Answer yes on the following question",
         )
         parser.add_argument("env", help="The key of the virtualenv")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         project.core.ui.echo("Virtualenvs created with this project:")
         venv = get_venv_with_name(project, options.env)
-        if options.yes or termui.confirm(f"[warning]Will remove: [success]{venv}[/], continue?", default=True):
-            shutil.rmtree(venv)
+        if options.yes or termui.confirm(f"[warning]Will remove: [success]{venv.root}[/], continue?", default=True):
+            shutil.rmtree(venv.root)
             saved_python = project._saved_python
-            if saved_python and Path(saved_python).parent.parent == venv:
+            if saved_python and Path(saved_python).parent.parent == venv.root:
                 project._saved_python = None
             project.core.ui.echo("Removed successfully!")
```

### Comparing `pdm-2.5.6/src/pdm/cli/commands/venv/utils.py` & `pdm-2.6.0/src/pdm/cli/commands/venv/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,55 @@
 from __future__ import annotations
 
 import base64
 import hashlib
-import sys
 from pathlib import Path
 from typing import Iterable, TypeVar
-from findpython import PythonVersion
 
+from findpython import PythonVersion
 from findpython.providers import BaseProvider
-from pdm.exceptions import PdmUsageError
 
+from pdm.exceptions import PdmUsageError
+from pdm.models.venv import VirtualEnv
 from pdm.project import Project
 
-IS_WIN = sys.platform == "win32"
-BIN_DIR = "Scripts" if IS_WIN else "bin"
-
 
 def hash_path(path: str) -> str:
     """Generate a hash for the given path."""
     return base64.urlsafe_b64encode(hashlib.new("md5", path.encode(), usedforsecurity=False).digest()).decode()[:8]
 
 
-def get_in_project_venv_python(root: Path) -> Path | None:
+def get_in_project_venv(root: Path) -> VirtualEnv | None:
     """Get the python interpreter path of venv-in-project"""
     for possible_dir in (".venv", "venv", "env"):
-        venv_python = get_venv_python(root / possible_dir)
-        if venv_python.exists():
-            return venv_python
+        venv = VirtualEnv.get(root / possible_dir)
+        if venv is not None:
+            return venv
     return None
 
 
 def get_venv_prefix(project: Project) -> str:
     """Get the venv prefix for the project"""
     path = project.root
     name_hash = hash_path(path.as_posix())
     return f"{path.name}-{name_hash}-"
 
 
-def iter_venvs(project: Project) -> Iterable[tuple[str, Path]]:
+def iter_venvs(project: Project) -> Iterable[tuple[str, VirtualEnv]]:
     """Return an iterable of venv paths associated with the project"""
-    in_project_venv_python = get_in_project_venv_python(project.root)
-    if in_project_venv_python is not None:
-        yield "in-project", Path(in_project_venv_python).parent.parent
+    in_project_venv = get_in_project_venv(project.root)
+    if in_project_venv is not None:
+        yield "in-project", in_project_venv
     venv_prefix = get_venv_prefix(project)
     venv_parent = Path(project.config["venv.location"])
-    for venv in venv_parent.glob(f"{venv_prefix}*"):
-        ident = venv.name[len(venv_prefix) :]
-        yield ident, venv
-
-
-def get_venv_python(venv: Path) -> Path:
-    """Get the interpreter path inside the given venv."""
-    suffix = ".exe" if IS_WIN else ""
-    return venv / BIN_DIR / f"python{suffix}"
+    for path in venv_parent.glob(f"{venv_prefix}*"):
+        ident = path.name[len(venv_prefix) :]
+        venv = VirtualEnv.get(path)
+        if venv is not None:
+            yield ident, venv
 
 
 def iter_central_venvs(project: Project) -> Iterable[tuple[str, Path]]:
     """Return an iterable of all managed venvs and their paths."""
     venv_parent = Path(project.config["venv.location"])
     for venv in venv_parent.glob("*"):
         ident = venv.name
@@ -74,21 +67,19 @@
 
     @classmethod
     def create(cls: type[T]) -> T | None:  # pragma: no cover
         return None
 
     def find_pythons(self) -> Iterable[PythonVersion]:
         for _, venv in iter_venvs(self.project):
-            python = get_venv_python(venv)
-            if python.exists():
-                yield PythonVersion(python, _interpreter=python, keep_symlink=True)
+            yield PythonVersion(venv.interpreter, _interpreter=venv.interpreter, keep_symlink=True)
 
 
-def get_venv_with_name(project: Project, name: str) -> Path:
+def get_venv_with_name(project: Project, name: str) -> VirtualEnv:
     all_venvs = dict(iter_venvs(project))
     try:
         return all_venvs[name]
     except KeyError:
         raise PdmUsageError(
             f"No virtualenv with key '{name}' is found, must be one of {list(all_venvs)}.\n"
             "You can create one with 'pdm venv create'.",
-        )
+        ) from None
```

### Comparing `pdm-2.5.6/src/pdm/cli/completions/pdm.bash` & `pdm-2.6.0/src/pdm/cli/completions/pdm.bash`

 * *Files 1% similar despite different names*

```diff
@@ -57,31 +57,31 @@
             ;;
 
             (import)
             opts="--dev --format --global --group --help --project --verbose"
             ;;
 
             (info)
-            opts="--env --global --help --packages --project --python --venv --verbose --where"
+            opts="--env --global --help --json --packages --project --python --venv --verbose --where"
             ;;
 
             (init)
             opts="--backend --global --help --lib --non-interactive --project --python --skip --verbose"
             ;;
 
             (install)
-            opts="--check --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-lock --no-self --production --project --skip --venv --verbose"
+            opts="--check --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-lock --no-self --plugins --production --project --skip --venv --verbose"
             ;;
 
             (list)
             opts="--csv --exclude --fields --freeze --global --graph --help --include --json --markdown --project --resolve --reverse --sort --venv --verbose"
             ;;
 
             (lock)
-            opts="--check --dev --global --group --help --lockfile --no-default --no-isolation --production --project --refresh --skip --verbose"
+            opts="--check --dev --global --group --help --lockfile --no-cross-platform --no-default --no-isolation --production --project --refresh --skip --verbose"
             ;;
 
             (plugin)
             opts="--help --verbose"
             ;;
 
             (publish)
@@ -89,15 +89,15 @@
             ;;
 
             (remove)
             opts="--dev --dry-run --fail-fast --global --group --help --lockfile --no-editable --no-isolation --no-self --no-sync --project --skip --venv --verbose"
             ;;
 
             (run)
-            opts="--global --help --list --project --site-packages --skip --venv --verbose"
+            opts="--global --help --json --list --project --site-packages --skip --venv --verbose"
             ;;
 
             (search)
             opts="--help --verbose"
             ;;
 
             (self)
```

### Comparing `pdm-2.5.6/src/pdm/cli/completions/pdm.fish` & `pdm-2.6.0/src/pdm/cli/completions/pdm.fish`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,19 @@
             return 1
         end
     end
     return 0
 end
 
 # global options
-complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l config -d 'Specify another config file path(env var: PDM_CONFIG_FILE)'
-complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l help -d 'show this help message and exit'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l config -d 'Specify another config file path [env var: PDM_CONFIG_FILE] '
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l help -d 'Show this help message and exit.'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l ignore-python -d 'Ignore the Python path saved in .pdm-python. [env var: PDM_IGNORE_SAVED_PYTHON]'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l pep582 -d 'Print the command line to be eval\'d by the shell'
-complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l version -d 'Show version'
 
 # commands
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a add -d 'Add package(s) to pyproject.toml and install them'
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a build -d 'Build artifacts for distribution'
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a cache -d 'Control the caches of PDM'
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a completion -d 'Generate completion scripts for the given shell'
@@ -49,15 +49,15 @@
 # add
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l dev -d 'Add packages into dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l editable -d 'Specify editable packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l group -d 'Specify the target dependency group to add into'
-complete -c pdm -A -n '__fish_seen_subcommand_from add' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from add' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-sync -d 'Only write pyproject.toml and do not sync the working set'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l prerelease -d 'Allow prereleases to be pinned'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
@@ -67,242 +67,246 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-wildcard -d 'Save wildcard version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l unconstrained -d 'Ignore the version constraint of packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from add' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from add' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # build
-complete -c pdm -A -n '__fish_seen_subcommand_from build' -l config-setting -d 'Pass options to the backend. options with a value must be specified after "=": "--config-setting=--opt(=value)" or "-C--opt(=value)"'
+complete -c pdm -A -n '__fish_seen_subcommand_from build' -l config-setting -d 'Pass options to the backend. options with a value must be specified after "=": `--config-setting=--opt(=value)` or `-C--opt(=value)`'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l dest -d 'Target directory to put artifacts'
-complete -c pdm -A -n '__fish_seen_subcommand_from build' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from build' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-clean -d 'Do not clean the target directory'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-sdist -d 'Don\'t build source tarballs'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-wheel -d 'Don\'t build wheels'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from build' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from build' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # cache
-complete -c pdm -A -n '__fish_seen_subcommand_from cache' -l help -d 'show this help message and exit'
-complete -c pdm -A -n '__fish_seen_subcommand_from cache' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from cache' -l help -d 'Show this help message and exit.'
+complete -c pdm -A -n '__fish_seen_subcommand_from cache' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # completion
-complete -c pdm -A -n '__fish_seen_subcommand_from completion' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from completion' -l help -d 'Show this help message and exit.'
 
 # config
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l delete -d 'Unset a configuration key'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from config' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from config' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l local -d 'Set config in the project\'s local configuration file'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
-complete -c pdm -A -n '__fish_seen_subcommand_from config' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from config' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # export
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l format -d 'Specify the export file format'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from export' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
-complete -c pdm -A -n '__fish_seen_subcommand_from export' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from export' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
+complete -c pdm -A -n '__fish_seen_subcommand_from export' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l output -d 'Write output to the given file, or print to stdout if not given'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l pyproject -d 'Read the list of packages from pyproject.toml'
-complete -c pdm -A -n '__fish_seen_subcommand_from export' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from export' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l without-hashes -d 'Don\'t include artifact hashes'
 
 # fix
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l dry-run -d 'Only show the problems'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
-complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # import
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l dev -d 'import packages into dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l format -d 'Specify the file format explicitly'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l group -d 'Specify the target dependency group to import into'
-complete -c pdm -A -n '__fish_seen_subcommand_from import' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from import' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
-complete -c pdm -A -n '__fish_seen_subcommand_from import' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from import' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # info
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l env -d 'Show PEP 508 environment markers'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from info' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from info' -l help -d 'Show this help message and exit.'
+complete -c pdm -A -n '__fish_seen_subcommand_from info' -l json -d 'Dump the information in JSON'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l packages -d 'Show the local packages root'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l python -d 'Show the interpreter path'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from info' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from info' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l where -d 'Show the project root path'
 
 # init
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l backend -d 'Specify the build backend'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from init' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from init' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l lib -d 'Create a library project'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l non-interactive -d 'Don\'t ask questions but use default values'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l python -d 'Specify the Python version/path to use'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from init' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from init' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # install
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l check -d 'Check if the lock file is up to date and fail otherwise'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from install' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
-complete -c pdm -A -n '__fish_seen_subcommand_from install' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from install' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
+complete -c pdm -A -n '__fish_seen_subcommand_from install' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-lock -d 'Don\'t do lock if the lock file is not found or outdated'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-self -d 'Don\'t install the project itself'
+complete -c pdm -A -n '__fish_seen_subcommand_from install' -l plugins -d 'Install the plugins specified in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from install' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from install' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # list
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l csv -d 'Output dependencies in CSV document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l exclude -d 'Exclude dependency groups from the output'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l fields -d 'Select information to output as a comma separated string. For example: name,version,homepage,licenses,groups.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l freeze -d 'Show the installed dependencies in pip\'s requirements.txt format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l graph -d 'Display a graph of dependencies'
-complete -c pdm -A -n '__fish_seen_subcommand_from list' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from list' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l include -d 'Dependency groups to include in the output. By default all are included'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l json -d 'Output dependencies in JSON document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l markdown -d 'Output dependencies and legal notices in markdown document format - best effort basis'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l resolve -d 'Resolve all requirements to output licenses (instead of just showing those currently installed)'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l reverse -d 'Reverse the dependency graph'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l sort -d 'Sort the output using a given field name. If nothing is set, no sort is applied. Multiple fields can be combined with \',\'.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from list' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from list' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # lock
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l check -d 'Check if the lock file is up to date and quit'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
-complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
+complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
+complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-cross-platform -d 'Only lock packages for the current platform'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l refresh -d 'Don\'t update pinned versions, only refresh the lock file'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # plugin
-complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l help -d 'show this help message and exit'
-complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l help -d 'Show this help message and exit.'
+complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # publish
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l ca-certs -d 'The path to a PEM-encoded Certificate Authority bundle to use for publish server validation [env var: PDM_PUBLISH_CA_CERTS]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l comment -d 'The comment to include with the distribution file.'
-complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l identity -d 'GPG identity used to sign files.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l no-build -d 'Don\'t build the package before publishing'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l password -d 'The password to access the repository [env var: PDM_PUBLISH_PASSWORD]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l repository -d 'The repository name or url to publish the package to [env var: PDM_PUBLISH_REPO]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l sign -d 'Upload the package with PGP signature'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l username -d 'The username to access the repository [env var: PDM_PUBLISH_USERNAME]'
-complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # remove
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l dev -d 'Remove packages from dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l group -d 'Specify the target dependency group to remove from'
-complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-sync -d 'Only write pyproject.toml and do not uninstall packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # run
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from run' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from run' -l help -d 'Show this help message and exit.'
+complete -c pdm -A -n '__fish_seen_subcommand_from run' -l json -d 'Output all scripts infos in JSON'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l list -d 'Show all available scripts defined in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l site-packages -d 'Load site-packages from the selected interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from run' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from run' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # search
-complete -c pdm -A -n '__fish_seen_subcommand_from search' -l help -d 'show this help message and exit'
-complete -c pdm -A -n '__fish_seen_subcommand_from search' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from search' -l help -d 'Show this help message and exit.'
+complete -c pdm -A -n '__fish_seen_subcommand_from search' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # self
-complete -c pdm -A -n '__fish_seen_subcommand_from self' -l help -d 'show this help message and exit'
-complete -c pdm -A -n '__fish_seen_subcommand_from self' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from self' -l help -d 'Show this help message and exit.'
+complete -c pdm -A -n '__fish_seen_subcommand_from self' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # show
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from show' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from show' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l keywords -d 'Show keywords'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l license -d 'Show license'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l name -d 'Show name'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l platform -d 'Show platform'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l summary -d 'Show summary'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from show' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from show' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l version -d 'Show version'
 
 # sync
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l clean -d 'clean packages not in the lockfile'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l clean -d 'Clean packages not in the lockfile'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-self -d 'Don\'t install the project itself'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l only-keep -d 'only keep the selected packages'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l only-keep -d 'Only keep the selected packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l reinstall -d 'Force reinstall existing dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # update
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from update' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
-complete -c pdm -A -n '__fish_seen_subcommand_from update' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from update' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
+complete -c pdm -A -n '__fish_seen_subcommand_from update' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-sync -d 'Only update lock file but do not sync packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l outdated -d 'Show the difference only without modifying the lockfile content'
@@ -316,23 +320,23 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l top -d 'Only update those listed in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l unconstrained -d 'Ignore the version constraint of packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
-complete -c pdm -A -n '__fish_seen_subcommand_from update' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from update' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # use
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l first -d 'Select the first matched interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l global -d 'Use the global project, supply the project root with `-p` option'
-complete -c pdm -A -n '__fish_seen_subcommand_from use' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from use' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l ignore-remembered -d 'Ignore the remembered selection'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l venv -d 'Use the interpreter in the virtual environment with the given name'
-complete -c pdm -A -n '__fish_seen_subcommand_from use' -l verbose -d '-v for detailed output and -vv for more detailed'
+complete -c pdm -A -n '__fish_seen_subcommand_from use' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # venv
-complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l help -d 'show this help message and exit'
+complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l path -d 'Show the path to the given virtualenv'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l python -d 'Show the python interpreter path for the given virtualenv'
```

### Comparing `pdm-2.5.6/src/pdm/cli/completions/pdm.ps1` & `pdm-2.6.0/src/pdm/cli/completions/pdm.ps1`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
                         $projectOption
                     ))
                 break
             }
             "info" {
                 $completer.AddOpts(
                     @(
-                        [Option]::new(@("--env", "--global", "-g", "--python", "--where", "--packages")),
+                        [Option]::new(@("--env", "--global", "-g", "--python", "--where", "--packages", "--json")),
                         $projectOption,
                         $venvOption
                     ))
                 break
             }
             "init" {
                 $completer.AddOpts(
@@ -290,15 +290,15 @@
                 break
             }
             "install" {
                 $completer.AddOpts(@(
                         [Option]::new((
                             "-d", "--dev", "-g", "--global", "--dry-run", "--no-default", "--no-lock", "--prod",
                             "--production", "--no-editable", "--no-self", "--no-isolation", "--check", "-L",
-                            "--lockfile", "--fail-fast", "-x"
+                            "--lockfile", "--fail-fast", "-x", "--plugins"
                         )),
                         $sectionOption,
                         $skipOption,
                         $venvOption,
                         $projectOption
                     ))
                 break
@@ -311,15 +311,15 @@
                         $projectOption
                     ))
                 break
             }
             "lock" {
                 $completer.AddOpts(
                     @(
-                        [Option]::new(@("--global", "-g", "--no-isolation", "--refresh", "-L", "--lockfile", "--check", "--dev", "--prod", "--production", "-d", "--no-default")),
+                        [Option]::new(@("--global", "-g", "--no-isolation", "--refresh", "-L", "--lockfile", "--check", "--dev", "--prod", "--production", "-d", "--no-default", "--no-cross-platform")),
                         $skipOption,
                         $sectionOption,
                         $projectOption
                     ))
                 break
             }
             "self" {
@@ -371,15 +371,15 @@
                     ))
                 $completer.AddParams(@(getPdmPackages), $true)
                 break
             }
             "run" {
                 $completer.AddOpts(
                     @(
-                        [Option]::new(@("--global", "-g", "-l", "--list", "-s", "--site-packages")),
+                        [Option]::new(@("--global", "-g", "-l", "--list", "-s", "--site-packages", "--json")),
                         $skipOption,
                         $venvOption,
                         $projectOption
                     ))
                 $completer.AddParams(@(getScripts), $false)
                 break
             }
```

### Comparing `pdm-2.5.6/src/pdm/cli/completions/pdm.zsh` & `pdm-2.6.0/src/pdm/cli/completions/pdm.zsh`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         '--save-exact[Save exact version specifiers]'
         '--save-minimum[Save minimum version specifiers]'
         '--update-reuse[Reuse pinned versions already present in lock file if possible]'
         '--update-eager[Try to update the packages and their dependencies recursively]'
         '--update-all[Update all dependencies and sub-dependencies]'
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         {-u,--unconstrained}'[Ignore the version constraint of packages]'
         {--pre,--prerelease}'[Allow prereleases to be pinned]'
         {-e+,--editable+}'[Specify editable packages]:packages'
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lockfile content]"
@@ -170,15 +170,16 @@
     info)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         '--python[Show the interpreter path]'
         '--where[Show the project root path]'
         '--env[Show PEP 508 environment markers]'
         '--packages[Show the packages root]'
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        '--json[Dump the information in JSON]'
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
       )
       ;;
     init)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-n,--non-interactive}"[Don't ask questions but use default values]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
@@ -199,15 +200,16 @@
         "--no-default[Don\'t include dependencies from the default group]"
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lock file content]"
         "--check[Check if the lock file is up to date and fail otherwise]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        "--plugins[Install the plugins specified in pyproject.toml]"
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
       )
       ;;
     list)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-r,--reverse}'[Reverse the dependency graph]'
         '--fields[Select information to output as a comma separated string.]:fields:'
@@ -215,30 +217,31 @@
         '--json[Output dependencies in JSON document format]'
         '--csv[Output dependencies in CSV document format]'
         '--markdown[Output dependencies and legal notices in markdown document format - best effort basis]'
         '--graph[Display a graph of dependencies]'
         "--freeze[Show the installed dependencies as pip's requirements.txt format]"
         "--include[Dependency groups to include in the output. By default all are included]:include:"
         "--exclude[Dependency groups to exclude from the output]:exclude:"
-        "--resolve[Resolve all requirements to output licenses (instead of just showing those currently installed)"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        "--resolve[Resolve all requirements to output licenses (instead of just showing those currently installed)]"
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
       )
       ;;
     lock)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
         "--no-isolation[Do not isolate the build in a clean environment]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         "--refresh[Don't update pinned versions, only refresh the lock file]"
         "--check[Check if the lock file is up to date and quit]"
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-d,--dev}"[Select dev dependencies]"
         {--prod,--production}"[Unselect dev dependencies]"
         "--no-default[Don\'t include dependencies from the default group]"
+        "--no-cross-platform[Only lock packages for the current platform]"
       )
       ;;
     self)
       _arguments -C \
         $arguments \
         ': :->command' \
         '*:: :->args' && ret=0
@@ -308,25 +311,26 @@
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         "--no-sync[Only write pyproject.toml and do not uninstall packages]"
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lockfile content]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
         "*:packages:_pdm_packages"
       )
       ;;
     run)
       _arguments -s \
         {-g,--global}'[Use the global project, supply the project root with `-p` option]' \
         {-l,--list}'[Show all available scripts defined in pyproject.toml]' \
+        '--json[Output all scripts infos in JSON]' \
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]' \
         {-s,--site-packages}'[Load site-packages from the selected interpreter]' \
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:' \
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:' \
         '(-)1:command:->command' \
         '*:arguments: _normal ' && return 0
       if [[ $state == command ]]; then
         _command_names -e
         local local_commands=($(_pdm_scripts))
         _describe "local command" local_commands
         return 0
@@ -342,15 +346,15 @@
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         '--name[Show name]'
         '--version[Show version]'
         '--summary[Show summary]'
         '--license[Show license]'
         '--platform[Show platform]'
         '--keywords[Show keywords]'
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
         '1:package:'
       )
       ;;
     sync)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
@@ -363,15 +367,15 @@
         '--clean[Clean unused packages]'
         "--only-keep[Only keep the selected packages]"
         "--no-default[Don\'t include dependencies from the default group]"
         {-x,--fail-fast}'[Abort on first installation error]'
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         "--no-isolation[do not isolate the build in a clean environment]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
       )
       ;;
     update)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
@@ -392,15 +396,15 @@
         {--prod,--production}"[Unselect dev dependencies]"
         "--no-default[Don\'t include dependencies from the default group]"
         {-t,--top}'[Only update those list in pyproject.toml]'
         "--dry-run[Show the difference only without modifying the lockfile content]"
         "--outdated[Show the difference only without modifying the lockfile content]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. (env var: PDM_IN_VENV)]:venv:'
         "*:packages:_pdm_packages"
       )
       ;;
     use)
       arguments+=(
         {-f,--first}'[Select the first matched interpreter]'
         {-i,--ignore-remembered}'[Ignore the remembered selection]'
```

### Comparing `pdm-2.5.6/src/pdm/cli/filters.py` & `pdm-2.6.0/src/pdm/cli/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,27 +47,32 @@
         return "dev" if self.dev else "default"
 
     @property
     def is_unset(self) -> bool:
         return self.default and self.dev is None and not self.groups
 
     def all(self) -> list[str] | None:
+        project_groups = list(self.project.iter_groups())
         if self.is_unset:
             if self.project.lockfile.exists():
-                return self.project.lockfile.groups
+                groups = self.project.lockfile.groups
+                if groups:
+                    groups = [g for g in groups if g in project_groups]
+                return groups
         return list(self)
 
     @cached_property
     def _translated_groups(self) -> list[str]:
         """Translate default, dev and groups containing ":all" into a list of groups"""
         if self.is_unset:
             # Default case, return what is in the lock file
             locked_groups = self.project.lockfile.groups
+            project_groups = list(self.project.iter_groups())
             if locked_groups:
-                return locked_groups
+                return [g for g in locked_groups if g in project_groups]
         default, dev, groups = self.default, self.dev, self.groups
         if dev is None:  # --prod is not set, include dev-dependencies
             dev = True
         project = self.project
         optional_groups = set(project.pyproject.metadata.get("optional-dependencies", {}))
         dev_groups = set(project.pyproject.settings.get("dev-dependencies", {}))
         groups_set = set(groups)
```

### Comparing `pdm-2.5.6/src/pdm/cli/hooks.py` & `pdm-2.6.0/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/cli/options.py` & `pdm-2.6.0/src/pdm/cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 
 verbose_option = Option(
     "-v",
     "--verbose",
     action="count",
     default=0,
-    help="-v for detailed output and -vv for more detailed",
+    help="Use `-v` for detailed output and `-vv` for more detailed",
 )
 
 
 dry_run_option = Option(
     "--dry-run",
     action="store_true",
     default=False,
@@ -180,15 +180,15 @@
 groups_group.add_argument(
     "-G",
     "--group",
     dest="groups",
     metavar="GROUP",
     action=split_lists(","),
     help="Select group of optional-dependencies separated by comma "
-    "or dev-dependencies(with -d). Can be supplied multiple times, "
+    "or dev-dependencies (with `-d`). Can be supplied multiple times, "
     'use ":all" to include all groups under the same species.',
     default=[],
 )
 groups_group.add_argument(
     "--no-default",
     dest="default",
     action="store_false",
@@ -292,20 +292,20 @@
     "--global",
     dest="global_project",
     action="store_true",
     help="Use the global project, supply the project root with `-p` option",
 )
 
 clean_group = ArgumentGroup("clean", is_mutually_exclusive=True)
-clean_group.add_argument("--clean", action="store_true", help="clean packages not in the lockfile")
-clean_group.add_argument("--only-keep", action="store_true", help="only keep the selected packages")
+clean_group.add_argument("--clean", action="store_true", help="Clean packages not in the lockfile")
+clean_group.add_argument("--only-keep", action="store_true", help="Only keep the selected packages")
 
 sync_group = ArgumentGroup("sync", is_mutually_exclusive=True)
-sync_group.add_argument("--sync", action="store_true", dest="sync", help="sync packages")
-sync_group.add_argument("--no-sync", action="store_false", dest="sync", help="don't sync packages")
+sync_group.add_argument("--sync", action="store_true", dest="sync", help="Sync packages")
+sync_group.add_argument("--no-sync", action="store_false", dest="sync", help="Don't sync packages")
 
 packages_group = ArgumentGroup("Package Arguments")
 packages_group.add_argument(
     "-e",
     "--editable",
     dest="editables",
     action="append",
```

### Comparing `pdm-2.5.6/src/pdm/cli/utils.py` & `pdm-2.6.0/src/pdm/cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import argparse
+import dataclasses as dc
 import json
 import os
 import sys
 from collections import ChainMap, OrderedDict
 from concurrent.futures import ThreadPoolExecutor
 from json import dumps
 from pathlib import Path
@@ -51,31 +52,14 @@
     from pdm.compat import Distribution
     from pdm.compat import importlib_metadata as im
     from pdm.models.candidates import Candidate
     from pdm.models.repositories import BaseRepository
     from pdm.project import Project
 
 
-class ErrorArgumentParser(argparse.ArgumentParser):
-    """A subclass of argparse.ArgumentParser that raises
-    parsing error rather than exiting.
-
-    This does the same as passing exit_on_error=False on Python 3.9+
-    """
-
-    def _parse_known_args(
-        self, arg_strings: list[str], namespace: argparse.Namespace
-    ) -> tuple[argparse.Namespace, list[str]]:
-        try:
-            return super()._parse_known_args(arg_strings, namespace)
-        except argparse.ArgumentError as e:
-            # We raise a dedicated error to avoid being caught by the caller
-            raise PdmArgumentError(e) from e
-
-
 class PdmFormatter(argparse.RawDescriptionHelpFormatter):
     def start_section(self, heading: str | None) -> None:
         return super().start_section(termui.style(heading.title() if heading else "", style="warning"))
 
     def _format_usage(
         self,
         usage: str | None,
@@ -133,33 +117,54 @@
         for subaction in self._iter_indented_subactions(action):
             parts.append(self._format_action(subaction))
 
         # return a single string
         return self._join_parts(parts)
 
 
+class ArgumentParser(argparse.ArgumentParser):
+    """A standard argument parser but with title-cased help."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        kwargs["formatter_class"] = PdmFormatter
+        kwargs["add_help"] = False
+        super().__init__(*args, **kwargs)
+        self.add_argument(
+            "-h", "--help", action="help", default=argparse.SUPPRESS, help="Show this help message and exit."
+        )
+
+
+class ErrorArgumentParser(ArgumentParser):
+    """A subclass of argparse.ArgumentParser that raises
+    parsing error rather than exiting.
+
+    This does the same as passing exit_on_error=False on Python 3.9+
+    """
+
+    def _parse_known_args(
+        self, arg_strings: list[str], namespace: argparse.Namespace
+    ) -> tuple[argparse.Namespace, list[str]]:
+        try:
+            return super()._parse_known_args(arg_strings, namespace)
+        except argparse.ArgumentError as e:
+            # We raise a dedicated error to avoid being caught by the caller
+            raise PdmArgumentError(e) from e
+
+
+@dc.dataclass(frozen=True)
 class Package:
     """An internal class for the convenience of dependency graph building."""
 
-    def __init__(self, name: str, version: str | None, requirements: dict[str, Requirement]) -> None:
-        self.name = name
-        self.version = version  # if version is None, the dist is not installed.
-        self.requirements = requirements
-
-    def __hash__(self) -> int:
-        return hash(self.name)
+    name: str = dc.field(hash=True, compare=True)
+    version: str | None = dc.field(compare=False)
+    requirements: dict[str, Requirement] = dc.field(compare=False)
 
     def __repr__(self) -> str:
         return f"<Package {self.name}=={self.version}>"
 
-    def __eq__(self, value: object) -> bool:
-        if not isinstance(value, Package):
-            return False
-        return self.name == value.name
-
 
 def build_dependency_graph(
     working_set: Mapping[str, im.Distribution],
     marker_env: dict[str, str] | None = None,
     selected: set[str] | None = None,
     include_sub: bool = True,
 ) -> DirectedGraph:
@@ -659,15 +664,15 @@
     script_dir.mkdir(parents=True, exist_ok=True)
     with resources_open_binary("pdm.pep582", "sitecustomize.py") as f:
         script_dir.joinpath("sitecustomize.py").write_bytes(f.read())
     return str(script_dir)
 
 
 def use_venv(project: Project, name: str) -> None:
-    from pdm.cli.commands.venv.utils import get_venv_python, get_venv_with_name
+    from pdm.cli.commands.venv.utils import get_venv_with_name
     from pdm.environments import PythonEnvironment
 
     venv = get_venv_with_name(project, cast(str, name))
     project.core.ui.echo(
-        f"In virtual environment: [success]{venv}[/]", err=True, style="info", verbosity=termui.Verbosity.DETAIL
+        f"In virtual environment: [success]{venv.root}[/]", err=True, style="info", verbosity=termui.Verbosity.DETAIL
     )
-    project.environment = PythonEnvironment(project, python=str(get_venv_python(venv)))
+    project.environment = PythonEnvironment(project, python=str(venv.interpreter))
```

### Comparing `pdm-2.5.6/src/pdm/compat.py` & `pdm-2.6.0/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/core.py` & `pdm-2.6.0/src/pdm/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from resolvelib import Resolver
 
 from pdm import termui
 from pdm.__version__ import __version__
 from pdm.cli.actions import check_update
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.options import ignore_python_option, pep582_option, verbose_option
-from pdm.cli.utils import ErrorArgumentParser, PdmFormatter
+from pdm.cli.utils import ArgumentParser, ErrorArgumentParser
 from pdm.compat import importlib_metadata
 from pdm.exceptions import PdmArgumentError, PdmUsageError
 from pdm.installers import InstallManager, Synchronizer
 from pdm.models.repositories import PyPIRepository
 from pdm.project import Project
 from pdm.project.config import Config, ConfigItem
 from pdm.utils import is_in_zipapp
@@ -53,38 +53,37 @@
         self.init_parser()
         self.load_plugins()
 
     def init_parser(self) -> None:
         self.parser = ErrorArgumentParser(
             prog="pdm",
             description=__doc__,
-            formatter_class=PdmFormatter,
         )
         self.parser.is_root = True  # type: ignore[attr-defined]
         self.parser.add_argument(
             "-V",
             "--version",
             action="version",
             version="{}, version {}".format(
                 termui.style("PDM", style="bold"),
                 termui.style(self.version, style="success"),
             ),
-            help="show the version and exit",
+            help="Show the version and exit",
         )
         self.parser.add_argument(
             "-c",
             "--config",
-            help="Specify another config file path(env var: PDM_CONFIG_FILE)",
+            help="Specify another config file path [env var: PDM_CONFIG_FILE] ",
         )
         self.parser._positionals.title = "Commands"
         verbose_option.add_to_parser(self.parser)
         ignore_python_option.add_to_parser(self.parser)
         pep582_option.add_to_parser(self.parser)
 
-        self.subparsers = self.parser.add_subparsers(parser_class=argparse.ArgumentParser)
+        self.subparsers = self.parser.add_subparsers(parser_class=ArgumentParser)
         for _, name, _ in pkgutil.iter_modules(COMMANDS_MODULE_PATH):
             module = importlib.import_module(f"pdm.cli.commands.{name}", __name__)
             try:
                 klass = module.Command
             except AttributeError:
                 continue
             self.register_command(klass, klass.name or name)
@@ -221,24 +220,38 @@
 
         Args:
             name (str): The name of the config item
             config_item (pdm.project.config.ConfigItem): The config item to add
         """
         Config.add_config(name, config_item)
 
+    def _add_project_plugins_library(self) -> None:
+        project = self.create_project(is_global=False)
+        if project.is_global or not project.root.joinpath(".pdm-plugins").exists():
+            return
+
+        import site
+        import sysconfig
+
+        base = str(project.root / ".pdm-plugins")
+        replace_vars = {"base": base, "platbase": base}
+        scheme = "nt" if os.name == "nt" else "posix_prefix"
+        site.addsitedir(sysconfig.get_path("purelib", scheme, replace_vars))
+
     def load_plugins(self) -> None:
         """Import and load plugins under `pdm.plugin` namespace
         A plugin is a callable that accepts the core object as the only argument.
 
         Example:
             ```python
             def my_plugin(core: pdm.core.Core) -> None:
                 ...
             ```
         """
+        self._add_project_plugins_library()
         entry_points: Iterable[importlib_metadata.EntryPoint] = itertools.chain(
             importlib_metadata.entry_points(group="pdm"),
             importlib_metadata.entry_points(group="pdm.plugin"),
         )
         for plugin in entry_points:
             try:
                 plugin.load()(self)
```

### Comparing `pdm-2.5.6/src/pdm/environments/base.py` & `pdm-2.6.0/src/pdm/environments/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,33 +29,37 @@
 
 
 class BaseEnvironment(abc.ABC):
     """Environment dependent stuff related to the selected Python interpreter."""
 
     is_local = False
 
-    def __init__(self, project: Project) -> None:
+    def __init__(self, project: Project, *, python: str | None = None) -> None:
         """
         :param project: the project instance
         """
         self.python_requires = project.python_requires
         self.project = project
         self.auth = PdmBasicAuth(
             self.project.sources,
             self.project.core.ui.verbosity >= termui.Verbosity.DETAIL,
         )
+        if python is None:
+            self._interpreter = project.python
+        else:
+            self._interpreter = PythonInfo.from_path(python)
 
     @property
     def is_global(self) -> bool:
         """For backward compatibility, it is opposite to ``is_local``."""
         return not self.is_local
 
     @property
     def interpreter(self) -> PythonInfo:
-        return self.project.python
+        return self._interpreter
 
     @abc.abstractmethod
     def get_paths(self) -> dict[str, str]:
         """Get paths like ``sysconfig.get_paths()`` for installation."""
         ...
 
     @property
@@ -203,24 +207,15 @@
         return command
 
 
 class BareEnvironment(BaseEnvironment):
     """Bare environment that does not depend on project files."""
 
     def __init__(self, project: Project) -> None:
-        self.python_requires = project.python_requires
-        self.project = project
-        self.auth = PdmBasicAuth(
-            self.project.sources,
-            self.project.core.ui.verbosity >= termui.Verbosity.DETAIL,
-        )
-
-    @property
-    def interpreter(self) -> PythonInfo:
-        return PythonInfo.from_path(sys.executable)
+        super().__init__(project, python=sys.executable)
 
     def get_paths(self) -> dict[str, str]:
         return {}
 
     def get_working_set(self) -> WorkingSet:
         if self.project.project_config.config_file.exists():
             return self.project.get_environment().get_working_set()
```

### Comparing `pdm-2.5.6/src/pdm/environments/local.py` & `pdm-2.6.0/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/environments/prefix.py` & `pdm-2.6.0/src/pdm/environments/python.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 from __future__ import annotations
 
+import os
 from typing import TYPE_CHECKING
 
 from pdm.environments.base import BaseEnvironment
 from pdm.models.in_process import get_sys_config_paths
 
 if TYPE_CHECKING:
     from pdm.project import Project
 
 
-class PrefixEnvironment(BaseEnvironment):
-    """An environment whose install scheme depends on the given prefix"""
+class PythonEnvironment(BaseEnvironment):
+    """A project environment that is directly derived from a Python interpreter"""
 
-    def __init__(self, project: Project, *, prefix: str) -> None:
-        super().__init__(project)
+    def __init__(self, project: Project, *, python: str | None = None, prefix: str | None = None) -> None:
+        super().__init__(project, python=python)
         self.prefix = prefix
 
     def get_paths(self) -> dict[str, str]:
-        paths = get_sys_config_paths(
-            str(self.interpreter.executable),
-            {"base": self.prefix, "platbase": self.prefix},
-            kind="prefix",
-        )
+        is_venv = self.interpreter.get_venv() is not None
+        if self.prefix is not None:
+            replace_vars = {"base": self.prefix, "platbase": self.prefix}
+            kind = "prefix"
+        else:
+            replace_vars = None
+            kind = "user" if not is_venv and self.project.global_config["global_project.user_site"] else "default"
+        paths = get_sys_config_paths(str(self.interpreter.executable), replace_vars, kind=kind)
+        if is_venv and self.prefix is None:
+            python_xy = f"python{self.interpreter.identifier}"
+            paths["include"] = os.path.join(paths["data"], "include", "site", python_xy)
         paths["prefix"] = paths["data"]
         paths["headers"] = paths["include"]
         return paths
+
+    @property
+    def process_env(self) -> dict[str, str]:
+        env = super().process_env
+        venv = self.interpreter.get_venv()
+        if venv is not None and self.prefix is None:
+            env.update(venv.env_vars())
+        return env
```

### Comparing `pdm-2.5.6/src/pdm/exceptions.py` & `pdm-2.6.0/src/pdm/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
 
 class UninstallError(PdmException):
     pass
 
 
 class NoConfigError(PdmUsageError, KeyError):
-    def __init__(self, key: str) -> None:
-        super().__init__(f"No such config item: {key}")
+    def __str__(self) -> str:
+        return f"Not such config key: {self.args[0]!r}"
 
 
 class NoPythonVersion(PdmUsageError):
     pass
 
 
 class BuildError(PdmException, RuntimeError):
```

### Comparing `pdm-2.5.6/src/pdm/formats/__init__.py` & `pdm-2.6.0/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/formats/base.py` & `pdm-2.6.0/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/formats/flit.py` & `pdm-2.6.0/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/formats/pipfile.py` & `pdm-2.6.0/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/formats/poetry.py` & `pdm-2.6.0/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/formats/requirements.py` & `pdm-2.6.0/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/formats/setup_py.py` & `pdm-2.6.0/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/installers/core.py` & `pdm-2.6.0/src/pdm/installers/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from __future__ import annotations
 
 from pdm.environments import BaseEnvironment
-from pdm.installers.manager import InstallManager
+from pdm.installers.synchronizers import BaseSynchronizer
 from pdm.models.requirements import Requirement
 from pdm.models.specifiers import PySpecSet
 from pdm.resolver.core import resolve
-from pdm.termui import logger
 
 
 def install_requirements(
-    reqs: list[Requirement],
-    environment: BaseEnvironment,
-    use_install_cache: bool = False,
+    reqs: list[Requirement], environment: BaseEnvironment, clean: bool = False
 ) -> None:  # pragma: no cover
     """Resolve and install the given requirements into the environment."""
     project = environment.project
     # Rewrite the python requires to only resolve for the current python version.
     environment.python_requires = PySpecSet(f"=={environment.interpreter.version}")
     provider = project.get_provider(ignore_compatibility=False)
     reporter = project.get_reporter(reqs)
@@ -27,19 +24,9 @@
             req.relocate(backend)  # type: ignore[attr-defined]
     resolved, _ = resolve(
         resolver,
         reqs,
         environment.python_requires,
         max_rounds=resolve_max_rounds,
     )
-    manager = InstallManager(environment, use_install_cache=use_install_cache)
-    working_set = environment.get_working_set()
-    for key, candidate in resolved.items():
-        if "[" in key:
-            # This is a candidate with extras, just skip it as it will be handled
-            # by the one without extras.
-            continue
-        logger.info("Installing %s %s", candidate.name, candidate.version)
-        if key in working_set:
-            # Force reinstall the package if it's already installed.
-            manager.uninstall(working_set[key])
-        manager.install(candidate)
+    syncer = BaseSynchronizer(resolved, environment, clean=clean, retry_times=0)
+    syncer.synchronize()
```

### Comparing `pdm-2.5.6/src/pdm/installers/installers.py` & `pdm-2.6.0/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/installers/manager.py` & `pdm-2.6.0/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/installers/packages.py` & `pdm-2.6.0/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/installers/synchronizers.py` & `pdm-2.6.0/src/pdm/installers/synchronizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 def editables_candidate(environment: BaseEnvironment) -> Candidate | None:
     """Return a candidate for `editables` package"""
     repository = environment.project.get_repository()
     return next(iter(repository.find_candidates(parse_requirement("editables"))), None)
 
 
-class Synchronizer:
+class BaseSynchronizer:
     """Synchronize the working set with given installation candidates
 
     :param candidates: a dict of candidates to be installed
     :param environment: the environment associated with the project
     :param clean: clean unneeded packages
     :param dry_run: only prints summary but do not install or uninstall
     :param retry_times: retry times when installation failed
@@ -104,27 +104,26 @@
         candidates: dict[str, Candidate],
         environment: BaseEnvironment,
         clean: bool = False,
         dry_run: bool = False,
         retry_times: int = 1,
         install_self: bool = False,
         no_editable: bool | Collection[str] = False,
-        use_install_cache: bool = False,
         reinstall: bool = False,
         only_keep: bool = False,
         fail_fast: bool = False,
     ) -> None:
         self.requested_candidates = candidates
         self.environment = environment
         self.clean = clean
         self.dry_run = dry_run
         self.retry_times = retry_times
         self.no_editable = no_editable
         self.install_self = install_self
-        self.use_install_cache = use_install_cache
+        self.use_install_cache = environment.project.config["install.cache"]
         self.reinstall = reinstall
         self.only_keep = only_keep
         self.parallel = environment.project.config["install.parallel"]
         self.fail_fast = fail_fast
 
         self.working_set = environment.get_working_set()
         self.ui = environment.project.core.ui
@@ -162,22 +161,14 @@
         """Return whether to add editables"""
         if not self.install_self or "editables" in self.requested_candidates:
             return False
         # As editables may be added by the backend, we need to check the metadata
         metadata = self.self_candidate.prepare(self.environment).metadata
         return any(req.startswith("editables") for req in metadata.requires or [])
 
-    def create_executor(
-        self,
-    ) -> ThreadPoolExecutor | DummyExecutor:
-        if self.parallel:
-            return ThreadPoolExecutor(max_workers=min(multiprocessing.cpu_count(), 8))
-        else:
-            return DummyExecutor()
-
     @property
     def manager(self) -> InstallManager:
         if not self._manager:
             self._manager = self.get_manager()
         return self._manager
 
     def get_manager(self) -> InstallManager:
@@ -215,15 +206,15 @@
         candidates = self.candidates.copy()
         to_update: set[str] = set()
         to_remove: set[str] = set()
         locked_repository = self.environment.project.locked_repository
         all_candidate_keys = list(locked_repository.all_candidates)
 
         for key, dist in working_set.items():
-            if key == self.self_key:
+            if key == self.self_key and self.install_self:
                 continue
             if key in candidates:
                 can = candidates.pop(key)
                 if self._should_update(dist, can):
                     to_update.add(key)
             elif (
                 self.only_keep or self.clean and key not in all_candidate_keys
@@ -238,14 +229,45 @@
         }
         return (
             sorted(to_add),
             sorted(to_update),
             sorted(to_remove),
         )
 
+    def synchronize(self) -> None:
+        """Synchronize the working set with pinned candidates."""
+        to_add, to_update, to_remove = self.compare_with_working_set()
+        manager = self.manager
+        for key in to_add:
+            can = self.candidates[key]
+            termui.logger.info("Installing %s@%s...", key, can.version)
+            manager.install(can)
+        for key in to_update:
+            can = self.candidates[key]
+            dist = self.working_set[strip_extras(key)[0]]
+            dist_version = dist.version
+            termui.logger.info("Updating %s@%s -> %s...", key, dist_version, can.version)
+            manager.uninstall(dist)
+            manager.install(can)
+        for key in to_remove:
+            dist = self.working_set[key]
+            termui.logger.info("Removing %s@%s...", key, dist.version)
+            manager.uninstall(dist)
+        termui.logger.info("Synchronization complete.")
+
+
+class Synchronizer(BaseSynchronizer):
+    def create_executor(
+        self,
+    ) -> ThreadPoolExecutor | DummyExecutor:
+        if self.parallel:
+            return ThreadPoolExecutor(max_workers=min(multiprocessing.cpu_count(), 8))
+        else:
+            return DummyExecutor()
+
     def install_candidate(self, key: str, progress: Progress) -> Candidate:
         """Install candidate"""
         can = self.candidates[key]
         job = progress.add_task(f"Installing {can.format()}...", total=1)
         try:
             self.manager.install(can)
         except Exception:
@@ -345,15 +367,14 @@
                 lines.append(f"  - [req]{dist.metadata['Name']}[/] [warning]{dist.version}[/]")
         if lines:
             self.ui.echo("\n".join(lines))
         else:
             self.ui.echo("All packages are synced to date, nothing to do.")
 
     def synchronize(self) -> None:
-        """Synchronize the working set with pinned candidates."""
         to_add, to_update, to_remove = self.compare_with_working_set()
         to_do = {"remove": to_remove, "update": to_update, "add": to_add}
 
         if self.dry_run:
             self._show_summary(to_do)
             return
```

### Comparing `pdm-2.5.6/src/pdm/installers/uninstallers.py` & `pdm-2.6.0/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/auth.py` & `pdm-2.6.0/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/backends.py` & `pdm-2.6.0/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/caches.py` & `pdm-2.6.0/src/pdm/models/caches.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 import contextlib
 import dataclasses
 import hashlib
 import json
 import os
+from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, BinaryIO, Generic, Iterable, TypeVar, cast
 
 import requests
 from cachecontrol.cache import BaseCache
 from cachecontrol.caches import FileCache
 from packaging.utils import canonicalize_name, parse_wheel_filename
 
 from pdm._types import CandidateInfo
 from pdm.exceptions import PdmException
 from pdm.models.candidates import Candidate
 from pdm.termui import logger
-from pdm.utils import atomic_open_for_write
+from pdm.utils import atomic_open_for_write, create_tracked_tempdir
 
 if TYPE_CHECKING:
+    from packaging.tags import Tag
     from unearth import Link, TargetPython
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
 
 class JSONFileCache(Generic[KT, VT]):
@@ -167,48 +169,64 @@
     Wheels are only cached when the URL contains egg-info or is a VCS repository
     with an *immutable* revision. There might be more than one wheels built for
     one sdist, the one with most preferred tag will be returned.
     """
 
     def __init__(self, directory: Path) -> None:
         self.directory = directory
+        self.ephemeral_directory = Path(create_tracked_tempdir(prefix="pdm-wheel-cache-"))
 
-    def _get_candidates(self, link: Link, target_python: TargetPython) -> Iterable[Path]:
-        path = self.get_path_for_link(link, target_python)
+    def _get_candidates(self, path: Path) -> Iterable[Path]:
         if not path.exists():
             return
         for candidate in path.iterdir():
             if candidate.name.endswith(".whl"):
                 yield candidate
 
-    def get_path_for_link(self, link: Link, target_python: TargetPython) -> Path:
+    def _get_path_parts(self, link: Link, target_python: TargetPython) -> tuple[str, ...]:
         hash_key = {
             "url": link.url_without_fragment,
             # target python participates in the hash key to handle the some cases
             # where the sdist produces different wheels on different Pythons, and
             # the differences are not encoded in compatibility tags.
             "target_python": dataclasses.astuple(target_python),
         }
         if link.subdirectory:
             hash_key["subdirectory"] = link.subdirectory
         if link.hash:
             hash_key[link.hash_name] = link.hash
         hashed = hashlib.sha224(
             json.dumps(hash_key, sort_keys=True, separators=(",", ":"), ensure_ascii=True).encode("utf-8")
         ).hexdigest()
-        parts = (hashed[:2], hashed[2:4], hashed[4:6], hashed[6:])
+        return (hashed[:2], hashed[2:4], hashed[4:6], hashed[6:])
+
+    def get_path_for_link(self, link: Link, target_python: TargetPython) -> Path:
+        parts = self._get_path_parts(link, target_python)
         return self.directory.joinpath(*parts)
 
+    def get_ephemeral_path_for_link(self, link: Link, target_python: TargetPython) -> Path:
+        parts = self._get_path_parts(link, target_python)
+        return self.ephemeral_directory.joinpath(*parts)
+
     def get(self, link: Link, project_name: str | None, target_python: TargetPython) -> Path | None:
         if not project_name:
             return None
         canonical_name = canonicalize_name(project_name)
         tags_priorities = {tag: i for i, tag in enumerate(target_python.supported_tags())}
+
+        candidate = self._get_from_path(self.get_path_for_link(link, target_python), canonical_name, tags_priorities)
+        if candidate is not None:
+            return candidate
+        return self._get_from_path(
+            self.get_ephemeral_path_for_link(link, target_python), canonical_name, tags_priorities
+        )
+
+    def _get_from_path(self, path: Path, canonical_name: str, tags_priorities: dict[Tag, int]) -> Path | None:
         candidates: list[tuple[int, Path]] = []
-        for candidate in self._get_candidates(link, target_python):
+        for candidate in self._get_candidates(path):
             try:
                 name, *_, tags = parse_wheel_filename(candidate.name)
             except ValueError:
                 logger.debug("Ignoring invalid cached wheel %s", candidate.name)
                 continue
             if canonical_name != canonicalize_name(name):
                 logger.debug(
@@ -258,7 +276,12 @@
             with atomic_open_for_write(path, mode="wb") as f:
                 cast(BinaryIO, f).write(value)
 
     def delete(self, key: str) -> None:
         path = self._get_cache_path(key)
         with contextlib.suppress(OSError):
             os.remove(path)
+
+
+@lru_cache(maxsize=128)
+def get_wheel_cache(directory: Path) -> WheelCache:
+    return WheelCache(directory)
```

### Comparing `pdm-2.5.6/src/pdm/models/candidates.py` & `pdm-2.6.0/src/pdm/models/candidates.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from pdm.models.specifiers import PySpecSet
 from pdm.project.project_file import PyProject
 from pdm.utils import (
     cd,
     convert_hashes,
     create_tracked_tempdir,
     get_rev_from_url,
-    get_venv_like_prefix,
     normalize_name,
     path_to_url,
     url_without_fragments,
 )
 
 if TYPE_CHECKING:
     from unearth import Package, PackageFinder
@@ -365,16 +364,15 @@
             if cached:
                 self.wheel = cached
                 return self.wheel
         assert self._source_dir, "Source directory isn't ready yet"
         builder_cls = EditableBuilder if self.req.editable else WheelBuilder
         builder = builder_cls(str(self._unpacked_dir), self.environment)
         build_dir = self._get_wheel_dir()
-        if not os.path.exists(build_dir):
-            os.makedirs(build_dir)
+        os.makedirs(build_dir, exist_ok=True)
         termui.logger.info("Running PEP 517 backend to build a wheel for %s", self.link)
         self.wheel = Path(builder.build(build_dir, metadata_directory=self._metadata_dir))
         return self.wheel
 
     def obtain(self, allow_all: bool = False) -> None:
         """Fetch the link of the candidate and unpack to local if necessary.
 
@@ -544,18 +542,21 @@
         assert original_link
         if original_link.is_file and original_link.file_path.is_dir():
             # Local directories are built in tree
             return str(original_link.file_path)
         if self.req.editable:
             # In this branch the requirement must be an editable VCS requirement.
             # The repository will be unpacked into a *persistent* src directory.
+            prefix: Path | None = None
             if self.environment.is_local:
                 prefix = self.environment.packages_path  # type: ignore[attr-defined]
             else:
-                prefix = get_venv_like_prefix(self.environment.interpreter.executable)
+                venv = self.environment.interpreter.get_venv()
+                if venv is not None:
+                    prefix = venv.root
             if prefix is not None:
                 src_dir = prefix / "src"
             else:
                 src_dir = Path("src")
             src_dir.mkdir(exist_ok=True, parents=True)
             dirname = self.candidate.name or self.req.name
             if not dirname:
@@ -569,20 +570,22 @@
             return True
         supported_tags = self.environment.target_python.supported_tags()
         file_tags = parse_wheel_filename(wheel_file)[-1]
         return not file_tags.isdisjoint(supported_tags)
 
     def _get_wheel_dir(self) -> str:
         assert self.candidate.link
+        wheel_cache = self.environment.project.make_wheel_cache()
         if self.should_cache():
             termui.logger.info("Saving wheel to cache: %s", self.candidate.link)
-            wheel_cache = self.environment.project.make_wheel_cache()
             return wheel_cache.get_path_for_link(self.candidate.link, self.environment.target_python).as_posix()
         else:
-            return create_tracked_tempdir(prefix="pdm-wheel-")
+            return wheel_cache.get_ephemeral_path_for_link(
+                self.candidate.link, self.environment.target_python
+            ).as_posix()
 
 
 @lru_cache(maxsize=None)
 def make_candidate(
     req: Requirement,
     name: str | None = None,
     version: str | None = None,
```

### Comparing `pdm-2.5.6/src/pdm/models/in_process/__init__.py` & `pdm-2.6.0/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.6.0/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/in_process/parse_setup.py` & `pdm-2.6.0/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/in_process/pep508.py` & `pdm-2.6.0/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.6.0/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/markers.py` & `pdm-2.6.0/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/project_info.py` & `pdm-2.6.0/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/python.py` & `pdm-2.6.0/src/pdm/models/python.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Any
 
 from findpython import PythonVersion
 from packaging.version import InvalidVersion, Version
 
 from pdm.compat import cached_property
-from pdm.utils import get_venv_like_prefix
+from pdm.models.venv import VirtualEnv
 
 
 class PythonInfo:
     """
     A convenient helper class that holds all information of a Python interepreter.
     """
 
@@ -76,10 +76,9 @@
         try:
             if os.name == "nt" and self.is_32bit:
                 return f"{self.major}.{self.minor}-32"
             return f"{self.major}.{self.minor}"
         except InvalidVersion:
             return "unknown"
 
-    @property
-    def is_venv(self) -> bool:
-        return get_venv_like_prefix(self.executable) is not None
+    def get_venv(self) -> VirtualEnv | None:
+        return VirtualEnv.from_interpreter(self.executable)
```

### Comparing `pdm-2.5.6/src/pdm/models/repositories.py` & `pdm-2.6.0/src/pdm/models/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,36 @@
     def _get_dependencies_from_metadata(self, candidate: Candidate) -> CandidateInfo:
         prepared = candidate.prepare(self.environment)
         deps = prepared.get_dependencies_from_metadata()
         requires_python = candidate.requires_python
         summary = prepared.metadata.metadata["Summary"]
         return deps, requires_python, summary
 
+    def _get_dependency_from_local_package(self, candidate: Candidate) -> CandidateInfo:
+        """Adds the local package as a candidate only if the candidate
+        name is the same as the local package."""
+        project = self.environment.project
+        if not project.name or candidate.name != project.name:
+            raise CandidateInfoNotFound(candidate) from None
+
+        reqs = project.pyproject.metadata.get("dependencies", [])
+        extra_dependencies = project.pyproject.settings.get("dev-dependencies", {})
+        extra_dependencies.update(project.pyproject.metadata.get("optional-dependencies", {}))
+        if candidate.req.extras is not None:
+            reqs = sum(
+                (extra_dependencies.get(g, []) for g in candidate.req.extras),
+                [],
+            )
+
+        return (
+            reqs,
+            str(self.environment.python_requires),
+            project.pyproject.metadata.get("description", "UNKNOWN"),
+        )
+
     def get_hashes(self, candidate: Candidate) -> dict[Link, str] | None:
         """Get hashes of all possible installable candidates
         of a given package version.
         """
         if (
             candidate.req.is_vcs
             or candidate.req.is_file_or_url
@@ -307,14 +329,15 @@
                     candidate.req.extras or (),
                 )
                 return requirements, requires_python, summary
         raise CandidateInfoNotFound(candidate)
 
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         yield self._get_dependencies_from_cache
+        yield self._get_dependency_from_local_package
         if self.environment.project.config["pypi.json_api"]:
             yield self._get_dependencies_from_json
         yield self._get_dependencies_from_metadata
 
     def _find_candidates(self, requirement: Requirement) -> Iterable[Candidate]:
         sources = self.get_filtered_sources(requirement)
         with self.environment.get_finder(sources, self.ignore_compatibility) as finder:
@@ -413,34 +436,14 @@
             url,
             candidate.req.editable,
         )
 
     def _get_dependencies_from_lockfile(self, candidate: Candidate) -> CandidateInfo:
         return self.candidate_info[self._identify_candidate(candidate)]
 
-    def _get_dependency_from_local_package(self, candidate: Candidate) -> CandidateInfo:
-        """Adds the local package as a candidate only if the candidate
-        name is the same as the local package."""
-        if candidate.name != self.environment.project.name:
-            raise CandidateInfoNotFound(candidate) from None
-
-        reqs = self.environment.project.pyproject.metadata.get("dependencies", [])
-        optional_dependencies = self.environment.project.pyproject.metadata.get("optional-dependencies", {})
-        if candidate.req.extras is not None:
-            reqs = sum(
-                (optional_dependencies.get(g, []) for g in candidate.req.extras),
-                [],
-            )
-
-        return (
-            reqs,
-            str(self.environment.python_requires),
-            self.environment.project.pyproject.metadata.get("description", "UNKNOWN"),
-        )
-
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         return (
             self._get_dependency_from_local_package,
             self._get_dependencies_from_lockfile,
         )
 
     def _matching_keys(self, requirement: Requirement) -> Iterable[tuple]:
```

### Comparing `pdm-2.5.6/src/pdm/models/requirements.py` & `pdm-2.6.0/src/pdm/models/requirements.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         try:
             pkg_req = parse_as_pkg_requirement(line)
         except InvalidRequirement as e:
             m = _file_req_re.match(line)
             if m is None:
                 raise RequirementError(str(e)) from None
             args = m.groupdict()
-            if not args["url"] and args["path"] and not os.path.exists(args["path"]):
+            if not line.startswith(".") and not args["url"] and args["path"] and not os.path.exists(args["path"]):
                 raise RequirementError(str(e)) from None
             r = FileRequirement.create(**args)
         else:
             r = Requirement.from_pkg_requirement(pkg_req)
         if replaced:
             assert isinstance(r, FileRequirement)
             r.url = r.url.replace(root_url, "{root:uri}")
```

### Comparing `pdm-2.5.6/src/pdm/models/search.py` & `pdm-2.6.0/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/session.py` & `pdm-2.6.0/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/setup.py` & `pdm-2.6.0/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/specifiers.py` & `pdm-2.6.0/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/versions.py` & `pdm-2.6.0/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/models/working_set.py` & `pdm-2.6.0/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/pep582/sitecustomize.py` & `pdm-2.6.0/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/project/config.py` & `pdm-2.6.0/src/pdm/project/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,27 +275,21 @@
             if len(parts) < 2:
                 raise PdmUsageError("Must specify a repository name")
             repo = self.get_repository_config(parts[1])
             if repo is None:
                 raise KeyError(f"No repository named {parts[1]}")
 
             value = getattr(repo, parts[2]) if len(parts) >= 3 else repo
-            if len(parts) >= 3 and parts[2] == "password" and value:
-                return "<hidden>"
             return value
-        elif parts[0] == "pypi" and key not in self._config_map:
+        elif parts[0] == "pypi" and key not in self._config_map and len(parts) >= 2:
             index_key = ".".join(parts[:2])
             if index_key not in self._data:
                 raise KeyError(f"No PyPI index named {parts[1]}")
             source = self._data[index_key]
-            if len(parts) >= 3 and parts[2] == "password":
-                return "<hidden>"
             return source[parts[2]] if len(parts) >= 3 else RepositoryConfig(**self._data[index_key])
-        elif key == "pypi.password":
-            return "<hidden>"
 
         if key not in self._config_map and key not in self.deprecated:
             raise NoConfigError(key)
         config_key = self.deprecated.get(key, key)
         config = self._config_map[config_key]
         env_var = config.env_var
         if env_var is not None and env_var in os.environ:
```

### Comparing `pdm-2.5.6/src/pdm/project/core.py` & `pdm-2.6.0/src/pdm/project/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.compat import cached_property
 from pdm.environments import BaseEnvironment, PythonEnvironment, PythonLocalEnvironment
 from pdm.exceptions import NoPythonVersion, PdmUsageError, ProjectError
 from pdm.models.backends import BuildBackend, get_backend_by_spec
-from pdm.models.caches import CandidateInfoCache, HashCache, WheelCache
+from pdm.models.caches import CandidateInfoCache, HashCache, WheelCache, get_wheel_cache
 from pdm.models.candidates import Candidate, make_candidate
 from pdm.models.python import PythonInfo
 from pdm.models.repositories import BaseRepository, LockedRepository
 from pdm.models.requirements import Requirement, parse_requirement, strip_extras
-from pdm.models.specifiers import PySpecSet, get_specifier
+from pdm.models.specifiers import PySpecSet
 from pdm.project.config import Config
 from pdm.project.lockfile import Lockfile
 from pdm.project.project_file import PyProject
 from pdm.utils import (
     cd,
     deprecation_warning,
     expand_env_vars_in_auth,
@@ -181,15 +181,16 @@
             with contextlib.suppress(FileNotFoundError):
                 python_file.unlink()
             return
         python_file.write_text(value, "utf-8")
 
     def resolve_interpreter(self) -> PythonInfo:
         """Get the Python interpreter path."""
-        from pdm.cli.commands.venv.utils import get_venv_python, iter_venvs
+        from pdm.cli.commands.venv.utils import iter_venvs
+        from pdm.models.venv import get_venv_python
 
         def match_version(python: PythonInfo) -> bool:
             return python.valid and self.python_requires.contains(python.version, True)
 
         def note(message: str) -> None:
             if not self.is_global:
                 self.core.ui.echo(message, style="info", err=True)
@@ -216,24 +217,24 @@
                     note(
                         f"Inside an active virtualenv [success]{venv_in_env}[/], reusing it.\n"
                         "Set env var [success]PDM_IGNORE_ACTIVE_VENV[/] to ignore it."
                     )
                     return python
             # otherwise, get a venv associated with the project
             for _, venv in iter_venvs(self):
-                python = PythonInfo.from_path(get_venv_python(venv))
+                python = PythonInfo.from_path(venv.interpreter)
                 if match_version(python):
-                    note(f"Virtualenv [success]{venv}[/] is reused.")
+                    note(f"Virtualenv [success]{venv.root}[/] is reused.")
                     self.python = python
                     return python
 
             if not self.root.joinpath("__pypackages__").exists():
                 note("python.use_venv is on, creating a virtualenv for this project...")
-                venv = self._create_virtualenv()
-                self.python = PythonInfo.from_path(get_venv_python(venv))
+                venv_path = self._create_virtualenv()
+                self.python = PythonInfo.from_path(get_venv_python(venv_path))
                 return self.python
 
         for py_version in self.find_interpreters():
             if match_version(py_version):
                 if config.get("python.use_venv"):
                     note("[success]__pypackages__[/] is detected, using the PEP 582 mode")
                 self.python = py_version
@@ -249,15 +250,15 @@
             # Rewrite global project's python requires to be
             # compatible with the exact version
             env.python_requires = PySpecSet(f"=={self.python.version}")
             return env
 
         return (
             PythonEnvironment(self)
-            if self.config["python.use_venv"] and self.python.is_venv
+            if self.config["python.use_venv"] and self.python.get_venv() is not None
             else PythonLocalEnvironment(self)
         )
 
     def _create_virtualenv(self) -> Path:
         from pdm.cli.commands.venv.backends import BACKENDS
 
         backend: str = self.config["venv.backend"]
@@ -486,30 +487,40 @@
         from pdm.resolver.reporters import SpinnerReporter
 
         if spinner is None:
             spinner = termui.SilentSpinner("")
 
         return SpinnerReporter(spinner, requirements)
 
-    def get_lock_metadata(self, groups: Iterable[str] | None = None) -> dict[str, Any]:
+    def get_lock_metadata(
+        self, groups: Iterable[str] | None = None, cross_platform: bool | None = None
+    ) -> dict[str, Any]:
         content_hash = tomlkit.string("sha256:" + self.pyproject.content_hash("sha256"))
         content_hash.trivia.trail = "\n\n"
         if groups is None:
             groups = self.iter_groups()
+        if cross_platform is None:
+            cross_platform = self.lockfile.cross_platform
         return {
             "lock_version": self.lockfile.spec_version,
+            "cross_platform": cross_platform,
             "groups": sorted(groups, key=lambda x: (x != "default", x)),
             "content_hash": content_hash,
         }
 
     def write_lockfile(
-        self, toml_data: dict, show_message: bool = True, write: bool = True, groups: Iterable[str] | None = None
+        self,
+        toml_data: dict,
+        show_message: bool = True,
+        write: bool = True,
+        groups: Iterable[str] | None = None,
+        cross_platform: bool | None = None,
     ) -> None:
         """Write the lock file to disk."""
-        toml_data["metadata"].update(self.get_lock_metadata(groups))
+        toml_data["metadata"].update(self.get_lock_metadata(groups, cross_platform=cross_platform))
         self.lockfile.set_data(toml_data)
 
         if write:
             self.lockfile.write(show_message)
 
     def make_self_candidate(self, editable: bool = True) -> Candidate:
         req = parse_requirement(path_to_url(self.root.as_posix()), editable)
@@ -523,28 +534,14 @@
         hash_in_lockfile = str(self.lockfile.hash)
         if not hash_in_lockfile:
             return False
         algo, hash_value = hash_in_lockfile.split(":")
         content_hash = self.pyproject.content_hash(algo)
         return content_hash == hash_value
 
-    def is_lockfile_compatible(self) -> bool:
-        """Within the same major version, the higher lockfile generator can work with
-        lower lockfile but not vice versa.
-        """
-        if not self.lockfile.exists():
-            return True
-        lockfile_version = str(self.lockfile.file_version)
-        if not lockfile_version:
-            return False
-        if "." not in lockfile_version:
-            lockfile_version += ".0"
-        accepted = get_specifier(f"~={lockfile_version},>={lockfile_version}")
-        return accepted.contains(self.lockfile.spec_version)
-
     def get_pyproject_dependencies(self, group: str, dev: bool = False) -> tuple[list[str], bool]:
         """Get the dependencies array in the pyproject.toml
         Return a tuple of two elements, the first is the dependencies array,
         and the second tells whether it is a dev-dependencies group.
         """
         metadata, settings = self.pyproject.metadata, self.pyproject.settings
         if group == "default":
@@ -609,15 +606,15 @@
             path.mkdir(parents=True, exist_ok=True)
         except OSError:
             # The path could be not accessible
             pass
         return path
 
     def make_wheel_cache(self) -> WheelCache:
-        return WheelCache(self.cache("wheels"))
+        return get_wheel_cache(self.cache("wheels"))
 
     def make_candidate_info_cache(self) -> CandidateInfoCache:
         python_hash = hashlib.sha1(str(self.environment.python_requires).encode()).hexdigest()
         file_name = f"package_meta_{python_hash}.json"
         return CandidateInfoCache(self.cache("metadata") / file_name)
 
     def make_hash_cache(self) -> HashCache:
```

### Comparing `pdm-2.5.6/src/pdm/project/lockfile.py` & `pdm-2.6.0/src/pdm/project/lockfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Iterable, Mapping
 
 import tomlkit
 
+from pdm.models.specifiers import get_specifier
 from pdm.project.toml_file import TOMLBase
 
 GENERATED_COMMENTS = [
     "This file is @generated by PDM.",
     "It is not intended for manual editing.",
 ]
 
@@ -23,14 +24,20 @@
     def file_version(self) -> str:
         return self._data.get("metadata", {}).get("lock_version", "")
 
     @property
     def groups(self) -> list[str] | None:
         return self._data.get("metadata", {}).get("groups")
 
+    @property
+    def cross_platform(self) -> bool:
+        if self.empty():
+            return True
+        return self._data.get("metadata", {}).get("cross_platform", True)
+
     def compare_groups(self, groups: Iterable[str]) -> list[str]:
         if not self.groups:
             return []
         return list(set(groups).difference(self.groups))
 
     def set_data(self, data: Mapping[str, Any]) -> None:
         self._data = tomlkit.document()
@@ -41,7 +48,21 @@
     def write(self, show_message: bool = True) -> None:
         super().write()
         if show_message:
             self.ui.echo(f"Changes are written to [success]{self._path.name}[/].")
 
     def __getitem__(self, key: str) -> dict:
         return self._data[key]
+
+    def is_compatible(self) -> bool:
+        """Within the same major version, the higher lockfile generator can work with
+        lower lockfile but not vice versa.
+        """
+        if not self.exists():
+            return True
+        lockfile_version = str(self.file_version)
+        if not lockfile_version:
+            return False
+        if "." not in lockfile_version:
+            lockfile_version += ".0"
+        accepted = get_specifier(f"~={lockfile_version},>={lockfile_version}")
+        return accepted.contains(self.spec_version)
```

### Comparing `pdm-2.5.6/src/pdm/project/project_file.py` & `pdm-2.6.0/src/pdm/project/project_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 from tomlkit import TOMLDocument, items
 
 from pdm.project.toml_file import TOMLBase
 from pdm.utils import deprecation_warning
 
 
+def _remove_empty_tables(doc: dict) -> None:
+    for k, v in list(doc.items()):
+        if isinstance(v, dict):
+            _remove_empty_tables(v)
+            if not v:
+                del doc[k]
+
+
 class PyProject(TOMLBase):
     """The data object representing th pyproject.toml file"""
 
     def read(self) -> TOMLDocument:
         from pdm.formats import flit, poetry
 
         data = super().read()
@@ -26,14 +34,15 @@
                     if settings:
                         data.setdefault("tool", {}).setdefault("pdm", {}).update(settings)
                     break
         return data
 
     def write(self, show_message: bool = True) -> None:
         """Write the TOMLDocument to the file."""
+        _remove_empty_tables(self._data)
         super().write()
         if show_message:
             self.ui.echo("Changes are written to [success]pyproject.toml[/].")
 
     @property
     def is_valid(self) -> bool:
         return bool(self._data.get("project"))
@@ -77,7 +86,11 @@
             "requires-python": self.metadata.get("requires-python", ""),
             "overrides": self.resolution_overrides,
         }
         pyproject_content = json.dumps(dump_data, sort_keys=True)
         hasher = hashlib.new(algo)
         hasher.update(pyproject_content.encode("utf-8"))
         return hasher.hexdigest()
+
+    @property
+    def plugins(self) -> list[str]:
+        return self.settings.get("plugins", [])
```

### Comparing `pdm-2.5.6/src/pdm/project/toml_file.py` & `pdm-2.6.0/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/pytest.py` & `pdm-2.6.0/src/pdm/pytest.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from pytest_mock import MockerFixture
 from unearth import Link
 
 from pdm.cli.actions import do_init
 from pdm.cli.hooks import HookManager
 from pdm.compat import Protocol
 from pdm.core import Core
-from pdm.environments import BaseEnvironment, PrefixEnvironment
+from pdm.environments import BaseEnvironment, PythonEnvironment
 from pdm.exceptions import CandidateInfoNotFound
 from pdm.installers.installers import install_wheel
 from pdm.models.backends import get_backend
 from pdm.models.candidates import Candidate
 from pdm.models.repositories import BaseRepository
 from pdm.models.requirements import (
     Requirement,
@@ -183,14 +183,15 @@
         deps = pypi_data.get("dependencies", [])
         deps = filter_requirements_with_extras(cast(str, candidate.req.name), deps, candidate.req.extras or ())
         return deps, pypi_data.get("requires_python", ""), ""
 
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         return (
             self._get_dependencies_from_cache,
+            self._get_dependency_from_local_package,
             self._get_dependencies_from_fixture,
             self._get_dependencies_from_metadata,
         )
 
     def get_hashes(self, candidate: Candidate) -> dict[Link, str] | None:
         return {}
 
@@ -315,15 +316,15 @@
         build_env_wheels: a list of wheel to install in the environment
 
     Returns:
         The build environment temporary path
     """
     d = tmp_path_factory.mktemp("pdm-test-env")
     p = Core().create_project(d)
-    env = PrefixEnvironment(p, prefix=str(d))
+    env = PythonEnvironment(p, prefix=str(d))
     for wheel in build_env_wheels:
         install_wheel(str(wheel), env)
     return d
 
 
 @pytest.fixture
 def pypi_indexes() -> IndexesDefinition:
```

### Comparing `pdm-2.5.6/src/pdm/resolver/core.py` & `pdm-2.6.0/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/resolver/providers.py` & `pdm-2.6.0/src/pdm/resolver/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import itertools
 import os
 from typing import TYPE_CHECKING, Callable, cast
 
 from packaging.specifiers import InvalidSpecifier, SpecifierSet
 from resolvelib import AbstractProvider
 
 from pdm.models.candidates import Candidate, make_candidate
@@ -131,15 +132,20 @@
         def matches_gen() -> Iterator[Candidate]:
             incompat = list(incompatibilities[identifier])
             if identifier == "python":
                 candidates = find_python_matches(identifier, requirements)
                 return (c for c in candidates if c not in incompat)
             elif identifier in self.overrides:
                 return iter(self.get_override_candidates(identifier))
-            reqs = sorted(requirements[identifier], key=self.requirement_preference)
+            reqs_iter = requirements[identifier]
+            bare_name, extras = strip_extras(identifier)
+            if extras and bare_name in requirements:
+                # We should consider the requirements for both foo and foo[extra]
+                reqs_iter = itertools.chain(reqs_iter, requirements[bare_name])
+            reqs = sorted(reqs_iter, key=self.requirement_preference)
             candidates = self._find_candidates(reqs[0])
             return (
                 can for can in candidates if can not in incompat and all(self.is_satisfied_by(r, can) for r in reqs)
             )
 
         return matches_gen
```

### Comparing `pdm-2.5.6/src/pdm/resolver/python.py` & `pdm-2.6.0/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/resolver/reporters.py` & `pdm-2.6.0/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/signals.py` & `pdm-2.6.0/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/termui.py` & `pdm-2.6.0/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/src/pdm/utils.py` & `pdm-2.6.0/src/pdm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,31 +267,36 @@
     try:
         Path(path).relative_to(other)
     except ValueError:
         return False
     return True
 
 
-def get_venv_like_prefix(interpreter: str | Path) -> Path | None:
+def get_venv_like_prefix(interpreter: str | Path) -> tuple[Path | None, bool]:
     """Check if the given interpreter path is from a virtualenv,
-    and return the prefix if found.
+    and return two values: the root path and whether it's a conda env.
     """
     interpreter = Path(interpreter)
     prefix = interpreter.parent
     if prefix.joinpath("conda-meta").exists():
-        return prefix
+        return prefix, True
 
     prefix = prefix.parent
-    if prefix.joinpath("pyvenv.cfg").exists() or prefix.joinpath("conda-meta").exists():
-        return prefix
+    if prefix.joinpath("pyvenv.cfg").exists():
+        return prefix, False
+    if prefix.joinpath("conda-meta").exists():
+        return prefix, True
 
-    virtual_env = os.getenv("VIRTUAL_ENV", os.getenv("CONDA_PREFIX"))
+    virtual_env = os.getenv("VIRTUAL_ENV")
+    if virtual_env and is_path_relative_to(interpreter, virtual_env):
+        return Path(virtual_env), False
+    virtual_env = os.getenv("CONDA_PREFIX")
     if virtual_env and is_path_relative_to(interpreter, virtual_env):
-        return Path(virtual_env)
-    return None
+        return Path(virtual_env), True
+    return None, False
 
 
 def find_python_in_path(path: str | Path) -> Path | None:
     """Find a python interpreter from the given path, the input argument could be:
 
     - A valid path to the interpreter
     - A Python root directory that contains the interpreter
```

### Comparing `pdm-2.5.6/tests/cli/conftest.py` & `pdm-2.6.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_add.py` & `pdm-2.6.0/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_build.py` & `pdm-2.6.0/tests/cli/test_build.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 
 def get_wheel_names(path):
     with zipfile.ZipFile(path) as zf:
         return zf.namelist()
 
 
-def test_build_command(project, invoke, mocker):
+def test_build_command(project, pdm, mocker):
     do_build = mocker.patch.object(actions, "do_build")
-    invoke(["build"], obj=project)
+    pdm(["build"], obj=project)
     do_build.assert_called_once()
 
 
-def test_build_global_project_forbidden(invoke):
-    result = invoke(["build", "-g"])
+def test_build_global_project_forbidden(pdm):
+    result = pdm(["build", "-g"])
     assert result.exit_code != 0
 
 
 def test_build_single_module(fixture_project):
     project = fixture_project("demo-module")
 
     actions.do_build(project)
@@ -131,32 +131,32 @@
 def test_build_with_config_settings(fixture_project):
     project = fixture_project("demo-src-package")
     actions.do_build(project, config_settings={"--plat-name": "win_amd64"})
 
     assert (project.root / "dist/demo_package-0.1.0-py3-none-win_amd64.whl").exists()
 
 
-def test_cli_build_with_config_settings(fixture_project, invoke):
+def test_cli_build_with_config_settings(fixture_project, pdm):
     project = fixture_project("demo-src-package")
-    result = invoke(["build", "-C--plat-name=win_amd64"], obj=project)
+    result = pdm(["build", "-C--plat-name=win_amd64"], obj=project)
     assert result.exit_code == 0
     assert (project.root / "dist/demo_package-0.1.0-py3-none-win_amd64.whl").exists()
 
 
 @pytest.mark.network
 @pytest.mark.parametrize("isolated", (True, False))
-def test_build_with_no_isolation(fixture_project, invoke, isolated):
+def test_build_with_no_isolation(fixture_project, pdm, isolated):
     project = fixture_project("demo-failure")
     project.pyproject.set_data({"project": {"name": "demo", "version": "0.1.0"}})
     project.pyproject.write()
-    invoke(["add", "first"], obj=project)
+    pdm(["add", "first"], obj=project)
     args = ["build"]
     if not isolated:
         args.append("--no-isolation")
-    result = invoke(args, obj=project)
+    result = pdm(args, obj=project)
     assert result.exit_code == int(isolated)
 
 
 def test_build_ignoring_pip_environment(fixture_project, monkeypatch):
     project = fixture_project("demo-module")
     monkeypatch.setenv("PIP_REQUIRE_VIRTUALENV", "1")
     actions.do_build(project)
```

### Comparing `pdm-2.5.6/tests/cli/test_cache.py` & `pdm-2.6.0/tests/cli/test_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,30 +28,30 @@
         "baz-0.3.0.tar.gz",
         "foobar-0.4.0.tar.gz",
     ):
         (cache_dir / "arbitrary/path" / name).touch()
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache")
-def test_cache_list(project, invoke):
-    result = invoke(["cache", "list"], obj=project)
+def test_cache_list(project, pdm):
+    result = pdm(["cache", "list"], obj=project)
     assert result.exit_code == 0
 
     for name in (
         "foo-0.1.0.whl",
         "bar-0.2.0.whl",
         "baz-0.3.0.whl",
         "foo_bar-0.4.0.whl",
     ):
         assert name in result.output
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache")
-def test_cache_list_pattern(project, invoke):
-    result = invoke(["cache", "list", "ba*"], obj=project)
+def test_cache_list_pattern(project, pdm):
+    result = pdm(["cache", "list", "ba*"], obj=project)
     assert result.exit_code == 0
 
     for name in (
         "bar-0.2.0.whl",
         "baz-0.3.0.whl",
     ):
         assert name in result.output
@@ -60,16 +60,16 @@
         "foo-0.1.0.whl",
         "foo_bar-0.4.0.whl",
     ):
         assert name not in result.output
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache", "prepare_http_cache")
-def test_cache_remove_pattern(project, invoke):
-    result = invoke(["cache", "remove", "ba*"], obj=project)
+def test_cache_remove_pattern(project, pdm):
+    result = pdm(["cache", "remove", "ba*"], obj=project)
     assert result.exit_code == 0
 
     for name in (
         "bar-0.2.0.whl",
         "baz-0.3.0.whl",
     ):
         assert not (project.cache("wheels") / "arbitrary/path" / name).exists()
@@ -80,54 +80,54 @@
     ):
         assert (project.cache("wheels") / "arbitrary/path" / name).exists()
 
     assert (project.cache("http") / "arbitrary/path/foo-0.1.0.tar.gz").exists()
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache", "prepare_http_cache")
-def test_cache_remove_wildcard(project, invoke):
-    result = invoke(["cache", "remove", "*"], obj=project)
+def test_cache_remove_wildcard(project, pdm):
+    result = pdm(["cache", "remove", "*"], obj=project)
     assert result.exit_code == 0
 
     for name in (
         "bar-0.2.0.whl",
         "baz-0.3.0.whl",
         "foo-0.1.0.whl",
         "foo_bar-0.4.0.whl",
     ):
         assert not (project.cache("wheels") / "arbitrary/path" / name).exists()
 
     assert (project.cache("http") / "arbitrary/path/foo-0.1.0.tar.gz").exists()
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache", "prepare_http_cache")
-def test_cache_clear(project, invoke):
-    result = invoke(["cache", "clear"], obj=project)
+def test_cache_clear(project, pdm):
+    result = pdm(["cache", "clear"], obj=project)
     assert result.exit_code == 0
 
     for name in (
         "bar-0.2.0.whl",
         "baz-0.3.0.whl",
         "foo-0.1.0.whl",
         "foo_bar-0.4.0.whl",
     ):
         assert not (project.cache("wheels") / "arbitrary/path" / name).exists()
 
     assert not (project.cache("http") / "arbitrary/path/foo-0.1.0.tar.gz").exists()
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache", "prepare_http_cache")
-def test_cache_remove_no_pattern(project, invoke):
-    result = invoke(["cache", "remove"], obj=project)
+def test_cache_remove_no_pattern(project, pdm):
+    result = pdm(["cache", "remove"], obj=project)
     assert result.exit_code != 0
 
 
 @pytest.mark.usefixtures("prepare_wheel_cache", "prepare_http_cache")
-def test_cache_info(project, invoke):
-    result = invoke(["cache", "info"], obj=project)
+def test_cache_info(project, pdm):
+    result = pdm(["cache", "info"], obj=project)
     assert result.exit_code == 0
 
     lines = result.output.splitlines()
     assert "Files: 4" in lines[4]
     assert "Files: 4" in lines[6]
 
 
@@ -157,19 +157,19 @@
 )
 def test_hash_cache(project, url, hash):
     with project.environment.get_finder() as finder:
         hash_cache = project.make_hash_cache()
         assert hash_cache.get_hash(Link(url), finder.session) == hash
 
 
-def test_clear_package_cache(project, invoke):
+def test_clear_package_cache(project, pdm):
     pkg = CachedPackage(project.cache("packages") / "test_package")
     pkg.path.mkdir()
     refer_pkg = project.root / "refer_pkg"
     refer_pkg.mkdir()
     pkg.add_referrer(str(refer_pkg))
     assert len(pkg.referrers) == 1
     pkg._referrers = None
 
     refer_pkg.rmdir()
-    invoke(["cache", "clear", "packages"], obj=project, strict=True)
+    pdm(["cache", "clear", "packages"], obj=project, strict=True)
     assert not pkg.path.exists()
```

### Comparing `pdm-2.5.6/tests/cli/test_config.py` & `pdm-2.6.0/tests/cli/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 import pytest
 
 from pdm.exceptions import PdmUsageError
 from pdm.utils import cd
 
 
-def test_config_command(project, invoke):
-    result = invoke(["config"], obj=project)
+def test_config_command(project, pdm):
+    result = pdm(["config"], obj=project)
     assert result.exit_code == 0
     assert "python.use_pyenv = True" in result.output
 
-    result = invoke(["config", "-v"], obj=project)
+    result = pdm(["config", "-v"], obj=project)
     assert result.exit_code == 0
     assert "Use the pyenv interpreter" in result.output
 
 
-def test_config_get_command(project, invoke):
-    result = invoke(["config", "python.use_pyenv"], obj=project)
+def test_config_get_command(project, pdm):
+    result = pdm(["config", "python.use_pyenv"], obj=project)
     assert result.exit_code == 0
     assert result.output.strip() == "True"
 
-    result = invoke(["config", "foo.bar"], obj=project)
+    result = pdm(["config", "foo.bar"], obj=project)
     assert result.exit_code != 0
 
 
-def test_config_set_command(project, invoke):
-    result = invoke(["config", "python.use_pyenv", "false"], obj=project)
+def test_config_set_command(project, pdm):
+    result = pdm(["config", "python.use_pyenv", "false"], obj=project)
     assert result.exit_code == 0
-    result = invoke(["config", "python.use_pyenv"], obj=project)
+    result = pdm(["config", "python.use_pyenv"], obj=project)
     assert result.output.strip() == "False"
 
-    result = invoke(["config", "foo.bar"], obj=project)
+    result = pdm(["config", "foo.bar"], obj=project)
     assert result.exit_code != 0
 
-    result = invoke(["config", "-l", "cache_dir", "/path/to/bar"], obj=project)
+    result = pdm(["config", "-l", "cache_dir", "/path/to/bar"], obj=project)
     assert result.exit_code != 0
 
 
-def test_config_del_command(project, invoke):
-    result = invoke(["config", "-l", "python.use_pyenv", "false"], obj=project)
+def test_config_del_command(project, pdm):
+    result = pdm(["config", "-l", "python.use_pyenv", "false"], obj=project)
     assert result.exit_code == 0
 
-    result = invoke(["config", "python.use_pyenv"], obj=project)
+    result = pdm(["config", "python.use_pyenv"], obj=project)
     assert result.output.strip() == "False"
 
-    result = invoke(["config", "-ld", "python.use_pyenv"], obj=project)
+    result = pdm(["config", "-ld", "python.use_pyenv"], obj=project)
     assert result.exit_code == 0
 
-    result = invoke(["config", "python.use_pyenv"], obj=project)
+    result = pdm(["config", "python.use_pyenv"], obj=project)
     assert result.output.strip() == "True"
 
 
-def test_config_env_var_shadowing(project, invoke, monkeypatch):
+def test_config_env_var_shadowing(project, pdm, monkeypatch):
     monkeypatch.setenv("PDM_PYPI_URL", "https://example.org/simple")
-    result = invoke(["config", "pypi.url"], obj=project)
+    result = pdm(["config", "pypi.url"], obj=project)
     assert result.output.strip() == "https://example.org/simple"
 
-    result = invoke(["config", "pypi.url", "https://test.pypi.org/pypi"], obj=project)
+    result = pdm(["config", "pypi.url", "https://test.pypi.org/pypi"], obj=project)
     assert "config is shadowed by env var 'PDM_PYPI_URL'" in result.output
-    result = invoke(["config", "pypi.url"], obj=project)
+    result = pdm(["config", "pypi.url"], obj=project)
     assert result.output.strip() == "https://example.org/simple"
 
     monkeypatch.delenv("PDM_PYPI_URL")
-    result = invoke(["config", "pypi.url"], obj=project)
+    result = pdm(["config", "pypi.url"], obj=project)
     assert result.output.strip() == "https://test.pypi.org/pypi"
 
 
-def test_config_project_global_precedence(project, invoke):
-    invoke(["config", "python.use_pyenv", "true"], obj=project)
-    invoke(["config", "-l", "python.use_pyenv", "false"], obj=project)
+def test_config_project_global_precedence(project, pdm):
+    pdm(["config", "python.use_pyenv", "true"], obj=project)
+    pdm(["config", "-l", "python.use_pyenv", "false"], obj=project)
 
-    result = invoke(["config", "python.use_pyenv"], obj=project)
+    result = pdm(["config", "python.use_pyenv"], obj=project)
     assert result.output.strip() == "False"
 
 
-def test_specify_config_file(tmp_path, invoke, monkeypatch):
+def test_specify_config_file(tmp_path, pdm, monkeypatch):
     tmp_path.joinpath("global_config.toml").write_text("project_max_depth = 9\n")
     with cd(tmp_path):
-        result = invoke(["-c", "global_config.toml", "config", "project_max_depth"])
+        result = pdm(["-c", "global_config.toml", "config", "project_max_depth"])
         assert result.exit_code == 0
         assert result.output.strip() == "9"
 
         monkeypatch.setenv("PDM_CONFIG_FILE", "global_config.toml")
-        result = invoke(["config", "project_max_depth"])
+        result = pdm(["config", "project_max_depth"])
         assert result.exit_code == 0
         assert result.output.strip() == "9"
 
 
 def test_default_repository_setting(project):
     repository = project.global_config.get_repository_config("pypi")
     assert repository.url == "https://upload.pypi.org/legacy/"
@@ -124,53 +124,53 @@
     assert repository.password == "bar"
 
     project.global_config["repository.pypi.url"] = "https://example.pypi.org/legacy/"
     repository = project.global_config.get_repository_config("pypi")
     assert repository.url == "https://example.pypi.org/legacy/"
 
 
-def test_hide_password_in_output_repository(project, invoke):
+def test_hide_password_in_output_repository(project, pdm):
     assert project.global_config["repository.pypi.password"] is None
     project.global_config["repository.pypi.username"] = "testuser"
     project.global_config["repository.pypi.password"] = "secret"
-    result = invoke(["config", "repository.pypi"], obj=project, strict=True)
+    result = pdm(["config", "repository.pypi"], obj=project, strict=True)
     assert "password = <hidden>" in result.output
-    result = invoke(["config", "repository.pypi.password"], obj=project, strict=True)
+    result = pdm(["config", "repository.pypi.password"], obj=project, strict=True)
     assert "<hidden>" == result.output.strip()
 
 
-def test_hide_password_in_output_pypi(project, invoke):
+def test_hide_password_in_output_pypi(project, pdm):
     with pytest.raises(KeyError):
         assert project.global_config["pypi.extra.password"] is None
     project.global_config["pypi.extra.username"] = "testuser"
     project.global_config["pypi.extra.password"] = "secret"
     project.global_config["pypi.extra.url"] = "https://test/simple"
-    result = invoke(["config", "pypi.extra"], obj=project, strict=True)
+    result = pdm(["config", "pypi.extra"], obj=project, strict=True)
     assert "password = <hidden>" in result.output
-    result = invoke(["config", "pypi.extra.password"], obj=project, strict=True)
+    result = pdm(["config", "pypi.extra.password"], obj=project, strict=True)
     assert "<hidden>" == result.output.strip()
-    result = invoke(["config"], obj=project)
+    result = pdm(["config"], obj=project)
     assert "pypi.extra.password" in result.output
     assert "<hidden>" in result.output
 
 
-def test_config_get_repository(project, invoke):
+def test_config_get_repository(project, pdm):
     config = project.global_config["repository.pypi"]
     assert config == project.global_config.get_repository_config("pypi")
     assert project.global_config["repository.pypi.url"] == "https://upload.pypi.org/legacy/"
 
-    result = invoke(["config", "repository.pypi"], obj=project, strict=True)
+    result = pdm(["config", "repository.pypi"], obj=project, strict=True)
     assert result.stdout.strip() == "url = https://upload.pypi.org/legacy/"
 
     assert (
         project.global_config.get_repository_config("https://example.pypi.org/legacy/").url
         == "https://example.pypi.org/legacy/"
     )
 
-    result = invoke(["config", "repository.pypi.url"], obj=project, strict=True)
+    result = pdm(["config", "repository.pypi.url"], obj=project, strict=True)
     assert result.stdout.strip() == "https://upload.pypi.org/legacy/"
 
 
 def test_config_set_repository(project):
     project.global_config["repository.pypi.url"] = "https://example.pypi.org/legacy/"
     project.global_config["repository.pypi.username"] = "foo"
     assert project.global_config["repository.pypi.url"] == "https://example.pypi.org/legacy/"
```

### Comparing `pdm-2.5.6/tests/cli/test_fix.py` & `pdm-2.6.0/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_hooks.py` & `pdm-2.6.0/tests/cli/test_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 from pdm.cli.options import from_splitted_env
 from pdm.models.requirements import parse_requirement
 from pdm.signals import pdm_signals
 
 pytestmark = pytest.mark.usefixtures("repository", "working_set", "local_finder")
 
 
-def test_pre_script_fail_fast(project, invoke, capfd, mocker):
+def test_pre_script_fail_fast(project, pdm, capfd, mocker):
     project.pyproject.settings["scripts"] = {
         "pre_install": "python -c \"print('PRE INSTALL CALLED'); exit(1)\"",
         "post_install": "python -c \"print('POST INSTALL CALLED')\"",
     }
     project.pyproject.write()
     synchronize = mocker.patch("pdm.installers.synchronizers.Synchronizer.synchronize")
-    result = invoke(["install"], obj=project)
+    result = pdm(["install"], obj=project)
     assert result.exit_code == 1
     out, _ = capfd.readouterr()
     assert "PRE INSTALL CALLED" in out
     assert "POST INSTALL CALLED" not in out
     synchronize.assert_not_called()
 
 
-def test_pre_and_post_scripts(project, invoke, capfd, _echo):
+def test_pre_and_post_scripts(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "pre_script": "python echo.py pre_script",
         "post_script": "python echo.py post_script",
         "pre_test": "python echo.py pre_test",
         "test": "python echo.py test",
         "post_test": "python echo.py post_test",
         "pre_run": "python echo.py pre_run",
         "post_run": "python echo.py post_run",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     expected = dedent(
         """
         pre_run CALLED
         pre_script CALLED
         pre_test CALLED
         test CALLED
@@ -52,15 +52,15 @@
         post_script CALLED
         post_run CALLED
         """
     ).strip()
     assert out.strip() == expected
 
 
-def test_composite_runs_all_hooks(project, invoke, capfd, _echo):
+def test_composite_runs_all_hooks(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second"]},
         "pre_test": "python echo.py Pre-Test",
         "post_test": "python echo.py Post-Test",
         "first": "python echo.py First",
         "pre_first": "python echo.py Pre-First",
         "second": "python echo.py Second",
@@ -68,15 +68,15 @@
         "pre_script": "python echo.py Pre-Script",
         "post_script": "python echo.py Post-Script",
         "pre_run": "python echo.py Pre-Run",
         "post_run": "python echo.py Post-Run",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     expected = dedent(
         """
         Pre-Run CALLED
         Pre-Script CALLED
         Pre-Test CALLED
         Pre-Script CALLED
@@ -92,15 +92,15 @@
         Post-Run CALLED
         """
     ).strip()
     assert out.strip() == expected
 
 
 @pytest.mark.parametrize("option", [":all", ":pre,:post"])
-def test_skip_all_hooks_option(project, invoke, capfd, option: str, _echo):
+def test_skip_all_hooks_option(project, pdm, capfd, option: str, _echo):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second"]},
         "pre_test": "python echo.py Pre-Test",
         "post_test": "python echo.py Post-Test",
         "first": "python echo.py First",
         "pre_first": "python echo.py Pre-First",
         "post_first": "python echo.py Post-First",
@@ -110,23 +110,23 @@
         "pre_script": "python echo.py Pre-Script",
         "post_script": "python echo.py Post-Script",
         "pre_run": "python echo.py Pre-Run",
         "post_run": "python echo.py Post-Run",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", f"--skip={option}", "first"], strict=True, obj=project)
+    pdm(["run", f"--skip={option}", "first"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-First CALLED" not in out
     assert "First CALLED" in out
     assert "Post-First CALLED" not in out
     assert "Pre-Script CALLED" not in out
     assert "Post-Script CALLED" not in out
     capfd.readouterr()
-    invoke(["run", f"--skip={option}", "test"], strict=True, obj=project)
+    pdm(["run", f"--skip={option}", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Test CALLED" not in out
     assert "Pre-First CALLED" not in out
     assert "First CALLED" in out
     assert "Post-First CALLED" not in out
     assert "Pre-Second CALLED" not in out
     assert "Second CALLED" in out
@@ -145,29 +145,29 @@
         "-k pre_test,post_first,second",
         "--skip pre_test --skip post_first --skip second",
         "-k pre_test -k post_first -k second",
         "--skip pre_test --skip post_first,second",
         "-k pre_test -k post_first,second",
     ],
 )
-def test_skip_option(project, invoke, capfd, args, _echo):
+def test_skip_option(project, pdm, capfd, args, _echo):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second"]},
         "pre_test": "python echo.py Pre-Test",
         "post_test": "python echo.py Post-Test",
         "first": "python echo.py First",
         "pre_first": "python echo.py Pre-First",
         "post_first": "python echo.py Post-First",
         "second": "python echo.py Second",
         "pre_second": "python echo.py Pre-Second",
         "post_second": "python echo.py Post-Second",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", *shlex.split(args), "test"], strict=True, obj=project)
+    pdm(["run", *shlex.split(args), "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Test CALLED" not in out
     assert "Pre-First CALLED" in out
     assert "First CALLED" in out
     assert "Post-First CALLED" not in out
     assert "Pre-Second CALLED" not in out
     assert "Second CALLED" not in out
@@ -250,48 +250,48 @@
 def lock(project, capfd):
     project.add_dependencies({"requests": parse_requirement("requests")})
     actions.do_lock(project)
     capfd.readouterr()
 
 
 @parametrize_with_commands
-def test_hooks(hooked_project, invoke, capfd, specs: HookSpecs):
-    invoke(shlex.split(specs.command), strict=True, obj=hooked_project)
+def test_hooks(hooked_project, pdm, capfd, specs: HookSpecs):
+    pdm(shlex.split(specs.command), strict=True, obj=hooked_project)
     out, _ = capfd.readouterr()
     for hook in specs.hooks:
         assert f"{hook} CALLED" in out
 
 
 @parametrize_with_hooks  # Iterate over hooks as we need a clean slate for each run
-def test_skip_option_from_signal(hooked_project, invoke, capfd, specs: HookSpecs, hook: str):
-    invoke([*shlex.split(specs.command), f"--skip={hook}"], strict=True, obj=hooked_project)
+def test_skip_option_from_signal(hooked_project, pdm, capfd, specs: HookSpecs, hook: str):
+    pdm([*shlex.split(specs.command), f"--skip={hook}"], strict=True, obj=hooked_project)
     out, _ = capfd.readouterr()
     assert f"{hook} CALLED" not in out
     for known_hook in specs.hooks:
         if known_hook != hook:
             assert f"{known_hook} CALLED" in out
 
 
 @parametrize_with_commands
 @pytest.mark.parametrize("option", [":all", ":pre,:post"])
-def test_skip_all_option_from_signal(hooked_project, invoke, capfd, specs: HookSpecs, option: str):
-    invoke(
+def test_skip_all_option_from_signal(hooked_project, pdm, capfd, specs: HookSpecs, option: str):
+    pdm(
         [*shlex.split(specs.command), f"--skip={option}"],
         strict=True,
         obj=hooked_project,
     )
     out, _ = capfd.readouterr()
     for hook in pdm_signals:
         assert f"{hook} CALLED" not in out
 
 
 @parametrize_with_commands
 @pytest.mark.parametrize("prefix", ["pre", "post"])
-def test_skip_pre_post_option_from_signal(hooked_project, invoke, capfd, specs: HookSpecs, prefix: str):
-    invoke(
+def test_skip_pre_post_option_from_signal(hooked_project, pdm, capfd, specs: HookSpecs, prefix: str):
+    pdm(
         [*shlex.split(specs.command), f"--skip=:{prefix}"],
         strict=True,
         obj=hooked_project,
     )
     out, _ = capfd.readouterr()
     for hook in specs.hooks:
         if hook.startswith(prefix):
```

### Comparing `pdm-2.5.6/tests/cli/test_init.py` & `pdm-2.6.0/tests/cli/test_init.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 
 def test_init_validate_python_requires(project_no_init):
     with pytest.raises(ValueError):
         actions.do_init(project_no_init, python_requires="3.7")
 
 
-def test_init_command(project_no_init, invoke, mocker):
+def test_init_command(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
     do_init = mocker.patch.object(actions, "do_init")
-    invoke(["init"], input="\n\n\n\n\n\n", strict=True, obj=project_no_init)
+    pdm(["init"], input="\n\n\n\n\n\n", strict=True, obj=project_no_init)
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_init.assert_called_with(
         project_no_init,
         name="",
         version="",
         description="",
         license="MIT",
@@ -33,21 +33,21 @@
         email="me@example.org",
         python_requires=f">={python_version}",
         build_backend=None,
         hooks=ANY,
     )
 
 
-def test_init_command_library(project_no_init, invoke, mocker):
+def test_init_command_library(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
     do_init = mocker.patch.object(actions, "do_init")
-    result = invoke(
+    result = pdm(
         ["init"],
         input="\ny\ntest-project\n\nTest Project\n1\n\n\n\n\n",
         obj=project_no_init,
     )
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_init.assert_called_with(
@@ -60,22 +60,22 @@
         email="me@example.org",
         python_requires=f">={python_version}",
         build_backend=get_backend("setuptools"),
         hooks=ANY,
     )
 
 
-def test_init_non_interactive(project_no_init, invoke, mocker):
+def test_init_non_interactive(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
     do_init = mocker.patch.object(actions, "do_init")
     do_use = mocker.patch.object(actions, "do_use", return_value=PythonInfo.from_path(sys.executable))
-    result = invoke(["init", "-n"], obj=project_no_init)
+    result = pdm(["init", "-n"], obj=project_no_init)
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_use.assert_called_once_with(
         project_no_init,
         ANY,
         first=True,
         ignore_remembered=True,
@@ -93,36 +93,36 @@
         email="me@example.org",
         python_requires=f">={python_version}",
         build_backend=None,
         hooks=ANY,
     )
 
 
-def test_init_auto_create_venv(project_no_init, invoke, mocker):
-    mocker.patch("pdm.cli.commands.init.get_venv_like_prefix", return_value=None)
+def test_init_auto_create_venv(project_no_init, pdm, mocker):
+    mocker.patch("pdm.models.python.PythonInfo.get_venv", return_value=None)
     project_no_init.project_config["python.use_venv"] = True
-    result = invoke(["init"], input="\n\n\n\n\n\n\n", obj=project_no_init)
+    result = pdm(["init"], input="\n\n\n\n\n\n\n", obj=project_no_init)
     assert result.exit_code == 0
     assert project_no_init.python.executable.parent.parent == project_no_init.root / ".venv"
     assert ".pdm-python" in (project_no_init.root / ".gitignore").read_text()
 
 
-def test_init_auto_create_venv_specify_python(project_no_init, invoke, mocker):
-    mocker.patch("pdm.cli.commands.init.get_venv_like_prefix", return_value=None)
+def test_init_auto_create_venv_specify_python(project_no_init, pdm, mocker):
+    mocker.patch("pdm.models.python.PythonInfo.get_venv", return_value=None)
     project_no_init.project_config["python.use_venv"] = True
-    result = invoke(
+    result = pdm(
         ["init", f"--python={PYTHON_VERSION}"],
         input="\n\n\n\n\n\n",
         obj=project_no_init,
     )
     assert result.exit_code == 0
     assert project_no_init.python.executable.parent.parent == project_no_init.root / ".venv"
 
 
-def test_init_auto_create_venv_answer_no(project_no_init, invoke, mocker):
-    mocker.patch("pdm.cli.commands.init.get_venv_like_prefix", return_value=None)
+def test_init_auto_create_venv_answer_no(project_no_init, pdm, mocker):
+    mocker.patch("pdm.models.python.PythonInfo.get_venv", return_value=None)
     creator = mocker.patch("pdm.cli.commands.venv.backends.Backend.create")
     project_no_init.project_config["python.use_venv"] = True
-    result = invoke(["init"], input="\nn\n\n\n\n\n\n\n", obj=project_no_init)
+    result = pdm(["init"], input="\nn\n\n\n\n\n\n\n", obj=project_no_init)
     assert result.exit_code == 0
     creator.assert_not_called()
     assert project_no_init.python.executable.parent.parent != project_no_init.root / ".venv"
```

### Comparing `pdm-2.5.6/tests/cli/test_install.py` & `pdm-2.6.0/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_list.py` & `pdm-2.6.0/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_others.py` & `pdm-2.6.0/tests/cli/test_others.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from pathlib import Path
 
 import pytest
 
 from pdm.cli import actions
 from pdm.models.requirements import parse_requirement
 from pdm.utils import cd
@@ -46,14 +47,27 @@
     result = pdm(["info", "--where"], obj=project)
     assert result.output.strip() == str(project.root)
 
     result = pdm(["info", "--env"], obj=project)
     assert result.exit_code == 0
 
 
+def test_info_command_json(project, pdm):
+    result = pdm(["info", "--json"], obj=project, strict=True)
+
+    data = json.loads(result.outputs)
+
+    assert data["pdm"]["version"] == project.core.version
+    assert data["python"]["version"] == project.environment.interpreter.identifier
+    assert data["python"]["interpreter"] == str(project.environment.interpreter.executable)
+    assert isinstance(data["python"]["markers"], dict)
+    assert data["project"]["root"] == str(project.root)
+    assert isinstance(data["project"]["pypackages"], str)
+
+
 def test_info_global_project(pdm, tmp_path):
     with cd(tmp_path):
         result = pdm(["info", "-g", "--where"])
     assert "global-project" in result.output.strip()
 
 
 def test_info_with_multiple_venvs(pdm, project):
```

### Comparing `pdm-2.5.6/tests/cli/test_publish.py` & `pdm-2.6.0/tests/cli/test_publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,51 +73,51 @@
     assert repository.get_release_urls(package_files) == {"https://pypi.org/project/demo/0.0.1/"}
 
     repository = Repository(project, "https://example.pypi.org/legacy/", "abc", "123", None)
     assert not repository.get_release_urls(package_files)
 
 
 @pytest.mark.usefixtures("prepare_packages")
-def test_publish_pick_up_asc_files(project, uploaded, invoke):
+def test_publish_pick_up_asc_files(project, uploaded, pdm):
     for p in list(project.root.joinpath("dist").iterdir()):
         with open(str(p) + ".asc", "w") as f:
             f.write("fake signature")
 
-    invoke(
+    pdm(
         ["publish", "--no-build", "--username=abc", "--password=123"],
         obj=project,
         strict=True,
     )
     # Test wheels are uploaded first
     assert uploaded[0].base_filename.endswith(".whl")
     for package in uploaded:
         assert package.gpg_signature == (
             package.base_filename + ".asc",
             b"fake signature",
         )
 
 
 @pytest.mark.usefixtures("prepare_packages")
-def test_publish_package_with_signature(project, uploaded, invoke):
-    invoke(
+def test_publish_package_with_signature(project, uploaded, pdm):
+    pdm(
         ["publish", "--no-build", "-S", "--username=abc", "--password=123"],
         obj=project,
         strict=True,
     )
     for package in uploaded:
         assert package.gpg_signature == (
             package.base_filename + ".asc",
             b"fake signature",
         )
 
 
 @pytest.mark.usefixtures("local_finder")
-def test_publish_and_build_in_one_run(fixture_project, invoke, mock_pypi):
+def test_publish_and_build_in_one_run(fixture_project, pdm, mock_pypi):
     project = fixture_project("demo-module")
-    result = invoke(["publish", "--username=abc", "--password=123"], obj=project, strict=True).output
+    result = pdm(["publish", "--username=abc", "--password=123"], obj=project, strict=True).output
 
     mock_pypi.assert_called()
     assert "Uploading demo_module-0.1.0-py3-none-any.whl" in result
     assert "Uploading demo-module-0.1.0.tar.gz" in result
     assert "https://pypi.org/project/demo-module/0.1.0/" in result
```

### Comparing `pdm-2.5.6/tests/cli/test_remove.py` & `pdm-2.6.0/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_run.py` & `pdm-2.6.0/tests/cli/test_run.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,169 +24,169 @@
             args = ", ".join(sys.argv[2:])
             print(f"{name} CALLED with {args}" if args else f"{name} CALLED")
             """
         )
     )
 
 
-def test_pep582_launcher_for_python_interpreter(project, local_finder, invoke):
+def test_pep582_launcher_for_python_interpreter(project, local_finder, pdm):
     project.root.joinpath("main.py").write_text("import first;print(first.first([0, False, 1, 2]))\n")
-    result = invoke(["add", "first"], obj=project)
+    result = pdm(["add", "first"], obj=project)
     assert result.exit_code == 0, result.stderr
     env = os.environ.copy()
     env.update({"PYTHONPATH": get_pep582_path(project)})
     output = subprocess.check_output(
         [str(project.python.executable), str(project.root.joinpath("main.py"))],
         env=env,
     )
     assert output.decode().strip() == "1"
 
 
-def test_auto_isolate_site_packages(project, invoke):
+def test_auto_isolate_site_packages(project, pdm):
     env = os.environ.copy()
     env.update({"PYTHONPATH": get_pep582_path(project)})
     proc = subprocess.run(
         [str(project.python.executable), "-c", "import sys;print(sys.path, sep='\\n')"],
         env=env,
         capture_output=True,
         text=True,
         cwd=str(project.root),
         check=True,
     )
     assert any("site-packages" in path for path in proc.stdout.splitlines())
 
-    result = invoke(
+    result = pdm(
         ["run", "python", "-c", "import sys;print(sys.path, sep='\\n')"],
         obj=project,
         strict=True,
     )
     assert not any("site-packages" in path for path in result.stdout.splitlines())
 
 
-def test_run_with_site_packages(project, invoke):
+def test_run_with_site_packages(project, pdm):
     project.pyproject.settings["scripts"] = {
         "foo": {
             "cmd": ["python", "-c", "import sys;print(sys.path, sep='\\n')"],
             "site_packages": True,
         }
     }
     project.pyproject.write()
-    result = invoke(
+    result = pdm(
         [
             "run",
             "--site-packages",
             "python",
             "-c",
             "import sys;print(sys.path, sep='\\n')",
         ],
         obj=project,
     )
     assert result.exit_code == 0
-    result = invoke(["run", "foo"], obj=project)
+    result = pdm(["run", "foo"], obj=project)
     assert result.exit_code == 0
 
 
-def test_run_command_not_found(invoke):
-    result = invoke(["run", "foobar"])
+def test_run_command_not_found(pdm):
+    result = pdm(["run", "foobar"])
     assert "Command 'foobar' is not found in your PATH." in result.stderr
     assert result.exit_code == 1
 
 
-def test_run_pass_exit_code(invoke):
-    result = invoke(["run", "python", "-c", "1/0"])
+def test_run_pass_exit_code(pdm):
+    result = pdm(["run", "python", "-c", "1/0"])
     assert result.exit_code == 1
 
 
-def test_run_cmd_script(project, invoke):
+def test_run_cmd_script(project, pdm):
     project.pyproject.settings["scripts"] = {"test_script": "python -V"}
     project.pyproject.write()
-    result = invoke(["run", "test_script"], obj=project)
+    result = pdm(["run", "test_script"], obj=project)
     assert result.exit_code == 0
 
 
-def test_run_cmd_script_with_array(project, invoke):
+def test_run_cmd_script_with_array(project, pdm):
     project.pyproject.settings["scripts"] = {"test_script": ["python", "-c", "import sys; sys.exit(22)"]}
     project.pyproject.write()
-    result = invoke(["run", "test_script"], obj=project)
+    result = pdm(["run", "test_script"], obj=project)
     assert result.exit_code == 22
 
 
-def test_run_script_pass_project_root(project, invoke, capfd):
+def test_run_script_pass_project_root(project, pdm, capfd):
     project.pyproject.settings["scripts"] = {
         "test_script": [
             "python",
             "-c",
             "import os;print(os.getenv('PDM_PROJECT_ROOT'))",
         ]
     }
     project.pyproject.write()
     capfd.readouterr()
-    result = invoke(["run", "test_script"], obj=project)
+    result = pdm(["run", "test_script"], obj=project)
     assert result.exit_code == 0
     out, _ = capfd.readouterr()
     assert Path(out.strip()) == project.root
 
 
-def test_run_shell_script(project, invoke):
+def test_run_shell_script(project, pdm):
     project.pyproject.settings["scripts"] = {
         "test_script": {
             "shell": "echo hello > output.txt",
             "help": "test it won't fail",
         }
     }
     project.pyproject.write()
     with cd(project.root):
-        result = invoke(["run", "test_script"], obj=project)
+        result = pdm(["run", "test_script"], obj=project)
     assert result.exit_code == 0
     assert (project.root / "output.txt").read_text().strip() == "hello"
 
 
 @pytest.mark.parametrize(
     "args,expected",
     (
         pytest.param(["hello"], "ok hello", id="with-args"),
         pytest.param([], "ok", id="without-args"),
     ),
 )
-def test_run_shell_script_with_args_placeholder(project, invoke, args, expected):
+def test_run_shell_script_with_args_placeholder(project, pdm, args, expected):
     project.pyproject.settings["scripts"] = {
         "test_script": {
             "shell": "echo ok {args} > output.txt",
             "help": "test it won't fail",
         }
     }
     project.pyproject.write()
     with cd(project.root):
-        result = invoke(["run", "test_script", *args], obj=project)
+        result = pdm(["run", "test_script", *args], obj=project)
     assert result.exit_code == 0
     assert (project.root / "output.txt").read_text().strip() == expected
 
 
 @pytest.mark.parametrize(
     "args,expected",
     (
         pytest.param(["hello"], "hello", id="with-args"),
         pytest.param([], "default", id="with-default"),
     ),
 )
-def test_run_shell_script_with_args_placeholder_with_default(project, invoke, args, expected):
+def test_run_shell_script_with_args_placeholder_with_default(project, pdm, args, expected):
     project.pyproject.settings["scripts"] = {
         "test_script": {
             "shell": "echo {args:default} > output.txt",
             "help": "test it won't fail",
         }
     }
     project.pyproject.write()
     with cd(project.root):
-        result = invoke(["run", "test_script", *args], obj=project)
+        result = pdm(["run", "test_script", *args], obj=project)
     assert result.exit_code == 0
     assert (project.root / "output.txt").read_text().strip() == expected
 
 
-def test_run_call_script(project, invoke):
+def test_run_call_script(project, pdm):
     (project.root / "test_script.py").write_text(
         textwrap.dedent(
             """
             import argparse
             import sys
 
             def main(argv=None):
@@ -199,34 +199,34 @@
     )
     project.pyproject.settings["scripts"] = {
         "test_script": {"call": "test_script:main"},
         "test_script_with_args": {"call": "test_script:main(['-c', '9'])"},
     }
     project.pyproject.write()
     with cd(project.root):
-        result = invoke(["run", "test_script", "-c", "8"], obj=project)
+        result = pdm(["run", "test_script", "-c", "8"], obj=project)
         assert result.exit_code == 8
 
-        result = invoke(["run", "test_script_with_args"], obj=project)
+        result = pdm(["run", "test_script_with_args"], obj=project)
         assert result.exit_code == 9
 
 
-def test_run_script_with_extra_args(project, invoke, capfd):
+def test_run_script_with_extra_args(project, pdm, capfd):
     (project.root / "test_script.py").write_text(
         textwrap.dedent(
             """
             import sys
             print(*sys.argv[1:], sep='\\n')
             """
         )
     )
     project.pyproject.settings["scripts"] = {"test_script": "python test_script.py"}
     project.pyproject.write()
     with cd(project.root):
-        invoke(["run", "test_script", "-a", "-b", "-c"], obj=project)
+        pdm(["run", "test_script", "-a", "-b", "-c"], obj=project)
     out, _ = capfd.readouterr()
     assert out.splitlines()[-3:] == ["-a", "-b", "-c"]
 
 
 @pytest.mark.parametrize(
     "args,expected",
     (
@@ -237,27 +237,27 @@
 @pytest.mark.parametrize(
     "script",
     (
         pytest.param("python test_script.py {args} -x", id="as-str"),
         pytest.param(["python", "test_script.py", "{args}", "-x"], id="as-list"),
     ),
 )
-def test_run_script_with_args_placeholder(project, invoke, capfd, script, args, expected):
+def test_run_script_with_args_placeholder(project, pdm, capfd, script, args, expected):
     (project.root / "test_script.py").write_text(
         textwrap.dedent(
             """
             import sys
             print(*sys.argv[1:], sep='\\n')
             """
         )
     )
     project.pyproject.settings["scripts"] = {"test_script": script}
     project.pyproject.write()
     with cd(project.root):
-        invoke(["run", "-v", "test_script", *args], obj=project)
+        pdm(["run", "-v", "test_script", *args], obj=project)
     out, _ = capfd.readouterr()
     assert out.strip().splitlines()[1:] == expected
 
 
 @pytest.mark.parametrize(
     "args,expected",
     (
@@ -268,148 +268,227 @@
 @pytest.mark.parametrize(
     "script",
     (
         pytest.param("python test_script.py {args:--default --value} -x", id="as-str"),
         pytest.param(["python", "test_script.py", "{args:--default --value}", "-x"], id="as-list"),
     ),
 )
-def test_run_script_with_args_placeholder_with_default(project, invoke, capfd, script, args, expected):
+def test_run_script_with_args_placeholder_with_default(project, pdm, capfd, script, args, expected):
     (project.root / "test_script.py").write_text(
         textwrap.dedent(
             """
             import sys
             print(*sys.argv[1:], sep='\\n')
             """
         )
     )
     project.pyproject.settings["scripts"] = {"test_script": script}
     project.pyproject.write()
     with cd(project.root):
-        invoke(["run", "-v", "test_script", *args], obj=project)
+        pdm(["run", "-v", "test_script", *args], obj=project)
     out, _ = capfd.readouterr()
     assert out.strip().splitlines()[1:] == expected
 
 
-def test_run_expand_env_vars(project, invoke, capfd, monkeypatch):
+def test_run_expand_env_vars(project, pdm, capfd, monkeypatch):
     (project.root / "test_script.py").write_text("import os; print(os.getenv('FOO'))")
     project.pyproject.settings["scripts"] = {
         "test_cmd": 'python -c "foo, bar = 0, 1;print($FOO)"',
         "test_cmd_no_expand": "python -c 'print($FOO)'",
         "test_script": "python test_script.py",
         "test_cmd_array": ["python", "test_script.py"],
         "test_shell": {"shell": "echo $FOO"},
     }
     project.pyproject.write()
     capfd.readouterr()
     with cd(project.root):
         monkeypatch.setenv("FOO", "bar")
-        invoke(["run", "test_cmd"], obj=project)
+        pdm(["run", "test_cmd"], obj=project)
         assert capfd.readouterr()[0].strip() == "1"
 
-        result = invoke(["run", "test_cmd_no_expand"], obj=project)
+        result = pdm(["run", "test_cmd_no_expand"], obj=project)
         assert result.exit_code == 1
 
-        invoke(["run", "test_script"], obj=project)
+        pdm(["run", "test_script"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar"
 
-        invoke(["run", "test_cmd_array"], obj=project)
+        pdm(["run", "test_cmd_array"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar"
 
-        invoke(["run", "test_shell"], obj=project)
+        pdm(["run", "test_shell"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar"
 
 
-def test_run_script_with_env_defined(project, invoke, capfd):
+def test_run_script_with_env_defined(project, pdm, capfd):
     (project.root / "test_script.py").write_text("import os; print(os.getenv('FOO'))")
     project.pyproject.settings["scripts"] = {"test_script": {"cmd": "python test_script.py", "env": {"FOO": "bar"}}}
     project.pyproject.write()
     capfd.readouterr()
     with cd(project.root):
-        invoke(["run", "test_script"], obj=project)
+        pdm(["run", "test_script"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar"
 
 
-def test_run_script_with_dotenv_file(project, invoke, capfd, monkeypatch):
+def test_run_script_with_dotenv_file(project, pdm, capfd, monkeypatch):
     (project.root / "test_script.py").write_text("import os; print(os.getenv('FOO'), os.getenv('BAR'))")
     project.pyproject.settings["scripts"] = {
         "test_override": {
             "cmd": "python test_script.py",
             "env_file": {"override": ".env"},
         },
         "test_default": {"cmd": "python test_script.py", "env_file": ".env"},
     }
     project.pyproject.write()
     monkeypatch.setenv("BAR", "foo")
     (project.root / ".env").write_text("FOO=bar\nBAR=override")
     capfd.readouterr()
     with cd(project.root):
-        invoke(["run", "test_default"], obj=project)
+        pdm(["run", "test_default"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar foo"
-        invoke(["run", "test_override"], obj=project)
+        pdm(["run", "test_override"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar override"
 
 
-def test_run_script_override_global_env(project, invoke, capfd):
+def test_run_script_override_global_env(project, pdm, capfd):
     (project.root / "test_script.py").write_text("import os; print(os.getenv('FOO'))")
     project.pyproject.settings["scripts"] = {
         "_": {"env": {"FOO": "bar"}},
         "test_env": {"cmd": "python test_script.py"},
         "test_env_override": {"cmd": "python test_script.py", "env": {"FOO": "foobar"}},
     }
     project.pyproject.write()
     capfd.readouterr()
     with cd(project.root):
-        invoke(["run", "test_env"], obj=project)
+        pdm(["run", "test_env"], obj=project)
         assert capfd.readouterr()[0].strip() == "bar"
-        invoke(["run", "test_env_override"], obj=project)
+        pdm(["run", "test_env_override"], obj=project)
         assert capfd.readouterr()[0].strip() == "foobar"
 
 
-def test_run_show_list_of_scripts(project, invoke):
+def test_run_show_list_of_scripts(project, pdm):
     project.pyproject.settings["scripts"] = {
         "test_composite": {"composite": ["test_cmd", "test_script", "test_shell"]},
         "test_cmd": "flask db upgrade",
         "test_multi": """\
             I am a multilines
             command
         """,
         "test_script": {"call": "test_script:main", "help": "call a python function"},
         "test_shell": {"shell": "echo $FOO", "help": "shell command"},
     }
     project.pyproject.write()
-    result = invoke(["run", "--list"], obj=project)
+    result = pdm(["run", "--list"], obj=project)
     result_lines = result.output.splitlines()[3:]
     assert result_lines[0][1:-1].strip() == "test_cmd       │ cmd       │ flask db upgrade"
     sep = termui.Emoji.ARROW_SEPARATOR
     assert result_lines[1][1:-1].strip() == f"test_composite │ composite │ test_cmd {sep} test_script {sep} test_shell"
     assert result_lines[2][1:-1].strip() == f"test_multi     │ cmd       │ I am a multilines{termui.Emoji.ELLIPSIS}"
     assert result_lines[3][1:-1].strip() == "test_script    │ call      │ call a python function"
     assert result_lines[4][1:-1].strip() == "test_shell     │ shell     │ shell command"
 
 
+def test_run_show_list_of_scripts_hide_internals(project, pdm):
+    project.pyproject.settings["scripts"] = {
+        "public": "true",
+        "_internal": "true",
+    }
+    project.pyproject.write()
+    result = pdm(["run", "--list"], obj=project)
+    assert "public" in result.output
+    assert "_internal" not in result.output
+
+
+def test_run_json_list_of_scripts(project, pdm):
+    project.pyproject.settings["scripts"] = {
+        "_": {"env_file": ".env"},
+        "test_composite": {"composite": ["test_cmd", "test_script", "test_shell"]},
+        "test_cmd": "flask db upgrade",
+        "test_multi": """\
+            I am a multilines
+            command
+        """,
+        "test_script": {"call": "test_script:main", "help": "call a python function"},
+        "test_shell": {"shell": "echo $FOO", "help": "shell command"},
+        "test_env": {"cmd": "true", "env": {"TEST": "value"}},
+        "test_env_file": {"cmd": "true", "env_file": ".env"},
+        "test_override": {"cmd": "true", "env_file": {"override": ".env"}},
+        "test_site_packages": {"cmd": "true", "site_packages": True},
+        "_private": "true",
+    }
+    project.pyproject.write()
+    result = pdm(["run", "--json"], obj=project, strict=True)
+
+    sep = termui.Emoji.ARROW_SEPARATOR
+    assert json.loads(result.outputs) == {
+        "_": {"name": "_", "help": "Shared options", "kind": "shared", "env_file": ".env"},
+        "test_cmd": {"name": "test_cmd", "help": "flask db upgrade", "kind": "cmd", "args": "flask db upgrade"},
+        "test_composite": {
+            "name": "test_composite",
+            "help": f"test_cmd {sep} test_script {sep} test_shell",
+            "kind": "composite",
+            "args": ["test_cmd", "test_script", "test_shell"],
+        },
+        "test_multi": {
+            "name": "test_multi",
+            "help": f"I am a multilines{termui.Emoji.ELLIPSIS}",
+            "kind": "cmd",
+            "args": "            I am a multilines\n            command\n        ",
+        },
+        "test_script": {
+            "name": "test_script",
+            "help": "call a python function",
+            "kind": "call",
+            "args": "test_script:main",
+        },
+        "test_shell": {"name": "test_shell", "help": "shell command", "kind": "shell", "args": "echo $FOO"},
+        "test_env": {"name": "test_env", "help": "true", "kind": "cmd", "args": "true", "env": {"TEST": "value"}},
+        "test_env_file": {"name": "test_env_file", "help": "true", "kind": "cmd", "args": "true", "env_file": ".env"},
+        "test_override": {
+            "name": "test_override",
+            "help": "true",
+            "kind": "cmd",
+            "args": "true",
+            "env_file.override": ".env",
+        },
+        "test_site_packages": {
+            "name": "test_site_packages",
+            "help": "true",
+            "kind": "cmd",
+            "args": "true",
+            "site_packages": True,
+        },
+        "_private": {
+            "name": "_private",
+            "help": "true",
+            "kind": "cmd",
+            "args": "true",
+        },
+    }
+
+
 @pytest.mark.usefixtures("local_finder")
 @pytest.mark.parametrize("explicit_python", [True, False])
-def test_run_with_another_project_root(project, invoke, capfd, explicit_python):
+def test_run_with_another_project_root(project, pdm, capfd, explicit_python):
     project.pyproject.metadata["requires-python"] = ">=3.6"
     project.pyproject.write()
-    invoke(["add", "first"], obj=project)
+    pdm(["add", "first"], obj=project)
     with TemporaryDirectory(prefix="pytest-run-") as tmp_dir:
         Path(tmp_dir).joinpath("main.py").write_text("import first;print(first.first([0, False, 1, 2]))\n")
         capfd.readouterr()
         with cd(tmp_dir):
             args = ["run", "-p", str(project.root), "main.py"]
             if explicit_python:
                 args.insert(len(args) - 1, "python")
-            ret = invoke(args)
+            ret = pdm(args)
             out, err = capfd.readouterr()
             assert ret.exit_code == 0, err
             assert out.strip() == "1"
 
 
-def test_import_another_sitecustomize(project, invoke, capfd):
+def test_import_another_sitecustomize(project, pdm, capfd):
     project.pyproject.metadata["requires-python"] = ">=2.7"
     project.pyproject.write()
     # a script for checking another sitecustomize is imported
     project.root.joinpath("foo.py").write_text("import os;print(os.getenv('FOO'))")
     # ensure there have at least one sitecustomize can be imported
     # there may have more than one sitecustomize.py in sys.path
     project.root.joinpath("sitecustomize.py").write_text("import os;os.environ['FOO'] = 'foo'")
@@ -417,158 +496,158 @@
     paths = env.get("PYTHONPATH")
     this_path = str(project.root)
     new_paths = [this_path] if not paths else [this_path, paths]
     env["PYTHONPATH"] = os.pathsep.join(new_paths)
     project._environment = None
     capfd.readouterr()
     with cd(project.root):
-        result = invoke(["run", "python", "foo.py"], env=env)
+        result = pdm(["run", "python", "foo.py"], env=env)
     assert result.exit_code == 0, result.stderr
     out, _ = capfd.readouterr()
     assert out.strip() == "foo"
 
 
-def test_run_with_patched_sysconfig(project, invoke, capfd):
+def test_run_with_patched_sysconfig(project, pdm, capfd):
     project.root.joinpath("script.py").write_text(
         """\
 import sysconfig
 import json
 print(json.dumps(sysconfig.get_paths()))
 """
     )
     capfd.readouterr()
     with cd(project.root):
-        result = invoke(["run", "python", "script.py"], obj=project)
+        result = pdm(["run", "python", "script.py"], obj=project)
     assert result.exit_code == 0
     out = json.loads(capfd.readouterr()[0])
     assert "__pypackages__" in out["purelib"]
 
 
-def test_run_composite(project, invoke, capfd, _echo):
+def test_run_composite(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "first": "python echo.py First",
         "second": "python echo.py Second",
         "test": {"composite": ["first", "second"]},
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "First CALLED" in out
     assert "Second CALLED" in out
 
 
-def test_composite_stops_on_first_failure(project, invoke, capfd):
+def test_composite_stops_on_first_failure(project, pdm, capfd):
     project.pyproject.settings["scripts"] = {
         "first": {"cmd": ["python", "-c", "print('First CALLED')"]},
         "fail": "python -c 'raise Exception'",
         "second": "echo 'Second CALLED'",
         "test": {"composite": ["first", "fail", "second"]},
     }
     project.pyproject.write()
     capfd.readouterr()
-    result = invoke(["run", "test"], obj=project)
+    result = pdm(["run", "test"], obj=project)
     assert result.exit_code == 1
     out, _ = capfd.readouterr()
     assert "First CALLED" in out
     assert "Second CALLED" not in out
 
 
-def test_composite_inherit_env(project, invoke, capfd, _echo):
+def test_composite_inherit_env(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "first": {
             "cmd": "python echo.py First VAR",
             "env": {"VAR": "42"},
         },
         "second": {
             "cmd": "python echo.py Second VAR",
             "env": {"VAR": "42"},
         },
         "test": {"composite": ["first", "second"], "env": {"VAR": "overriden"}},
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "First CALLED with VAR=overriden" in out
     assert "Second CALLED with VAR=overriden" in out
 
 
-def test_composite_fail_on_first_missing_task(project, invoke, capfd, _echo):
+def test_composite_fail_on_first_missing_task(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "first": "python echo.py First",
         "second": "python echo.py Second",
         "test": {"composite": ["first", "fail", "second"]},
     }
     project.pyproject.write()
     capfd.readouterr()
-    result = invoke(["run", "test"], obj=project)
+    result = pdm(["run", "test"], obj=project)
     assert result.exit_code == 1
     out, _ = capfd.readouterr()
     assert "First CALLED" in out
     assert "Second CALLED" not in out
 
 
-def test_composite_runs_all_hooks(project, invoke, capfd, _echo):
+def test_composite_runs_all_hooks(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second"]},
         "pre_test": "python echo.py Pre-Test",
         "post_test": "python echo.py Post-Test",
         "first": "python echo.py First",
         "pre_first": "python echo.py Pre-First",
         "second": "python echo.py Second",
         "post_second": "python echo.py Post-Second",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Test CALLED" in out
     assert "Pre-First CALLED" in out
     assert "First CALLED" in out
     assert "Second CALLED" in out
     assert "Post-Second CALLED" in out
     assert "Post-Test CALLED" in out
 
 
-def test_composite_pass_parameters_to_subtasks(project, invoke, capfd, _args):
+def test_composite_pass_parameters_to_subtasks(project, pdm, capfd, _args):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second"]},
         "pre_test": "python args.py Pre-Test",
         "post_test": "python args.py Post-Test",
         "first": "python args.py First",
         "pre_first": "python args.py Pre-First",
         "second": "python args.py Second",
         "post_second": "python args.py Post-Second",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test", "param=value"], strict=True, obj=project)
+    pdm(["run", "test", "param=value"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Test CALLED" in out
     assert "Pre-First CALLED" in out
     assert "First CALLED with param=value" in out
     assert "Second CALLED with param=value" in out
     assert "Post-Second CALLED" in out
     assert "Post-Test CALLED" in out
 
 
-def test_composite_can_pass_parameters(project, invoke, capfd, _args):
+def test_composite_can_pass_parameters(project, pdm, capfd, _args):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first param=first", "second param=second"]},
         "pre_test": "python args.py Pre-Test",
         "post_test": "python args.py Post-Test",
         "first": "python args.py First",
         "pre_first": "python args.py Pre-First",
         "second": "python args.py Second",
         "post_second": "python args.py Post-Second",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Test CALLED" in out
     assert "Pre-First CALLED" in out
     assert "First CALLED with param=first" in out
     assert "Second CALLED with param=second" in out
     assert "Post-Second CALLED" in out
     assert "Post-Test CALLED" in out
@@ -577,68 +656,66 @@
 @pytest.mark.parametrize(
     "args,expected",
     (
         pytest.param(["-a"], "-a, ", id="with-args"),
         pytest.param([], "", id="without-args"),
     ),
 )
-def test_composite_only_pass_parameters_to_subtasks_with_args(project, invoke, capfd, _args, args, expected):
+def test_composite_only_pass_parameters_to_subtasks_with_args(project, pdm, capfd, _args, args, expected):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second {args} key=value"]},
         "first": "python args.py First",
         "second": "python args.py Second",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "-v", "test", *args], strict=True, obj=project)
+    pdm(["run", "-v", "test", *args], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "First CALLED" in out
     assert f"Second CALLED with {expected}key=value" in out
 
 
 @pytest.mark.parametrize(
     "args,expected",
     (
         pytest.param(["-a"], "-a", id="with-args"),
         pytest.param([], "--default", id="default"),
     ),
 )
-def test_composite_only_pass_parameters_to_subtasks_with_args_with_default(
-    project, invoke, capfd, _args, args, expected
-):
+def test_composite_only_pass_parameters_to_subtasks_with_args_with_default(project, pdm, capfd, _args, args, expected):
     project.pyproject.settings["scripts"] = {
         "test": {"composite": ["first", "second {args:--default} key=value"]},
         "first": "python args.py First",
         "second": "python args.py Second",
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "-v", "test", *args], strict=True, obj=project)
+    pdm(["run", "-v", "test", *args], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "First CALLED" in out
     assert f"Second CALLED with {expected}, key=value" in out
 
 
-def test_composite_hooks_inherit_env(project, invoke, capfd, _echo):
+def test_composite_hooks_inherit_env(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "pre_task": {"cmd": "python echo.py Pre-Task VAR", "env": {"VAR": "42"}},
         "task": "python echo.py Task",
         "post_task": {"cmd": "python echo.py Post-Task VAR", "env": {"VAR": "42"}},
         "test": {"composite": ["task"], "env": {"VAR": "overriden"}},
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Task CALLED with VAR=overriden" in out
     assert "Task CALLED" in out
     assert "Post-Task CALLED with VAR=overriden" in out
 
 
-def test_composite_inherit_env_in_cascade(project, invoke, capfd, _echo):
+def test_composite_inherit_env_in_cascade(project, pdm, capfd, _echo):
     project.pyproject.settings["scripts"] = {
         "_": {"env": {"FOO": "BAR", "TIK": "TOK"}},
         "pre_task": {
             "cmd": "python echo.py Pre-Task VAR FOO TIK",
             "env": {"VAR": "42", "FOO": "foobar"},
         },
         "task": {
@@ -649,92 +726,92 @@
             "cmd": "python echo.py Post-Task VAR FOO TIK",
             "env": {"VAR": "42", "FOO": "foobar"},
         },
         "test": {"composite": ["task"], "env": {"VAR": "overriden"}},
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Task CALLED with VAR=overriden FOO=foobar TIK=TOK" in out
     assert "Task CALLED with VAR=overriden FOO=foobar TIK=TOK" in out
     assert "Post-Task CALLED with VAR=overriden FOO=foobar TIK=TOK" in out
 
 
-def test_composite_inherit_dotfile(project, invoke, capfd, _echo):
+def test_composite_inherit_dotfile(project, pdm, capfd, _echo):
     (project.root / ".env").write_text("VAR=42")
     (project.root / "override.env").write_text("VAR=overriden")
     project.pyproject.settings["scripts"] = {
         "pre_task": {"cmd": "python echo.py Pre-Task VAR", "env_file": ".env"},
         "task": {"cmd": "python echo.py Task VAR", "env_file": ".env"},
         "post_task": {"cmd": "python echo.py Post-Task VAR", "env_file": ".env"},
         "test": {"composite": ["task"], "env_file": "override.env"},
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "test"], strict=True, obj=project)
+    pdm(["run", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Pre-Task CALLED with VAR=overriden" in out
     assert "Task CALLED with VAR=overriden" in out
     assert "Post-Task CALLED with VAR=overriden" in out
 
 
-def test_composite_can_have_commands(project, invoke, capfd):
+def test_composite_can_have_commands(project, pdm, capfd):
     project.pyproject.settings["scripts"] = {
         "task": {"cmd": ["python", "-c", 'print("Task CALLED")']},
         "test": {"composite": ["task", "python -c 'print(\"Command CALLED\")'"]},
     }
     project.pyproject.write()
     capfd.readouterr()
-    invoke(["run", "-v", "test"], strict=True, obj=project)
+    pdm(["run", "-v", "test"], strict=True, obj=project)
     out, _ = capfd.readouterr()
     assert "Task CALLED" in out
     assert "Command CALLED" in out
 
 
-def test_run_shortcut(project, invoke, capfd):
+def test_run_shortcut(project, pdm, capfd):
     project.pyproject.settings["scripts"] = {
         "test": "echo 'Everything is fine'",
     }
     project.pyproject.write()
     capfd.readouterr()
-    result = invoke(["test"], obj=project, strict=True)
+    result = pdm(["test"], obj=project, strict=True)
     assert result.exit_code == 0
     out, _ = capfd.readouterr()
     assert "Everything is fine" in out
 
 
-def test_run_shortcuts_dont_override_commands(project, invoke, capfd, mocker):
+def test_run_shortcuts_dont_override_commands(project, pdm, capfd, mocker):
     do_lock = mocker.patch.object(actions, "do_lock")
     do_sync = mocker.patch.object(actions, "do_sync")
     project.pyproject.settings["scripts"] = {
         "install": "echo 'Should not run'",
     }
     project.pyproject.write()
     capfd.readouterr()
-    result = invoke(["install"], obj=project, strict=True)
+    result = pdm(["install"], obj=project, strict=True)
     assert result.exit_code == 0
     out, _ = capfd.readouterr()
     assert "Should not run" not in out
     do_lock.assert_called_once()
     do_sync.assert_called_once()
 
 
-def test_run_shortcut_fail_with_usage_if_script_not_found(project, invoke):
-    result = invoke(["whatever"], obj=project)
+def test_run_shortcut_fail_with_usage_if_script_not_found(project, pdm):
+    result = pdm(["whatever"], obj=project)
     assert result.exit_code != 0
     assert "Script unknown: whatever" in result.stderr
     assert "Usage" in result.stderr
 
 
 @pytest.mark.parametrize(
     "args",
     [
         pytest.param([], id="no args"),
         pytest.param(["-ko"], id="unknown param"),
         pytest.param(["pip", "--version"], id="not an user script"),
     ],
 )
-def test_empty_positionnal_args_still_display_usage(project, invoke, args):
-    result = invoke(args, obj=project)
+def test_empty_positionnal_args_still_display_usage(project, pdm, args):
+    result = pdm(args, obj=project)
     assert result.exit_code != 0
     assert "Usage" in result.stderr
```

### Comparing `pdm-2.5.6/tests/cli/test_self_command.py` & `pdm-2.6.0/tests/cli/test_self_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,53 +34,53 @@
 def mock_latest_pdm_version(mocker):
     return mocker.patch(
         "pdm.cli.commands.self_cmd.get_latest_pdm_version_from_pypi",
     )
 
 
 @pytest.mark.usefixtures("mock_all_distributions")
-def test_self_list(invoke):
-    result = invoke(["self", "list"])
+def test_self_list(pdm):
+    result = pdm(["self", "list"])
     assert result.exit_code == 0, result.stderr
     packages = [line.split()[0] for line in result.stdout.splitlines()]
     assert packages == ["bar", "baz", "foo"]
 
 
 @pytest.mark.usefixtures("mock_all_distributions")
-def test_self_list_plugins(invoke):
-    result = invoke(["self", "list", "--plugins"])
+def test_self_list_plugins(pdm):
+    result = pdm(["self", "list", "--plugins"])
     assert result.exit_code == 0, result.stderr
     packages = [line.split()[0] for line in result.stdout.splitlines()]
     assert packages == ["bar", "foo"]
 
 
-def test_self_add(invoke, mock_pip):
-    result = invoke(["self", "add", "foo"])
+def test_self_add(pdm, mock_pip):
+    result = pdm(["self", "add", "foo"])
     assert result.exit_code == 0, result.stderr
     mock_pip.assert_called_with(ANY, ["install", "foo"])
 
-    result = invoke(["self", "add", "--pip-args", "--force-reinstall --upgrade", "foo"])
+    result = pdm(["self", "add", "--pip-args", "--force-reinstall --upgrade", "foo"])
     assert result.exit_code == 0, result.stderr
     mock_pip.assert_called_with(ANY, ["install", "--force-reinstall", "--upgrade", "foo"])
 
 
-def test_self_remove(invoke, mock_pip, monkeypatch):
+def test_self_remove(pdm, mock_pip, monkeypatch):
     def _mock_resolve(self, packages):
         return ["demo", "pytz"] if "demo" in packages else packages
 
     monkeypatch.setattr(
         self_cmd.RemoveCommand,
         "_resolve_dependencies_to_remove",
         _mock_resolve,
     )
 
-    result = invoke(["self", "remove", "foo"])
+    result = pdm(["self", "remove", "foo"])
     assert result.exit_code != 0
 
-    result = invoke(["self", "remove", "-y", "demo"])
+    result = pdm(["self", "remove", "-y", "demo"])
     assert result.exit_code == 0, result.stderr
     mock_pip.assert_called_with(ANY, ["uninstall", "-y", "demo", "pytz"])
 
 
 @pytest.mark.parametrize(
     "args,expected",
     [
@@ -88,25 +88,25 @@
         (["self", "update", "--pre"], ["install", "--upgrade", "pdm==99.0.1b1"]),
         (
             ["self", "update", "--head"],
             ["install", "--upgrade", f"pdm @ git+{self_cmd.PDM_REPO}@main"],
         ),
     ],
 )
-def test_self_update(invoke, mock_pip, mock_latest_pdm_version, args, expected):
+def test_self_update(pdm, mock_pip, mock_latest_pdm_version, args, expected):
     def mocked_latest_version(project, pre):
         return "99.0.1b1" if pre else "99.0.0"
 
     mock_latest_pdm_version.side_effect = mocked_latest_version
 
-    result = invoke(args)
+    result = pdm(args)
     assert result.exit_code == 0, result.stderr
     mock_pip.assert_called_with(ANY, expected)
 
 
-def test_self_update_already_latest(invoke, mock_pip, mock_latest_pdm_version):
+def test_self_update_already_latest(pdm, mock_pip, mock_latest_pdm_version):
     mock_latest_pdm_version.return_value = "0.0.0"
 
-    result = invoke(["self", "update"])
+    result = pdm(["self", "update"])
     assert result.exit_code == 0, result.stderr
     assert "Already up-to-date" in result.stdout
     mock_pip.assert_not_called()
```

### Comparing `pdm-2.5.6/tests/cli/test_update.py` & `pdm-2.6.0/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/cli/test_use.py` & `pdm-2.6.0/tests/cli/test_use.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 import pytest
 
 from pdm.cli import actions
 from pdm.exceptions import NoPythonVersion
 from pdm.models.caches import JSONFileCache
 
 
-def test_use_command(project, invoke):
+def test_use_command(project, pdm):
     python = "python" if os.name == "nt" else "python3"
     python_path = shutil.which(python)
-    result = invoke(["use", "-f", python], obj=project)
+    result = pdm(["use", "-f", python], obj=project)
     assert result.exit_code == 0
     config_content = project.root.joinpath(".pdm-python").read_text()
     assert Path(python_path).as_posix() in config_content
 
-    result = invoke(["use", "-f", python_path], obj=project)
+    result = pdm(["use", "-f", python_path], obj=project)
     assert result.exit_code == 0
     project.pyproject.metadata["requires-python"] = ">=3.6"
-    result = invoke(["use", "2.7"], obj=project)
+    result = pdm(["use", "2.7"], obj=project)
     assert result.exit_code == 1
 
 
-def test_use_python_by_version(project, invoke):
+def test_use_python_by_version(project, pdm):
     python_version = ".".join(map(str, sys.version_info[:2]))
-    result = invoke(["use", "-f", python_version], obj=project)
+    result = pdm(["use", "-f", python_version], obj=project)
     assert result.exit_code == 0
 
 
 @pytest.mark.skipif(os.name != "posix", reason="Run on POSIX platforms only")
 def test_use_wrapper_python(project):
     wrapper_script = """#!/bin/bash
 exec "{}" "$@"
```

### Comparing `pdm-2.5.6/tests/cli/test_venv.py` & `pdm-2.6.0/tests/cli/test_venv.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,196 +25,196 @@
 
     monkeypatch.setattr(backends.VirtualenvBackend, "perform_create", fake_create)
     monkeypatch.setattr(backends.VenvBackend, "perform_create", fake_create)
     monkeypatch.setattr(backends.CondaBackend, "perform_create", fake_create)
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_create(invoke, project):
+def test_venv_create(pdm, project):
     project._saved_python = None
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
     assert os.path.exists(venv_path)
     assert not project._saved_python
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_create_in_project(invoke, project):
+def test_venv_create_in_project(pdm, project):
     project.project_config["venv.in_project"] = True
-    invoke(["venv", "create"], obj=project, strict=True)
+    pdm(["venv", "create"], obj=project, strict=True)
     venv_path = project.root / ".venv"
     assert venv_path.exists()
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 1
     assert "is not empty" in result.stderr
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_show_path(invoke, project):
+def test_venv_show_path(pdm, project):
     project.project_config["venv.in_project"] = True
-    invoke(["venv", "create"], obj=project, strict=True)
-    invoke(["venv", "create", "--name", "test"], obj=project, strict=True)
-    result = invoke(["venv", "--path", "in-project"], obj=project, strict=True)
+    pdm(["venv", "create"], obj=project, strict=True)
+    pdm(["venv", "create", "--name", "test"], obj=project, strict=True)
+    result = pdm(["venv", "--path", "in-project"], obj=project, strict=True)
     assert result.output.strip() == str(project.root / ".venv")
-    result = invoke(["venv", "--path", "test"], obj=project)
+    result = pdm(["venv", "--path", "test"], obj=project)
     assert result.exit_code == 0
-    result = invoke(["venv", "--path", "foo"], obj=project)
+    result = pdm(["venv", "--path", "foo"], obj=project)
     assert result.exit_code == 1
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_list(invoke, project):
+def test_venv_list(pdm, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
 
-    result = invoke(["venv", "list"], obj=project)
+    result = pdm(["venv", "list"], obj=project)
     assert result.exit_code == 0, result.stderr
     assert venv_path in result.output
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_remove(invoke, project):
+def test_venv_remove(pdm, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
     key = os.path.basename(venv_path)[len(get_venv_prefix(project)) :]
 
-    result = invoke(["venv", "remove", "non-exist"], obj=project)
+    result = pdm(["venv", "remove", "non-exist"], obj=project)
     assert result.exit_code != 0
 
-    result = invoke(["venv", "remove", "-y", key], obj=project)
+    result = pdm(["venv", "remove", "-y", key], obj=project)
     assert result.exit_code == 0, result.stderr
 
     assert not os.path.exists(venv_path)
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_recreate(invoke, project):
+def test_venv_recreate(pdm, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
 
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code != 0
 
-    result = invoke(["venv", "create", "-f"], obj=project)
+    result = pdm(["venv", "create", "-f"], obj=project)
     assert result.exit_code == 0, result.stderr
 
 
 @pytest.mark.usefixtures("venv_backends")
-def test_venv_activate(invoke, mocker, project):
+def test_venv_activate(pdm, mocker, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
     key = os.path.basename(venv_path)[len(get_venv_prefix(project)) :]
 
     mocker.patch("shellingham.detect_shell", return_value=("bash", None))
-    result = invoke(["venv", "activate", key], obj=project)
+    result = pdm(["venv", "activate", key], obj=project)
     assert result.exit_code == 0, result.stderr
     backend = project.config["venv.backend"]
 
     if backend == "conda":
         assert result.output.startswith("conda activate")
     else:
         assert result.output.strip("'\"\n").endswith("activate")
         assert result.output.startswith("source")
 
 
 @pytest.mark.usefixtures("venv_backends")
-def test_venv_activate_custom_prompt(invoke, mocker, project):
+def test_venv_activate_custom_prompt(pdm, mocker, project):
     project.project_config["venv.in_project"] = False
     creator = mocker.patch("pdm.cli.commands.venv.backends.Backend.create")
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     creator.assert_called_once_with(
         None, [], False, False, prompt=project.project_config["venv.prompt"], with_pip=False
     )
 
 
-def test_venv_activate_project_without_python(invoke, project):
+def test_venv_activate_project_without_python(pdm, project):
     project._saved_python = None
-    result = invoke(["venv", "activate"], obj=project)
+    result = pdm(["venv", "activate"], obj=project)
     assert result.exit_code != 0
     assert "The project doesn't have a saved python.path" in result.stderr
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_activate_error(invoke, project):
+def test_venv_activate_error(pdm, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project, strict=True)
+    result = pdm(["venv", "create"], obj=project, strict=True)
 
-    result = invoke(["venv", "activate", "foo"], obj=project)
+    result = pdm(["venv", "activate", "foo"], obj=project)
     assert result.exit_code != 0
     assert "No virtualenv with key" in result.stderr
 
     project._saved_python = os.path.abspath("fake/bin/python")
-    result = invoke(["venv", "activate"], obj=project)
+    result = pdm(["venv", "activate"], obj=project)
     assert result.exit_code != 0, result.output + result.stderr
     assert "Can't activate a non-venv Python" in result.stderr
 
 
 @pytest.mark.usefixtures("fake_create")
 @pytest.mark.parametrize("keep_pypackages", [True, False])
-def test_venv_auto_create(invoke, mocker, project, keep_pypackages):
+def test_venv_auto_create(pdm, mocker, project, keep_pypackages):
     creator = mocker.patch("pdm.cli.commands.venv.backends.Backend.create")
     project._saved_python = None
     if keep_pypackages:
         project.root.joinpath("__pypackages__").mkdir(exist_ok=True)
     else:
         shutil.rmtree(project.root / "__pypackages__", ignore_errors=True)
     project.project_config["python.use_venv"] = True
-    invoke(["install"], obj=project)
+    pdm(["install"], obj=project)
     if keep_pypackages:
         creator.assert_not_called()
     else:
         creator.assert_called_once()
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_purge(invoke, project):
+def test_venv_purge(pdm, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "purge"], obj=project)
+    result = pdm(["venv", "purge"], obj=project)
     assert result.exit_code == 0, result.stderr
 
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
-    result = invoke(["venv", "purge"], input="y", obj=project)
+    result = pdm(["venv", "purge"], input="y", obj=project)
     assert result.exit_code == 0, result.stderr
     assert not os.path.exists(venv_path)
 
 
 @pytest.mark.usefixtures("fake_create")
-def test_venv_purge_force(invoke, project):
+def test_venv_purge_force(pdm, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
-    result = invoke(["venv", "purge", "-f"], obj=project)
+    result = pdm(["venv", "purge", "-f"], obj=project)
     assert result.exit_code == 0, result.stderr
     assert not os.path.exists(venv_path)
 
 
 user_options = [("none", True), ("0", False), ("all", False)]
 
 
 @pytest.mark.usefixtures("venv_backends")
 @pytest.mark.parametrize("user_choices, is_path_exists", user_options)
-def test_venv_purge_interactive(invoke, user_choices, is_path_exists, project):
+def test_venv_purge_interactive(pdm, user_choices, is_path_exists, project):
     project.project_config["venv.in_project"] = False
-    result = invoke(["venv", "create"], obj=project)
+    result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 0, result.stderr
     venv_path = re.match(r"Virtualenv (.+) is created successfully", result.output).group(1)
-    result = invoke(["venv", "purge", "-i"], input=user_choices, obj=project)
+    result = pdm(["venv", "purge", "-i"], input=user_choices, obj=project)
     assert result.exit_code == 0, result.stderr
     assert os.path.exists(venv_path) == is_path_exists
 
 
 def test_virtualenv_backend_create(project, mocker, with_pip):
     backend = backends.VirtualenvBackend(project, None)
     assert backend.ident
```

### Comparing `pdm-2.5.6/tests/conftest.py` & `pdm-2.6.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import pytest
 from unearth.vcs import Git, vcs_support
 
 from tests import FIXTURES
 
 if TYPE_CHECKING:
-    from pdm.pytest import IndexesDefinition, PDMCallable
+    from pdm.pytest import IndexesDefinition
 
 
 os.environ.update(CI="1", PDM_CHECK_UPDATE="0")
 
 pytest_plugins = [
     "pdm.pytest",
 ]
@@ -77,15 +77,15 @@
             "zipp-3.7.0-py3-none-any.whl",
             "typing_extensions-4.4.0-py3-none-any.whl",
         )
     ]
 
 
 @pytest.fixture
-def local_finder_artifacts() -> Path():
+def local_finder_artifacts() -> Path:
     return FIXTURES / "artifacts"
 
 
 def copytree(src: Path, dst: Path) -> None:
     if not dst.exists():
         dst.mkdir(parents=True)
     for subpath in src.iterdir():
@@ -119,12 +119,7 @@
 def is_editable(request):
     return request.param
 
 
 @pytest.fixture(params=[False, True])
 def dev_option(request) -> Iterable[str]:
     return ("--dev",) if request.param else ()
-
-
-@pytest.fixture
-def invoke(pdm: PDMCallable) -> PDMCallable:
-    return pdm
```

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.6.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.6.0/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.6.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.6.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.6.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.6.0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.6.0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.6.0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.6.0/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.6.0/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.6.0/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/pypi.json` & `pdm-2.6.0/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/fixtures/pyproject.toml` & `pdm-2.6.0/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/models/test_backends.py` & `pdm-2.6.0/tests/models/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         )
     project.pyproject.write()
     project._environment = None
     assert isinstance(project.backend, backend_cls)
 
 
 @pytest.mark.parametrize("backend", _BACKENDS.keys())
-def test_project_backend(project, working_set, backend, invoke):
+def test_project_backend(project, working_set, backend, pdm):
     _setup_backend(project, backend)
     shutil.copytree(FIXTURES / "projects/demo", project.root / "demo")
     project.root.joinpath("sub").mkdir()
     with cd(project.root.joinpath("sub")):
-        invoke(["add", "--no-self", "../demo"], obj=project, strict=True)
+        pdm(["add", "--no-self", "../demo"], obj=project, strict=True)
         assert "idna" in working_set
         assert "demo" in working_set
         dep = project.pyproject.metadata["dependencies"][0]
         demo_path = project.root.joinpath("demo").as_posix()
         demo_url = path_to_url(demo_path)
         if backend in ("pdm-pep517", "pdm-backend"):
             assert dep == "demo @ file:///${PROJECT_ROOT}/demo"
```

### Comparing `pdm-2.5.6/tests/models/test_candidates.py` & `pdm-2.6.0/tests/models/test_candidates.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,7 +322,14 @@
 
 def test_parse_metadata_with_dynamic_fields(project, local_finder):
     req = parse_requirement(f"demo-package @ file://{FIXTURES.as_posix()}/projects/demo-src-package")
     candidate = Candidate(req)
     metadata = candidate.prepare(project.environment).metadata
     assert not metadata.requires
     assert metadata.version == "0.1.0"
+
+
+def test_get_metadata_for_non_existing_path(project):
+    req = parse_requirement("file:///${PROJECT_ROOT}/non-existing-path")
+    candidate = Candidate(req)
+    with pytest.raises(FileNotFoundError, match="No such file or directory"):
+        candidate.prepare(project.environment).metadata
```

### Comparing `pdm-2.5.6/tests/models/test_marker.py` & `pdm-2.6.0/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/models/test_requirements.py` & `pdm-2.6.0/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/models/test_setup_parsing.py` & `pdm-2.6.0/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/models/test_specifiers.py` & `pdm-2.6.0/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/models/test_versions.py` & `pdm-2.6.0/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/resolver/test_resolve.py` & `pdm-2.6.0/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/test_formats.py` & `pdm-2.6.0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/tests/test_installer.py` & `pdm-2.6.0/tests/test_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         "celery.exe" if os.name == "nt" else "celery",
     )
     assert os.path.exists(celery_script)
     installer.uninstall(project.environment.get_working_set()["celery"])
     assert not os.path.exists(celery_script)
 
 
-def test_install_wheel_with_cache(project, invoke):
+def test_install_wheel_with_cache(project, pdm):
     supports_symlink = fs_supports_symlink()
     req = parse_requirement("future-fstrings")
     candidate = Candidate(
         req,
         link=Link("http://fixtures.test/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl"),
     )
     installer = InstallManager(project.environment, use_install_cache=True)
@@ -113,16 +113,16 @@
         assert os.path.islink(os.path.join(lib_path, "aaaaa_future_fstrings.pth"))
     else:
         assert os.path.isfile(os.path.join(lib_path, "aaa_future_fstrings.pth"))
         assert os.path.isfile(os.path.join(lib_path, "aaaaa_future_fstrings.pth"))
 
     cache_path = project.cache("packages") / "future_fstrings-1.2.0-py2.py3-none-any"
     assert cache_path.is_dir()
-    invoke(["run", "python", "-m", "site"], object=project)
-    r = invoke(["run", "python", "-c", "import future_fstrings"], obj=project)
+    pdm(["run", "python", "-m", "site"], object=project)
+    r = pdm(["run", "python", "-c", "import future_fstrings"], obj=project)
     assert r.exit_code == 0
 
     dist = project.environment.get_working_set()["future-fstrings"]
     installer.uninstall(dist)
     if supports_symlink:
         assert not os.path.exists(os.path.join(lib_path, "future_fstrings.py"))
         assert not os.path.exists(os.path.join(lib_path, "aaaaa_future_fstrings.pth"))
```

### Comparing `pdm-2.5.6/tests/test_integration.py` & `pdm-2.6.0/tests/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,28 +20,28 @@
     return available_versions
 
 
 @pytest.mark.integration
 @pytest.mark.network
 @pytest.mark.flaky(reruns=3)
 @pytest.mark.parametrize("python_version", get_python_versions())
-def test_basic_integration(python_version, core, tmp_path, invoke):
+def test_basic_integration(python_version, core, tmp_path, pdm):
     """An e2e test case to ensure PDM works on all supported Python versions"""
     project = core.create_project(tmp_path)
     project.pyproject.set_data(PYPROJECT)
     project.root.joinpath("foo.py").write_text("import django\n")
     project._environment = None
-    invoke(["use", "-f", python_version], obj=project, strict=True)
-    invoke(["add", "django", "-v"], obj=project, strict=True)
+    pdm(["use", "-f", python_version], obj=project, strict=True)
+    pdm(["add", "django", "-v"], obj=project, strict=True)
     with cd(project.root):
-        invoke(["run", "python", "foo.py"], obj=project, strict=True)
-        invoke(["build", "-v"], obj=project, strict=True)
-    invoke(["remove", "-v", "django"], obj=project, strict=True)
-    result = invoke(["list"], obj=project, strict=True)
+        pdm(["run", "python", "foo.py"], obj=project, strict=True)
+        pdm(["build", "-v"], obj=project, strict=True)
+    pdm(["remove", "-v", "django"], obj=project, strict=True)
+    result = pdm(["list"], obj=project, strict=True)
     assert not any(line.strip().lower().startswith("django") for line in result.output.splitlines())
 
 
-def test_actual_list_freeze(project, local_finder, invoke):
-    invoke(["config", "-l", "install.parallel", "false"], obj=project, strict=True)
-    invoke(["add", "first"], obj=project, strict=True)
-    r = invoke(["list", "--freeze"], obj=project)
+def test_actual_list_freeze(project, local_finder, pdm):
+    pdm(["config", "-l", "install.parallel", "false"], obj=project, strict=True)
+    pdm(["add", "first"], obj=project, strict=True)
+    r = pdm(["list", "--freeze"], obj=project)
     assert "first==2.0.2" in r.output
```

### Comparing `pdm-2.5.6/tests/test_plugin.py` & `pdm-2.6.0/tests/test_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from unittest import mock
 
+import pytest
+
 from pdm.cli.commands.base import BaseCommand
 from pdm.compat import importlib_metadata
 from pdm.project.config import ConfigItem
+from pdm.utils import cd
 
 
 class HelloCommand(BaseCommand):
     def add_arguments(self, parser) -> None:
         parser.add_argument("-n", "--name", help="The person's name")
 
     def handle(self, project, options) -> None:
@@ -30,74 +33,86 @@
 
 def make_entry_point(plugin):
     ret = mock.Mock()
     ret.load.return_value = plugin
     return ret
 
 
-def test_plugin_new_command(invoke, mocker, project, core):
+def test_plugin_new_command(pdm, mocker, project, core):
     mocker.patch.object(
         importlib_metadata,
         "entry_points",
         return_value=[make_entry_point(new_command)],
     )
     core.init_parser()
     core.load_plugins()
-    result = invoke(["--help"], obj=project)
+    result = pdm(["--help"], obj=project)
     assert "hello" in result.output
 
-    result = invoke(["hello"], obj=project)
+    result = pdm(["hello"], obj=project)
     assert result.output.strip() == "Hello world"
 
-    result = invoke(["hello", "-n", "Frost"], obj=project)
+    result = pdm(["hello", "-n", "Frost"], obj=project)
     assert result.output.strip() == "Hello, Frost"
 
 
-def test_plugin_replace_command(invoke, mocker, project, core):
+def test_plugin_replace_command(pdm, mocker, project, core):
     mocker.patch.object(
         importlib_metadata,
         "entry_points",
         return_value=[make_entry_point(replace_command)],
     )
     core.init_parser()
     core.load_plugins()
 
-    result = invoke(["info"], obj=project)
+    result = pdm(["info"], obj=project)
     assert result.output.strip() == "Hello world"
 
-    result = invoke(["info", "-n", "Frost"], obj=project)
+    result = pdm(["info", "-n", "Frost"], obj=project)
     assert result.output.strip() == "Hello, Frost"
 
 
-def test_load_multiple_plugings(invoke, mocker, core):
+def test_load_multiple_plugings(pdm, mocker, core):
     mocker.patch.object(
         importlib_metadata,
         "entry_points",
         return_value=[make_entry_point(new_command), make_entry_point(add_new_config)],
     )
     core.init_parser()
     core.load_plugins()
 
-    result = invoke(["hello"])
+    result = pdm(["hello"])
     assert result.output.strip() == "Hello world", result.outputs
 
-    result = invoke(["config", "foo"])
+    result = pdm(["config", "foo"])
     assert result.output.strip() == "bar"
 
 
-def test_old_entry_point_compatibility(invoke, mocker, core):
+def test_old_entry_point_compatibility(pdm, mocker, core):
     def get_entry_points(group):
         if group == "pdm":
             return [make_entry_point(new_command)]
         if group == "pdm.plugin":
             return [make_entry_point(add_new_config)]
         return []
 
     mocker.patch.object(importlib_metadata, "entry_points", side_effect=get_entry_points)
     core.init_parser()
     core.load_plugins()
 
-    result = invoke(["hello"])
+    result = pdm(["hello"])
     assert result.output.strip() == "Hello world"
 
-    result = invoke(["config", "foo"])
+    result = pdm(["config", "foo"])
     assert result.output.strip() == "bar"
+
+
+@pytest.mark.usefixtures("local_finder")
+def test_project_plugin_library(pdm, project, core):
+    project.pyproject.settings["plugins"] = ["pdm-hello"]
+    pdm(["install", "--plugins"], obj=project, strict=True)
+    assert project.root.joinpath(".pdm-plugins").exists()
+    assert "pdm-hello" not in project.environment.get_working_set()
+    with cd(project.root):
+        core.load_plugins()
+        result = pdm(["hello", "Frost"], strict=True)
+    assert result.stdout.strip() == "Hello, Frost!"
```

### Comparing `pdm-2.5.6/tests/test_project.py` & `pdm-2.6.0/tests/test_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import sys
 import venv
 from pathlib import Path
 
 import pytest
 from packaging.version import parse
+from pytest_httpserver import HTTPServer
 
-from pdm.cli.commands.venv.utils import get_venv_python
 from pdm.environments import PythonEnvironment
 from pdm.exceptions import PdmException
+from pdm.models.venv import get_venv_python
 from pdm.utils import cd
 
 
 def test_project_python_with_pyenv_support(project, mocker, monkeypatch):
     project._saved_python = None
     project._python = None
     monkeypatch.setenv("PDM_IGNORE_SAVED_PYTHON", "1")
@@ -184,73 +185,76 @@
 def test_set_non_exist_python_path(project_no_init):
     project_no_init._saved_python = "non-exist-python"
     project_no_init._python = None
     assert project_no_init.python.executable.name != "non-exist-python"
 
 
 @pytest.mark.usefixtures("venv_backends")
-def test_create_venv_first_time(invoke, project, local_finder):
+def test_create_venv_first_time(pdm, project, local_finder):
     project.project_config.update({"venv.in_project": False})
     project._saved_python = None
-    result = invoke(["install"], obj=project)
+    result = pdm(["install"], obj=project)
     assert result.exit_code == 0
     venv_parent = project.root / "venvs"
     venv_path = next(venv_parent.iterdir(), None)
     assert venv_path is not None
 
     assert Path(project._saved_python).relative_to(venv_path)
 
 
 @pytest.mark.usefixtures("venv_backends", "local_finder")
 @pytest.mark.parametrize("with_pip", [True, False])
-def test_create_venv_in_project(invoke, project, with_pip):
+def test_create_venv_in_project(pdm, project, with_pip):
     project.project_config.update({"venv.in_project": True, "venv.with_pip": with_pip})
     project._saved_python = None
-    result = invoke(["install"], obj=project)
+    result = pdm(["install"], obj=project)
     assert result.exit_code == 0
     assert project.root.joinpath(".venv").exists()
     working_set = project.environment.get_working_set()
     assert ("pip" in working_set) is with_pip
 
 
 @pytest.mark.usefixtures("venv_backends")
-def test_find_interpreters_from_venv(invoke, project, local_finder):
+def test_find_interpreters_from_venv(pdm, project, local_finder):
     project.project_config.update({"venv.in_project": False})
     project._saved_python = None
-    result = invoke(["install"], obj=project)
+    result = pdm(["install"], obj=project)
     assert result.exit_code == 0
     venv_parent = project.root / "venvs"
     venv_path = next(venv_parent.iterdir(), None)
     venv_python = get_venv_python(venv_path)
 
     assert any(venv_python == p.executable for p in project.find_interpreters())
 
 
 @pytest.mark.usefixtures("local_finder")
-def test_find_interpreters_without_duplicate_relative_paths(invoke, project):
+def test_find_interpreters_without_duplicate_relative_paths(pdm, project):
     project._saved_python = None
     venv.create(project.root / ".venv", clear=True)
     with cd(project.root):
         bin_dir = "Scripts" if os.name == "nt" else "bin"
         suffix = ".exe" if os.name == "nt" else ""
         found = list(project.find_interpreters(f".venv/{bin_dir}/python{suffix}"))
         assert len(found) == 1
 
 
 def test_iter_project_venvs(project):
-    from pdm.cli.commands.venv import utils
+    from pdm.cli.commands.venv.utils import get_venv_prefix, iter_venvs
+    from pdm.models.venv import get_venv_python
 
     venv_parent = Path(project.config["venv.location"])
-    venv_prefix = utils.get_venv_prefix(project)
+    venv_prefix = get_venv_prefix(project)
     for name in ("foo", "bar", "baz"):
-        venv_parent.joinpath(venv_prefix + name).mkdir(parents=True)
-    dot_venv_python = utils.get_venv_python(project.root / ".venv")
+        venv_python = get_venv_python(venv_parent / (venv_prefix + name))
+        venv_python.parent.mkdir(parents=True)
+        venv_python.touch()
+    dot_venv_python = get_venv_python(project.root / ".venv")
     dot_venv_python.parent.mkdir(parents=True)
     dot_venv_python.touch()
-    venv_keys = [key for key, _ in utils.iter_venvs(project)]
+    venv_keys = [key for key, _ in iter_venvs(project)]
     assert sorted(venv_keys) == ["bar", "baz", "foo", "in-project"]
 
 
 def test_load_extra_sources(project):
     project.pyproject.settings["source"] = [
         {
             "name": "custom",
@@ -271,27 +275,28 @@
 def test_no_index_raise_error(project):
     project.global_config["pypi.ignore_stored_index"] = True
     with pytest.raises(PdmException, match="You must specify at least one index"):
         with project.environment.get_finder():
             pass
 
 
-@pytest.mark.network
-def test_access_index_with_auth(project):
-    url = "https://httpbin.org/basic-auth/foo/bar"
+def test_access_index_with_auth(project, httpserver: HTTPServer):
+    httpserver.expect_request(
+        "/simple/my-package", method="GET", headers={"Authorization": "Basic Zm9vOmJhcg=="}
+    ).respond_with_data("OK")
     project.global_config.update(
         {
-            "pypi.extra.url": "https://httpbin.org",
+            "pypi.extra.url": httpserver.url_for("/simple"),
             "pypi.extra.username": "foo",
             "pypi.extra.password": "bar",
         }
     )
     with project.environment.get_finder() as finder:
         session = finder.session
-        resp = session.get(url)
+        resp = session.get(httpserver.url_for("/simple/my-package"))
         assert resp.ok
 
 
 def test_configured_source_overwriting(project):
     project.pyproject.settings["source"] = [
         {
             "name": "custom",
```

### Comparing `pdm-2.5.6/tests/test_signals.py` & `pdm-2.6.0/tests/test_signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest import mock
 
 import pytest
 
 from pdm import signals
 
 
-def test_post_init_signal(project_no_init, invoke):
+def test_post_init_signal(project_no_init, pdm):
     mock_handler = mock.Mock()
     with signals.post_init.connected_to(mock_handler):
-        result = invoke(["init"], input="\n\n\n\n\n\n", obj=project_no_init)
+        result = pdm(["init"], input="\n\n\n\n\n\n", obj=project_no_init)
         assert result.exit_code == 0
     mock_handler.assert_called_once_with(project_no_init, hooks=mock.ANY)
 
 
 @pytest.mark.usefixtures("working_set")
 def test_post_lock_and_install_signals(project, pdm):
     pre_lock = signals.pre_lock.connect(mock.Mock(), weak=False)
```

### Comparing `pdm-2.5.6/tests/test_utils.py` & `pdm-2.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.6/PKG-INFO` & `pdm-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.5.6
+Version: 2.6.0
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.5.6 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.6.0 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

