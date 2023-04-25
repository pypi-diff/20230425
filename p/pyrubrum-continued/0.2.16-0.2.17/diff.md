# Comparing `tmp/pyrubrum-continued-0.2.16.tar.gz` & `tmp/pyrubrum-continued-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubrum-continued-0.2.16.tar", last modified: Mon Apr 24 11:34:06 2023, max compression
+gzip compressed data, was "pyrubrum-continued-0.2.17.tar", last modified: Tue Apr 25 09:11:16 2023, max compression
```

## Comparing `pyrubrum-continued-0.2.16.tar` & `pyrubrum-continued-0.2.17.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       28 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.flake8
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/.github/
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      635 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      397 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      625 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      334 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/typo.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      270 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.github/dependabot.yml
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2475 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.gitignore
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      125 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.gitmodules
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      571 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/.pre-commit-config.yaml
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    31212 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/CHANGELOG.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3355 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/CODE_OF_CONDUCT.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/CONTRIBUTING.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1984 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/FEATURES.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34878 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/LICENSE
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      282 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/MANIFEST.in
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      715 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/NOTICE
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/PKG-INFO
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4225 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/README.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1081 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/SECURITY.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6810 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/changelog_generator.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       52 2023-03-19 17:52:13.000000 pyrubrum-continued-0.2.16/dev-requirements.txt
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      638 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/Makefile
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      764 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/make.bat
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      716 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/CONTRIBUTING.md
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/_static/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/CONTRIBUTING.md
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/attributes.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    56344 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/cafe_bot.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34720 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/calendar_bot.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      469 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/deep_link.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    25806 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/hitchhiker_bot.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      299 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/inheritance.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5363 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/link.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3783 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/menu.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    42294 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/overview-1.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    28709 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/overview.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3887 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/page_menu.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    26253 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/sample_bot.png
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/database/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/base_database.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/dict_database.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/database_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/delete_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/expire_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/get_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      177 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/not_found_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/errors/set_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      117 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       80 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/database/redis_database.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       74 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/base_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      197 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      113 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/parameterized_base_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      101 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/parameterized_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/pass_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      109 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/handlers/pass_parameterized_handler.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/keyboard/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       59 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/keyboard/button.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/keyboard/element.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       98 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/keyboard/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/keyboard/keyboard.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/base_menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/deep_link_menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      127 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/link_menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/menus/page_menu.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/objects/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       70 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/objects/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       54 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/objects/user.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/styles/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/styles/base_style.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      104 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/styles/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/styles/menu_style.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/styles/page_style.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/tree/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       95 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/tree/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/tree/node.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/tree/recursive_add.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       57 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/tree/transform.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/api/types/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/types/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       56 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/api/types/types.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5306 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/docs/source/conf.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/examples/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      147 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/examples/sample.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1388 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/flowchart.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1458 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/glossary.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2453 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/license.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/docs/source/quickstart/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      761 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/quickstart/installation.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     7519 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs/source/quickstart/overview.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/docs-requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3825 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/docs_updater.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/examples/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3255 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.16/examples/cafe_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3578 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/examples/calendar_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2394 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/examples/hitchhiker_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       24 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/examples/requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1471 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/examples/sample.env
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1678 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/examples/sample_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       16 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/fast-requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       30 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyproject.toml
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2404 2023-04-24 11:33:44.000000 pyrubrum-continued-0.2.16/pyrubrum/__init__.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      924 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/database/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3615 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/database/base_database.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3369 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/database/dict_database.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1042 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1072 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/delete_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      915 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1102 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/expire_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1069 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/get_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1049 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/not_found_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1097 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/errors/set_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4714 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/database/redis_database.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/handlers/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1120 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/handlers/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5594 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.16/pyrubrum/handlers/base_handler.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6280 2023-04-18 19:58:27.000000 pyrubrum-continued-0.2.16/pyrubrum/handlers/handler.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9330 2023-04-18 19:58:44.000000 pyrubrum-continued-0.2.16/pyrubrum/handlers/parameterized_base_handler.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4203 2023-04-18 19:58:52.000000 pyrubrum-continued-0.2.16/pyrubrum/handlers/parameterized_handler.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/keyboard/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      889 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/keyboard/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3743 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/keyboard/button.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1319 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/keyboard/element.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2042 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/keyboard/keyboard.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1071 2023-03-20 08:21:09.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3695 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/base_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3229 2023-04-24 02:38:53.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/content_page_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4692 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/deep_link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3247 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9091 2023-04-24 02:33:47.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4892 2023-03-20 11:18:25.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/page_menu.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/styles/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      904 2023-03-20 07:53:10.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/styles/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2033 2023-03-20 08:34:39.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/styles/base_style.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3778 2023-04-24 11:33:29.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/styles/menu_style.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    11719 2023-04-24 11:32:39.000000 pyrubrum-continued-0.2.16/pyrubrum/menus/styles/page_style.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum/objects/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      829 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/objects/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4469 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/pyrubrum/objects/user.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/pyrubrum/tree/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      885 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/tree/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6184 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/pyrubrum/tree/node.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/pyrubrum/types/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4370 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/pyrubrum/types/__init__.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/PKG-INFO
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4626 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/SOURCES.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        1 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/dependency_links.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/requires.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        9 2023-04-24 11:34:05.000000 pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/top_level.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       14 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/setup.cfg
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3131 2023-03-19 14:42:30.000000 pyrubrum-continued-0.2.16/setup.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-24 11:34:06.000000 pyrubrum-continued-0.2.16/tests/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2001 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/tests/test_deep_link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1280 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/tests/test_dict_database.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1406 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/tests/test_link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3119 2023-03-24 07:38:17.000000 pyrubrum-continued-0.2.16/tests/test_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2747 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.16/tests/test_node.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      957 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.16/tests/test_version.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       28 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.flake8
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/.github/
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      635 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      397 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      625 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      334 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/typo.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      270 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.github/dependabot.yml
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2475 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.gitignore
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      125 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.gitmodules
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      571 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/.pre-commit-config.yaml
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    31212 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/CHANGELOG.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3355 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/CODE_OF_CONDUCT.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/CONTRIBUTING.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1984 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/FEATURES.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34878 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/LICENSE
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      282 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/MANIFEST.in
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      715 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/NOTICE
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/PKG-INFO
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4225 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/README.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1081 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/SECURITY.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6810 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/changelog_generator.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       52 2023-03-19 17:52:13.000000 pyrubrum-continued-0.2.17/dev-requirements.txt
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      638 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/Makefile
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      764 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/make.bat
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      716 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/CONTRIBUTING.md
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/_static/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/CONTRIBUTING.md
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/attributes.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    56344 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/cafe_bot.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34720 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/calendar_bot.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      469 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/deep_link.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    25806 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/hitchhiker_bot.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      299 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/inheritance.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5363 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/link.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3783 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/menu.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    42294 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/overview-1.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    28709 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/overview.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3887 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/page_menu.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    26253 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/sample_bot.png
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/database/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/base_database.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/dict_database.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/database_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/delete_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/expire_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/get_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      177 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/not_found_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/errors/set_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      117 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       80 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/database/redis_database.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       74 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/base_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      197 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      113 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/parameterized_base_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      101 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/parameterized_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/pass_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      109 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/handlers/pass_parameterized_handler.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/keyboard/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       59 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/keyboard/button.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/keyboard/element.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       98 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/keyboard/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/keyboard/keyboard.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/base_menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/deep_link_menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      127 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/link_menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/menus/page_menu.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/objects/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       70 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/objects/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       54 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/objects/user.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/styles/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/styles/base_style.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      104 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/styles/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/styles/menu_style.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/styles/page_style.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/tree/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       95 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/tree/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/tree/node.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/tree/recursive_add.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       57 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/tree/transform.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/api/types/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/types/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       56 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/api/types/types.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5306 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/docs/source/conf.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/examples/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      147 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/examples/sample.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1388 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/flowchart.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1458 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/glossary.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2453 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/license.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/docs/source/quickstart/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      761 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/quickstart/installation.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     7519 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs/source/quickstart/overview.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/docs-requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3825 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/docs_updater.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/examples/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3255 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.17/examples/cafe_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3578 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/examples/calendar_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2394 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/examples/hitchhiker_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       24 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/examples/requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1471 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/examples/sample.env
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1678 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/examples/sample_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       16 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/fast-requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       30 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyproject.toml
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2404 2023-04-25 09:10:28.000000 pyrubrum-continued-0.2.17/pyrubrum/__init__.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/database/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      924 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/database/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3615 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/database/base_database.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3369 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/database/dict_database.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1042 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1072 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/delete_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      915 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1102 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/expire_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1069 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/get_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1049 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/not_found_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1097 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/database/errors/set_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4714 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/database/redis_database.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/handlers/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1120 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/handlers/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5594 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.17/pyrubrum/handlers/base_handler.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6280 2023-04-18 19:58:27.000000 pyrubrum-continued-0.2.17/pyrubrum/handlers/handler.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9330 2023-04-18 19:58:44.000000 pyrubrum-continued-0.2.17/pyrubrum/handlers/parameterized_base_handler.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4203 2023-04-18 19:58:52.000000 pyrubrum-continued-0.2.17/pyrubrum/handlers/parameterized_handler.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/keyboard/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      889 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/keyboard/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3743 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/keyboard/button.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1319 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/keyboard/element.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2042 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/keyboard/keyboard.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1071 2023-03-20 08:21:09.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3695 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/base_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3229 2023-04-25 09:10:01.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/content_page_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4692 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/deep_link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3247 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9076 2023-04-25 09:10:06.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4892 2023-03-20 11:18:25.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/page_menu.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/styles/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      904 2023-03-20 07:53:10.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/styles/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2033 2023-03-20 08:34:39.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/styles/base_style.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3778 2023-04-24 11:33:29.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/styles/menu_style.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    11719 2023-04-24 11:32:39.000000 pyrubrum-continued-0.2.17/pyrubrum/menus/styles/page_style.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/objects/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      829 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/objects/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4469 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/pyrubrum/objects/user.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/tree/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      885 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/tree/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6184 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/pyrubrum/tree/node.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum/types/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4370 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/pyrubrum/types/__init__.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-04-25 09:11:15.000000 pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/PKG-INFO
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4626 2023-04-25 09:11:15.000000 pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/SOURCES.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        1 2023-04-25 09:11:15.000000 pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/dependency_links.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-04-25 09:11:15.000000 pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/requires.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        9 2023-04-25 09:11:15.000000 pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/top_level.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       14 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/setup.cfg
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3131 2023-03-19 14:42:30.000000 pyrubrum-continued-0.2.17/setup.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-25 09:11:16.000000 pyrubrum-continued-0.2.17/tests/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2001 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/tests/test_deep_link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1280 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/tests/test_dict_database.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1406 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/tests/test_link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3119 2023-03-24 07:38:17.000000 pyrubrum-continued-0.2.17/tests/test_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2747 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.17/tests/test_node.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      957 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.17/tests/test_version.py
```

### Comparing `pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/bug_report.md` & `pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/.github/ISSUE_TEMPLATE/feature_request.md` & `pyrubrum-continued-0.2.17/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/.gitignore` & `pyrubrum-continued-0.2.17/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/.pre-commit-config.yaml` & `pyrubrum-continued-0.2.17/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/CHANGELOG.md` & `pyrubrum-continued-0.2.17/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/CODE_OF_CONDUCT.md` & `pyrubrum-continued-0.2.17/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/CONTRIBUTING.md` & `pyrubrum-continued-0.2.17/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/FEATURES.md` & `pyrubrum-continued-0.2.17/FEATURES.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/LICENSE` & `pyrubrum-continued-0.2.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/NOTICE` & `pyrubrum-continued-0.2.17/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/PKG-INFO` & `pyrubrum-continued-0.2.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubrum-continued
-Version: 0.2.16
+Version: 0.2.17
 Summary: An intuitive framework for creating Telegram bots
 Home-page: https://github.com/hearot/pyrubrum
 Author: Hearot
 Author-email: gabriel@hearot.it
 License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues
 Project-URL: Source, https://github.com/hearot/pyrubrum
@@ -95,33 +95,33 @@
    - LRU caching with [functools.lru_cache](https://docs.python.org/3/library/functools.html#functools.lru_cache)
    - Native support for the *"Go back"* button
    - No limit for `callback_data` (see [Telegram Bot API](https://core.telegram.org/bots/api#inlinekeyboardbutton))
    - Paging integration with `PageMenu`
 
 ### Examples
 
-In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/sample.env) into `.env` and editing all the necessary variables.
+In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/sample.env) into `.env` and editing all the necessary variables.
 
-   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
-   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
-   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
+   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
+   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
+   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
+   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
 
 ### Changelog
 
-> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/CHANGELOG.md).
-> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/FEATURES.md).
+> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/CHANGELOG.md).
+> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/FEATURES.md).
 
 ### Commit messages
 
 > See [Conventional Commits](https://www.conventionalcommits.org).
 
 ### Contributing
 
-> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/CONTRIBUTING.md).
+> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/CONTRIBUTING.md).
 
 ### Versioning
 
 > See [PEP 440](https://www.python.org/dev/peps/pep-0440/).
 
 ### Thanks
 
@@ -131,8 +131,8 @@
 ### Branding
 
 > See [hearot/pyrubrum-assets](https://github.com/hearot/pyrubrum-assets).
 
 ### Copyright & License
 
 - Copyright (C) 2020 [Hearot](https://github.com/hearot).
-- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.16/LICENSE).
+- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.17/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.16 Summary: An
+Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.17 Summary: An
 intuitive framework for creating Telegram bots Home-page: https://github.com/
 hearot/pyrubrum Author: Hearot Author-email: gabriel@hearot.it License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues Project-URL:
 Source, https://github.com/hearot/pyrubrum Keywords: bot bots chat messenger
 mtproto pyrogram python telegram Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Natural Language ::
@@ -42,35 +42,35 @@
 encrypted parameters - Intuitive creation of inline keyboards - LRU caching
 with [functools.lru_cache](https://docs.python.org/3/library/
 functools.html#functools.lru_cache) - Native support for the *"Go back"* button
 - No limit for `callback_data` (see [Telegram Bot API](https://
 core.telegram.org/bots/api#inlinekeyboardbutton)) - Paging integration with
 `PageMenu` ### Examples In order to make use of the proposed examples, you need
 to create your own environment file by renaming [sample.env](https://
-github.com/hearot/pyrubrum/blob/v0.2.16/examples/sample.env) into `.env` and
+github.com/hearot/pyrubrum/blob/v0.2.17/examples/sample.env) into `.env` and
 editing all the necessary variables. - [CafÃ©](https://github.com/hearot/
-pyrubrum/blob/v0.2.16/examples/cafe_bot.py) - Get an overview of the design
+pyrubrum/blob/v0.2.17/examples/cafe_bot.py) - Get an overview of the design
 which lies inside Pyrubrum while interacting with multiple commands and pages.
-- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/
+- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/
 calendar_bot.py) - Get what day of the week a day is by simply choosing a year,
 a month and a day while discovering the potential of Pyrubrum page menus. -
-[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/
+[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/
 hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...
 [get an existential question answered](https://en.wikipedia.org/wiki/
 Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/
+- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/
 sample_bot.py) - Interact with inline menus while understanding how Pyrubrum
 works. ### Changelog > See [CHANGELOG.md](https://github.com/hearot/pyrubrum/
-blob/v0.2.16/CHANGELOG.md). > Find new features in [FEATURES.md](https://
-github.com/hearot/pyrubrum/blob/v0.2.16/FEATURES.md). ### Commit messages > See
+blob/v0.2.17/CHANGELOG.md). > Find new features in [FEATURES.md](https://
+github.com/hearot/pyrubrum/blob/v0.2.17/FEATURES.md). ### Commit messages > See
 [Conventional Commits](https://www.conventionalcommits.org). ### Contributing >
-See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/
+See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/
 CONTRIBUTING.md). ### Versioning > See [PEP 440](https://www.python.org/dev/
 peps/pep-0440/). ### Thanks - [veggero/tytg](https://github.com/veggero/tytg)
 for giving me the idea of developing a simple framework with which you can code
 a folder-like bot. - [bakhoraliev](https://github.com/bakhoraliev) for letting
 me understand that an object-oriented library would make the difference in
 developing this project. ### Branding > See [hearot/pyrubrum-assets](https://
 github.com/hearot/pyrubrum-assets). ### Copyright & License - Copyright (C)
 2020 [Hearot](https://github.com/hearot). - Licensed under the terms of the
 [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/
-blob/v0.2.16/LICENSE).
+blob/v0.2.17/LICENSE).
```

### Comparing `pyrubrum-continued-0.2.16/README.md` & `pyrubrum-continued-0.2.17/README.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/SECURITY.md` & `pyrubrum-continued-0.2.17/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/changelog_generator.py` & `pyrubrum-continued-0.2.17/changelog_generator.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/Makefile` & `pyrubrum-continued-0.2.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/make.bat` & `pyrubrum-continued-0.2.17/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/CONTRIBUTING.md` & `pyrubrum-continued-0.2.17/docs/source/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/CONTRIBUTING.md` & `pyrubrum-continued-0.2.17/docs/source/_static/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/attributes.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/attributes.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/cafe_bot.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/cafe_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/calendar_bot.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/calendar_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/hitchhiker_bot.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/hitchhiker_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/link.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/link.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/menu.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/menu.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/overview-1.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/overview-1.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/overview.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/overview.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/page_menu.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/page_menu.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/_static/flowcharts/sample_bot.png` & `pyrubrum-continued-0.2.17/docs/source/_static/flowcharts/sample_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/conf.py` & `pyrubrum-continued-0.2.17/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/flowchart.rst` & `pyrubrum-continued-0.2.17/docs/source/flowchart.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/glossary.rst` & `pyrubrum-continued-0.2.17/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/index.rst` & `pyrubrum-continued-0.2.17/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/license.rst` & `pyrubrum-continued-0.2.17/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/quickstart/installation.rst` & `pyrubrum-continued-0.2.17/docs/source/quickstart/installation.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs/source/quickstart/overview.rst` & `pyrubrum-continued-0.2.17/docs/source/quickstart/overview.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/docs_updater.py` & `pyrubrum-continued-0.2.17/docs_updater.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/examples/cafe_bot.py` & `pyrubrum-continued-0.2.17/examples/cafe_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/examples/calendar_bot.py` & `pyrubrum-continued-0.2.17/examples/calendar_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/examples/hitchhiker_bot.py` & `pyrubrum-continued-0.2.17/examples/hitchhiker_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/examples/sample.env` & `pyrubrum-continued-0.2.17/examples/sample.env`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/examples/sample_bot.py` & `pyrubrum-continued-0.2.17/examples/sample_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __author__ = "Hearot"
 __author_email__ = "gabriel@hearot.it"
 __copyright__ = "Copyright (C) 2020 Hearot <https://github.com/hearot>"
 __license__ = "GNU General Public License v3"
 __package__ = "pyrubrum"
 __url__ = "https://github.com/hearot/pyrubrum"
-__version__ = "0.2.16"
+__version__ = "0.2.17"
 
 from .database import BaseDatabase  # noqa
 from .database import DictDatabase  # noqa
 from .database import RedisDatabase  # noqa
 from .database.errors import DatabaseError  # noqa
 from .database.errors import DeleteError  # noqa
 from .database.errors import ExpireError  # noqa
```

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/base_database.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/base_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/dict_database.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/dict_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/delete_error.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/delete_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/error.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/expire_error.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/expire_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/get_error.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/get_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/not_found_error.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/not_found_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/errors/set_error.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/errors/set_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/database/redis_database.py` & `pyrubrum-continued-0.2.17/pyrubrum/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/handlers/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/handlers/base_handler.py` & `pyrubrum-continued-0.2.17/pyrubrum/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/handlers/handler.py` & `pyrubrum-continued-0.2.17/pyrubrum/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/handlers/parameterized_base_handler.py` & `pyrubrum-continued-0.2.17/pyrubrum/handlers/parameterized_base_handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/handlers/parameterized_handler.py` & `pyrubrum-continued-0.2.17/pyrubrum/handlers/parameterized_handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/keyboard/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/keyboard/button.py` & `pyrubrum-continued-0.2.17/pyrubrum/keyboard/button.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/keyboard/element.py` & `pyrubrum-continued-0.2.17/pyrubrum/keyboard/element.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/keyboard/keyboard.py` & `pyrubrum-continued-0.2.17/pyrubrum/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/base_menu.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/content_page_menu.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/content_page_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/deep_link_menu.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/deep_link_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/link_menu.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/link_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/menu.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                 await context.reply_cached_media(
                     file_id=content.media, caption=content.caption, reply_markup=keyboard, **self.kwargs
                 )
             else:
                 await context.reply_text(content, reply_markup=keyboard, **self.kwargs)
         elif isinstance(context, CallbackQuery):
             if isinstance(content, InputMedia):
-                await context.edit_message_media(content, reply_markup=keyboard, **self.kwargs)
+                await context.edit_message_media(content, reply_markup=keyboard)
             else:
                 await context.edit_message_text(content, reply_markup=keyboard, **self.kwargs)
 
     async def on_callback(
         self,
         handler: "Handler",  # noqa
         client: Client,
```

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/page_menu.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/page_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/styles/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/styles/base_style.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/styles/base_style.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/styles/menu_style.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/styles/menu_style.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/menus/styles/page_style.py` & `pyrubrum-continued-0.2.17/pyrubrum/menus/styles/page_style.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/objects/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/objects/user.py` & `pyrubrum-continued-0.2.17/pyrubrum/objects/user.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/tree/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/tree/node.py` & `pyrubrum-continued-0.2.17/pyrubrum/tree/node.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum/types/__init__.py` & `pyrubrum-continued-0.2.17/pyrubrum/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/PKG-INFO` & `pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubrum-continued
-Version: 0.2.16
+Version: 0.2.17
 Summary: An intuitive framework for creating Telegram bots
 Home-page: https://github.com/hearot/pyrubrum
 Author: Hearot
 Author-email: gabriel@hearot.it
 License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues
 Project-URL: Source, https://github.com/hearot/pyrubrum
@@ -95,33 +95,33 @@
    - LRU caching with [functools.lru_cache](https://docs.python.org/3/library/functools.html#functools.lru_cache)
    - Native support for the *"Go back"* button
    - No limit for `callback_data` (see [Telegram Bot API](https://core.telegram.org/bots/api#inlinekeyboardbutton))
    - Paging integration with `PageMenu`
 
 ### Examples
 
-In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/sample.env) into `.env` and editing all the necessary variables.
+In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/sample.env) into `.env` and editing all the necessary variables.
 
-   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
-   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
-   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
+   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
+   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
+   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
+   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
 
 ### Changelog
 
-> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/CHANGELOG.md).
-> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/FEATURES.md).
+> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/CHANGELOG.md).
+> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/FEATURES.md).
 
 ### Commit messages
 
 > See [Conventional Commits](https://www.conventionalcommits.org).
 
 ### Contributing
 
-> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/CONTRIBUTING.md).
+> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/CONTRIBUTING.md).
 
 ### Versioning
 
 > See [PEP 440](https://www.python.org/dev/peps/pep-0440/).
 
 ### Thanks
 
@@ -131,8 +131,8 @@
 ### Branding
 
 > See [hearot/pyrubrum-assets](https://github.com/hearot/pyrubrum-assets).
 
 ### Copyright & License
 
 - Copyright (C) 2020 [Hearot](https://github.com/hearot).
-- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.16/LICENSE).
+- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.17/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.16 Summary: An
+Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.17 Summary: An
 intuitive framework for creating Telegram bots Home-page: https://github.com/
 hearot/pyrubrum Author: Hearot Author-email: gabriel@hearot.it License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues Project-URL:
 Source, https://github.com/hearot/pyrubrum Keywords: bot bots chat messenger
 mtproto pyrogram python telegram Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Natural Language ::
@@ -42,35 +42,35 @@
 encrypted parameters - Intuitive creation of inline keyboards - LRU caching
 with [functools.lru_cache](https://docs.python.org/3/library/
 functools.html#functools.lru_cache) - Native support for the *"Go back"* button
 - No limit for `callback_data` (see [Telegram Bot API](https://
 core.telegram.org/bots/api#inlinekeyboardbutton)) - Paging integration with
 `PageMenu` ### Examples In order to make use of the proposed examples, you need
 to create your own environment file by renaming [sample.env](https://
-github.com/hearot/pyrubrum/blob/v0.2.16/examples/sample.env) into `.env` and
+github.com/hearot/pyrubrum/blob/v0.2.17/examples/sample.env) into `.env` and
 editing all the necessary variables. - [CafÃ©](https://github.com/hearot/
-pyrubrum/blob/v0.2.16/examples/cafe_bot.py) - Get an overview of the design
+pyrubrum/blob/v0.2.17/examples/cafe_bot.py) - Get an overview of the design
 which lies inside Pyrubrum while interacting with multiple commands and pages.
-- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/
+- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/
 calendar_bot.py) - Get what day of the week a day is by simply choosing a year,
 a month and a day while discovering the potential of Pyrubrum page menus. -
-[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/
+[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/
 hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...
 [get an existential question answered](https://en.wikipedia.org/wiki/
 Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.16/examples/
+- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.17/examples/
 sample_bot.py) - Interact with inline menus while understanding how Pyrubrum
 works. ### Changelog > See [CHANGELOG.md](https://github.com/hearot/pyrubrum/
-blob/v0.2.16/CHANGELOG.md). > Find new features in [FEATURES.md](https://
-github.com/hearot/pyrubrum/blob/v0.2.16/FEATURES.md). ### Commit messages > See
+blob/v0.2.17/CHANGELOG.md). > Find new features in [FEATURES.md](https://
+github.com/hearot/pyrubrum/blob/v0.2.17/FEATURES.md). ### Commit messages > See
 [Conventional Commits](https://www.conventionalcommits.org). ### Contributing >
-See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.16/
+See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.17/
 CONTRIBUTING.md). ### Versioning > See [PEP 440](https://www.python.org/dev/
 peps/pep-0440/). ### Thanks - [veggero/tytg](https://github.com/veggero/tytg)
 for giving me the idea of developing a simple framework with which you can code
 a folder-like bot. - [bakhoraliev](https://github.com/bakhoraliev) for letting
 me understand that an object-oriented library would make the difference in
 developing this project. ### Branding > See [hearot/pyrubrum-assets](https://
 github.com/hearot/pyrubrum-assets). ### Copyright & License - Copyright (C)
 2020 [Hearot](https://github.com/hearot). - Licensed under the terms of the
 [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/
-blob/v0.2.16/LICENSE).
+blob/v0.2.17/LICENSE).
```

### Comparing `pyrubrum-continued-0.2.16/pyrubrum_continued.egg-info/SOURCES.txt` & `pyrubrum-continued-0.2.17/pyrubrum_continued.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/setup.py` & `pyrubrum-continued-0.2.17/setup.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/tests/test_deep_link_menu.py` & `pyrubrum-continued-0.2.17/tests/test_deep_link_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/tests/test_dict_database.py` & `pyrubrum-continued-0.2.17/tests/test_dict_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/tests/test_link_menu.py` & `pyrubrum-continued-0.2.17/tests/test_link_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/tests/test_menu.py` & `pyrubrum-continued-0.2.17/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/tests/test_node.py` & `pyrubrum-continued-0.2.17/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.16/tests/test_version.py` & `pyrubrum-continued-0.2.17/tests/test_version.py`

 * *Files identical despite different names*

