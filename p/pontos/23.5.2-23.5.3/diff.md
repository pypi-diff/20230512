# Comparing `tmp/pontos-23.5.2.tar.gz` & `tmp/pontos-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.5.2.tar", max compression
+gzip compressed data, was "pontos-23.5.3.tar", max compression
```

## Comparing `pontos-23.5.2.tar` & `pontos-23.5.3.tar`

### file list

```diff
@@ -1,251 +1,253 @@
--rw-r--r--   0        0        0    35149 2023-05-10 11:10:28.776647 pontos-23.5.2/LICENSE
--rw-r--r--   0        0        0     3836 2023-05-10 11:10:28.776647 pontos-23.5.2/README.md
--rw-r--r--   0        0        0    97053 2023-05-10 11:10:28.780647 pontos-23.5.2/poetry.lock
--rw-r--r--   0        0        0       32 2023-05-10 11:10:28.780647 pontos-23.5.2/poetry.toml
--rw-r--r--   0        0        0      791 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9995 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7327 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/parser.py
--rw-r--r--   0        0        0    14408 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-05-10 11:10:28.792646 pontos-23.5.2/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17925 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5430 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_version.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-12 07:33:16.578426 pontos-23.5.3/LICENSE
+-rw-r--r--   0        0        0     3836 2023-05-12 07:33:16.578426 pontos-23.5.3/README.md
+-rw-r--r--   0        0        0   109652 2023-05-12 07:33:16.582426 pontos-23.5.3/poetry.lock
+-rw-r--r--   0        0        0       32 2023-05-12 07:33:16.582426 pontos-23.5.3/poetry.toml
+-rw-r--r--   0        0        0      791 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9995 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-05-12 07:33:16.582426 pontos-23.5.3/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/release/parser.py
+-rw-r--r--   0        0        0    14408 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1596 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     4043 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_java.py
+-rw-r--r--   0        0        0     6263 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-05-12 07:33:16.586426 pontos-23.5.3/pontos/version/version.py
+-rw-r--r--   0        0        0     2911 2023-05-12 07:33:16.586426 pontos-23.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-05-12 07:33:16.586426 pontos-23.5.3/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17925 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.586426 pontos-23.5.3/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-05-12 07:33:16.590426 pontos-23.5.3/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0     8737 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/test_java.py
+-rw-r--r--   0        0        0    15376 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25664 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-05-12 07:33:16.594426 pontos-23.5.3/tests/version/test_version.py
+-rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 pontos-23.5.3/PKG-INFO
```

### Comparing `pontos-23.5.2/LICENSE` & `pontos-23.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/README.md` & `pontos-23.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/poetry.lock` & `pontos-23.5.3/poetry.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.4.0 and should not be changed by hand.
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 description = "A configurable sidebar-enabled Sphinx theme"
 category = "dev"
 optional = false
@@ -685,14 +685,107 @@
 ]
 
 [package.dependencies]
 six = "*"
 tornado = {version = "*", markers = "python_version > \"2.7\""}
 
 [[package]]
+name = "lxml"
+version = "4.9.2"
+description = "Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API."
+category = "main"
+optional = false
+python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*"
+files = [
+    {file = "lxml-4.9.2-cp27-cp27m-macosx_10_15_x86_64.whl", hash = "sha256:76cf573e5a365e790396a5cc2b909812633409306c6531a6877c59061e42c4f2"},
+    {file = "lxml-4.9.2-cp27-cp27m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b1f42b6921d0e81b1bcb5e395bc091a70f41c4d4e55ba99c6da2b31626c44892"},
+    {file = "lxml-4.9.2-cp27-cp27m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:9f102706d0ca011de571de32c3247c6476b55bb6bc65a20f682f000b07a4852a"},
+    {file = "lxml-4.9.2-cp27-cp27m-win32.whl", hash = "sha256:8d0b4612b66ff5d62d03bcaa043bb018f74dfea51184e53f067e6fdcba4bd8de"},
+    {file = "lxml-4.9.2-cp27-cp27m-win_amd64.whl", hash = "sha256:4c8f293f14abc8fd3e8e01c5bd86e6ed0b6ef71936ded5bf10fe7a5efefbaca3"},
+    {file = "lxml-4.9.2-cp27-cp27mu-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:2899456259589aa38bfb018c364d6ae7b53c5c22d8e27d0ec7609c2a1ff78b50"},
+    {file = "lxml-4.9.2-cp27-cp27mu-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:6749649eecd6a9871cae297bffa4ee76f90b4504a2a2ab528d9ebe912b101975"},
+    {file = "lxml-4.9.2-cp310-cp310-macosx_10_15_x86_64.whl", hash = "sha256:a08cff61517ee26cb56f1e949cca38caabe9ea9fbb4b1e10a805dc39844b7d5c"},
+    {file = "lxml-4.9.2-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:85cabf64adec449132e55616e7ca3e1000ab449d1d0f9d7f83146ed5bdcb6d8a"},
+    {file = "lxml-4.9.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:8340225bd5e7a701c0fa98284c849c9b9fc9238abf53a0ebd90900f25d39a4e4"},
+    {file = "lxml-4.9.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:1ab8f1f932e8f82355e75dda5413a57612c6ea448069d4fb2e217e9a4bed13d4"},
+    {file = "lxml-4.9.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:699a9af7dffaf67deeae27b2112aa06b41c370d5e7633e0ee0aea2e0b6c211f7"},
+    {file = "lxml-4.9.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b9cc34af337a97d470040f99ba4282f6e6bac88407d021688a5d585e44a23184"},
+    {file = "lxml-4.9.2-cp310-cp310-win32.whl", hash = "sha256:d02a5399126a53492415d4906ab0ad0375a5456cc05c3fc0fc4ca11771745cda"},
+    {file = "lxml-4.9.2-cp310-cp310-win_amd64.whl", hash = "sha256:a38486985ca49cfa574a507e7a2215c0c780fd1778bb6290c21193b7211702ab"},
+    {file = "lxml-4.9.2-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:c83203addf554215463b59f6399835201999b5e48019dc17f182ed5ad87205c9"},
+    {file = "lxml-4.9.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:2a87fa548561d2f4643c99cd13131acb607ddabb70682dcf1dff5f71f781a4bf"},
+    {file = "lxml-4.9.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:d6b430a9938a5a5d85fc107d852262ddcd48602c120e3dbb02137c83d212b380"},
+    {file = "lxml-4.9.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:3efea981d956a6f7173b4659849f55081867cf897e719f57383698af6f618a92"},
+    {file = "lxml-4.9.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:df0623dcf9668ad0445e0558a21211d4e9a149ea8f5666917c8eeec515f0a6d1"},
+    {file = "lxml-4.9.2-cp311-cp311-win32.whl", hash = "sha256:da248f93f0418a9e9d94b0080d7ebc407a9a5e6d0b57bb30db9b5cc28de1ad33"},
+    {file = "lxml-4.9.2-cp311-cp311-win_amd64.whl", hash = "sha256:3818b8e2c4b5148567e1b09ce739006acfaa44ce3156f8cbbc11062994b8e8dd"},
+    {file = "lxml-4.9.2-cp35-cp35m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:ca989b91cf3a3ba28930a9fc1e9aeafc2a395448641df1f387a2d394638943b0"},
+    {file = "lxml-4.9.2-cp35-cp35m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:822068f85e12a6e292803e112ab876bc03ed1f03dddb80154c395f891ca6b31e"},
+    {file = "lxml-4.9.2-cp35-cp35m-win32.whl", hash = "sha256:be7292c55101e22f2a3d4d8913944cbea71eea90792bf914add27454a13905df"},
+    {file = "lxml-4.9.2-cp35-cp35m-win_amd64.whl", hash = "sha256:998c7c41910666d2976928c38ea96a70d1aa43be6fe502f21a651e17483a43c5"},
+    {file = "lxml-4.9.2-cp36-cp36m-macosx_10_15_x86_64.whl", hash = "sha256:b26a29f0b7fc6f0897f043ca366142d2b609dc60756ee6e4e90b5f762c6adc53"},
+    {file = "lxml-4.9.2-cp36-cp36m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:ab323679b8b3030000f2be63e22cdeea5b47ee0abd2d6a1dc0c8103ddaa56cd7"},
+    {file = "lxml-4.9.2-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:689bb688a1db722485e4610a503e3e9210dcc20c520b45ac8f7533c837be76fe"},
+    {file = "lxml-4.9.2-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:f49e52d174375a7def9915c9f06ec4e569d235ad428f70751765f48d5926678c"},
+    {file = "lxml-4.9.2-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:36c3c175d34652a35475a73762b545f4527aec044910a651d2bf50de9c3352b1"},
+    {file = "lxml-4.9.2-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:a35f8b7fa99f90dd2f5dc5a9fa12332642f087a7641289ca6c40d6e1a2637d8e"},
+    {file = "lxml-4.9.2-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:58bfa3aa19ca4c0f28c5dde0ff56c520fbac6f0daf4fac66ed4c8d2fb7f22e74"},
+    {file = "lxml-4.9.2-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:bc718cd47b765e790eecb74d044cc8d37d58562f6c314ee9484df26276d36a38"},
+    {file = "lxml-4.9.2-cp36-cp36m-win32.whl", hash = "sha256:d5bf6545cd27aaa8a13033ce56354ed9e25ab0e4ac3b5392b763d8d04b08e0c5"},
+    {file = "lxml-4.9.2-cp36-cp36m-win_amd64.whl", hash = "sha256:3ab9fa9d6dc2a7f29d7affdf3edebf6ece6fb28a6d80b14c3b2fb9d39b9322c3"},
+    {file = "lxml-4.9.2-cp37-cp37m-macosx_10_15_x86_64.whl", hash = "sha256:05ca3f6abf5cf78fe053da9b1166e062ade3fa5d4f92b4ed688127ea7d7b1d03"},
+    {file = "lxml-4.9.2-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:a5da296eb617d18e497bcf0a5c528f5d3b18dadb3619fbdadf4ed2356ef8d941"},
+    {file = "lxml-4.9.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:04876580c050a8c5341d706dd464ff04fd597095cc8c023252566a8826505726"},
+    {file = "lxml-4.9.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:c9ec3eaf616d67db0764b3bb983962b4f385a1f08304fd30c7283954e6a7869b"},
+    {file = "lxml-4.9.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:2a29ba94d065945944016b6b74e538bdb1751a1db6ffb80c9d3c2e40d6fa9894"},
+    {file = "lxml-4.9.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:a82d05da00a58b8e4c0008edbc8a4b6ec5a4bc1e2ee0fb6ed157cf634ed7fa45"},
+    {file = "lxml-4.9.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:223f4232855ade399bd409331e6ca70fb5578efef22cf4069a6090acc0f53c0e"},
+    {file = "lxml-4.9.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d17bc7c2ccf49c478c5bdd447594e82692c74222698cfc9b5daae7ae7e90743b"},
+    {file = "lxml-4.9.2-cp37-cp37m-win32.whl", hash = "sha256:b64d891da92e232c36976c80ed7ebb383e3f148489796d8d31a5b6a677825efe"},
+    {file = "lxml-4.9.2-cp37-cp37m-win_amd64.whl", hash = "sha256:a0a336d6d3e8b234a3aae3c674873d8f0e720b76bc1d9416866c41cd9500ffb9"},
+    {file = "lxml-4.9.2-cp38-cp38-macosx_10_15_x86_64.whl", hash = "sha256:da4dd7c9c50c059aba52b3524f84d7de956f7fef88f0bafcf4ad7dde94a064e8"},
+    {file = "lxml-4.9.2-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:821b7f59b99551c69c85a6039c65b75f5683bdc63270fec660f75da67469ca24"},
+    {file = "lxml-4.9.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:e5168986b90a8d1f2f9dc1b841467c74221bd752537b99761a93d2d981e04889"},
+    {file = "lxml-4.9.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:8e20cb5a47247e383cf4ff523205060991021233ebd6f924bca927fcf25cf86f"},
+    {file = "lxml-4.9.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:13598ecfbd2e86ea7ae45ec28a2a54fb87ee9b9fdb0f6d343297d8e548392c03"},
+    {file = "lxml-4.9.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:880bbbcbe2fca64e2f4d8e04db47bcdf504936fa2b33933efd945e1b429bea8c"},
+    {file = "lxml-4.9.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:7d2278d59425777cfcb19735018d897ca8303abe67cc735f9f97177ceff8027f"},
+    {file = "lxml-4.9.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5344a43228767f53a9df6e5b253f8cdca7dfc7b7aeae52551958192f56d98457"},
+    {file = "lxml-4.9.2-cp38-cp38-win32.whl", hash = "sha256:925073b2fe14ab9b87e73f9a5fde6ce6392da430f3004d8b72cc86f746f5163b"},
+    {file = "lxml-4.9.2-cp38-cp38-win_amd64.whl", hash = "sha256:9b22c5c66f67ae00c0199f6055705bc3eb3fcb08d03d2ec4059a2b1b25ed48d7"},
+    {file = "lxml-4.9.2-cp39-cp39-macosx_10_15_x86_64.whl", hash = "sha256:5f50a1c177e2fa3ee0667a5ab79fdc6b23086bc8b589d90b93b4bd17eb0e64d1"},
+    {file = "lxml-4.9.2-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:090c6543d3696cbe15b4ac6e175e576bcc3f1ccfbba970061b7300b0c15a2140"},
+    {file = "lxml-4.9.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:63da2ccc0857c311d764e7d3d90f429c252e83b52d1f8f1d1fe55be26827d1f4"},
+    {file = "lxml-4.9.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:5b4545b8a40478183ac06c073e81a5ce4cf01bf1734962577cf2bb569a5b3bbf"},
+    {file = "lxml-4.9.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:2e430cd2824f05f2d4f687701144556646bae8f249fd60aa1e4c768ba7018947"},
+    {file = "lxml-4.9.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:6804daeb7ef69e7b36f76caddb85cccd63d0c56dedb47555d2fc969e2af6a1a5"},
+    {file = "lxml-4.9.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a6e441a86553c310258aca15d1c05903aaf4965b23f3bc2d55f200804e005ee5"},
+    {file = "lxml-4.9.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ca34efc80a29351897e18888c71c6aca4a359247c87e0b1c7ada14f0ab0c0fb2"},
+    {file = "lxml-4.9.2-cp39-cp39-win32.whl", hash = "sha256:6b418afe5df18233fc6b6093deb82a32895b6bb0b1155c2cdb05203f583053f1"},
+    {file = "lxml-4.9.2-cp39-cp39-win_amd64.whl", hash = "sha256:f1496ea22ca2c830cbcbd473de8f114a320da308438ae65abad6bab7867fe38f"},
+    {file = "lxml-4.9.2-pp37-pypy37_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:b264171e3143d842ded311b7dccd46ff9ef34247129ff5bf5066123c55c2431c"},
+    {file = "lxml-4.9.2-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:0dc313ef231edf866912e9d8f5a042ddab56c752619e92dfd3a2c277e6a7299a"},
+    {file = "lxml-4.9.2-pp38-pypy38_pp73-macosx_10_15_x86_64.whl", hash = "sha256:16efd54337136e8cd72fb9485c368d91d77a47ee2d42b057564aae201257d419"},
+    {file = "lxml-4.9.2-pp38-pypy38_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:0f2b1e0d79180f344ff9f321327b005ca043a50ece8713de61d1cb383fb8ac05"},
+    {file = "lxml-4.9.2-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:7b770ed79542ed52c519119473898198761d78beb24b107acf3ad65deae61f1f"},
+    {file = "lxml-4.9.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:efa29c2fe6b4fdd32e8ef81c1528506895eca86e1d8c4657fda04c9b3786ddf9"},
+    {file = "lxml-4.9.2-pp39-pypy39_pp73-macosx_10_15_x86_64.whl", hash = "sha256:7e91ee82f4199af8c43d8158024cbdff3d931df350252288f0d4ce656df7f3b5"},
+    {file = "lxml-4.9.2-pp39-pypy39_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:b23e19989c355ca854276178a0463951a653309fb8e57ce674497f2d9f208746"},
+    {file = "lxml-4.9.2-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:01d36c05f4afb8f7c20fd9ed5badca32a2029b93b1750f571ccc0b142531caf7"},
+    {file = "lxml-4.9.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:7b515674acfdcadb0eb5d00d8a709868173acece5cb0be3dd165950cbfdf5409"},
+    {file = "lxml-4.9.2.tar.gz", hash = "sha256:2455cfaeb7ac70338b3257f41e21f0724f4b5b0c0e7702da67ee6c3640835b67"},
+]
+
+[package.extras]
+cssselect = ["cssselect (>=0.7)"]
+html5 = ["html5lib"]
+htmlsoup = ["BeautifulSoup4"]
+source = ["Cython (>=0.29.7)"]
+
+[[package]]
 name = "markdown-it-py"
 version = "2.2.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -1493,8 +1586,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "64b657301d020637ad10adf1db862bc58f7c22064164c63e51a23ccfcfec57c2"
+content-hash = "20135b00adda6b208eb69709519c1b57bfb96b35395f97392b9181b0390230a5"
```

### Comparing `pontos-23.5.2/pontos/__init__.py` & `pontos-23.5.3/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/changelog/__init__.py` & `pontos-23.5.3/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/changelog/conventional_commits.py` & `pontos-23.5.3/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/changelog/errors.py` & `pontos-23.5.3/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/changelog/main.py` & `pontos-23.5.3/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/errors.py` & `pontos-23.5.3/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/git/__init__.py` & `pontos-23.5.3/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/git/git.py` & `pontos-23.5.3/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/git/status.py` & `pontos-23.5.3/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/__init__.py` & `pontos-23.5.3/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/__init__.py` & `pontos-23.5.3/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/argparser.py` & `pontos-23.5.3/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/cmds.py` & `pontos-23.5.3/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/core.py` & `pontos-23.5.3/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/env.py` & `pontos-23.5.3/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/errors.py` & `pontos-23.5.3/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/event.py` & `pontos-23.5.3/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/actions/main.py` & `pontos-23.5.3/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/__init__.py` & `pontos-23.5.3/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/api.py` & `pontos-23.5.3/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/artifacts.py` & `pontos-23.5.3/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/branch.py` & `pontos-23.5.3/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/client.py` & `pontos-23.5.3/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/contents.py` & `pontos-23.5.3/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/errors.py` & `pontos-23.5.3/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/helper.py` & `pontos-23.5.3/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/labels.py` & `pontos-23.5.3/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/organizations.py` & `pontos-23.5.3/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/pull_requests.py` & `pontos-23.5.3/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/release.py` & `pontos-23.5.3/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/repositories.py` & `pontos-23.5.3/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/search.py` & `pontos-23.5.3/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/tags.py` & `pontos-23.5.3/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/teams.py` & `pontos-23.5.3/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/api/workflows.py` & `pontos-23.5.3/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/argparser.py` & `pontos-23.5.3/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/cmds.py` & `pontos-23.5.3/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/main.py` & `pontos-23.5.3/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/__init__.py` & `pontos-23.5.3/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/artifact.py` & `pontos-23.5.3/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/base.py` & `pontos-23.5.3/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/branch.py` & `pontos-23.5.3/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/organization.py` & `pontos-23.5.3/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/pull_request.py` & `pontos-23.5.3/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/release.py` & `pontos-23.5.3/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/search.py` & `pontos-23.5.3/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/tag.py` & `pontos-23.5.3/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/models/workflow.py` & `pontos-23.5.3/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/pr_template.md` & `pontos-23.5.3/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/script/__init__.py` & `pontos-23.5.3/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/script/errors.py` & `pontos-23.5.3/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/script/load.py` & `pontos-23.5.3/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/github/script/parser.py` & `pontos-23.5.3/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/helper.py` & `pontos-23.5.3/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/models/__init__.py` & `pontos-23.5.3/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/__init__.py` & `pontos-23.5.3/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/api.py` & `pontos-23.5.3/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/cpe/__init__.py` & `pontos-23.5.3/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/cpe/api.py` & `pontos-23.5.3/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/cve/__init__.py` & `pontos-23.5.3/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/cve/api.py` & `pontos-23.5.3/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/models/__init__.py` & `pontos-23.5.3/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/models/cpe.py` & `pontos-23.5.3/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/models/cve.py` & `pontos-23.5.3/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/models/cvss_v2.py` & `pontos-23.5.3/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/nvd/models/cvss_v3.py` & `pontos-23.5.3/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/pontos.py` & `pontos-23.5.3/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/release/__init__.py` & `pontos-23.5.3/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/release/helper.py` & `pontos-23.5.3/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/release/main.py` & `pontos-23.5.3/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/release/parser.py` & `pontos-23.5.3/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/release/release.py` & `pontos-23.5.3/pontos/release/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/release/sign.py` & `pontos-23.5.3/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/terminal/__init__.py` & `pontos-23.5.3/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/terminal/null.py` & `pontos-23.5.3/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/terminal/rich.py` & `pontos-23.5.3/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/terminal/terminal.py` & `pontos-23.5.3/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/testing/__init__.py` & `pontos-23.5.3/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/updateheader/__init__.py` & `pontos-23.5.3/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/updateheader/__main__.py` & `pontos-23.5.3/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/updateheader/updateheader.py` & `pontos-23.5.3/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/__init__.py` & `pontos-23.5.3/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/__main__.py` & `pontos-23.5.3/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/_calculator.py` & `pontos-23.5.3/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/commands/__init__.py` & `pontos-23.5.3/pontos/version/commands/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,34 +13,37 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Iterable, Tuple, Type
 
+from ._cargo import CargoVersionCommand
 from ._cmake import CMakeVersionCommand
 from ._command import VersionCommand
 from ._go import GoVersionCommand
+from ._java import JavaVersionCommand
 from ._javascript import JavaScriptVersionCommand
 from ._python import PythonVersionCommand
-from ._cargo import CargoVersionCommand
 
 __all__ = (
     "VersionCommand",
     "CMakeVersionCommand",
     "GoVersionCommand",
     "JavaScriptVersionCommand",
+    "JavaVersionCommand",
     "PythonVersionCommand",
     "CargoVersionCommand",
     "get_commands",
 )
 
 __COMMANDS: Tuple[Type[VersionCommand]] = (
     CMakeVersionCommand,
     GoVersionCommand,
+    JavaVersionCommand,
     JavaScriptVersionCommand,
     PythonVersionCommand,
     CargoVersionCommand,
 )
 
 
 def get_commands() -> Iterable[Type[VersionCommand]]:
```

### Comparing `pontos-23.5.2/pontos/version/commands/_cargo.py` & `pontos-23.5.3/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/commands/_cmake.py` & `pontos-23.5.3/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/commands/_command.py` & `pontos-23.5.3/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/commands/_go.py` & `pontos-23.5.3/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/commands/_javascript.py` & `pontos-23.5.3/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/commands/_python.py` & `pontos-23.5.3/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/errors.py` & `pontos-23.5.3/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/helper.py` & `pontos-23.5.3/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/main.py` & `pontos-23.5.3/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/parser.py` & `pontos-23.5.3/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/project.py` & `pontos-23.5.3/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/schemes/__init__.py` & `pontos-23.5.3/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/schemes/_pep440.py` & `pontos-23.5.3/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/schemes/_scheme.py` & `pontos-23.5.3/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/schemes/_semantic.py` & `pontos-23.5.3/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pontos/version/version.py` & `pontos-23.5.3/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/pyproject.toml` & `pontos-23.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.5.2"
+version = "23.5.3"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -40,14 +40,15 @@
 tomlkit = ">=0.5.11"
 packaging = ">=20.3"
 httpx = {extras = ["http2"], version = ">=0.23,<0.25"}
 rich = ">=12.4.4"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 python-dateutil = "^2.8.2"
 semver = ">=2.13,<4.0"
+lxml = "^4.9.0"
 
 [tool.poetry.dev-dependencies]
 autohooks = ">=22.7.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-isort = ">=22.3.0"
 rope = "^1.8.0"
```

### Comparing `pontos-23.5.2/scripts/github/artifacts-download.py` & `pontos-23.5.3/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/artifacts.py` & `pontos-23.5.3/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/branchprotection.py` & `pontos-23.5.3/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/create-repository.py` & `pontos-23.5.3/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/enforce-admins.py` & `pontos-23.5.3/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/lock-branch.py` & `pontos-23.5.3/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/members.py` & `pontos-23.5.3/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/release-assets-download.py` & `pontos-23.5.3/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/repositories.py` & `pontos-23.5.3/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/search-repositories.py` & `pontos-23.5.3/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/team-repositories.py` & `pontos-23.5.3/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/teams.py` & `pontos-23.5.3/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/scripts/github/workflow-runs.py` & `pontos-23.5.3/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/__init__.py` & `pontos-23.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/changelog/__init__.py` & `pontos-23.5.3/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/changelog/test_conventional_commits.py` & `pontos-23.5.3/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/changelog/test_parser.py` & `pontos-23.5.3/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/git/__init__.py` & `pontos-23.5.3/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/git/test_git.py` & `pontos-23.5.3/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/git/test_status.py` & `pontos-23.5.3/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/__init__.py` & `pontos-23.5.3/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/actions/__init__.py` & `pontos-23.5.3/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/actions/test-pull-request-event.json` & `pontos-23.5.3/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/actions/test_core.py` & `pontos-23.5.3/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/actions/test_env.py` & `pontos-23.5.3/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/actions/test_event.py` & `pontos-23.5.3/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/__init__.py` & `pontos-23.5.3/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/pr-files.json` & `pontos-23.5.3/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/release-response.json` & `pontos-23.5.3/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_artifacts.py` & `pontos-23.5.3/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_branch.py` & `pontos-23.5.3/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_client.py` & `pontos-23.5.3/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_contents.py` & `pontos-23.5.3/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_labels.py` & `pontos-23.5.3/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_organizations.py` & `pontos-23.5.3/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_pull_requests.py` & `pontos-23.5.3/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_release.py` & `pontos-23.5.3/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_repositories.py` & `pontos-23.5.3/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_search.py` & `pontos-23.5.3/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_tags.py` & `pontos-23.5.3/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_teams.py` & `pontos-23.5.3/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/api/test_workflows.py` & `pontos-23.5.3/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/__init__.py` & `pontos-23.5.3/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_artifact.py` & `pontos-23.5.3/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_base.py` & `pontos-23.5.3/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_branch.py` & `pontos-23.5.3/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_organization.py` & `pontos-23.5.3/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_pull_request.py` & `pontos-23.5.3/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_release.py` & `pontos-23.5.3/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_search.py` & `pontos-23.5.3/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_tag.py` & `pontos-23.5.3/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/models/test_workflow.py` & `pontos-23.5.3/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/script/__init__.py` & `pontos-23.5.3/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/script/test_load.py` & `pontos-23.5.3/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/script/test_parser.py` & `pontos-23.5.3/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/test_argparser.py` & `pontos-23.5.3/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/github/test_cmds.py` & `pontos-23.5.3/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/models/__init__.py` & `pontos-23.5.3/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/models/test_models.py` & `pontos-23.5.3/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/__init__.py` & `pontos-23.5.3/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/cpe/__init__.py` & `pontos-23.5.3/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/cpe/test_api.py` & `pontos-23.5.3/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/cve/__init__.py` & `pontos-23.5.3/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/cve/test_api.py` & `pontos-23.5.3/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/models/__init__.py` & `pontos-23.5.3/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/models/test_cpe.py` & `pontos-23.5.3/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/models/test_cve.py` & `pontos-23.5.3/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/nvd/test_api.py` & `pontos-23.5.3/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/release/__init__.py` & `pontos-23.5.3/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/release/test_helper.py` & `pontos-23.5.3/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/release/test_parser.py` & `pontos-23.5.3/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/release/test_release.py` & `pontos-23.5.3/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/release/test_sign.py` & `pontos-23.5.3/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/terminal/__init__.py` & `pontos-23.5.3/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/terminal/test_terminal.py` & `pontos-23.5.3/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/test_helper.py` & `pontos-23.5.3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/test_pontos.py` & `pontos-23.5.3/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/testing/__init__.py` & `pontos-23.5.3/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/testing/test_testing.py` & `pontos-23.5.3/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/updateheader/__init__.py` & `pontos-23.5.3/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/updateheader/test_header.py` & `pontos-23.5.3/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/__init__.py` & `pontos-23.5.3/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/commands/__init__.py` & `pontos-23.5.3/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/commands/test_cargo.py` & `pontos-23.5.3/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/commands/test_cmake.py` & `pontos-23.5.3/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/commands/test_go.py` & `pontos-23.5.3/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/commands/test_javascript.py` & `pontos-23.5.3/tests/version/commands/test_javascript.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Greenbone AG
+# Copyright (C) 2022-2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `pontos-23.5.2/tests/version/commands/test_python.py` & `pontos-23.5.3/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/schemes/__init__.py` & `pontos-23.5.3/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/schemes/test_pep440.py` & `pontos-23.5.3/tests/version/schemes/test_pep440.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,16 @@
             "1.2.3b1",
             "1.2.3rc1",
             "1.2.3a1+dev1",
             "1.2.3a1.dev1",
             "22.4.1",
             "22.4.1.dev1",
             "22.4.1.dev3",
+            "2022.4.1.dev3",
+            "2022.4.1",
         ]
         for version in versions:
             self.assertEqual(Version.from_string(version), Version(version))
 
     def test_parse_version_from_semver(self):
         versions = [
             "0.0.1",
@@ -473,14 +475,15 @@
             ("1.2.3rc1", "1.2.3"),
             ("1.2.3a1.dev1", "1.2.3"),
             ("1.2.3b1.dev1", "1.2.3"),
             ("1.2.3rc1.dev1", "1.2.3"),
             ("22.4.1", "22.4.2"),
             ("22.4.1.dev1", "22.4.1"),
             ("22.4.1.dev3", "22.4.1"),
+            ("2022.4.1.dev3", "2022.4.1"),
         ]
 
         for current_version, assert_version in versions:
             release_version = calculator.next_patch_version(
                 Version.from_string(current_version)
             )
 
@@ -550,14 +553,15 @@
             ("22.4.1", "22.5.0"),
             ("22.4.1.dev1", "22.5.0"),
             ("22.4.1.dev3", "22.5.0"),
             ("1.0.0a1", "1.0.0"),
             ("1.1.0a1", "1.1.0"),
             ("1.0.0.dev1", "1.0.0"),
             ("1.1.0.dev1", "1.1.0"),
+            ("2022.1.0.dev1", "2022.1.0"),
         ]
 
         for current_version, assert_version in versions:
             release_version = calculator.next_minor_version(
                 Version.from_string(current_version),
             )
             self.assertEqual(
```

### Comparing `pontos-23.5.2/tests/version/schemes/test_semantic.py` & `pontos-23.5.3/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/test_commands.py` & `pontos-23.5.3/tests/version/test_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 import unittest
 
 from pontos.version.commands import get_commands
 
 
 class GetCommandsTestCase(unittest.TestCase):
     def test_available_commands(self):
-        self.assertEqual(len(get_commands()), 5)
+        self.assertEqual(len(get_commands()), 6)
```

### Comparing `pontos-23.5.2/tests/version/test_errors.py` & `pontos-23.5.3/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/test_helper.py` & `pontos-23.5.3/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/test_main.py` & `pontos-23.5.3/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/test_parser.py` & `pontos-23.5.3/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/test_project.py` & `pontos-23.5.3/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/tests/version/test_version.py` & `pontos-23.5.3/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.2/PKG-INFO` & `pontos-23.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.5.2
+Version: 23.5.3
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: colorful (>=0.5.4,<0.6.0)
 Requires-Dist: httpx[http2] (>=0.23,<0.25)
+Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: packaging (>=20.3)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: rich (>=12.4.4)
 Requires-Dist: semver (>=2.13,<4.0)
 Requires-Dist: tomlkit (>=0.5.11)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Project-URL: Documentation, https://greenbone.github.io/pontos/
```

