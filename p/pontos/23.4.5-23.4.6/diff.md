# Comparing `tmp/pontos-23.4.5.tar.gz` & `tmp/pontos-23.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.5.tar", max compression
+gzip compressed data, was "pontos-23.4.6.tar", max compression
```

## Comparing `pontos-23.4.5.tar` & `pontos-23.4.6.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-04-24 12:47:13.902953 pontos-23.4.5/LICENSE
--rw-r--r--   0        0        0     3349 2023-04-24 12:47:13.902953 pontos-23.4.5/README.md
--rw-r--r--   0        0        0    97087 2023-04-24 12:47:13.906953 pontos-23.4.5/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-24 12:47:13.906953 pontos-23.4.5/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4427 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/main.py
--rw-r--r--   0        0        0     8044 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/parser.py
--rw-r--r--   0        0        0    12786 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     7786 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13419 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2145 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16023 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-04-24 12:47:13.914953 pontos-23.4.5/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_helper.py
--rw-r--r--   0        0        0     8597 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_parser.py
--rw-r--r--   0        0        0    76187 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_version.py
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 pontos-23.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-25 10:07:35.281387 pontos-23.4.6/LICENSE
+-rw-r--r--   0        0        0     3349 2023-04-25 10:07:35.281387 pontos-23.4.6/README.md
+-rw-r--r--   0        0        0    97087 2023-04-25 10:07:35.285387 pontos-23.4.6/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-25 10:07:35.285387 pontos-23.4.6/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4427 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/main.py
+-rw-r--r--   0        0        0     8044 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/parser.py
+-rw-r--r--   0        0        0    12786 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13419 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2145 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16023 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-04-25 10:07:35.293387 pontos-23.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/release/test_helper.py
+-rw-r--r--   0        0        0     8597 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/release/test_parser.py
+-rw-r--r--   0        0        0    76187 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_version.py
+-rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 pontos-23.4.6/PKG-INFO
```

### Comparing `pontos-23.4.5/LICENSE` & `pontos-23.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/README.md` & `pontos-23.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/poetry.lock` & `pontos-23.4.6/poetry.lock`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/__init__.py` & `pontos-23.4.6/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/changelog/__init__.py` & `pontos-23.4.6/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/changelog/conventional_commits.py` & `pontos-23.4.6/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/changelog/errors.py` & `pontos-23.4.6/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/changelog/main.py` & `pontos-23.4.6/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/errors.py` & `pontos-23.4.6/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/git/__init__.py` & `pontos-23.4.6/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/git/git.py` & `pontos-23.4.6/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/git/status.py` & `pontos-23.4.6/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/__init__.py` & `pontos-23.4.6/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/__init__.py` & `pontos-23.4.6/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/argparser.py` & `pontos-23.4.6/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/cmds.py` & `pontos-23.4.6/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/core.py` & `pontos-23.4.6/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/env.py` & `pontos-23.4.6/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/errors.py` & `pontos-23.4.6/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/event.py` & `pontos-23.4.6/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/actions/main.py` & `pontos-23.4.6/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/__init__.py` & `pontos-23.4.6/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/api.py` & `pontos-23.4.6/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/artifacts.py` & `pontos-23.4.6/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/branch.py` & `pontos-23.4.6/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/client.py` & `pontos-23.4.6/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/contents.py` & `pontos-23.4.6/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/errors.py` & `pontos-23.4.6/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/helper.py` & `pontos-23.4.6/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/labels.py` & `pontos-23.4.6/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/organizations.py` & `pontos-23.4.6/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/pull_requests.py` & `pontos-23.4.6/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/release.py` & `pontos-23.4.6/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/repositories.py` & `pontos-23.4.6/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/search.py` & `pontos-23.4.6/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/tags.py` & `pontos-23.4.6/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/teams.py` & `pontos-23.4.6/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/api/workflows.py` & `pontos-23.4.6/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/argparser.py` & `pontos-23.4.6/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/cmds.py` & `pontos-23.4.6/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/main.py` & `pontos-23.4.6/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/__init__.py` & `pontos-23.4.6/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/artifact.py` & `pontos-23.4.6/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/base.py` & `pontos-23.4.6/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/branch.py` & `pontos-23.4.6/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/organization.py` & `pontos-23.4.6/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/pull_request.py` & `pontos-23.4.6/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/release.py` & `pontos-23.4.6/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/search.py` & `pontos-23.4.6/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/tag.py` & `pontos-23.4.6/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/models/workflow.py` & `pontos-23.4.6/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/pr_template.md` & `pontos-23.4.6/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/script/__init__.py` & `pontos-23.4.6/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/script/errors.py` & `pontos-23.4.6/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/script/load.py` & `pontos-23.4.6/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/github/script/parser.py` & `pontos-23.4.6/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/helper.py` & `pontos-23.4.6/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/models/__init__.py` & `pontos-23.4.6/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/__init__.py` & `pontos-23.4.6/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/api.py` & `pontos-23.4.6/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/cpe/__init__.py` & `pontos-23.4.6/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/cpe/api.py` & `pontos-23.4.6/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/cve/__init__.py` & `pontos-23.4.6/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/cve/api.py` & `pontos-23.4.6/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/models/__init__.py` & `pontos-23.4.6/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/models/cpe.py` & `pontos-23.4.6/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/models/cve.py` & `pontos-23.4.6/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.6/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.6/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/pontos.py` & `pontos-23.4.6/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/release/__init__.py` & `pontos-23.4.6/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/release/helper.py` & `pontos-23.4.6/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/release/main.py` & `pontos-23.4.6/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/release/parser.py` & `pontos-23.4.6/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/release/release.py` & `pontos-23.4.6/pontos/release/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/release/sign.py` & `pontos-23.4.6/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/terminal/__init__.py` & `pontos-23.4.6/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/terminal/null.py` & `pontos-23.4.6/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/terminal/rich.py` & `pontos-23.4.6/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/terminal/terminal.py` & `pontos-23.4.6/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/testing/__init__.py` & `pontos-23.4.6/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/updateheader/__init__.py` & `pontos-23.4.6/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/updateheader/__main__.py` & `pontos-23.4.6/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/updateheader/updateheader.py` & `pontos-23.4.6/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/__init__.py` & `pontos-23.4.6/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/__main__.py` & `pontos-23.4.6/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/_calculator.py` & `pontos-23.4.6/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/__init__.py` & `pontos-23.4.6/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/_cargo.py` & `pontos-23.4.6/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/_cmake.py` & `pontos-23.4.6/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/_command.py` & `pontos-23.4.6/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/_go.py` & `pontos-23.4.6/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/_javascript.py` & `pontos-23.4.6/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/commands/_python.py` & `pontos-23.4.6/pontos/version/commands/_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
         """
 
         if (
             "tool" in self.pyproject_toml
             and "poetry" in self.pyproject_toml["tool"]  # type: ignore
             and "version" in self.pyproject_toml["tool"]["poetry"]  # type: ignore # pylint: disable=line-too-long
         ):
-            return self.versioning_scheme.parse_version(self.pyproject_toml["tool"]["poetry"]["version"])  # type: ignore # pylint: disable=line-too-long
+            return PEP440VersioningScheme.parse_version(
+                self.pyproject_toml["tool"]["poetry"]["version"]
+            )  # type: ignore
 
         raise VersionError(
             "Version information not found in "
             f"{self.project_file_path} file."
         )
 
     def _update_version_file(self, new_version: Version) -> None:
@@ -196,16 +198,28 @@
         )
 
         if not force and new_pep440_version == current_version:
             return VersionUpdate(
                 previous=current_converted_version, new=new_version
             )
 
-        self._update_pyproject_version(new_version=new_pep440_version)
+        try:
+            self._update_pyproject_version(new_version=new_pep440_version)
+        except OSError as e:
+            raise VersionError(
+                "Unable to update version in "
+                f"{self.project_file_path.absolute()}. Error was {e}"
+            ) from e
 
-        self._update_version_file(new_version=new_pep440_version)
+        try:
+            self._update_version_file(new_version=new_pep440_version)
+        except OSError as e:
+            raise VersionError(
+                "Unable to update version in "
+                f"{self.version_file_path.absolute()}. Error was {e}"
+            ) from e
 
         return VersionUpdate(
             previous=current_converted_version,
             new=new_version,
             changed_files=[self.version_file_path, self.project_file_path],
         )
```

### Comparing `pontos-23.4.5/pontos/version/errors.py` & `pontos-23.4.6/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/helper.py` & `pontos-23.4.6/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/main.py` & `pontos-23.4.6/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/parser.py` & `pontos-23.4.6/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/project.py` & `pontos-23.4.6/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/schemes/__init__.py` & `pontos-23.4.6/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/schemes/_pep440.py` & `pontos-23.4.6/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/schemes/_scheme.py` & `pontos-23.4.6/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/schemes/_semantic.py` & `pontos-23.4.6/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pontos/version/version.py` & `pontos-23.4.6/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/pyproject.toml` & `pontos-23.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.5"
+version = "23.4.6"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.4.5/scripts/github/artifacts-download.py` & `pontos-23.4.6/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/artifacts.py` & `pontos-23.4.6/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/branchprotection.py` & `pontos-23.4.6/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/create-repository.py` & `pontos-23.4.6/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/enforce-admins.py` & `pontos-23.4.6/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/lock-branch.py` & `pontos-23.4.6/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/members.py` & `pontos-23.4.6/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/release-assets-download.py` & `pontos-23.4.6/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/repositories.py` & `pontos-23.4.6/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/search-repositories.py` & `pontos-23.4.6/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/team-repositories.py` & `pontos-23.4.6/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/teams.py` & `pontos-23.4.6/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/scripts/github/workflow-runs.py` & `pontos-23.4.6/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/__init__.py` & `pontos-23.4.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/changelog/__init__.py` & `pontos-23.4.6/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/changelog/test_conventional_commits.py` & `pontos-23.4.6/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/changelog/test_parser.py` & `pontos-23.4.6/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/git/__init__.py` & `pontos-23.4.6/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/git/test_git.py` & `pontos-23.4.6/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/git/test_status.py` & `pontos-23.4.6/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/__init__.py` & `pontos-23.4.6/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/actions/__init__.py` & `pontos-23.4.6/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.6/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/actions/test_core.py` & `pontos-23.4.6/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/actions/test_env.py` & `pontos-23.4.6/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/actions/test_event.py` & `pontos-23.4.6/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/__init__.py` & `pontos-23.4.6/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/pr-files.json` & `pontos-23.4.6/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/release-response.json` & `pontos-23.4.6/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_artifacts.py` & `pontos-23.4.6/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_branch.py` & `pontos-23.4.6/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_client.py` & `pontos-23.4.6/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_contents.py` & `pontos-23.4.6/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_labels.py` & `pontos-23.4.6/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_organizations.py` & `pontos-23.4.6/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_pull_requests.py` & `pontos-23.4.6/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_release.py` & `pontos-23.4.6/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_repositories.py` & `pontos-23.4.6/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_search.py` & `pontos-23.4.6/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_tags.py` & `pontos-23.4.6/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_teams.py` & `pontos-23.4.6/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/api/test_workflows.py` & `pontos-23.4.6/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/__init__.py` & `pontos-23.4.6/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_artifact.py` & `pontos-23.4.6/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_base.py` & `pontos-23.4.6/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_branch.py` & `pontos-23.4.6/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_organization.py` & `pontos-23.4.6/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_pull_request.py` & `pontos-23.4.6/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_release.py` & `pontos-23.4.6/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_search.py` & `pontos-23.4.6/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_tag.py` & `pontos-23.4.6/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/models/test_workflow.py` & `pontos-23.4.6/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/script/__init__.py` & `pontos-23.4.6/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/script/test_load.py` & `pontos-23.4.6/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/script/test_parser.py` & `pontos-23.4.6/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/test_argparser.py` & `pontos-23.4.6/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/github/test_cmds.py` & `pontos-23.4.6/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/models/__init__.py` & `pontos-23.4.6/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/models/test_models.py` & `pontos-23.4.6/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/__init__.py` & `pontos-23.4.6/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/cpe/__init__.py` & `pontos-23.4.6/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/cpe/test_api.py` & `pontos-23.4.6/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/cve/__init__.py` & `pontos-23.4.6/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/cve/test_api.py` & `pontos-23.4.6/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/models/__init__.py` & `pontos-23.4.6/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/models/test_cpe.py` & `pontos-23.4.6/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/models/test_cve.py` & `pontos-23.4.6/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/nvd/test_api.py` & `pontos-23.4.6/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/release/__init__.py` & `pontos-23.4.6/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/release/test_helper.py` & `pontos-23.4.6/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/release/test_parser.py` & `pontos-23.4.6/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/release/test_release.py` & `pontos-23.4.6/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/release/test_sign.py` & `pontos-23.4.6/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/terminal/__init__.py` & `pontos-23.4.6/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/terminal/test_terminal.py` & `pontos-23.4.6/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/test_helper.py` & `pontos-23.4.6/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/test_pontos.py` & `pontos-23.4.6/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/testing/__init__.py` & `pontos-23.4.6/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/testing/test_testing.py` & `pontos-23.4.6/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/updateheader/__init__.py` & `pontos-23.4.6/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/updateheader/test_header.py` & `pontos-23.4.6/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/__init__.py` & `pontos-23.4.6/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/commands/__init__.py` & `pontos-23.4.6/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/commands/test_cargo.py` & `pontos-23.4.6/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/commands/test_cmake.py` & `pontos-23.4.6/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/commands/test_go.py` & `pontos-23.4.6/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/commands/test_javascript.py` & `pontos-23.4.6/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/commands/test_python.py` & `pontos-23.4.6/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/schemes/__init__.py` & `pontos-23.4.6/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/schemes/test_pep440.py` & `pontos-23.4.6/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/schemes/test_semantic.py` & `pontos-23.4.6/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_commands.py` & `pontos-23.4.6/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_errors.py` & `pontos-23.4.6/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_helper.py` & `pontos-23.4.6/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_main.py` & `pontos-23.4.6/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_parser.py` & `pontos-23.4.6/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_project.py` & `pontos-23.4.6/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/tests/version/test_version.py` & `pontos-23.4.6/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.5/PKG-INFO` & `pontos-23.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.5
+Version: 23.4.6
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

