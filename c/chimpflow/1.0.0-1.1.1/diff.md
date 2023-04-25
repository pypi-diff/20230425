# Comparing `tmp/chimpflow-1.0.0.tar.gz` & `tmp/chimpflow-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chimpflow-1.0.0.tar", last modified: Sun Apr  9 09:29:21 2023, max compression
+gzip compressed data, was "chimpflow-1.1.1.tar", last modified: Tue Apr 25 09:09:33 2023, max compression
```

## Comparing `chimpflow-1.0.0.tar` & `chimpflow-1.1.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.093390 chimpflow-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.081390 chimpflow-1.0.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.081390 chimpflow-1.0.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.081390 chimpflow-1.0.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.081390 chimpflow-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.077390 chimpflow-1.0.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.081390 chimpflow-1.0.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 09:29:12.000000 chimpflow-1.0.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 09:29:12.000000 chimpflow-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-04-09 09:29:21.093390 chimpflow-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-09 09:29:12.000000 chimpflow-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-09 09:29:12.000000 chimpflow-1.0.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.077390 chimpflow-1.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.085390 chimpflow-1.0.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 09:29:12.000000 chimpflow-1.0.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-09 09:29:12.000000 chimpflow-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:29:21.093390 chimpflow-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.081390 chimpflow-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-04-09 09:29:21.000000 chimpflow-1.0.0/src/chimpflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-09 09:29:21.000000 chimpflow-1.0.0/src/chimpflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:29:21.000000 chimpflow-1.0.0/src/chimpflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 09:29:21.000000 chimpflow-1.0.0/src/chimpflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 09:29:21.000000 chimpflow-1.0.0/src/chimpflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-09 09:29:21.000000 chimpflow-1.0.0/src/chimpflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow_api/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:29:20.000000 chimpflow-1.0.0/src/chimpflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/base_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/chimp_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.089390 chimpflow-1.0.0/src/chimpflow_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.093390 chimpflow-1.0.0/src/chimpflow_lib/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-09 09:29:12.000000 chimpflow-1.0.0/src/chimpflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.093390 chimpflow-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.093390 chimpflow-1.0.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:29:21.093390 chimpflow-1.0.0/tests/echo_test_imgs/
--rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/echo_test_imgs/97wo_01A_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/echo_test_imgs/echo_test_im_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/echo_test_imgs/echo_test_im_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/test_chimp_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-09 09:29:12.000000 chimpflow-1.0.0/tests/test_miner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.288864 chimpflow-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.272864 chimpflow-1.1.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 09:09:18.000000 chimpflow-1.1.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 09:09:18.000000 chimpflow-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-04-25 09:09:33.284864 chimpflow-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-25 09:09:18.000000 chimpflow-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-25 09:09:18.000000 chimpflow-1.1.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.272864 chimpflow-1.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.276864 chimpflow-1.1.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 09:09:18.000000 chimpflow-1.1.1/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-25 09:09:18.000000 chimpflow-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 09:09:33.288864 chimpflow-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.272864 chimpflow-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/src/chimpflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/src/chimpflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/src/chimpflow_api/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/src/chimpflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.280864 chimpflow-1.1.1/src/chimpflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.284864 chimpflow-1.1.1/src/chimpflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 09:09:33.000000 chimpflow-1.1.1/src/chimpflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/base_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/chimp_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.284864 chimpflow-1.1.1/src/chimpflow_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.284864 chimpflow-1.1.1/src/chimpflow_lib/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-25 09:09:18.000000 chimpflow-1.1.1/src/chimpflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.284864 chimpflow-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.284864 chimpflow-1.1.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:09:33.284864 chimpflow-1.1.1/tests/echo_test_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)   156218 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/echo_test_imgs/97wo_01A_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   146361 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/echo_test_imgs/97wo_01A_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   142418 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/echo_test_imgs/97wo_01A_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/test_chimp_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-25 09:09:18.000000 chimpflow-1.1.1/tests/test_miner.py
```

### Comparing `chimpflow-1.0.0/.dae-devops/Makefile` & `chimpflow-1.1.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/docs/conventions.rst` & `chimpflow-1.1.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/docs/developing.rst` & `chimpflow-1.1.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/docs/devops.rst` & `chimpflow-1.1.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/docs/docs_structure.rst` & `chimpflow-1.1.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/docs/installing.rst` & `chimpflow-1.1.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/docs/testing.rst` & `chimpflow-1.1.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.dae-devops/project.yaml` & `chimpflow-1.1.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.devcontainer/Dockerfile` & `chimpflow-1.1.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.devcontainer/devcontainer.json` & `chimpflow-1.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/CONTRIBUTING.rst` & `chimpflow-1.1.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/actions/install_requirements/action.yml` & `chimpflow-1.1.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/dependabot.yml` & `chimpflow-1.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/pages/make_switcher.py` & `chimpflow-1.1.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/workflows/code.yml` & `chimpflow-1.1.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/workflows/docs.yml` & `chimpflow-1.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/workflows/docs_clean.yml` & `chimpflow-1.1.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.github/workflows/linkcheck.yml` & `chimpflow-1.1.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.gitignore` & `chimpflow-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.gitlab-ci.yml` & `chimpflow-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/.vscode/launch.json` & `chimpflow-1.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/LICENSE` & `chimpflow-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/PKG-INFO` & `chimpflow-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.0.0
+Version: 1.1.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `chimpflow-1.0.0/README.rst` & `chimpflow-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/configurations/development.yaml` & `chimpflow-1.1.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/docs/conf.py` & `chimpflow-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/docs/images/dls-favicon.ico` & `chimpflow-1.1.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/docs/images/dls-logo.svg` & `chimpflow-1.1.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/docs/index.rst` & `chimpflow-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/docs/user/explanations/25-docs-structure.rst` & `chimpflow-1.1.1/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/docs/user/index.rst` & `chimpflow-1.1.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/pyproject.toml` & `chimpflow-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow.egg-info/PKG-INFO` & `chimpflow-1.1.1/src/chimpflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chimpflow
-Version: 1.0.0
+Version: 1.1.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `chimpflow-1.0.0/src/chimpflow.egg-info/SOURCES.txt` & `chimpflow-1.1.1/src/chimpflow.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -90,9 +90,9 @@
 tests/base.py
 tests/conftest.py
 tests/test_chimp_adapter.py
 tests/test_miner.py
 tests/configurations/direct_poll.yaml
 tests/configurations/service.yaml
 tests/echo_test_imgs/97wo_01A_1.jpg
-tests/echo_test_imgs/echo_test_im_1.jpg
-tests/echo_test_imgs/echo_test_im_3.jpg
+tests/echo_test_imgs/97wo_01A_2.jpg
+tests/echo_test_imgs/97wo_01A_3.jpg
```

### Comparing `chimpflow-1.0.0/src/chimpflow_api/context_base.py` & `chimpflow-1.1.1/src/chimpflow_api/context_base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_api/exceptions.py` & `chimpflow-1.1.1/src/chimpflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_api/miners/aiohttp.py` & `chimpflow-1.1.1/src/chimpflow_api/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_api/miners/context.py` & `chimpflow-1.1.1/src/chimpflow_api/miners/context.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_api/miners/miners.py` & `chimpflow-1.1.1/src/chimpflow_api/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_api/thing.py` & `chimpflow-1.1.1/src/chimpflow_api/thing.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_api/things.py` & `chimpflow-1.1.1/src/chimpflow_api/things.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_cli/main.py` & `chimpflow-1.1.1/src/chimpflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_cli/subcommands/base.py` & `chimpflow-1.1.1/src/chimpflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_cli/subcommands/service.py` & `chimpflow-1.1.1/src/chimpflow_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_cli/version.py` & `chimpflow-1.1.1/src/chimpflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/__main__.py` & `chimpflow-1.1.1/src/chimpflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/chimp_adapter.py` & `chimpflow-1.1.1/src/chimpflow_lib/chimp_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import warnings
 from pathlib import Path
 from typing import Dict
 
+from dls_utilpack.describe import describe
 from dls_utilpack.require import require
 from xchem_chimp.detector.coord_generator import ChimpXtalCoordGenerator, PointsMode
 from xchembku_api.models.crystal_well_autolocation_model import (
     CrystalWellAutolocationModel,
 )
 from xchembku_api.models.crystal_well_model import CrystalWellModel
 
@@ -58,14 +59,17 @@
         Returns:
             CrystalWellAutolocationModel: The autolocation data mined from the image for the crystal well.
         """
 
         # Filename is full path to the input filename.
         filename: Path = Path(crystal_well_model.filename)
 
+        if not filename.exists():
+            raise RuntimeError(f"could not find file {str(filename)}")
+
         # Make a detector object.
         # TODO: Arrange ChimpDetector internals so that we only have to load
         # the torch model once per server, instead of once per detection request.
         detector = ChimpDetector(
             self.__model_path,
             [str(filename)],
             self.__num_classes,
@@ -77,35 +81,41 @@
         )
 
         # Extract the crystal coordinates.
         coord_generator.extract_coordinates()
 
         # Calculate well centers.
         coord_generator.calculate_well_centres()
+
+        # Get the output stucture for the first (only) image.
+        # TODO: Store the chimp detector output structure as json in the database.
         output_dict = coord_generator.combined_coords_list[0]
 
+        logger.debug(describe("output_dict", output_dict))
+
         # Construct a new autolocation object to hold the results.
         model = CrystalWellAutolocationModel(
             crystal_well_uuid=crystal_well_model.uuid,
         )
         model.drop_detected = output_dict["drop_detected"]
         target_position = output_dict["echo_coordinate"]
         if len(target_position) > 0:
             # The target position is a list of (np.int64, np.int64), so have to convert to int.
+            # Coordinate pairs are vertical-first.
             # TODO: Change the CrystalWellAutolocationModel to do type checking on field assignment.
-            model.auto_target_position_x = int(target_position[0][0])
-            model.auto_target_position_y = int(target_position[0][1])
+            model.auto_target_x = int(target_position[0][1])
+            model.auto_target_y = int(target_position[0][0])
         well_centroid = output_dict["well_centroid"]
         if well_centroid is not None:
-            model.well_centroid_x = int(well_centroid[0])
-            model.well_centroid_y = int(well_centroid[1])
+            model.well_centroid_x = int(well_centroid[1])
+            model.well_centroid_y = int(well_centroid[0])
         model.number_of_crystals = len(output_dict["xtal_coordinates"])
 
-        # We store the crystal coordinates in the model too.
-        model.crystal_coordinates = list(output_dict["xtal_coordinates"])
+        # TODO: Store the chimp detected crystal coordinates in the model too.
+        # model.crystal_coordinates = list(output_dict["xtal_coordinates"])
 
         # request_dict[ImageFieldnames.FILENAME] = str(im_path)
         # if output_dict["drop_detected"] is True:
         #     request_dict[ImageFieldnames.IS_DROP] = True
         #     echo_y, echo_x = output_dict["echo_coordinate"][0]
         #     request_dict[ImageFieldnames.TARGET_POSITION_Y] = int(echo_y)
         #     request_dict[ImageFieldnames.TARGET_POSITION_X] = int(echo_x)
```

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/contexts/base.py` & `chimpflow-1.1.1/src/chimpflow_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/exceptions.py` & `chimpflow-1.1.1/src/chimpflow_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/miners/aiohttp.py` & `chimpflow-1.1.1/src/chimpflow_lib/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/miners/base.py` & `chimpflow-1.1.1/src/chimpflow_lib/miners/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/miners/context.py` & `chimpflow-1.1.1/src/chimpflow_lib/miners/context.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/miners/direct_poll.py` & `chimpflow-1.1.1/src/chimpflow_lib/miners/direct_poll.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/miners/miners.py` & `chimpflow-1.1.1/src/chimpflow_lib/miners/miners.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/src/chimpflow_lib/version.py` & `chimpflow-1.1.1/src/chimpflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/base.py` & `chimpflow-1.1.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/configurations/direct_poll.yaml` & `chimpflow-1.1.1/tests/configurations/direct_poll.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -13,7 +13,9 @@
     type: "chimpflow_lib.miners.direct_poll"
     type_specific_tbd:
         chimp_adapter:
             # In pytest conftest.py, this file gets downloaded from Zenodo.
             model_path: "2022-12-07_CHiMP_Mask_R_CNN_XChem_50eph_VMXi_finetune_DICT_NZ.pytorch"
             num_classes: 3
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
+    context:
+        start_as: direct
```

### Comparing `chimpflow-1.0.0/tests/configurations/service.yaml` & `chimpflow-1.1.1/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/conftest.py` & `chimpflow-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/echo_test_imgs/97wo_01A_1.jpg` & `chimpflow-1.1.1/tests/echo_test_imgs/97wo_01A_1.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/echo_test_imgs/echo_test_im_1.jpg` & `chimpflow-1.1.1/tests/echo_test_imgs/97wo_01A_2.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/echo_test_imgs/echo_test_im_3.jpg` & `chimpflow-1.1.1/tests/echo_test_imgs/97wo_01A_3.jpg`

 * *Files identical despite different names*

### Comparing `chimpflow-1.0.0/tests/test_miner.py` & `chimpflow-1.1.1/tests/test_miner.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,22 +127,23 @@
             visit=visit,
         )
 
         await xchembku.upsert_crystal_plates([crystal_plate_model])
 
         # Make a well model to serve as the input to the autolocation finder.
         crystal_well_model = CrystalWellModel(
-            filename="tests/echo_test_imgs/echo_test_im_3.jpg",
+            position="01A_1",
+            filename="tests/echo_test_imgs/97wo_01A_1.jpg",
             crystal_plate_uuid=crystal_plate_model.uuid,
         )
-        await xchembku.originate_crystal_wells([crystal_well_model])
+        await xchembku.upsert_crystal_wells([crystal_well_model])
 
         # Wait long enough for the miner to activate and start ticking and pick up the work and do it.
         time0 = time.time()
-        timeout = 10.0
+        timeout = 30.0
         while True:
 
             # Get all which have gotten autolocations from the xchem-chimp.
             records = await xchembku.fetch_crystal_wells_needing_droplocation(
                 CrystalWellFilterModel()
             )
```

