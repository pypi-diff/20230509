# Comparing `tmp/pontos-23.5.0.tar.gz` & `tmp/pontos-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.5.0.tar", max compression
+gzip compressed data, was "pontos-23.5.1.tar", max compression
```

## Comparing `pontos-23.5.0.tar` & `pontos-23.5.1.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-05-04 07:27:17.318049 pontos-23.5.0/LICENSE
--rw-r--r--   0        0        0     3836 2023-05-04 07:27:17.318049 pontos-23.5.0/README.md
--rw-r--r--   0        0        0    97083 2023-05-04 07:27:17.322049 pontos-23.5.0/poetry.lock
--rw-r--r--   0        0        0       32 2023-05-04 07:27:17.322049 pontos-23.5.0/poetry.toml
--rw-r--r--   0        0        0      791 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-05-04 07:27:17.322049 pontos-23.5.0/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-05-04 07:27:17.326050 pontos-23.5.0/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/release/parser.py
--rw-r--r--   0        0        0    13491 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-05-04 07:27:17.330050 pontos-23.5.0/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-05-04 07:27:17.330050 pontos-23.5.0/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-05-04 07:27:17.330050 pontos-23.5.0/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.330050 pontos-23.5.0/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.334050 pontos-23.5.0/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/release/test_parser.py
--rw-r--r--   0        0        0    81080 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-05-04 07:27:17.338050 pontos-23.5.0/tests/version/test_version.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-09 06:59:43.236978 pontos-23.5.1/LICENSE
+-rw-r--r--   0        0        0     3836 2023-05-09 06:59:43.236978 pontos-23.5.1/README.md
+-rw-r--r--   0        0        0    97053 2023-05-09 06:59:43.240978 pontos-23.5.1/poetry.lock
+-rw-r--r--   0        0        0       32 2023-05-09 06:59:43.240978 pontos-23.5.1/poetry.toml
+-rw-r--r--   0        0        0      791 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/parser.py
+-rw-r--r--   0        0        0    14408 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-05-09 06:59:43.248978 pontos-23.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_version.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.5.1/PKG-INFO
```

### Comparing `pontos-23.5.0/LICENSE` & `pontos-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/README.md` & `pontos-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/poetry.lock` & `pontos-23.5.1/poetry.lock`

 * *Files 1% similar despite different names*

```diff
@@ -197,22 +197,22 @@
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "certifi"
-version = "2022.12.7"
+version = "2023.5.7"
 description = "Python package for providing Mozilla's CA Bundle."
 category = "main"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "certifi-2022.12.7-py3-none-any.whl", hash = "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"},
-    {file = "certifi-2022.12.7.tar.gz", hash = "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3"},
+    {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
+    {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
 ]
 
 [[package]]
 name = "charset-normalizer"
 version = "3.1.0"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
 category = "dev"
@@ -909,22 +909,22 @@
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pylint"
-version = "2.17.3"
+version = "2.17.4"
 description = "python code static checker"
 category = "dev"
 optional = false
 python-versions = ">=3.7.2"
 files = [
-    {file = "pylint-2.17.3-py3-none-any.whl", hash = "sha256:a6cbb4c6e96eab4a3c7de7c6383c512478f58f88d95764507d84c899d656a89a"},
-    {file = "pylint-2.17.3.tar.gz", hash = "sha256:761907349e699f8afdcd56c4fe02f3021ab5b3a0fc26d19a9bfdc66c7d0d5cd5"},
+    {file = "pylint-2.17.4-py3-none-any.whl", hash = "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"},
+    {file = "pylint-2.17.4.tar.gz", hash = "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1"},
 ]
 
 [package.dependencies]
 astroid = ">=2.15.4,<=2.17.0-dev0"
 colorama = {version = ">=0.4.5", markers = "sys_platform == \"win32\""}
 dill = [
     {version = ">=0.2", markers = "python_version < \"3.11\""},
@@ -1027,29 +1027,29 @@
     {file = "PyYAML-6.0-cp39-cp39-win32.whl", hash = "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb"},
     {file = "PyYAML-6.0-cp39-cp39-win_amd64.whl", hash = "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c"},
     {file = "PyYAML-6.0.tar.gz", hash = "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2"},
 ]
 
 [[package]]
 name = "requests"
-version = "2.29.0"
+version = "2.30.0"
 description = "Python HTTP for Humans."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "requests-2.29.0-py3-none-any.whl", hash = "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b"},
-    {file = "requests-2.29.0.tar.gz", hash = "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"},
+    {file = "requests-2.30.0-py3-none-any.whl", hash = "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294"},
+    {file = "requests-2.30.0.tar.gz", hash = "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"},
 ]
 
 [package.dependencies]
 certifi = ">=2017.4.17"
 charset-normalizer = ">=2,<4"
 idna = ">=2.5,<4"
-urllib3 = ">=1.21.1,<1.27"
+urllib3 = ">=1.21.1,<3"
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
 name = "rich"
@@ -1068,29 +1068,29 @@
 pygments = ">=2.13.0,<3.0.0"
 
 [package.extras]
 jupyter = ["ipywidgets (>=7.5.1,<9)"]
 
 [[package]]
 name = "rope"
-version = "1.7.0"
+version = "1.8.0"
 description = "a python refactoring library..."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "rope-1.7.0-py3-none-any.whl", hash = "sha256:893dd80ba7077fc9f6f42b0a849372076b70f1d6e405b9f0cc52781ffa0e6890"},
-    {file = "rope-1.7.0.tar.gz", hash = "sha256:ba39581d0f8dee4ae8b5b5e82e35d03cebad965ccb127b7eaab9755cdc85e85a"},
+    {file = "rope-1.8.0-py3-none-any.whl", hash = "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd"},
+    {file = "rope-1.8.0.tar.gz", hash = "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"},
 ]
 
 [package.dependencies]
 pytoolconfig = {version = ">=1.2.2", extras = ["global"]}
 
 [package.extras]
-dev = ["build (>=0.7.0)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)"]
+dev = ["build (>=0.7.0)", "pip-tools (>=6.12.1)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)", "toml (>=0.10.2)"]
 doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
 
 [[package]]
 name = "semver"
 version = "3.0.0"
 description = "Python helper for Semantic Versioning (https://semver.org)"
 category = "main"
@@ -1373,28 +1373,29 @@
 files = [
     {file = "typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
     {file = "typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
 
 [[package]]
 name = "urllib3"
-version = "1.26.15"
+version = "2.0.2"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 category = "dev"
 optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*"
+python-versions = ">=3.7"
 files = [
-    {file = "urllib3-1.26.15-py2.py3-none-any.whl", hash = "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"},
-    {file = "urllib3-1.26.15.tar.gz", hash = "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305"},
+    {file = "urllib3-2.0.2-py3-none-any.whl", hash = "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"},
+    {file = "urllib3-2.0.2.tar.gz", hash = "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc"},
 ]
 
 [package.extras]
-brotli = ["brotli (>=1.0.9)", "brotlicffi (>=0.8.0)", "brotlipy (>=0.6.0)"]
-secure = ["certifi", "cryptography (>=1.3.4)", "idna (>=2.0.0)", "ipaddress", "pyOpenSSL (>=0.14)", "urllib3-secure-extra"]
-socks = ["PySocks (>=1.5.6,!=1.5.7,<2.0)"]
+brotli = ["brotli (>=1.0.9)", "brotlicffi (>=0.8.0)"]
+secure = ["certifi", "cryptography (>=1.9)", "idna (>=2.0.0)", "pyopenssl (>=17.1.0)", "urllib3-secure-extra"]
+socks = ["pysocks (>=1.5.6,!=1.5.7,<2.0)"]
+zstd = ["zstandard (>=0.18.0)"]
 
 [[package]]
 name = "wrapt"
 version = "1.15.0"
 description = "Module for decorators, wrappers and monkey patching."
 category = "dev"
 optional = false
@@ -1492,8 +1493,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "3a6fb4535ecb820025e59c291d720d5895770603d1fd3fc52d3c83359fe3ca35"
+content-hash = "64b657301d020637ad10adf1db862bc58f7c22064164c63e51a23ccfcfec57c2"
```

### Comparing `pontos-23.5.0/pontos/__init__.py` & `pontos-23.5.1/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/changelog/__init__.py` & `pontos-23.5.1/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/changelog/conventional_commits.py` & `pontos-23.5.1/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/changelog/errors.py` & `pontos-23.5.1/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/changelog/main.py` & `pontos-23.5.1/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/errors.py` & `pontos-23.5.1/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/git/__init__.py` & `pontos-23.5.1/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/git/git.py` & `pontos-23.5.1/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/git/status.py` & `pontos-23.5.1/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/__init__.py` & `pontos-23.5.1/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/__init__.py` & `pontos-23.5.1/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/argparser.py` & `pontos-23.5.1/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/cmds.py` & `pontos-23.5.1/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/core.py` & `pontos-23.5.1/pontos/github/actions/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import contextlib
 import os
+from contextlib import contextmanager
+from io import TextIOWrapper
 from pathlib import Path
-from typing import Optional
+from typing import Generator, Optional
 
 from pontos.github.actions.errors import GitHubActionsError
 
 
 def _to_options(
     name: Optional[str] = None,
     line: Optional[str] = None,
@@ -64,15 +65,15 @@
 
 class Console:
     """
     Class for printing messages to the action console
     """
 
     @classmethod
-    @contextlib.contextmanager
+    @contextmanager
     def group(cls, title: str):
         """
         ContextManager to display a foldable group
 
         Args:
             title: Title of the group
         """
@@ -195,16 +196,58 @@
 
         These messages are only shown if the secret ACTIONS_STEP_DEBUG is set to true.
         See https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/enabling-debug-logging#enabling-step-debug-logging
         """
         print(f"::debug::{message}")
 
 
+class ActionOutput:
+    def __init__(self, file: TextIOWrapper) -> None:
+        self._file = file
+
+    def write(self, name: str, value: str):
+        """
+        Set action output
+
+        An action output can be consumed by another job
+
+        Args:
+            name: Name of the output variable
+            value: Value of the output variable
+        """
+        self._file.write(f"{name}={value}\n")
+
+
 class ActionIO:
     @staticmethod
+    def has_output() -> bool:
+        """
+        Check if GITHUB_OUTPUT is set
+        """
+        return "GITHUB_OUTPUT" in os.environ
+
+    @staticmethod
+    @contextmanager
+    def out() -> Generator[ActionOutput, None, None]:
+        """
+        Create action output
+
+        An action output can be consumed by another job
+        """
+        output_filename = os.environ.get("GITHUB_OUTPUT")
+        if not output_filename:
+            raise GitHubActionsError(
+                "GITHUB_OUTPUT environment variable not set. Can't write "
+                "action output."
+            )
+
+        with Path(output_filename).open("a", encoding="utf8") as f:
+            yield ActionOutput(f)
+
+    @staticmethod
     def output(name: str, value: str):
         """
         Set action output
 
         An action output can be consumed by another job
 
         Args:
```

### Comparing `pontos-23.5.0/pontos/github/actions/env.py` & `pontos-23.5.1/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/errors.py` & `pontos-23.5.1/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/event.py` & `pontos-23.5.1/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/actions/main.py` & `pontos-23.5.1/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/__init__.py` & `pontos-23.5.1/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/api.py` & `pontos-23.5.1/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/artifacts.py` & `pontos-23.5.1/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/branch.py` & `pontos-23.5.1/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/client.py` & `pontos-23.5.1/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/contents.py` & `pontos-23.5.1/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/errors.py` & `pontos-23.5.1/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/helper.py` & `pontos-23.5.1/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/labels.py` & `pontos-23.5.1/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/organizations.py` & `pontos-23.5.1/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/pull_requests.py` & `pontos-23.5.1/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/release.py` & `pontos-23.5.1/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/repositories.py` & `pontos-23.5.1/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/search.py` & `pontos-23.5.1/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/tags.py` & `pontos-23.5.1/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/teams.py` & `pontos-23.5.1/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/api/workflows.py` & `pontos-23.5.1/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/argparser.py` & `pontos-23.5.1/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/cmds.py` & `pontos-23.5.1/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/main.py` & `pontos-23.5.1/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/__init__.py` & `pontos-23.5.1/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/artifact.py` & `pontos-23.5.1/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/base.py` & `pontos-23.5.1/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/branch.py` & `pontos-23.5.1/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/organization.py` & `pontos-23.5.1/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/pull_request.py` & `pontos-23.5.1/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/release.py` & `pontos-23.5.1/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/search.py` & `pontos-23.5.1/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/tag.py` & `pontos-23.5.1/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/models/workflow.py` & `pontos-23.5.1/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/pr_template.md` & `pontos-23.5.1/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/script/__init__.py` & `pontos-23.5.1/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/script/errors.py` & `pontos-23.5.1/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/script/load.py` & `pontos-23.5.1/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/github/script/parser.py` & `pontos-23.5.1/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/helper.py` & `pontos-23.5.1/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/models/__init__.py` & `pontos-23.5.1/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/__init__.py` & `pontos-23.5.1/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/api.py` & `pontos-23.5.1/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/cpe/__init__.py` & `pontos-23.5.1/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/cpe/api.py` & `pontos-23.5.1/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/cve/__init__.py` & `pontos-23.5.1/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/cve/api.py` & `pontos-23.5.1/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/models/__init__.py` & `pontos-23.5.1/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/models/cpe.py` & `pontos-23.5.1/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/models/cve.py` & `pontos-23.5.1/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/models/cvss_v2.py` & `pontos-23.5.1/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/nvd/models/cvss_v3.py` & `pontos-23.5.1/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/pontos.py` & `pontos-23.5.1/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/release/__init__.py` & `pontos-23.5.1/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/release/helper.py` & `pontos-23.5.1/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/release/main.py` & `pontos-23.5.1/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/release/parser.py` & `pontos-23.5.1/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/release/release.py` & `pontos-23.5.1/pontos/release/release.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,33 +14,50 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import asyncio
 from argparse import Namespace
+from dataclasses import dataclass
 from enum import IntEnum, auto
 from pathlib import Path
 from typing import Optional
 
 import httpx
 
 from pontos.changelog.conventional_commits import ChangelogBuilder
 from pontos.errors import PontosError
 from pontos.git import Git
+from pontos.github.actions.core import ActionIO
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.terminal import Terminal
 from pontos.version import Version, VersionCalculator, VersionError
 from pontos.version.helper import get_last_release_version
 from pontos.version.project import Project
 from pontos.version.schemes import VersioningScheme
 
 from .helper import ReleaseType, find_signing_key, get_git_repository_name
 
 
+@dataclass
+class ReleaseInformation:
+    last_release_version: Version
+    release_version: Version
+    git_release_tag: str
+    next_version: Version
+
+    def write_github_output(self):
+        with ActionIO.out() as output:
+            output.write("last-release-version", self.last_release_version)
+            output.write("release-version", self.release_version)
+            output.write("git-release-tag", self.git_release_tag)
+            output.write("next-version", self.next_version)
+
+
 class ReleaseReturnValue(IntEnum):
     """
     Possible return values of ReleaseCommand
     """
 
     SUCCESS = 0
     PROJECT_SETTINGS_NOT_FOUND = auto()
@@ -341,14 +358,23 @@
                 commit_msg, verify=False, gpg_signing_key=git_signing_key
             )
 
         if not local:
             self.terminal.info("Pushing changes")
             self.git.push(follow_tags=True, remote=git_remote_name)
 
+        self.release_information = ReleaseInformation(
+            last_release_version=last_release_version,
+            release_version=release_version,
+            git_release_tag=git_version,
+            next_version=next_version,
+        )
+        if ActionIO.has_output():
+            self.release_information.write_github_output()
+
         return ReleaseReturnValue.SUCCESS
 
 
 def release(
     terminal: Terminal,
     args: Namespace,
     *,
```

### Comparing `pontos-23.5.0/pontos/release/sign.py` & `pontos-23.5.1/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/terminal/__init__.py` & `pontos-23.5.1/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/terminal/null.py` & `pontos-23.5.1/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/terminal/rich.py` & `pontos-23.5.1/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/terminal/terminal.py` & `pontos-23.5.1/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/testing/__init__.py` & `pontos-23.5.1/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/updateheader/__init__.py` & `pontos-23.5.1/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/updateheader/__main__.py` & `pontos-23.5.1/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/updateheader/updateheader.py` & `pontos-23.5.1/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/__init__.py` & `pontos-23.5.1/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/__main__.py` & `pontos-23.5.1/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/_calculator.py` & `pontos-23.5.1/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/__init__.py` & `pontos-23.5.1/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/_cargo.py` & `pontos-23.5.1/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/_cmake.py` & `pontos-23.5.1/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/_command.py` & `pontos-23.5.1/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/_go.py` & `pontos-23.5.1/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/_javascript.py` & `pontos-23.5.1/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/commands/_python.py` & `pontos-23.5.1/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/errors.py` & `pontos-23.5.1/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/helper.py` & `pontos-23.5.1/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/main.py` & `pontos-23.5.1/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/parser.py` & `pontos-23.5.1/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/project.py` & `pontos-23.5.1/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/schemes/__init__.py` & `pontos-23.5.1/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/schemes/_pep440.py` & `pontos-23.5.1/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/schemes/_scheme.py` & `pontos-23.5.1/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/schemes/_semantic.py` & `pontos-23.5.1/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pontos/version/version.py` & `pontos-23.5.1/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/pyproject.toml` & `pontos-23.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.5.0"
+version = "23.5.1"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -46,15 +46,15 @@
 semver = ">=2.13,<4.0"
 
 [tool.poetry.dev-dependencies]
 autohooks = ">=22.7.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-isort = ">=22.3.0"
-rope = "^1.7.0"
+rope = "^1.8.0"
 coverage = "^7.2"
 myst-parser = ">=0.19.1"
 Sphinx = "^6.2.1"
 furo = "^2023.3.27"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.black]
```

### Comparing `pontos-23.5.0/scripts/github/artifacts-download.py` & `pontos-23.5.1/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/artifacts.py` & `pontos-23.5.1/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/branchprotection.py` & `pontos-23.5.1/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/create-repository.py` & `pontos-23.5.1/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/enforce-admins.py` & `pontos-23.5.1/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/lock-branch.py` & `pontos-23.5.1/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/members.py` & `pontos-23.5.1/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/release-assets-download.py` & `pontos-23.5.1/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/repositories.py` & `pontos-23.5.1/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/search-repositories.py` & `pontos-23.5.1/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/team-repositories.py` & `pontos-23.5.1/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/teams.py` & `pontos-23.5.1/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/scripts/github/workflow-runs.py` & `pontos-23.5.1/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/__init__.py` & `pontos-23.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/changelog/__init__.py` & `pontos-23.5.1/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/changelog/test_conventional_commits.py` & `pontos-23.5.1/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/changelog/test_parser.py` & `pontos-23.5.1/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/git/__init__.py` & `pontos-23.5.1/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/git/test_git.py` & `pontos-23.5.1/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/git/test_status.py` & `pontos-23.5.1/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/__init__.py` & `pontos-23.5.1/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/actions/__init__.py` & `pontos-23.5.1/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/actions/test-pull-request-event.json` & `pontos-23.5.1/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/actions/test_core.py` & `pontos-23.5.1/tests/github/actions/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -115,18 +115,49 @@
                 ActionIO.output("foo", "bar")
                 ActionIO.output("lorem", "ipsum")
 
                 output = file_path.read_text(encoding="utf8")
 
                 self.assertEqual(output, "foo=bar\nlorem=ipsum\n")
 
+    @patch.dict("os.environ", {}, clear=True)
     def test_output_no_env(self):
-        with patch.dict("os.environ", {}, clear=True), self.assertRaises(
-            GitHubActionsError
-        ):
+        with self.assertRaises(GitHubActionsError):
             ActionIO.output("foo", "bar")
 
+    @patch.dict("os.environ", {"GITHUB_OUTPUT": ""}, clear=True)
     def test_output_empty_env(self):
-        with patch.dict(
-            "os.environ", {"GITHUB_OUTPUT": ""}, clear=True
-        ), self.assertRaises(GitHubActionsError):
+        with self.assertRaises(GitHubActionsError):
             ActionIO.output("foo", "bar")
+
+    @patch.dict("os.environ", {}, clear=True)
+    def test_no_github_output(self):
+        self.assertFalse(ActionIO.has_output())
+
+    @patch.dict(
+        "os.environ", {"GITHUB_OUTPUT": "/foo/github.output"}, clear=True
+    )
+    def test_has_github_output(self):
+        self.assertTrue(ActionIO.has_output())
+
+    def test_out(self):
+        with temp_directory() as temp_dir:
+            outfile = temp_dir / "github.output"
+            with patch.dict(
+                "os.environ",
+                {"GITHUB_OUTPUT": str(outfile.absolute())},
+                clear=True,
+            ):
+                with ActionIO.out() as output:
+                    output.write("foo", "bar")
+
+            self.assertEqual(outfile.read_text(encoding="utf8"), "foo=bar\n")
+
+    @patch.dict("os.environ", {}, clear=True)
+    def test_out_failure(self):
+        with self.assertRaisesRegex(
+            GitHubActionsError,
+            "GITHUB_OUTPUT environment variable not set. Can't write "
+            "action output.",
+        ):
+            with ActionIO.out():
+                pass
```

### Comparing `pontos-23.5.0/tests/github/actions/test_env.py` & `pontos-23.5.1/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/actions/test_event.py` & `pontos-23.5.1/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/__init__.py` & `pontos-23.5.1/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/pr-files.json` & `pontos-23.5.1/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/release-response.json` & `pontos-23.5.1/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_artifacts.py` & `pontos-23.5.1/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_branch.py` & `pontos-23.5.1/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_client.py` & `pontos-23.5.1/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_contents.py` & `pontos-23.5.1/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_labels.py` & `pontos-23.5.1/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_organizations.py` & `pontos-23.5.1/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_pull_requests.py` & `pontos-23.5.1/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_release.py` & `pontos-23.5.1/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_repositories.py` & `pontos-23.5.1/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_search.py` & `pontos-23.5.1/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_tags.py` & `pontos-23.5.1/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_teams.py` & `pontos-23.5.1/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/api/test_workflows.py` & `pontos-23.5.1/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/__init__.py` & `pontos-23.5.1/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_artifact.py` & `pontos-23.5.1/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_base.py` & `pontos-23.5.1/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_branch.py` & `pontos-23.5.1/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_organization.py` & `pontos-23.5.1/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_pull_request.py` & `pontos-23.5.1/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_release.py` & `pontos-23.5.1/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_search.py` & `pontos-23.5.1/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_tag.py` & `pontos-23.5.1/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/models/test_workflow.py` & `pontos-23.5.1/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/script/__init__.py` & `pontos-23.5.1/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/script/test_load.py` & `pontos-23.5.1/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/script/test_parser.py` & `pontos-23.5.1/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/test_argparser.py` & `pontos-23.5.1/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/github/test_cmds.py` & `pontos-23.5.1/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/models/__init__.py` & `pontos-23.5.1/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/models/test_models.py` & `pontos-23.5.1/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/__init__.py` & `pontos-23.5.1/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/cpe/__init__.py` & `pontos-23.5.1/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/cpe/test_api.py` & `pontos-23.5.1/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/cve/__init__.py` & `pontos-23.5.1/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/cve/test_api.py` & `pontos-23.5.1/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/models/__init__.py` & `pontos-23.5.1/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/models/test_cpe.py` & `pontos-23.5.1/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/models/test_cve.py` & `pontos-23.5.1/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/nvd/test_api.py` & `pontos-23.5.1/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/release/__init__.py` & `pontos-23.5.1/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/release/test_helper.py` & `pontos-23.5.1/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/release/test_parser.py` & `pontos-23.5.1/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/release/test_release.py` & `pontos-23.5.1/tests/release/test_release.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,23 @@
 from typing import Iterable, Optional, Union
 from unittest.mock import AsyncMock, MagicMock, call, patch
 
 from httpx import HTTPStatusError, Request, Response
 
 from pontos.git.git import ConfigScope, Git
 from pontos.git.status import StatusEntry
+from pontos.github.actions.errors import GitHubActionsError
 from pontos.release.main import parse_args
-from pontos.release.release import ReleaseReturnValue, release
+from pontos.release.release import (
+    ReleaseInformation,
+    ReleaseReturnValue,
+    release,
+)
 from pontos.terminal.terminal import Terminal
-from pontos.testing import temp_git_repository
+from pontos.testing import temp_directory, temp_git_repository
 from pontos.version import VersionError, VersionUpdate
 from pontos.version.commands import GoVersionCommand
 from pontos.version.schemes._pep440 import PEP440Version, PEP440VersioningScheme
 
 
 def mock_terminal() -> MagicMock:
     return MagicMock(spec=Terminal)
@@ -72,14 +77,76 @@
         if tags:
             for tag in str_or_list(tags):
                 git.tag(f"v{tag}")
 
         yield tmp_git
 
 
+class ReleaseInformationTestCase(unittest.TestCase):
+    def test_release_info(self):
+        release_info = ReleaseInformation(
+            last_release_version=PEP440Version.from_string("1.2.3"),
+            release_version=PEP440Version.from_string("2.0.0"),
+            git_release_tag="v2.0.0",
+            next_version=PEP440Version.from_string("2.0.1.dev1"),
+        )
+
+        self.assertEqual(
+            release_info.last_release_version,
+            PEP440Version.from_string("1.2.3"),
+        )
+        self.assertEqual(
+            release_info.release_version, PEP440Version.from_string("2.0.0")
+        )
+        self.assertEqual(release_info.git_release_tag, "v2.0.0")
+        self.assertEqual(
+            release_info.next_version, PEP440Version.from_string("2.0.1.dev1")
+        )
+
+    @patch.dict("os.environ", {}, clear=True)
+    def test_no_github_output(self):
+        release_info = ReleaseInformation(
+            last_release_version=PEP440Version.from_string("1.2.3"),
+            release_version=PEP440Version.from_string("2.0.0"),
+            git_release_tag="v2.0.0",
+            next_version=PEP440Version.from_string("2.0.1.dev1"),
+        )
+
+        with self.assertRaisesRegex(
+            GitHubActionsError,
+            "GITHUB_OUTPUT environment variable not set. Can't write "
+            "action output.",
+        ):
+            release_info.write_github_output()
+
+    def test_github_output(self):
+        expected = """last-release-version=1.2.3
+release-version=2.0.0
+git-release-tag=v2.0.0
+next-version=2.0.1.dev1
+"""
+        with temp_directory() as temp_dir:
+            out_file = temp_dir / "out.txt"
+            with patch.dict(
+                "os.environ", {"GITHUB_OUTPUT": str(out_file.absolute())}
+            ):
+                release_info = ReleaseInformation(
+                    last_release_version=PEP440Version.from_string("1.2.3"),
+                    release_version=PEP440Version.from_string("2.0.0"),
+                    git_release_tag="v2.0.0",
+                    next_version=PEP440Version.from_string("2.0.1.dev1"),
+                )
+
+                release_info.write_github_output()
+
+            self.assertTrue(out_file.exists())
+            actual = out_file.read_text(encoding="utf8")
+            self.assertEqual(actual, expected)
+
+
 @patch.dict(
     "os.environ",
     {
         "GITHUB_TOKEN": "foo",
         "GITHUB_USER": "user",
         "GPG_SIGNING_KEY": "1234",
     },
```

### Comparing `pontos-23.5.0/tests/release/test_sign.py` & `pontos-23.5.1/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/terminal/__init__.py` & `pontos-23.5.1/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/terminal/test_terminal.py` & `pontos-23.5.1/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/test_helper.py` & `pontos-23.5.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/test_pontos.py` & `pontos-23.5.1/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/testing/__init__.py` & `pontos-23.5.1/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/testing/test_testing.py` & `pontos-23.5.1/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/updateheader/__init__.py` & `pontos-23.5.1/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/updateheader/test_header.py` & `pontos-23.5.1/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/__init__.py` & `pontos-23.5.1/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/commands/__init__.py` & `pontos-23.5.1/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/commands/test_cargo.py` & `pontos-23.5.1/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/commands/test_cmake.py` & `pontos-23.5.1/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/commands/test_go.py` & `pontos-23.5.1/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/commands/test_javascript.py` & `pontos-23.5.1/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/commands/test_python.py` & `pontos-23.5.1/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/schemes/__init__.py` & `pontos-23.5.1/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/schemes/test_pep440.py` & `pontos-23.5.1/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/schemes/test_semantic.py` & `pontos-23.5.1/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_commands.py` & `pontos-23.5.1/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_errors.py` & `pontos-23.5.1/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_helper.py` & `pontos-23.5.1/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_main.py` & `pontos-23.5.1/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_parser.py` & `pontos-23.5.1/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_project.py` & `pontos-23.5.1/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/tests/version/test_version.py` & `pontos-23.5.1/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.0/PKG-INFO` & `pontos-23.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.5.0
+Version: 23.5.1
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

