# Comparing `tmp/rockingester-1.0.1.tar.gz` & `tmp/rockingester-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-1.0.1.tar", last modified: Sun Apr  9 09:28:22 2023, max compression
+gzip compressed data, was "rockingester-1.1.0.tar", last modified: Tue Apr 25 07:37:28 2023, max compression
```

## Comparing `rockingester-1.0.1.tar` & `rockingester-1.1.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.608137 rockingester-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-09 09:28:12.000000 rockingester-1.0.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-09 09:28:12.000000 rockingester-1.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-09 09:28:12.000000 rockingester-1.0.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.596138 rockingester-1.0.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 09:28:12.000000 rockingester-1.0.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-09 09:28:12.000000 rockingester-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-09 09:28:12.000000 rockingester-1.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 09:28:12.000000 rockingester-1.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 09:28:12.000000 rockingester-1.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 09:28:12.000000 rockingester-1.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 09:28:12.000000 rockingester-1.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 09:28:12.000000 rockingester-1.0.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 09:28:12.000000 rockingester-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-09 09:28:22.608137 rockingester-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-09 09:28:12.000000 rockingester-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-09 09:28:12.000000 rockingester-1.0.1/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.596138 rockingester-1.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.600138 rockingester-1.0.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 09:28:12.000000 rockingester-1.0.1/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-09 09:28:12.000000 rockingester-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:28:22.608137 rockingester-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.596138 rockingester-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.604138 rockingester-1.0.1/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.608137 rockingester-1.0.1/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:28:22.000000 rockingester-1.0.1/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.608137 rockingester-1.0.1/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.608137 rockingester-1.0.1/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-09 09:28:12.000000 rockingester-1.0.1/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.608137 rockingester-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:12.000000 rockingester-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-09 09:28:12.000000 rockingester-1.0.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:28:22.608137 rockingester-1.0.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-09 09:28:12.000000 rockingester-1.0.1/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-09 09:28:12.000000 rockingester-1.0.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-09 09:28:12.000000 rockingester-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-04-09 09:28:12.000000 rockingester-1.0.1/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.610096 rockingester-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 07:37:20.000000 rockingester-1.1.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-25 07:37:20.000000 rockingester-1.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-25 07:37:20.000000 rockingester-1.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.598096 rockingester-1.1.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 07:37:20.000000 rockingester-1.1.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 07:37:20.000000 rockingester-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-25 07:37:20.000000 rockingester-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-25 07:37:20.000000 rockingester-1.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 07:37:20.000000 rockingester-1.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-25 07:37:20.000000 rockingester-1.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 07:37:20.000000 rockingester-1.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 07:37:20.000000 rockingester-1.1.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 07:37:20.000000 rockingester-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-25 07:37:28.610096 rockingester-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-25 07:37:20.000000 rockingester-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-25 07:37:20.000000 rockingester-1.1.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.598096 rockingester-1.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.602096 rockingester-1.1.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 07:37:20.000000 rockingester-1.1.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-25 07:37:20.000000 rockingester-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:37:28.610096 rockingester-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.598096 rockingester-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.606096 rockingester-1.1.0/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 07:37:28.000000 rockingester-1.1.0/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.610096 rockingester-1.1.0/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.610096 rockingester-1.1.0/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-25 07:37:20.000000 rockingester-1.1.0/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.610096 rockingester-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:20.000000 rockingester-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-25 07:37:20.000000 rockingester-1.1.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:37:28.610096 rockingester-1.1.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-25 07:37:20.000000 rockingester-1.1.0/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-25 07:37:20.000000 rockingester-1.1.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-25 07:37:20.000000 rockingester-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-25 07:37:20.000000 rockingester-1.1.0/tests/test_collector.py
```

### Comparing `rockingester-1.0.1/.dae-devops/Makefile` & `rockingester-1.1.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/docs/conventions.rst` & `rockingester-1.1.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/docs/developing.rst` & `rockingester-1.1.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/docs/devops.rst` & `rockingester-1.1.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/docs/docs_structure.rst` & `rockingester-1.1.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/docs/installing.rst` & `rockingester-1.1.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/docs/testing.rst` & `rockingester-1.1.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.dae-devops/project.yaml` & `rockingester-1.1.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.devcontainer/Dockerfile` & `rockingester-1.1.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.devcontainer/devcontainer.json` & `rockingester-1.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/CONTRIBUTING.rst` & `rockingester-1.1.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/actions/install_requirements/action.yml` & `rockingester-1.1.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/dependabot.yml` & `rockingester-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/pages/make_switcher.py` & `rockingester-1.1.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/workflows/code.yml` & `rockingester-1.1.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/workflows/docs.yml` & `rockingester-1.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/workflows/docs_clean.yml` & `rockingester-1.1.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.github/workflows/linkcheck.yml` & `rockingester-1.1.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.gitignore` & `rockingester-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.gitlab-ci.yml` & `rockingester-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/.vscode/launch.json` & `rockingester-1.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/LICENSE` & `rockingester-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/PKG-INFO` & `rockingester-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 1.0.1
+Version: 1.1.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-1.0.1/README.rst` & `rockingester-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/configurations/development.yaml` & `rockingester-1.1.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/docs/conf.py` & `rockingester-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/docs/images/dls-favicon.ico` & `rockingester-1.1.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/docs/images/dls-logo.svg` & `rockingester-1.1.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/docs/index.rst` & `rockingester-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/docs/user/explanations/25-docs-structure.rst` & `rockingester-1.1.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/docs/user/index.rst` & `rockingester-1.1.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/pyproject.toml` & `rockingester-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester.egg-info/PKG-INFO` & `rockingester-1.1.0/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 1.0.1
+Version: 1.1.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-1.0.1/src/rockingester.egg-info/SOURCES.txt` & `rockingester-1.1.0/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/collectors/aiohttp.py` & `rockingester-1.1.0/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/collectors/collectors.py` & `rockingester-1.1.0/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/collectors/context.py` & `rockingester-1.1.0/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/context_base.py` & `rockingester-1.1.0/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/exceptions.py` & `rockingester-1.1.0/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/thing.py` & `rockingester-1.1.0/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_api/things.py` & `rockingester-1.1.0/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_cli/main.py` & `rockingester-1.1.0/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_cli/subcommands/base.py` & `rockingester-1.1.0/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_cli/subcommands/service.py` & `rockingester-1.1.0/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_cli/version.py` & `rockingester-1.1.0/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/__main__.py` & `rockingester-1.1.0/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-1.1.0/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/collectors/base.py` & `rockingester-1.1.0/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/collectors/collectors.py` & `rockingester-1.1.0/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/collectors/context.py` & `rockingester-1.1.0/src/rockingester_lib/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-1.1.0/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import shutil
 from pathlib import Path
 from typing import Dict
 
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
+from dls_utilpack.visit import get_xchem_directory
 from PIL import Image
 
 # Dataface client context.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 
 # Crystal plate pydantic model.
@@ -42,16 +43,22 @@
             self, thing_type, specification, predefined_uuid=predefined_uuid
         )
 
         s = f"{callsign(self)} specification", self.specification()
 
         type_specific_tbd = require(s, self.specification(), "type_specific_tbd")
         self.__plates_directories = require(s, type_specific_tbd, "plates_directories")
-        self.__ingested_directory = Path(
-            require(s, type_specific_tbd, "ingested_directory")
+        self.__visits_directory = Path(
+            require(s, type_specific_tbd, "visits_directory")
+        )
+        self.__visit_plates_subdirectory = Path(
+            require(s, type_specific_tbd, "visit_plates_subdirectory")
+        )
+        self.__novisit_directory = Path(
+            require(s, type_specific_tbd, "novisit_directory")
         )
         self.__nobarcode_directory = Path(
             require(s, type_specific_tbd, "nobarcode_directory")
         )
 
         self.__ingest_only_barcodes = type_specific_tbd.get("ingest_only_barcodes")
 
@@ -72,23 +79,23 @@
     async def activate(self) -> None:
         """
         Activate the object.
 
         Then it starts the coro task to awaken every few seconds to scrape the directories.
         """
 
-        # Make sure the nobarcode_directory is created.
+        # Make sure the novisit_directory is created.
         try:
-            self.__nobarcode_directory.mkdir(parents=True)
+            self.__novisit_directory.mkdir(parents=True)
         except FileExistsError:
             pass
 
-        # Make sure the ingested_directory is created.
+        # Make sure the nobarcode_directory is created.
         try:
-            self.__ingested_directory.mkdir(parents=True)
+            self.__nobarcode_directory.mkdir(parents=True)
         except FileExistsError:
             pass
 
         # Make the xchembku client context.
         s = require(
             f"{callsign(self)} specification",
             self.specification(),
@@ -202,15 +209,15 @@
             return
 
         plate_names = [
             entry.name for entry in os.scandir(plates_directory) if entry.is_dir()
         ]
 
         logger.info(
-            f"[SCRDIR] found {len(plate_names)} plate directories in {plates_directory}"
+            f"[ROCKINGESTER POLL] found {len(plate_names)} plate directories in {plates_directory}"
         )
 
         for plate_name in plate_names:
             # Get the plate's barcode from the directory name.
             plate_barcode = plate_name[0:4]
 
             # We have a specific list we want to process?
@@ -221,138 +228,193 @@
             # Get the matching plate record from the database.
             crystal_plate_model = self.__crystal_plate_models_by_barcode.get(
                 plate_barcode
             )
 
             # This plate is in the database?
             if crystal_plate_model is not None:
-                await self.scrape_plate_directory(
-                    plates_directory / plate_name,
-                    crystal_plate_model,
-                )
+                visit_directory = None
+                try:
+                    visit_directory = Path(
+                        get_xchem_directory(
+                            self.__visits_directory, crystal_plate_model.visit
+                        )
+                    )
+
+                    await self.scrape_plate_directory(
+                        plates_directory / plate_name,
+                        crystal_plate_model,
+                        visit_directory,
+                    )
+                except Exception as exception:
+                    logger.debug(f"novisit because: {str(exception)}")
+                    await self.__move_without_ingesting(
+                        plates_directory / plate_name,
+                        self.__novisit_directory,
+                    )
+
             # Not in the database?
             else:
-                await self.move_to_nobarcode(plates_directory / plate_name)
+                await self.__move_without_ingesting(
+                    plates_directory / plate_name,
+                    self.__nobarcode_directory,
+                )
 
     # ----------------------------------------------------------------------------------------
-    async def move_to_nobarcode(
+    async def __move_without_ingesting(
         self,
         plate_directory: Path,
+        target_directory: Path,
     ) -> None:
         """
-        Move a plate directory's well images to the "nobarcode" area.
+        Move a plate directory's well images to the given target without ingesting it.
 
         Then remove the plate directory.
         """
 
-        target = self.__nobarcode_directory / plate_directory.name
+        target = target_directory / plate_directory.name
         try:
             target.mkdir(parents=True)
         except FileExistsError:
             pass
 
         # Get all the well images in the plate directory.
         well_names = [
             entry.name for entry in os.scandir(plate_directory) if entry.is_file()
         ]
 
         for well_name in well_names:
-            # Move to nobarcode, replacing what might already be there.
+            # Move to target, replacing what might already be there.
             # TODO: Protect against moving an image file which is currently being written by Luigi.
             shutil.move(
                 plate_directory / well_name,
                 target / well_name,
             )
 
         # Remove the source directory, which should now be empty.
         # TODO: Protect against removing an plate directory which is currently being written by Luigi.
         try:
             plate_directory.rmdir()
         except OSError:
             pass
 
+        logger.info(f"moved plate {plate_directory.name} to {target_directory}")
+
     # ----------------------------------------------------------------------------------------
     async def scrape_plate_directory(
         self,
         plate_directory: Path,
         crystal_plate_model: CrystalPlateModel,
+        visit_directory: Path,
     ) -> None:
         """
         Scrape a single directory looking for new files.
 
         Adds discovered files to internal list which gets pushed when it reaches a configurable size.
         """
 
+        # Update the path stem in the crystal plate record.
+        # TODO: Consider if important to report/record same barcodes on different rockmaker directories.
+        if crystal_plate_model.rockminer_collected_stem is None:
+            crystal_plate_model.rockminer_collected_stem = plate_directory.stem
+            await self.__xchembku.upsert_crystal_plates(
+                [crystal_plate_model], "update rockminer_collected_stem"
+            )
+
         # Get all the well images in the plate directory.
         well_names = [
             entry.name for entry in os.scandir(plate_directory) if entry.is_file()
         ]
 
+        # Sort so that tests are deterministic.
+        well_names.sort()
+
         for well_name in well_names:
             # Process well's image file.
+            # TODO: Improve safety by ignoring wrongly formatted and non-jpg well filenames.
             await self.ingest_well(
                 plate_directory,
                 well_name,
                 crystal_plate_model,
+                visit_directory,
             )
 
         # Remove the source directory, which should now be empty.
         # TODO: Protect against removing an plate directory which is currently being written by Luigi.
         try:
             plate_directory.rmdir()
         except OSError:
             pass
 
+        logger.info(
+            f"moved well images from plate {plate_directory.name} to {self.__novisit_directory}"
+        )
+
     # ----------------------------------------------------------------------------------------
     async def ingest_well(
         self,
         plate_directory: Path,
         well_name: str,
         crystal_plate_model: CrystalPlateModel,
+        visit_directory: Path,
     ) -> None:
         """
         Ingest the well into the database.
 
         Move the well image file to the ingested area.
 
         TODO: Protect against ingesting an image file which is currently being written by Luigi.
         """
 
-        well_filename = plate_directory / well_name
+        # Make the "object store" directory where we will permanently store ingested well image files.
+        target = (
+            visit_directory / self.__visit_plates_subdirectory / plate_directory.name
+        )
+        try:
+            target.mkdir(parents=True)
+        except FileExistsError:
+            pass
+
+        input_well_filename = plate_directory / well_name
+        ingested_well_filename = target / well_name
+
+        # Stems are like "9acx_01A_1".
+        parts = Path(well_name).stem.split("_")
+        if len(parts) > 1:
+            # Strip off the leading 4-letter barcode and underscore.
+            position = "".join(parts[1:])
+        else:
+            position = parts[0]
+
         error = None
         try:
-            image = Image.open(well_filename)
+            image = Image.open(input_well_filename)
             width, height = image.size
         except Exception as exception:
             error = str(exception)
             width = None
             height = None
 
         crystal_well_model = CrystalWellModel(
-            filename=str(well_filename),
+            position=position,
+            filename=str(ingested_well_filename),
             crystal_plate_uuid=crystal_plate_model.uuid,
             error=error,
             width=width,
             height=height,
         )
 
         # Here we originate the crystal well records into xchembku.
-        # TODO: Handle case where the same crystal well filename has already been originated.
-        await self.__xchembku.originate_crystal_wells([crystal_well_model])
-
-        target = self.__ingested_directory / plate_directory.name
-        try:
-            target.mkdir(parents=True)
-        except FileExistsError:
-            pass
+        # TODO: Handle case where we upsert the crystal_well record bit the image object store fails to accept image binary.
+        await self.__xchembku.upsert_crystal_wells([crystal_well_model])
 
         # Move to ingested, replacing what might already be there.
         shutil.move(
-            well_filename,
-            target / well_name,
+            input_well_filename,
+            ingested_well_filename,
         )
 
     # ----------------------------------------------------------------------------------------
     async def close_client_session(self):
         """"""
 
         pass
```

### Comparing `rockingester-1.0.1/src/rockingester_lib/contexts/base.py` & `rockingester-1.1.0/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/exceptions.py` & `rockingester-1.1.0/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/src/rockingester_lib/version.py` & `rockingester-1.1.0/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/tests/base.py` & `rockingester-1.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/tests/configurations/direct_poll.yaml` & `rockingester-1.1.0/tests/configurations/direct_poll.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
     type: "xchembku_lib.xchembku_datafaces.direct"
     database:
         type: "xchembku_lib.xchembku_databases.normsql"
         filename: "${output_directory}/xchembku.sqlite"
         log_level: "WARNING"
 
-ingested_directory: &INGESTED_DIRECTORY "${output_directory}/SubwellImages_ingested"
+visits_directory: &VISITS_DIRECTORY "${output_directory}/visits"
+visit_plates_subdirectory: &VISIT_PLATES_SUBDIRECTORY "processing/rockingester"
+novisit_directory: &NONVISIT_DIRECTORY "${output_directory}/SubwellImages_novisit"
 nobarcode_directory: &NOBARCODE_DIRECTORY "${output_directory}/SubwellImages_nobarcode"
 
 # The rockingester direct access.
 rockingester_collector_specification:
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
-        ingested_directory: *INGESTED_DIRECTORY
+        visits_directory: *VISITS_DIRECTORY
+        visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
+        novisit_directory: *NONVISIT_DIRECTORY
         nobarcode_directory: *NOBARCODE_DIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
+            - 98ad
     context:
         start_as: direct
```

### Comparing `rockingester-1.0.1/tests/configurations/service.yaml` & `rockingester-1.1.0/tests/configurations/service.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
     type: "xchembku_lib.xchembku_datafaces.direct"
     database:
         type: "xchembku_lib.xchembku_databases.normsql"
         filename: "${output_directory}/xchembku.sqlite"
         log_level: "WARNING"
 
-ingested_directory: &INGESTED_DIRECTORY "${output_directory}/SubwellImages_ingested"
+visits_directory: &VISITS_DIRECTORY "${output_directory}/visits"
+visit_plates_subdirectory: &VISIT_PLATES_SUBDIRECTORY "processing/rockingester"
+novisit_directory: &NONVISIT_DIRECTORY "${output_directory}/SubwellImages_novisit"
 nobarcode_directory: &NOBARCODE_DIRECTORY "${output_directory}/SubwellImages_nobarcode"
 
 # The rockingester direct access.
 rockingester_collector_specification_direct_poll:
     &ROCKINGESTER_COLLECTOR_SPECIFICATION_DIRECT_POLL
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
-        ingested_directory: *INGESTED_DIRECTORY
+        visits_directory: *VISITS_DIRECTORY
+        visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
+        novisit_directory: *NONVISIT_DIRECTORY
         nobarcode_directory: *NOBARCODE_DIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
+            - 98ad
 
 # The rockingester client/server composite.
 rockingester_collector_specification:
     type: "rockingester_lib.collectors.aiohttp"
     type_specific_tbd:
         # The remote rockingester server access.
         aiohttp_specification:
```

### Comparing `rockingester-1.0.1/tests/conftest.py` & `rockingester-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-1.0.1/tests/test_collector.py` & `rockingester-1.1.0/tests/test_collector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import asyncio
 import logging
 import time
 from pathlib import Path
 
+from dls_utilpack.visit import get_xchem_subdirectory
+
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
+from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
 # Client context creator.
 from rockingester_api.collectors.context import Context as CollectorClientContext
 
 # Server context creator.
 from rockingester_lib.collectors.context import Context as CollectorServerContext
@@ -90,16 +93,20 @@
         # Make the server context.
         collector_server_context = CollectorServerContext(collector_specification)
 
         # Make the client context.
         collector_client_context = CollectorClientContext(collector_specification)
 
         # Remember the collector specification so we can assert some things later.
-        self.__ingested_directory = Path(multiconf_dict["ingested_directory"])
+        self.__visits_directory = Path(multiconf_dict["visits_directory"])
+        self.__visit_plates_subdirectory = Path(
+            multiconf_dict["visit_plates_subdirectory"]
+        )
         self.__nobarcode_directory = Path(multiconf_dict["nobarcode_directory"])
+        self.__novisit_directory = Path(multiconf_dict["novisit_directory"])
 
         image_count = 2
 
         # Start the client context for the direct access to the xchembku.
         async with xchembku_client_context:
             # Start the collector client context.
             async with collector_client_context:
@@ -120,115 +127,185 @@
 
     async def __run_part1(self, image_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
         # Make the plate on which the wells reside.
-        visit = "cm00001-1"
-        crystal_plate_model = CrystalPlateModel(
-            formulatrix__plate__id=10,
-            barcode="98ab",
-            visit=visit,
+        visit = "cm00001-1_otherstuff"
+        created_crystal_plate_models = []
+        created_crystal_plate_models.append(
+            CrystalPlateModel(
+                formulatrix__plate__id=10,
+                barcode="98ab",
+                visit=visit,
+            )
         )
 
-        await xchembku.upsert_crystal_plates([crystal_plate_model])
+        nobarcode_barcode = "98ac"
+
+        # Create a crystal plate model with a good barcode but bad visit.
+        novisit_barcode = "98ad"
+        created_crystal_plate_models.append(
+            CrystalPlateModel(
+                formulatrix__plate__id=11,
+                barcode=novisit_barcode,
+                visit=("X" + visit),
+            )
+        )
+
+        excluded_barcode = "98ae"
+
+        await xchembku.upsert_crystal_plates(created_crystal_plate_models)
+
+        visit_directory = self.__visits_directory / get_xchem_subdirectory(visit)
+        visit_directory.mkdir(parents=True)
+        rockingester_directory = visit_directory / self.__visit_plates_subdirectory
 
         # Get list of images before we create any of the scrape-able files.
-        records = await xchembku.fetch_crystal_wells_filenames()
+        crystal_well_models = await xchembku.fetch_crystal_wells_filenames()
 
-        assert len(records) == 0, "images before any new files are put in scrapable"
+        assert (
+            len(crystal_well_models) == 0
+        ), "images before any new files are put in scrapable"
 
         plates_directory = Path(output_directory) / "SubwellImages"
 
         # Make the scrapable directory with some files.
+        # This one gets scraped as normal.
         plate_directory1 = plates_directory / "98ab_2023-04-06_RI1000-0276-3drop"
         plate_directory1.mkdir(parents=True)
         for i in range(10, 10 + image_count):
             filename = plate_directory1 / ("98ab_%02dA_1.jpg" % (i))
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make another scrapable directory with a different barcode.
-        plate_directory2 = plates_directory / "98ac_2023-04-06_RI1000-0276-3drop"
+        # This one gets moved into nobarcode since it doesn't match any plate.
+        plate_directory2 = (
+            plates_directory / f"{nobarcode_barcode}_2023-04-06_RI1000-0276-3drop"
+        )
         plate_directory2.mkdir(parents=True)
-        for i in range(10, 10 + image_count + 1):
-            filename = plate_directory2 / ("98ac_%02dA_1.jpg" % (i))
+        nobarcode_extra_images = 3
+        for i in range(10, 10 + image_count + nobarcode_extra_images):
+            filename = plate_directory2 / ("%s_%02dA_1.jpg" % (nobarcode_barcode, i))
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make yet another scrapable directory with a different barcode.
-        plate_directory3 = plates_directory / "98ad_2023-04-06_RI1000-0276-3drop"
+        # This one gets moved into novisit since it matches a plate with a bad visit name.
+        plate_directory3 = (
+            plates_directory / f"{novisit_barcode}_2023-04-06_RI1000-0276-3drop"
+        )
         plate_directory3.mkdir(parents=True)
-        for i in range(10, 10 + image_count + 2):
-            filename = plate_directory3 / ("98ad_%02dA_1.jpg" % (i))
+        for i in range(10, 10 + image_count):
+            filename = plate_directory3 / ("%s_%02dA_1.jpg" % (novisit_barcode, i))
+            with open(filename, "w") as stream:
+                stream.write("")
+
+        # Make yet another scrapable directory with a different barcode.
+        # This one gets completely ignored because it's not in the explicit list.
+        plate_directory4 = (
+            plates_directory / f"{excluded_barcode}_2023-04-06_RI1000-0276-3drop"
+        )
+        plate_directory4.mkdir(parents=True)
+        excluded_extra_images = 2
+        for i in range(10, 10 + image_count + excluded_extra_images):
+            filename = plate_directory4 / ("%s_%02dA_1.jpg" % (excluded_barcode, i))
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Wait for all the images to appear.
         time0 = time.time()
         timeout = 5.0
         while True:
 
             # Get all images.
-            records = await xchembku.fetch_crystal_wells_filenames()
+            crystal_well_models = await xchembku.fetch_crystal_wells_filenames()
 
             # Stop looping when we got the images we expect.
-            if len(records) >= image_count:
+            if len(crystal_well_models) >= image_count:
                 break
 
             if time.time() - time0 > timeout:
                 raise RuntimeError(
-                    f"only {len(records)} images out of {image_count}"
+                    f"only {len(crystal_well_models)} images out of {image_count}"
                     f" registered within {timeout} seconds"
                 )
             await asyncio.sleep(1.0)
 
         # Wait a couple more seconds to make sure there are no extra images appearing.
         await asyncio.sleep(2.0)
 
+        # Make sure the crystal plate record got its collector stem recorded.
+        crystal_plate_models = await xchembku.fetch_crystal_plates(
+            CrystalPlateFilterModel()
+        )
+        assert crystal_plate_models[0].rockminer_collected_stem == plate_directory1.stem
+
         # Get all images in the database.
-        records = await xchembku.fetch_crystal_wells_filenames()
-        assert len(records) == image_count, "images after scraping"
+        crystal_well_models = await xchembku.fetch_crystal_wells_filenames()
+        assert len(crystal_well_models) == image_count, "images after scraping"
 
-        # The two plate directories should have been emptied.
+        # Make sure the positions got recorded right in the wells.
+        i = 10
+        for crystal_well_model in crystal_well_models:
+            assert crystal_well_model.position == f"{i}A1"
+            i += 1
+
+        # The three explicit plate directories should have been emptied.
         count = sum(1 for _ in plate_directory1.glob("*") if _.is_file())
         assert count == 0, "first plate_directory"
 
         count = sum(1 for _ in plate_directory2.glob("*") if _.is_file())
         assert count == 0, "second plate_directory"
 
-        # The third plate directory is left intact.
         count = sum(1 for _ in plate_directory3.glob("*") if _.is_file())
-        assert count == image_count + 2, "third plate_directory"
+        assert count == 0, "third plate_directory"
+
+        # The fourth plate directory is left intact.
+        count = sum(1 for _ in plate_directory4.glob("*") if _.is_file())
+        assert count == image_count + excluded_extra_images, "fourth plate_directory"
 
         # We should have ingested the first barcode.
-        count = sum(1 for _ in self.__ingested_directory.glob("*") if _.is_dir())
-        assert count == 1, f"ingested_directory {str(self.__ingested_directory)}"
+        count = sum(1 for _ in rockingester_directory.glob("*") if _.is_dir())
+        assert count == 1, f"rockingester_directory {str(rockingester_directory)}"
         count = sum(
             1
-            for _ in (self.__ingested_directory / plate_directory1.name).glob("*")
+            for _ in (rockingester_directory / plate_directory1.name).glob("*")
             if _.is_file()
         )
         assert (
             count == image_count
-        ), f"ingested_directory images {str(self.__ingested_directory)}"
+        ), f"ingested_directory images {str(rockingester_directory)}"
 
-        # We should have send the second barcode to the nobarcode area.
+        # We should have sent the second barcode to the nobarcode area.
         count = sum(1 for _ in self.__nobarcode_directory.glob("*") if _.is_dir())
         assert count == 1, f"nobarcode_directory {str(self.__nobarcode_directory)}"
         count = sum(
             1
             for _ in (self.__nobarcode_directory / plate_directory2.name).glob("*")
             if _.is_file()
         )
         assert (
-            count == image_count + 1
+            count == image_count + nobarcode_extra_images
         ), f"nobarcode_directory images {str(self.__nobarcode_directory)}"
 
+        # We should have sent the third barcode to the novisit area.
+        count = sum(1 for _ in self.__novisit_directory.glob("*") if _.is_dir())
+        assert count == 1, f"novisit_directory {str(self.__novisit_directory)}"
+        count = sum(
+            1
+            for _ in (self.__novisit_directory / plate_directory3.name).glob("*")
+            if _.is_file()
+        )
+        assert (
+            count == image_count
+        ), f"novisit_directory images {str(self.__novisit_directory)}"
+
     # ----------------------------------------------------------------------------------------
 
     async def __run_part2(self, image_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
```

