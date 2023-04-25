# Comparing `tmp/echolocator-0.0.1.tar.gz` & `tmp/echolocator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-0.0.1.tar", last modified: Sat Feb  4 09:07:37 2023, max compression
+gzip compressed data, was "echolocator-1.0.1.tar", last modified: Tue Apr 25 05:07:33 2023, max compression
```

## Comparing `echolocator-0.0.1.tar` & `echolocator-1.0.1.tar`

### file list

```diff
@@ -1,264 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.615996 echolocator-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-04 09:07:28.000000 echolocator-0.0.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-04 09:07:28.000000 echolocator-0.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-02-04 09:07:28.000000 echolocator-0.0.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.587995 echolocator-0.0.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-04 09:07:28.000000 echolocator-0.0.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-04 09:07:28.000000 echolocator-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-02-04 09:07:28.000000 echolocator-0.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-04 09:07:28.000000 echolocator-0.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-04 09:07:28.000000 echolocator-0.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-04 09:07:28.000000 echolocator-0.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-04 09:07:28.000000 echolocator-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-04 09:07:28.000000 echolocator-0.0.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-04 09:07:28.000000 echolocator-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-02-04 09:07:28.000000 echolocator-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-02-04 09:07:37.615996 echolocator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-04 09:07:28.000000 echolocator-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-02-04 09:07:28.000000 echolocator-0.0.1/configurations/development.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-04 09:07:28.000000 echolocator-0.0.1/configurations/tutorial.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/1_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/1_tutorials/101_run_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/1_tutorials/102_update_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/1_tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/2_how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/2_how-to/201_add_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/2_how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/3_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/3_explanations/301_naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/3_explanations/302_process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/3_explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/4_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/4_reference/402_building_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/4_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.595995 echolocator-0.0.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.599995 echolocator-0.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/image_details.png
--rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/image_list.png
--rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/images/swiss3.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-04 09:07:28.000000 echolocator-0.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.599995 echolocator-0.0.1/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-04 09:07:28.000000 echolocator-0.0.1/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-04 09:07:28.000000 echolocator-0.0.1/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-02-04 09:07:28.000000 echolocator-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 09:07:37.615996 echolocator-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.591995 echolocator-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.599995 echolocator-0.0.1/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.599995 echolocator-0.0.1/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.599995 echolocator-0.0.1/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.599995 echolocator-0.0.1/src/echolocator_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-04 09:07:37.000000 echolocator-0.0.1/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/collectors/scrape_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_lib/configurators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/configurators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/configurators/configurators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/configurators/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/contexts/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/contexts/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.603996 echolocator-0.0.1/src/echolocator_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.591995 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.591995 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.607996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.591995 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.591995 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.611996 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/targeting.html
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/guis/html/targeting.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-04 09:07:28.000000 echolocator-0.0.1/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.615996 echolocator-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.615996 echolocator-0.0.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/configurations/laptop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.615996 echolocator-0.0.1/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.615996 echolocator-0.0.1/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/test_gui_image_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/test_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 09:07:37.615996 echolocator-0.0.1/tests/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-04 09:07:28.000000 echolocator-0.0.1/tests/tutorials/tutorial2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.023209 echolocator-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.999209 echolocator-1.0.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.999209 echolocator-1.0.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 05:07:24.000000 echolocator-1.0.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-25 05:07:24.000000 echolocator-1.0.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-25 05:07:24.000000 echolocator-1.0.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.983209 echolocator-1.0.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.003209 echolocator-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-25 05:07:24.000000 echolocator-1.0.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 05:07:24.000000 echolocator-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-25 05:07:24.000000 echolocator-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-25 05:07:24.000000 echolocator-1.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 05:07:24.000000 echolocator-1.0.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 05:07:24.000000 echolocator-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-25 05:07:24.000000 echolocator-1.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-25 05:07:33.023209 echolocator-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-25 05:07:24.000000 echolocator-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 05:07:24.000000 echolocator-1.0.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/1_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/1_tutorials/101_run_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/1_tutorials/102_update_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/1_tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/2_how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/2_how-to/201_add_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/2_how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/3_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/3_explanations/301_naming_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/3_explanations/302_process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/3_explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/4_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/4_reference/402_building_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/4_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/image_details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/image_list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/images/swiss3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 05:07:24.000000 echolocator-1.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.007209 echolocator-1.0.1/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-25 05:07:24.000000 echolocator-1.0.1/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 05:07:24.000000 echolocator-1.0.1/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-25 05:07:24.000000 echolocator-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 05:07:33.023209 echolocator-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.987209 echolocator-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 05:07:32.000000 echolocator-1.0.1/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.011209 echolocator-1.0.1/src/echolocator_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.015209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:32.991209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 05:07:24.000000 echolocator-1.0.1/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.019209 echolocator-1.0.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.023209 echolocator-1.0.1/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:07:33.023209 echolocator-1.0.1/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-04-25 05:07:24.000000 echolocator-1.0.1/tests/test_fetch_images.py
```

### Comparing `echolocator-0.0.1/.dae-devops/Makefile` & `echolocator-1.0.1/.dae-devops/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint fa91d06926a32d8ff4980e6c5026842a
+# dae_devops_fingerprint e508c365997a16fba9003f0e2c7345fc
```

### Comparing `echolocator-0.0.1/.dae-devops/docs/developing.rst` & `echolocator-1.0.1/.dae-devops/docs/developing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.2.
 .. # ********** For repository_name echolocator
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
@@ -32,8 +32,8 @@
 If you plan to modify the docs, you will need to::
 
     $ pip install -e .[docs]
 
     
 
 
-.. # dae_devops_fingerprint c3acd7bd04d4c567174c7ba12f90efb0
+.. # dae_devops_fingerprint 8802592ab610cd9de3e657aeacb9c8c1
```

### Comparing `echolocator-0.0.1/.dae-devops/docs/devops.rst` & `echolocator-1.0.1/.dae-devops/docs/devops.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.2.
 .. # ********** For repository_name echolocator
 
 Devops
 =======================================================================
 
 There exists a a configuration file called ``.dae-devops/project.yaml``.
 
@@ -39,8 +39,8 @@
 Publishing::
 
     $ make -f .dae-devops/Makefile publish_pip
     $ make -f .dae-devops/Makefile publish_docs
     
 
 
-.. # dae_devops_fingerprint 28cb19a7e59bd4e67a85edec626a491e
+.. # dae_devops_fingerprint 67a3e9939abb47f483bfd1180117473f
```

### Comparing `echolocator-0.0.1/.dae-devops/docs/docs_structure.rst` & `echolocator-1.0.1/.dae-devops/docs/docs_structure.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.2.
 .. # ********** For repository_name echolocator
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 8ded9698d9d71eda17e2c49cd737a2e2
+.. # dae_devops_fingerprint 58611b915d52f7b59bbed09020e30356
```

### Comparing `echolocator-0.0.1/.dae-devops/docs/installing.rst` & `echolocator-1.0.1/.dae-devops/docs/installing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.2.
 .. # ********** For repository_name echolocator
 
 Installing
 =======================================================================
 
 
 You will need python 3.9 or later. 
@@ -36,8 +36,8 @@
 
 The library should now be installed and the commandline interface on your path.
 You can check the version that has been installed by typing::
 
     $ echolocator --version
     $ echolocator --version-json
 
-.. # dae_devops_fingerprint 3b5d52d009337767488822fafe22e1e7
+.. # dae_devops_fingerprint c6472f1053e4ee44f3e70cc67c9fbddd
```

### Comparing `echolocator-0.0.1/.dae-devops/docs/testing.rst` & `echolocator-1.0.1/.dae-devops/docs/testing.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.2.
 .. # ********** For repository_name echolocator
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
@@ -31,8 +31,8 @@
 
 The tests clear their directory when they start, but not when they finish.
 This allows peeking in there to see what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint a5fefb92ded789eda5a2e4423a4e58e6
+.. # dae_devops_fingerprint 7daed3c9e65a523a0fbf7d347dfa6ebe
```

### Comparing `echolocator-0.0.1/.devcontainer/Dockerfile` & `echolocator-1.0.1/.devcontainer/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["echolocator"]
 CMD ["--version"]
 
-# dae_devops_fingerprint b2386a8edacc7cf00dbcde0bcfe434a4
+# dae_devops_fingerprint 9302e007f97570a60d29bb25449a92bb
```

### Comparing `echolocator-0.0.1/.devcontainer/devcontainer.json` & `echolocator-1.0.1/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.1.
+// ********** It has been generated automatically by dae_devops version 0.5.2.
 // ********** For repository_name echolocator
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint 2507140a2722f4fa02e13592d5038e0e
+// dae_devops_fingerprint 529b4c792a9fdad91835e1a4b32e0138
```

### Comparing `echolocator-0.0.1/.github/CONTRIBUTING.rst` & `echolocator-1.0.1/.github/CONTRIBUTING.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.2.
 .. # ********** For repository_name echolocator
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/echolocator/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint aed6364e5eff2f9face6b54b84a417f7
+.. # dae_devops_fingerprint d17faed109d26c120150d4cad9b012bd
```

### Comparing `echolocator-0.0.1/.github/actions/install_requirements/action.yml` & `echolocator-1.0.1/.github/actions/install_requirements/action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint 6290682d4770755c7566572965cef561
+# dae_devops_fingerprint 1fae1b6e8b391bfca7aad4310624e6c4
```

### Comparing `echolocator-0.0.1/.github/pages/make_switcher.py` & `echolocator-1.0.1/.github/pages/make_switcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint 5eddb1e43a2e9f5696fb135b3351e1e0
+# dae_devops_fingerprint e707603d7cbd385a51462ce91214bed6
```

### Comparing `echolocator-0.0.1/.github/workflows/code.yml` & `echolocator-1.0.1/.github/workflows/code.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -208,8 +208,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 3cd3d1b7aa3767bc7752d04d0cff1b98
+# dae_devops_fingerprint febe27315441a7232f0895dff16de450
```

### Comparing `echolocator-0.0.1/.github/workflows/docs.yml` & `echolocator-1.0.1/.github/workflows/docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint 516501c026fa1f7af1e7a6d88d046406
+# dae_devops_fingerprint 248b6927066389c57cb985f999015228
```

### Comparing `echolocator-0.0.1/.github/workflows/docs_clean.yml` & `echolocator-1.0.1/.github/workflows/docs_clean.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint 923700bb09fb043a8cdcb2b78e384f09
+# dae_devops_fingerprint 13b4db6f5b6317157d8d36b632434d2d
```

### Comparing `echolocator-0.0.1/.github/workflows/linkcheck.yml` & `echolocator-1.0.1/.github/workflows/linkcheck.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 name: Link Check
 
 on:
   workflow_dispatch:
   schedule:
@@ -23,8 +23,8 @@
         with:
           requirements_file: requirements-dev-3.x.txt
           install_options: -e .[dev]
 
       - name: Check links
         run: tox -e docs build -- -b linkcheck
 
-# dae_devops_fingerprint d1ce8eee255cbe72206419b8b28d43df
+# dae_devops_fingerprint 75b08200910c30409c75d4d16a6e4d9a
```

### Comparing `echolocator-0.0.1/.gitignore` & `echolocator-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/.gitlab-ci.yml` & `echolocator-1.0.1/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 32c6a111d128370b1daac92e1f2aecbe
+# dae_devops_fingerprint 14d3e80d54ae3da9497b0ce79d6fa611
```

### Comparing `echolocator-0.0.1/.vscode/launch.json` & `echolocator-1.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/LICENSE` & `echolocator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/Makefile` & `echolocator-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/PKG-INFO` & `echolocator-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 0.0.1
+Version: 1.0.1
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -238,12 +238,8 @@
 
 ---------------------------
 Viewing the docs
 ---------------------------
 
 You can view the docs from Diamond's internal server
 
-    http://www.cs.diamond.ac.uk/reports/gitlab-ci/echolocator/docs/latest/index.html
-
-Or from the cloned repository
-
-    file:///source_path/echolocator/public/index.html
+    https://diamondlightsource.github.io/echolocator
```

### Comparing `echolocator-0.0.1/README.rst` & `echolocator-1.0.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -19,12 +19,8 @@
 
 ---------------------------
 Viewing the docs
 ---------------------------
 
 You can view the docs from Diamond's internal server
 
-    http://www.cs.diamond.ac.uk/reports/gitlab-ci/echolocator/docs/latest/index.html
-
-Or from the cloned repository
-
-    file:///source_path/echolocator/public/index.html
+    https://diamondlightsource.github.io/echolocator
```

### Comparing `echolocator-0.0.1/docs/1_tutorials/101_run_conda.rst` & `echolocator-1.0.1/docs/1_tutorials/101_run_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/1_tutorials/102_update_image.rst` & `echolocator-1.0.1/docs/1_tutorials/102_update_image.rst`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/2_how-to/201_add_fields.rst` & `echolocator-1.0.1/docs/2_how-to/201_add_fields.rst`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/3_explanations/301_naming_conventions.rst` & `echolocator-1.0.1/docs/3_explanations/301_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/3_explanations/302_process.rst` & `echolocator-1.0.1/docs/3_explanations/302_process.rst`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/4_reference/402_building_conda.rst` & `echolocator-1.0.1/docs/4_reference/402_building_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/_static/theme_overrides.css` & `echolocator-1.0.1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/conf.py` & `echolocator-1.0.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 20b12f1e3c3fe99e0b1b302ef56d79fc
+# dae_devops_fingerprint 522695c29baed7676543987e99fc61dd
```

### Comparing `echolocator-0.0.1/docs/images/dls-favicon.ico` & `echolocator-1.0.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/images/dls-logo.svg` & `echolocator-1.0.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/images/excalidraw-example.svg` & `echolocator-1.0.1/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/images/git_merge.png` & `echolocator-1.0.1/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/images/image_details.png` & `echolocator-1.0.1/docs/images/image_details.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/images/image_list.png` & `echolocator-1.0.1/docs/images/image_list.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/docs/images/swiss3.png` & `echolocator-1.0.1/docs/images/swiss3.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/modulefiles/conda` & `echolocator-1.0.1/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/pyproject.toml` & `echolocator-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.2.
 # ********** For repository_name echolocator
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -12,15 +12,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "XChem GUI for manually targeting drop points for the Echo dispenser."
-dependencies = ["dls_servbase", "dls_mainiac", "dls_utilpack"]
+dependencies = ["xchembku", "dls_servbase", "dls_mainiac", "dls_utilpack", "beautifulsoup4"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
@@ -30,14 +30,15 @@
     "Flake8-pyproject",
     "pipdeptree",
     "pre-commit",
     "pytest-cov",
     "pydocstyle[toml]",
     "tox-direct",
     "types-mock",
+    "types-PyYAML",
 ]
 docs = [
     "pydata-sphinx-theme>=0.12",
     "sphinx-argparse",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
@@ -98,8 +99,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 69fbb150408506fd907682cb5b2f8e24
+# dae_devops_fingerprint 8d6ec2f437b47d4156e639a67957fdc1
```

### Comparing `echolocator-0.0.1/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.0.1/src/echolocator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 0.0.1
+Version: 1.0.1
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -238,12 +238,8 @@
 
 ---------------------------
 Viewing the docs
 ---------------------------
 
 You can view the docs from Diamond's internal server
 
-    http://www.cs.diamond.ac.uk/reports/gitlab-ci/echolocator/docs/latest/index.html
-
-Or from the cloned repository
-
-    file:///source_path/echolocator/public/index.html
+    https://diamondlightsource.github.io/echolocator
```

### Comparing `echolocator-0.0.1/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.0.1/src/echolocator.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 .github/workflows/docs_clean.yml
 .github/workflows/linkcheck.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 configurations/development.yaml
-configurations/tutorial.yaml
 docs/1_tutorials.rst
 docs/2_how-to.rst
 docs/3_explanations.rst
 docs/4_reference.rst
 docs/conf.py
 docs/index.rst
 docs/1_tutorials/101_run_conda.rst
@@ -60,66 +59,39 @@
 src/echolocator.egg-info/entry_points.txt
 src/echolocator.egg-info/requires.txt
 src/echolocator.egg-info/top_level.txt
 src/echolocator_api/__init__.py
 src/echolocator_api/aiohttp_client.py
 src/echolocator_api/context_base.py
 src/echolocator_api/exceptions.py
-src/echolocator_api/thing.py
-src/echolocator_api/things.py
-src/echolocator_api/databases/__init__.py
 src/echolocator_api/databases/constants.py
-src/echolocator_api/datafaces/__init__.py
-src/echolocator_api/datafaces/aiohttp.py
-src/echolocator_api/datafaces/constants.py
-src/echolocator_api/datafaces/context.py
-src/echolocator_api/datafaces/datafaces.py
+src/echolocator_api/guis/__init__.py
+src/echolocator_api/guis/aiohttp.py
+src/echolocator_api/guis/constants.py
+src/echolocator_api/guis/context.py
+src/echolocator_api/guis/guis.py
 src/echolocator_cli/__init__.py
 src/echolocator_cli/main.py
 src/echolocator_cli/version.py
 src/echolocator_cli/subcommands/__init__.py
 src/echolocator_cli/subcommands/base.py
-src/echolocator_cli/subcommands/start_services.py
+src/echolocator_cli/subcommands/service.py
 src/echolocator_lib/__init__.py
 src/echolocator_lib/__main__.py
 src/echolocator_lib/_version.py
 src/echolocator_lib/base_aiohttp.py
 src/echolocator_lib/envvar.py
 src/echolocator_lib/version.py
-src/echolocator_lib/collectors/__init__.py
-src/echolocator_lib/collectors/aiohttp.py
-src/echolocator_lib/collectors/base.py
-src/echolocator_lib/collectors/collectors.py
-src/echolocator_lib/collectors/constants.py
-src/echolocator_lib/collectors/context.py
-src/echolocator_lib/collectors/manual.py
-src/echolocator_lib/collectors/scrape_to_database.py
 src/echolocator_lib/composers/__init__.py
 src/echolocator_lib/composers/composers.py
 src/echolocator_lib/composers/html.py
 src/echolocator_lib/composers/prettyhelper.py
 src/echolocator_lib/composers/text.py
-src/echolocator_lib/configurators/__init__.py
-src/echolocator_lib/configurators/base.py
-src/echolocator_lib/configurators/configurators.py
-src/echolocator_lib/configurators/yaml.py
 src/echolocator_lib/contexts/__init__.py
 src/echolocator_lib/contexts/base.py
-src/echolocator_lib/contexts/classic.py
-src/echolocator_lib/contexts/contexts.py
-src/echolocator_lib/databases/__init__.py
-src/echolocator_lib/databases/aiosqlite.py
-src/echolocator_lib/databases/database_definition.py
-src/echolocator_lib/databases/databases.py
-src/echolocator_lib/databases/table_definitions.py
-src/echolocator_lib/datafaces/__init__.py
-src/echolocator_lib/datafaces/aiohttp.py
-src/echolocator_lib/datafaces/aiosqlite.py
-src/echolocator_lib/datafaces/context.py
-src/echolocator_lib/datafaces/datafaces.py
 src/echolocator_lib/guis/__init__.py
 src/echolocator_lib/guis/aiohttp.py
 src/echolocator_lib/guis/base.py
 src/echolocator_lib/guis/constants.py
 src/echolocator_lib/guis/context.py
 src/echolocator_lib/guis/guis.py
 src/echolocator_lib/guis/html/index.html
@@ -172,26 +144,20 @@
 src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
 src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
 src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
 src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
 src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
 tests/__init__.py
 tests/base.py
-tests/base_context_tester.py
-tests/base_specification_tester.py
-tests/base_tester.py
 tests/conftest.py
-tests/test_configurator.py
-tests/test_database.py
-tests/test_dataface.py
-tests/test_gui.py
-tests/test_gui_image_edit.py
-tests/test_tutorial.py
-tests/configurations/laptop.yaml
+tests/test_droplocation.py
+tests/test_export.py
+tests/test_fetch_image.py
+tests/test_fetch_images.py
+tests/configurations/service.yaml
 tests/example_images/1.jpg
 tests/example_images/2.jpg
 tests/example_images/3.jpg
 tests/example_images/4.png
 tests/images/1.jpg
 tests/images/2.jpg
-tests/images/3.jpg
-tests/tutorials/tutorial2.py
+tests/images/3.jpg
```

### Comparing `echolocator-0.0.1/src/echolocator_api/context_base.py` & `echolocator-1.0.1/src/echolocator_api/context_base.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_api/databases/constants.py` & `echolocator-1.0.1/src/echolocator_api/databases/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,14 @@
     CREATED_ON = CommonFieldnames.CREATED_ON
     FILENAME = "filename"
     ERROR = "error"
     WIDTH = "width"
     HEIGHT = "height"
     WELL_CENTER_X = "well_center_x"
     WELL_CENTER_Y = "well_center_y"
-    TARGET_POSITION_X = "target_position_x"
-    TARGET_POSITION_Y = "target_position_y"
+    TARGET_POSITION_X = "confirmed_target_x"
+    TARGET_POSITION_Y = "confirmed_target_y"
     PLATE_TYPE = "plate_type"
     CRYSTAL_PROBABILITY = "crystal_probability"
     NUMBER_OF_CRYSTALS = "number_of_crystals"
     IS_DROP = "is_drop"
     IS_USABLE = "is_usable"
```

### Comparing `echolocator-0.0.1/src/echolocator_api/datafaces/aiohttp.py` & `echolocator-1.0.1/src/echolocator_api/guis/aiohttp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 
 # Class for an aiohttp client.
 from echolocator_api.aiohttp_client import AiohttpClient
 
 # Dataface protocolj things.
-from echolocator_api.datafaces.constants import Commands, Keywords
+from echolocator_api.guis.constants import Commands, Keywords
 
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------------------
 class Aiohttp:
     """
-    Object implementing client side API for talking to the echolocator_dataface server.
+    Object implementing client side API for talking to the echolocator_gui server.
     Please see doctopic [A01].
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None):
         self.__specification = specification
 
@@ -25,65 +25,19 @@
         )
 
     # ----------------------------------------------------------------------------------------
     def specification(self):
         return self.__specification
 
     # ----------------------------------------------------------------------------------------
-    async def query(self, sql, subs=None, why=None):
-        """"""
-        return await self.__send_protocolj("query", sql, subs=subs, why=why)
-
-    # ----------------------------------------------------------------------------------------
-    async def execute(self, sql, subs=None, why=None):
-        """"""
-        return await self.__send_protocolj("execute", sql, subs=subs, why=why)
-
-    # ----------------------------------------------------------------------------------------
-    async def insert(self, table_name, records, why=None):
-        """"""
-        return await self.__send_protocolj("insert", table_name, records, why=why)
-
-    # ----------------------------------------------------------------------------------------
-    async def update(self, table_name, record, where, subs=None, why=None):
-        """"""
-        return await self.__send_protocolj(
-            "update", table_name, record, where, subs=subs, why=why
-        )
-
-    # ----------------------------------------------------------------------------------------
-    async def update_image(self, record, why=None):
-        """"""
-
-        return await self.__send_protocolj("update_image", record, why=why)
-
-    # ----------------------------------------------------------------------------------------
     async def report_health(self):
         """"""
         return await self.__send_protocolj("report_health")
 
     # ----------------------------------------------------------------------------------------
-    async def set_cookie(self, cookie_dict):
-        """ """
-        return await self.__send_protocolj("set_cookie", cookie_dict)
-
-    # ----------------------------------------------------------------------------------------
-    async def get_cookie(self, cookie_uuid):
-        """
-        Get single cookie from its uuid.
-        Returns database record format.
-        """
-        return await self.__send_protocolj("get_cookie", cookie_uuid)
-
-    # ----------------------------------------------------------------------------------------
-    async def update_cookie(self, row):
-        """"""
-        return await self.__send_protocolj("update_cookie", row)
-
-    # ----------------------------------------------------------------------------------------
     async def __send_protocolj(self, function, *args, **kwargs):
         """"""
 
         return await self.__aiohttp_client.client_protocolj(
             {
                 Keywords.COMMAND: Commands.EXECUTE,
                 Keywords.PAYLOAD: {
```

### Comparing `echolocator-0.0.1/src/echolocator_api/datafaces/context.py` & `echolocator-1.0.1/src/echolocator_api/guis/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import logging
 
 # Base class.
 from echolocator_api.context_base import ContextBase
 
 # Things created in the context.
-from echolocator_api.datafaces.datafaces import (
-    Datafaces,
-    echolocator_datafaces_set_default,
-)
+from echolocator_api.guis.guis import Guis, echolocator_guis_set_default
 
 logger = logging.getLogger(__name__)
 
 
 class Context(ContextBase):
     """
-    Client context for a echolocator_dataface object.
+    Client context for a echolocator_gui object.
     On entering, it creates the object according to the specification (a dict).
     On exiting, it closes client connection.
 
     The aenter and aexit methods are exposed for use by an enclosing context.
     """
 
     # ----------------------------------------------------------------------------------------
@@ -26,21 +23,21 @@
         self.__specification = specification
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
         # Build the object according to the specification.
-        self.interface = Datafaces().build_object(self.__specification)
+        self.interface = Guis().build_object(self.__specification)
 
-        # If there is more than one dataface, the last one defined will be the default.
-        echolocator_datafaces_set_default(self.interface)
+        # If there is more than one gui, the last one defined will be the default.
+        echolocator_guis_set_default(self.interface)
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
 
         if self.interface is not None:
             await self.interface.close_client_session()
 
             # Clear the global variable.  Important between pytests.
-            echolocator_datafaces_set_default(None)
+            echolocator_guis_set_default(None)
```

### Comparing `echolocator-0.0.1/src/echolocator_api/exceptions.py` & `echolocator-1.0.1/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_cli/main.py` & `echolocator-1.0.1/src/echolocator_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import multiprocessing
 
 # Base class with methods supporting MaxIV command-line programs.
 from dls_mainiac_lib.mainiac import Mainiac
 
 # The subcommands.
-from echolocator_cli.subcommands.start_services import StartServices
+from echolocator_cli.subcommands.service import Service
 
 # The package version.
 from echolocator_cli.version import meta as version_meta
 from echolocator_cli.version import version
 
 logger = logging.getLogger(__name__)
 
@@ -22,16 +22,16 @@
     def __init__(self, app_name):
         super().__init__(app_name)
 
     # ----------------------------------------------------------
     def run(self):
         """"""
 
-        if self._args.subcommand == "start_services":
-            StartServices(self._args, self).run()
+        if self._args.subcommand == "service":
+            Service(self._args, self).run()
 
         else:
             raise RuntimeError("unhandled subcommand %s" % (self._args.subcommand))
 
     # ----------------------------------------------------------
     def build_parser(self, arglist=None):
         """
@@ -57,16 +57,16 @@
         )
 
         # --------------------------------------------------------------------
         subparsers = parser.add_subparsers(help="subcommands", dest="subcommand")
         subparsers.required = True
 
         # --------------------------------------------------------------------
-        subparser = subparsers.add_parser("start_services", help="Start service(s).")
-        StartServices.add_arguments(subparser)
+        subparser = subparsers.add_parser("service", help="Start service (blocking).")
+        Service.add_arguments(subparser)
 
         return parser
 
     # --------------------------------------------------------------------------
     def configure_logging(self, settings=None):
         """
         Configure runtime logging, override base class.
```

### Comparing `echolocator-0.0.1/src/echolocator_cli/version.py` & `echolocator-1.0.1/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/__main__.py` & `echolocator-1.0.1/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/collectors/collectors.py` & `echolocator-1.0.1/src/echolocator_lib/composers/composers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,74 @@
 # Use standard logging in this module.
 import logging
 
+# Class managing list of things.
+from dls_utilpack.things import Things
+
 # Exceptions.
 from echolocator_api.exceptions import NotFound
 
-# Class managing list of things.
-from echolocator_api.things import Things
-
 logger = logging.getLogger(__name__)
 
 # -----------------------------------------------------------------------------------------
-__default_collector = None
+__default_composer = None
+
 
+def echolocator_composers_set_default(composer):
+    global __default_composer
+    __default_composer = composer
 
-def collectors_set_default(collector):
-    global __default_collector
-    __default_collector = collector
 
+def echolocator_composers_get_default():
+    global __default_composer
+    if __default_composer is None:
+        raise RuntimeError("echolocator_composers_get_default instance is None")
+    return __default_composer
 
-def collectors_get_default():
-    global __default_collector
-    if __default_collector is None:
-        raise RuntimeError("collectors_get_default instance is None")
-    return __default_collector
 
+def echolocator_composers_has_default():
+    global __default_composer
+    return __default_composer is not None
 
-class Collectors(Things):
+
+# -----------------------------------------------------------------------------------------
+
+
+class Composers(Things):
     """
-    List of available collectors.
+    List of available echolocator_composers.
     """
 
     # ----------------------------------------------------------------------------------------
-    def __init__(self, name="collectors"):
+    def __init__(self, name=None):
         Things.__init__(self, name)
 
     # ----------------------------------------------------------------------------------------
-    def build_object(self, specification, predefined_uuid=None):
+    def build_object(self, specification):
         """"""
 
-        collector_class = self.lookup_class(specification["type"])
+        composer_class = self.lookup_class(specification["type"])
 
         try:
-            collector_object = collector_class(
-                specification, predefined_uuid=predefined_uuid
-            )
+            composer_object = composer_class(specification)
         except Exception as exception:
             raise RuntimeError(
-                "unable to build collector object of class %s"
-                % (collector_class.__name__)
+                "unable to build composer object for type %s" % (composer_class)
             ) from exception
 
-        return collector_object
+        return composer_object
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
         """"""
 
-        if class_type == "dls_echolocator_lib.echolocator_collectors.aiohttp":
-            from echolocator_lib.collectors.aiohttp import Aiohttp
+        if class_type == "echolocator_lib.echolocator_composers.html":
+            from echolocator_lib.composers.html import Html
+
+            return Html
 
-            return Aiohttp
+        elif class_type == "echolocator_lib.echolocator_composers.text":
+            from echolocator_lib.composers.text import Text
 
-        elif class_type == "dls_echolocator_lib.echolocator_collectors.manual":
-            from echolocator_lib.collectors.manual import Manual
+            return Text
 
-            return Manual
-
-        elif (
-            class_type
-            == "dls_echolocator_lib.echolocator_collectors.scrape_to_database"
-        ):
-            from echolocator_lib.collectors.scrape_to_database import ScrapeToDatabase
-
-            return ScrapeToDatabase
-
-        else:
-            try:
-                RuntimeClass = Things.lookup_class(self, class_type)
-                return RuntimeClass
-            except NotFound:
-                raise NotFound("unable to get collector class for %s" % (class_type))
+        raise NotFound("unable to get composer class for type %s" % (class_type))
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/composers/html.py` & `echolocator-1.0.1/src/echolocator_lib/composers/html.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import html
 import logging
-import re
 from pathlib import Path
-from typing import Optional, Sequence, Union
+from typing import List, Optional, Sequence, Union
 
 import numpy as np
 
-# Database record field names coming from database fields.
-from echolocator_api.databases.constants import ImageFieldnames
-
 # Base class for generic things.
-from echolocator_api.thing import Thing
+from dls_utilpack.thing import Thing
+
+# Models which we can compose.
+from xchembku_api.models.crystal_well_needing_droplocation_model import (
+    CrystalWellNeedingDroplocationModel,
+)
 
 # Class to do the work using prettytable.
 from echolocator_lib.composers.prettyhelper import PrettyHelper
 
 logger = logging.getLogger(__name__)
 
 thing_type = "echolocator_lib.echolocator_composers.html"
@@ -34,29 +35,32 @@
         Thing.__init__(self, thing_type, specification)
 
         self.__prettyhelper = PrettyHelper()
 
         self.__indent = 0
 
     # ----------------------------------------------------------------------------------------
-    def compose_image_list(self, records):
+    def compose_image_list(self, models: List[CrystalWellNeedingDroplocationModel]):
         """
         Compose the image list as an html table.
         """
 
         field_names = [
-            {"text": "autoid", "class": "T_autoid"},
-            {"text": "filename", "class": "T_filename"},
-            {"text": "Barcode", "class": "T_barcode"},
-            {"text": "Subwell", "class": "T_plate_position"},
+            {"text": "uuid", "class": "T_uuid"},
+            {"text": "well", "class": "T_well"},
             {"text": "#Crystals", "class": "T_number_of_crystals"},
             {"text": "Offset x (\u03BCm)", "class": "T_real_space_target_x"},
             {"text": "Offset y (\u03BCm)", "class": "T_real_space_target_y"},
-            {"text": "drop?", "class": "T_is_drop"},
-            {"text": "use?", "class": "T_is_usable"},
+            {"text": "drop", "class": "T_is_drop"},
+            {"text": "well centroid x,y", "class": "T_well_centroid_x_y"},
+            {"text": "auto x,y", "class": "T_auto_target__x_y"},
+            {"text": "confirmed x,y", "class": "T_confirmed_target_x_y"},
+            {"text": "echo coordinate x,y", "class": "T_echo_coordinate_x_y"},
+            {"text": "use", "class": "T_is_usable"},
+            {"text": "error", "class": "T_error"},
         ]
 
         html_lines = []
 
         html_lines.append("<table>")
         html_lines.append("<thead>")
         html_lines.append("<tr>")
@@ -69,110 +73,116 @@
                 html_lines.append(f"<th>{field_name}</th>")
         html_lines.append("</tr>")
         html_lines.append("</thead>")
 
         html_lines.append("<tbody>")
 
         # Traverse all the given records.
-        for record in records:
-            autoid = record[ImageFieldnames.AUTOID]
-            error = record[ImageFieldnames.ERROR]
+        for model in models:
+            uuid = model.uuid
+            error = model.error
             if error is None:
                 error = "-"
-            html_lines.append(f"<tr autoid='{autoid}'>")
-            html_lines.append(f"<td>{autoid}</td>")
-            html_lines.append(
-                f"<td>{html.escape(record[ImageFieldnames.FILENAME])}</td>"
-            )
+            html_lines.append(f"<tr crystal_well_uuid='{uuid}'>")
+            html_lines.append(f"<td class='T_uuid'>{uuid}</td>")
 
             # Extract derived info from filename
-            filename = Path(record[ImageFieldnames.FILENAME]).name
-            barcode, plate_position = self.extract_plate_info_from_filename(
-                str(filename)
-            )
-
-            html_lines.append(f"<td>{barcode}</td>")
+            filestem = Path(model.filename).stem
 
-            html_lines.append(f"<td>{plate_position}</td>")
+            html_lines.append(
+                f"<td class='T_filename' title='{html.escape(model.filename)}'>{html.escape(filestem)}</td>"
+            )
 
-            t = record[ImageFieldnames.NUMBER_OF_CRYSTALS]
+            t = model.number_of_crystals
             if t is None:
                 t = "-"
             html_lines.append("<td id='number_of_crystals'>" + str(t) + "</td>")
 
-            target_x = record[ImageFieldnames.TARGET_POSITION_X]
-            target_y = record[ImageFieldnames.TARGET_POSITION_Y]
-            well_centre_x = record[ImageFieldnames.WELL_CENTER_X]
-            well_centre_y = record[ImageFieldnames.WELL_CENTER_Y]
+            target_x = model.auto_target_x
+            target_y = model.auto_target_y
+            well_centre_x = model.well_centroid_x
+            well_centre_y = model.well_centroid_y
             t = self.calculate_realspace_offset(
                 [target_y, target_x],
                 [well_centre_y, well_centre_x],
                 SCALE_FACTORS,
             )
             if t is None:
                 t = ["-", "-"]
-            html_lines.append("<td id='real_space_target_x'>" + str(t[1]) + "</td>")
-            html_lines.append("<td id='real_space_target_y'>" + str(t[0]) + "</td>")
+            html_lines.append(
+                "<td class='T_real_space_target_x' id='real_space_target_x'>"
+                + str(t[1])
+                + "</td>"
+            )
+            html_lines.append(
+                "<td class='T_real_space_target_y' id='real_space_target_y'>"
+                + str(t[0])
+                + "</td>"
+            )
 
-            t = record[ImageFieldnames.IS_DROP]
+            t = model.drop_detected
             if t is None:
                 t = "-"
             elif t:
                 t = "yes"
             else:
                 t = "no"
-            html_lines.append("<td id='is_drop'>" + str(t) + "</td>")
+            html_lines.append("<td class='T_is_drop'>" + str(t) + "</td>")
+
+            t = f"{model.well_centroid_x}, {model.well_centroid_y}"
+            html_lines.append("<td class='T_well_centroid_x_y'>" + t + "</td>")
+
+            t = f"{model.auto_target_x}, {model.auto_target_y}"
+            html_lines.append("<td class='T_auto_target_x_y'>" + t + "</td>")
+
+            if model.confirmed_target_x is None or model.confirmed_target_y is None:
+                t = "-"
+            else:
+                t = f"{model.confirmed_target_x}, {model.confirmed_target_y}"
+            html_lines.append("<td class='T_confirmed_target_x_y'>" + t + "</td>")
 
-            t = record[ImageFieldnames.IS_USABLE]
+            if model.echo_coordinate_x is None or model.echo_coordinate_y is None:
+                t = "-"
+            else:
+                t = f"{model.echo_coordinate_x}, {model.echo_coordinate_y}"
+            html_lines.append("<td class='T_echo_coordinate_x_y'>" + t + "</td>")
+
+            t = model.is_usable
             if t is None:
                 t = "-"
             elif t:
                 t = "yes"
             else:
                 t = "no"
-            html_lines.append("<td id='is_usable'>" + str(t) + "</td>")
+            html_lines.append("<td class='T_is_usable'>" + str(t) + "</td>")
 
-            html_lines.append("<td id='error'>" + html.escape(error) + "</td>")
+            html_lines.append("<td class='T_error'>" + html.escape(error) + "</td>")
 
             html_lines.append("</td>")
 
             html_lines.append("</tr>")
 
         html_lines.append("</tbody>")
 
         html_lines.append("</table>")
 
         return "\n".join(html_lines)
 
     # ----------------------------------------------------------------------------------------
-    def extract_plate_info_from_filename(self, filename: str) -> tuple[str, str]:
-        barcode = None
-        position = None
-        subwell = None
-        pattern = re.compile(r"(\w{4})_(\w{3})_(\d).jpg")
-        match = re.findall(pattern, filename)
-        if match:
-            barcode, position, subwell = match[0]
-            position = f"{position[-1]}{position[:2]}_{subwell}"
-            return barcode, position
-        else:
-            logging.error("Unable to get barcode and position from filename!")
-            return "X", "X"
-
-    # ----------------------------------------------------------------------------------------
     def calculate_realspace_offset(
         self,
-        target_position: Sequence[int],
+        confirmed_target: Sequence[int],
         well_centre: Sequence[int],
         scale_factor: Sequence[float],
     ) -> Optional[int]:
-        if self.list_has_none(target_position) or self.list_has_none(well_centre):
+        if self.list_has_none(confirmed_target) or self.list_has_none(well_centre):
             return None
         return np.rint(
-            (np.array(target_position) - np.array(well_centre)) * np.array(scale_factor)
+            (np.array(confirmed_target) - np.array(well_centre))
+            * np.array(scale_factor)
         ).astype(int)
 
     # ----------------------------------------------------------------------------------------
     def list_has_none(self, input_list: Sequence[Union[int, None]]) -> bool:
         return any(x is None for x in input_list)
 
     # ----------------------------------------------------------------------------------------
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.0.1/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/composers/text.py` & `echolocator-1.0.1/src/echolocator_lib/composers/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 # Base class for generic things.
-from echolocator_api.thing import Thing
+from dls_utilpack.thing import Thing
 
 # Class to do the work using prettytable.
 from echolocator_lib.composers.prettyhelper import PrettyHelper
 
 logger = logging.getLogger(__name__)
 
 thing_type = "echolocator_lib.echolocator_composers.text"
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/contexts/base.py` & `echolocator-1.0.1/src/echolocator_lib/contexts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 # Utilities.
 from dls_utilpack.callsign import callsign
 
 # Base class for a Thing which has a name and traits.
-from echolocator_api.thing import Thing
+from dls_utilpack.thing import Thing
 
 logger = logging.getLogger(__name__)
 
 
 class Base(Thing):
     """ """
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/databases/databases.py` & `echolocator-1.0.1/src/echolocator_lib/guis/guis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,73 @@
 # Use standard logging in this module.
 import logging
 
+# Class managing list of things.
+from dls_utilpack.things import Things
+
 # Exceptions.
 from echolocator_api.exceptions import NotFound
 
-# Class managing list of things.
-from echolocator_api.things import Things
+# Types.
+from echolocator_api.guis.constants import Types
 
 logger = logging.getLogger(__name__)
 
+# -----------------------------------------------------------------------------------------
+__default_echolocator_gui = None
+
+
+def echolocator_guis_set_default(echolocator_gui):
+    global __default_echolocator_gui
+    __default_echolocator_gui = echolocator_gui
+
+
+def echolocator_guis_get_default():
+    global __default_echolocator_gui
+    if __default_echolocator_gui is None:
+        raise RuntimeError("echolocator_guis_get_default instance is None")
+    return __default_echolocator_gui
 
-class Databases(Things):
+
+def echolocator_guis_has_default():
+    global __default_echolocator_gui
+    return __default_echolocator_gui is not None
+
+
+# -----------------------------------------------------------------------------------------
+
+
+class Guis(Things):
     """
-    List of available databases.
+    List of available echolocator_guis.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, name=None):
         Things.__init__(self, name)
 
     # ----------------------------------------------------------------------------------------
     def build_object(self, specification):
         """"""
 
-        database_class = self.lookup_class(specification["type"])
+        echolocator_gui_class = self.lookup_class(specification["type"])
 
         try:
-            database_object = database_class(specification)
+            echolocator_gui_object = echolocator_gui_class(specification)
         except Exception as exception:
             raise RuntimeError(
-                "unable to build database object for type %s" % (database_class)
+                "unable to build echolocator_gui object for type %s"
+                % (echolocator_gui_class)
             ) from exception
 
-        return database_object
+        return echolocator_gui_object
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
-        """
-        Given the class type as string, return a class object.
-        """
+        """"""
 
-        if class_type == "echolocator_lib.echolocator_databases.aiosqlite":
-            from echolocator_lib.databases.aiosqlite import Aiosqlite
+        if class_type == Types.AIOHTTP:
+            from echolocator_lib.guis.aiohttp import Aiohttp
 
-            return Aiosqlite
+            return Aiohttp
 
-        raise NotFound("unable to get database class for type %s" % (class_type))
+        raise NotFound("unable to get echolocator_gui class for type %s" % (class_type))
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/datafaces/context.py` & `echolocator-1.0.1/src/echolocator_lib/guis/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 import logging
 
-from echolocator_api.datafaces.context import Context as DatafaceContext
-
-# Base class for an asyncio context
+# Base class which maps flask requests to methods.
 from echolocator_lib.contexts.base import Base as ContextBase
 
 # Things created in the context.
-from echolocator_lib.datafaces.datafaces import Datafaces
+from echolocator_lib.guis.guis import Guis, echolocator_guis_set_default
 
 logger = logging.getLogger(__name__)
 
 
-thing_type = "echolocator_lib.echolocator_datafaces.context"
+thing_type = "echolocator_lib.echolocator_guis.context"
 
 
 class Context(ContextBase):
     """
-    Asyncio context for a echolocator_dataface server object.
-    On entering, it creates the object according to the specification (a dict).
-    If configured, it starts the server as a coroutine, thread or process.
-    On exiting, it commands the server to shut down.
-
-    The enter and exit methods are exposed for use during testing.
+    Object representing an event echolocator_dataface connection.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification):
         ContextBase.__init__(self, thing_type, specification)
-        self.__api_echolocator_dataface_context = None
 
     # ----------------------------------------------------------------------------------------
     async def aenter(self):
         """ """
 
-        # Build the object according to the specification.
-        self.server = Datafaces().build_object(self.specification())
+        self.server = Guis().build_object(self.specification())
+
+        # If there is more than one gui, the last one defined will be the default.
+        echolocator_guis_set_default(self.server)
 
         if self.context_specification.get("start_as") == "coro":
             await self.server.activate_coro()
 
         elif self.context_specification.get("start_as") == "thread":
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
+            logger.debug("starting gui context")
             await self.server.start_process()
 
-        self.__api_echolocator_dataface_context = DatafaceContext(self.specification())
-        await self.__api_echolocator_dataface_context.aenter()
-
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
+        logger.debug(f"[ECHDON] {thing_type} aexit")
 
         if self.server is not None:
-            # Put in request to shutdown the server.
-            await self.server.client_shutdown()
+            if self.context_specification.get("start_as") == "process":
+                logger.debug(f"[ECHDON] {thing_type} calling client_shutdown")
+                # Put in request to shutdown the server.
+                await self.server.client_shutdown()
 
-        if self.__api_echolocator_dataface_context is not None:
-            await self.__api_echolocator_dataface_context.aexit()
+            if self.context_specification.get("start_as") == "coro":
+                await self.server.direct_shutdown()
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/envvar.py` & `echolocator-1.0.1/src/echolocator_lib/envvar.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 logger = logging.getLogger(__name__)
 
 
 class Envvar:
     """Class which covers environment variables, with default values."""
 
     ECHOLOCATOR_CONFIGFILE = "ECHOLOCATOR_CONFIGFILE"
-    XCHEM_BEFLOW_DATA = "XCHEM_BEFLOW_DATA"
-    XCHEM_BEFLOW_DLS_ROOT = "XCHEM_BEFLOW_DLS_ROOT"
-    BEAMLINE = "BEAMLINE"
-    VISIT_YEAR = "VISIT_YEAR"
-    VISIT = "VISIT"
 
     def __init__(self, name, **kwargs):
 
         environ = kwargs.get("environ")
 
         if environ is None:
             environ = os.environ
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.0.1/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,27 @@
     cursor: pointer
 }
 
 #image_list_ux_interaction_parent .T_picked {
     color: red;
 }
 
+#image_list_ux_interaction_parent .T_uuid {
+    display: none;
+}
 
 #image_list_ux_interaction_parent TH,
 #image_list_ux_interaction_parent TD {
     vertical-align: bottom;
 }
 
 #image_list_ux_interaction_parent #width,
 #image_list_ux_interaction_parent #height,
-#image_list_ux_interaction_parent #target_position_x,
-#image_list_ux_interaction_parent #target_position_y,
+#image_list_ux_interaction_parent #confirmed_target_x,
+#image_list_ux_interaction_parent #confirmed_target_y,
 #image_list_ux_interaction_parent #number_of_crystals {
     text-align: right;
 }
 
 
 /* Job states for images list and image details */
 
@@ -50,10 +53,19 @@
 #image_list_ux_interaction_parent .T_image_state.T_cancelled {
     background-color: gray;
     color: white;
     font-weight: bold;
 }
 
 
-#image_list_ux_interaction_parent .T_name_pattern {
+#image_list_ux_interaction_parent .T_barcode_filter {
     width: 320px;
+}
+
+#image_list_ux_interaction_parent .T_is_drop {
+    display: none;
+}
+
+#image_list_ux_interaction_parent .T_real_space_target_x,
+#image_list_ux_interaction_parent .T_real_space_target_y {
+    display: none;
 }
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.0.1/src/echolocator_lib/guis/html/css/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,25 @@
   overflow: hidden;
   position: absolute;
   top: 0px;
   left: 0px;
 }
 
 /* --------------------------------------------------------------------------- */
+.T_ajax_confirmation_message_container {
+  border-radius: 4px;
+  border: 1px solid darkgreen;
+  color: darkgreen;
+}
+
+.T_ajax_confirmation_message {
+  margin: 4px;
+}
+
+/* --------------------------------------------------------------------------- */
 .T_ajax_error_message_container {
   border-radius: 4px;
   border: 1px solid orangered;
   color: orangered;
 }
 
 .T_ajax_error_message {
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/index.html` & `echolocator-1.0.1/src/echolocator_lib/guis/html/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -60,22 +60,27 @@
             <div id="tab-image-list">
                 <div id="image_list_ux_interaction_parent">
                     <div class="T_auto_update">
                         <div class="T_toggle">AUTO</div>
                         <div class="T_status">-</div>
                     </div>
                     <div class="T_buttons" style="margin-top: 8px; margin-bottom: 8px;">
-                        <button class="T_export_button" title="export">Export</button>
+                        <div class="T_field">
+                            <div class="T_prompt">visit</div>
+                            <div class="T_input"><input type="text" class="T_visit"></div>
+                            <div class="T_separator"></div>
+                            <button class="T_export_button" title="export">Export</button>
+                        </div>
                     </div>
-                    <div class="T_help">Exports all images matching the name pattern whether decided or not.</div>
+                    <div class="T_help">Exports all images on the plate which have been decided.</div>
                     <div class="T_inputs" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_row">
                             <div class="T_field">
-                                <div class="T_prompt">name pattern</div>
-                                <div class="T_input"><input type="text" class="T_name_pattern"></div>
+                                <div class="T_prompt">barcode</div>
+                                <div class="T_input"><input type="text" class="T_barcode_filter"></div>
                                 <div class="T_separator"></div>
                                 <div class="T_prompt">show only undecided</div>
                                 <div class="T_input"><input type="checkbox" class="T_should_show_only_undecided"></div>
                             </div>
                         </div>
                     </div>
                     <div class="T_section">
@@ -83,24 +88,24 @@
                         <div class="T_composed T_image_list" style="overflow:scroll;height: 100%;">-</div>
                     </div>
                 </div>
             </div><!-- tab-image-list -->
 
             <div id="tab-image-edit">
                 <div id="image_edit_ux_interaction_parent">
-                    <div class="T_buttons" style="margin-top: 8px; margin-bottom: 8px;">
+                    <div class="T_buttons T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
                         <button class="T_previous_button" title="previous image">Previous</button>
                         <button class="T_accept_button" title="accept image">Usable</button>
                         <button class="T_reject_button" title="reject image">Not Usable</button>
                         <button class="T_reset_button" title="reset image">Undecided</button>
                         <button class="T_next_button" title="next image">Next</button>
                     </div>
-                    <div class="T_help">Right-click in the image to mark as not usable.</div>
+                    <div class="T_help T_hide_when_no_image">Right-click in the image to mark as not usable.</div>
 
-                    <div class="T_image_info" style="margin-top: 8px; margin-bottom: 8px;">
+                    <div class="T_image_info T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_field">
                             <div class="T_prompt">filename:</div>
                             <div class="T_input">
                                 <div class="T_filename"></div>
                             </div>
                             <div class="T_separator"></div>
                             <div class="T_prompt">Num crystals:</div>
@@ -111,15 +116,15 @@
                             <div class="T_prompt">is usable?</div>
                             <div class="T_input">
                                 <div class="T_is_usable"></div>
                             </div>
                         </div>
                     </div>
 
-                    <div id="image1" class="dataframe" style="width: 100%;">
+                    <div id="image1" class="dataframe T_hide_when_no_image" style="width: 100%;">
                         <div class="container view-container">
                             <div id="image1_viewport" class="viewport">
                                 <img id="detector1_image" src="images/radial1.666.png"
                                     style="image-rendering: pixelated;">
                             </div>
                             <div id="raphael1_viewport" class="viewport">
                                 <div id="raphael1_paper"></div>
```

#### html2text {}

```diff
@@ -11,17 +11,19 @@
 
 
 
     * Image_List
     * Image_Details
 AUTO
 -
+visit
+[                    ]
 Export
-Exports all images matching the name pattern whether decided or not.
-name pattern
+Exports all images on the plate which have been decided.
+barcode
 [                    ]
 show only undecided
 ⁰
 Image List
 -
 Previous Usable Not Usable Undecided Next
 Right-click in the image to mark as not usable.
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/index.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -156,18 +156,18 @@
     } // end method
 
     // -----------------------------------------------------------------------
     // Propagate event where user clicks a filename, such as in image_list_ux.
     handle_image_picked(event) {
         var F = "Index::handle_image_picked";
 
-        var autoid = event.detail.autoid;
+        var crystal_well_uuid = event.detail.crystal_well_uuid;
 
         // Tell the image editor to show the new image.
-        this.#image_edit_ux.set_autoid(autoid);
+        this.#image_edit_ux.set_crystal_well_uuid(crystal_well_uuid);
 
         this.#tabs_manager.switch_to_tab("tab-image-edit")
 
         // Resize the displayed image according to the current screen size.
         // this.resize_image()
 
     } // end method
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/events.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,23 @@
 // Class backing the actions ux.
 
 class echolocator__ImageEditUx extends echolocator__UxAutoUpdate {
     COOKIE_NAME = "IMAGE_EDIT_UX";
     FETCH_IMAGE = "echolocator_guis::commands::fetch_image";
-    SET_IMAGE_IS_USABLE = "echolocator_guis::commands::set_image_is_usable";
+    UPDATE = "echolocator_guis::commands::update";
+    SHOULD_ADVANCE = "echolocator_guis::keywords::should_advance";
 
     #jquery_objects = {};
-    #autoid = null;
+    #crystal_well_uuid = null;
     #record = null;
     #raphael = null;
+    #is_dragging = null;
     #transformer = null;
-    #pixel_ux = null;
+    #confirmed_target_ux = null;
+    #well_centroid_ux = null;
 
 
     constructor(runtime, plugin_link_name, $interaction_parent) {
         super(runtime);
 
         this.plugin_link_name = plugin_link_name;
         this.$interaction_parent = $interaction_parent;
@@ -27,24 +30,28 @@
         var F = "echolocator__ImageEditUx::activate"
         super.activate()
 
         // Make a spreader which reacts to resizing of the window.
         this.image1_spreader = new webviz__Spreader(this);
 
         // Make a raphael drawing object.
+        // TODO: Make Raphael drawing object big enough for future jumbo-size images.
         this.#raphael = Raphael("raphael1_paper", 4000, 4000);
 
+        this.#is_dragging = false;
+
         // For transforming coordinates between data and view.
         this.#transformer = new webviz__Transformer(this.runtime);
 
         // Pass this transformer to anyone who wants to use the raphael for drawing.
         this.#raphael.webviz_transformer = this.#transformer;
 
         this.#jquery_objects.$raphael1_paper = $("#raphael1_paper SVG", this.$interaction_parent);
         this.#jquery_objects.$image = $("IMG", this.$interaction_parent);
+        this.#jquery_objects.$hide_when_no_image = $(".T_hide_when_no_image", this.$interaction_parent);
         this.#jquery_objects.$filename = $(".T_filename", this.$interaction_parent);
         this.#jquery_objects.$number_of_crystals = $(".T_number_of_crystals", this.$interaction_parent);
         this.#jquery_objects.$is_usable = $(".T_is_usable", this.$interaction_parent);
         this.#jquery_objects.previous_button = $(".T_previous_button", this.$interaction_parent);
         this.#jquery_objects.accept_button = $(".T_accept_button", this.$interaction_parent);
         this.#jquery_objects.reject_button = $(".T_reject_button", this.$interaction_parent);
         this.#jquery_objects.reset_button = $(".T_reset_button", this.$interaction_parent);
@@ -56,118 +63,156 @@
         // Window size changes.
         this.image1_spreader.addEventListener(
             webviz__Spreader__SpreadEvent,
             function(event) {
                 that.handle_spread_event(event);
             });
 
-        // Set up jquery event handling for DOM elements.
+        // A click on the "paper" <div> sets the target location, unless dragging.
         this.#jquery_objects.$raphael1_paper.click(
             function(jquery_event_object) {
-                that._handle_canvas_left_click(jquery_event_object);
+                if (!that.#is_dragging)
+                    that._handle_canvas_left_click(jquery_event_object);
             });
 
         // Disable context menu for right-click on the image.
         this.#jquery_objects.$raphael1_paper.contextmenu(function(jquery_event_object) {
             that._handle_canvas_right_click(jquery_event_object);
             return false;
         });
 
+        // Set up jquery event handling for DOM elements.
         this.#jquery_objects.previous_button.click(
             function(jquery_event_object) {
                 console.log(F + ": clicked previous");
                 that._handle_previous_or_next(-1);
             });
 
         this.#jquery_objects.accept_button.click(
             function(jquery_event_object) {
-                that._handle_is_usable_change(true);
+                that._send_update(true);
             });
 
         this.#jquery_objects.reject_button.click(
             function(jquery_event_object) {
-                that._handle_is_usable_change(false);
+                that._send_update(false);
             });
 
         this.#jquery_objects.reset_button.click(
             function(jquery_event_object) {
-                that._handle_is_usable_change(null);
+                that._send_update(null);
             });
 
         this.#jquery_objects.next_button.click(
             function(jquery_event_object) {
                 that._handle_previous_or_next(1);
             });
 
-        this.#pixel_ux = new echolocator__PixelUx(
+
+        // ----------------------------------------------------------
+        // Make the draggable crosshair for the target location.
+        this.#confirmed_target_ux = new echolocator__PixelUx(
+            self.runtime,
+            "confirmed_target",
+            this.$interaction_parent,
+            "yellowgreen",
+            true);
+
+        // Handle when user has finished moving the crosshair, event comes from pixel_ux widget.
+        this.#confirmed_target_ux.addEventListener(
+            echolocator__PixelUx__UserChangeEvent,
+            function(event) {
+                that._handle_confirmed_target_ux_change_event(event);
+                that.#is_dragging = false;
+            });
+
+        // Handle when user is moving the crosshair.
+        this.#confirmed_target_ux.addEventListener(
+            echolocator__PixelUx__UserMotionEvent,
+            function(event) {
+                that.#is_dragging = true;
+            });
+
+        // ----------------------------------------------------------
+        // Make the crosshair for the well centroid, but it is not draggable.
+        this.#well_centroid_ux = new echolocator__PixelUx(
             self.runtime,
-            "pixel",
-            $("#pixel_ux_interaction_parent"));
+            "well_centroid",
+            this.$interaction_parent,
+            "lightblue",
+            false);
+
+        // ----------------------------------------------------------
 
         // Activate the spreader to react on window size changes.
         this.image1_spreader.activate($("#image1"), window);
 
-        this.#pixel_ux.activate(this.#raphael);
+        // Activate well_centroid first, so it lies "under" the confirmed target in case they overlap.
+        this.#well_centroid_ux.activate(this.#raphael);
+        this.#confirmed_target_ux.activate(this.#raphael);
 
         this.request_update()
     } // end method
 
 
     // -------------------------------------------------------------
     // When the selected filename changes, we get notified.
     // We will load the image into the display.
 
-    set_autoid(autoid) {
-        var F = "echolocator__ImageEditUx::set_autoid";
+    set_crystal_well_uuid(crystal_well_uuid) {
+        var F = "echolocator__ImageEditUx::set_crystal_well_uuid";
 
         // Remember the image info.
-        this.#autoid = autoid;
+        this.#crystal_well_uuid = crystal_well_uuid;
 
-        if (this.#autoid === undefined) {
+        if (this.#crystal_well_uuid === undefined) {
             this.display_ajax_error("there are no more images to view");
         } else {
             this.display_ajax_error(null);
 
             // Request image info from the server.
             this.request_update()
 
         }
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle accept or reject button click.
 
-    _handle_is_usable_change(is_usable) {
+    _send_update(is_usable, confirmed_target) {
         var F = "echolocator__ImageEditUx::_handle_is_usable_change";
 
-        if (this.#autoid) {
+        if (this.#crystal_well_uuid) {
             // Build json request.
             var json_object = {}
             // TODO: Remove hardcoded "IMAGE_LIST_UX" in image edit's cookie list.
             json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME, "IMAGE_LIST_UX"]
-            json_object[this.COMMAND] = this.SET_IMAGE_IS_USABLE;
-            json_object["autoid"] = this.#autoid;
-            json_object["is_usable"] = is_usable;
+            json_object[this.COMMAND] = this.UPDATE;
 
-            // Send request to update database immediately.
-            this.send(json_object);
+            // We pass the fields of the database we want updated.
+            var model = {
+                "crystal_well_uuid": this.#crystal_well_uuid,
+                "is_usable": is_usable
+            }
 
-            if (!is_usable) {
-                // Notify pixel_ux of requested change in position.
-                // TODO: Combine usable change with position change into single ajax.
-                this.#pixel_ux.set_autoid(this.#autoid, {
-                    x: 10,
-                    y: 10
-                });
+            if (confirmed_target !== undefined) {
+                model["confirmed_target_x"] = confirmed_target.x;
+                model["confirmed_target_y"] = confirmed_target.y;
 
-                // Tell pixel_ux to send change to the database.
-                this.#pixel_ux.update_database();
             }
 
+            json_object["crystal_well_droplocation_model"] = model;
+
+            // Tell server to add response["html"] for next image in series.
+            json_object[this.SHOULD_ADVANCE] = true;
+
+            // Send request to update database immediately.
+            this.send(json_object);
+
             // Move to next image.
             this.request_update(1);
         }
 
     } // end method
 
     // -------------------------------------------------------------
@@ -178,121 +223,183 @@
 
         // Request an update from the database.
         this.request_update(direction);
 
     } // end method
 
     // -------------------------------------------------------------
+    // Handle where the user has moved the crosshairs, event comes from pixel_ux widget.
+    // Units are transformed to underlying image pixel target.
+
+    _handle_confirmed_target_ux_change_event(pixel_ux__user_change_event) {
+        var F = "echolocator__ImageEditUx::_handle_confirmed_target_ux_change_event";
+
+        var confirmed_target = pixel_ux__user_change_event.detail.target;
+
+        // Mark image usable and save target location.
+        this._send_update(true, confirmed_target)
+
+    } // end method
+
+    // -------------------------------------------------------------
     // Handle left click on the raphael paper.
 
     _handle_canvas_left_click(jquery_event_object) {
         var F = "echolocator__ImageEditUx::_handle_canvas_left_click";
 
+        console.log(F + ": seeing canvas left click");
+
         var view_position = {
             x: jquery_event_object.offsetX,
             y: jquery_event_object.offsetY
         }
 
         // Convert to target position before giving to pixel_ux.
-        var target_position = this.#transformer.view_to_data(view_position);
-
-        console.log(F + ": clicked view_position" +
-            " [" + view_position.x + ", " + view_position.y + "]" +
-            " transformed to target_position" +
-            " [" + target_position.x + ", " + target_position.y + "]");
+        var confirmed_target = this.#transformer.view_to_data(view_position);
 
         // Notify pixel_ux of requested change in position.
-        this.#pixel_ux.set_autoid(this.#autoid, target_position);
-
-        // Tell pixel_ux to send change to the database.
-        this.#pixel_ux.update_database();
+        this.#confirmed_target_ux.set_uuid(this.#crystal_well_uuid, confirmed_target);
 
-        // Mark image usable.
-        this._handle_is_usable_change(true)
+        // Mark image usable and save target location.
+        this._send_update(true, confirmed_target)
 
     } // end method
 
     // -------------------------------------------------------------
     // Handle right click on the raphael paper.
 
     _handle_canvas_right_click(jquery_event_object) {
         var F = "echolocator__ImageEditUx::_handle_canvas_right_click";
 
         // Mark image unusable.
-        this._handle_is_usable_change(false)
+        this._send_update(false)
 
     } // end method
+
     // -------------------------------------------------------------
     // Request update from database.
 
     request_update(direction = 0) {
 
         var json_object = {}
         // TODO: Remove hardcoded "IMAGE_LIST_UX" in image edit's cookie list.
         json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME, "IMAGE_LIST_UX"]
         json_object[this.COMMAND] = this.FETCH_IMAGE;
-        json_object["autoid"] = this.#autoid;
+        json_object["crystal_well_uuid"] = this.#crystal_well_uuid;
         json_object["direction"] = direction;
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
+    // Handle an error response.
+
+    handle_ajax_failure(response, status, jqXHR) {
+        var F = "echolocator__ImageEditUx::handle_ajax_failure";
+
+        // Let the base class check for and display any error or confirmation in the response.
+        super.handle_ajax_failure(response, status, jqXHR);
+
+        this.#jquery_objects.$hide_when_no_image.hide();
+
+    } // end method
+
+    // -------------------------------------------------------------
     // Handle the response when it comes.
 
     handle_ajax_success(response, status, jqXHR) {
         var F = "echolocator__ImageEditUx::_handle_ajax_success";
 
-        // Let the base class check for and display any error in the response.
+        // Let the base class check for and display any error or confirmation in the response.
         var error_message = super.handle_ajax_success(response, status, jqXHR);
 
-        if (error_message !== null)
+        if (error_message !== null) {
+            this.#jquery_objects.$hide_when_no_image.hide();
             return;
+        }
 
         // Response is expected to contain the database record.
         var record = response.record;
 
         if (record === null) {
-            console.log(F + ": response record had value of null");
-            this.display_ajax_error("Please choose an image.");
+            if (response.confirmation === undefined) {
+                console.log(F + ": response record had value of null");
+                this.display_ajax_error("no image has been selected from the image list tab");
+            }
+            this.#jquery_objects.$hide_when_no_image.hide();
             return;
         }
 
-        // Remember which autoid we are showing.
-        this.#autoid = record.autoid;
+        this.#jquery_objects.$hide_when_no_image.show();
+
+        // Remember which crystal_well_uuid we are showing.
+        this.#crystal_well_uuid = record.uuid;
 
         // Update the display with the new file's contents.
         var src = record.filename;
         this.#jquery_objects.$image.prop("src", src)
 
-        // Render the autoid stuff.
+        // Render the crystal_well_uuid stuff.
         this.#jquery_objects.$filename.text(record.filename);
         if (record.is_usable === null)
             record.is_usable = "-";
-        if (record.is_usable === 1)
+        if (record.is_usable === true)
             record.is_usable = "yes";
-        if (record.is_usable === 0)
+        if (record.is_usable === false)
             record.is_usable = "no";
 
         if (record.number_of_crystals === null)
             record.number_of_crystals = "-";
 
         this.#jquery_objects.$number_of_crystals.text(record.number_of_crystals);
         this.#jquery_objects.$is_usable.text(record.is_usable);
 
         // Keep the last record loaded.
         this.#record = record;
 
-        // The the pixel ux about the autoid so it can be included in sending changes.
-        var target_position = {
-            x: record.target_position_x ? record.target_position_x : 10,
-            y: record.target_position_y ? record.target_position_y : 10
-        }
-        this.#pixel_ux.set_autoid(this.#autoid, target_position);
+        // The the pixel ux about the crystal_well_uuid so it can be included in sending changes.
+        var x = record.confirmed_target_x;
+        if (x === null)
+            x = record.auto_target_x;
+        if (x === null)
+            x = 10;
+
+        var y = record.confirmed_target_y;
+        if (y === null)
+            y = record.auto_target_y;
+        if (y === null)
+            y = 10;
+
+        var confirmed_target = {
+            x: x,
+            y: y
+        };
+
+        this.#confirmed_target_ux.set_uuid(this.#crystal_well_uuid, confirmed_target);
+
+        // The the pixel ux about the crystal_well_uuid so it can be included in sending changes.
+        var x = record.well_centroid_x;
+        if (x === null)
+            x = record.auto_target_x;
+        if (x === null)
+            x = 10;
+
+        var y = record.well_centroid_y;
+        if (y === null)
+            y = record.auto_target_y;
+        if (y === null)
+            y = 10;
+
+        var well_centroid = {
+            x: x,
+            y: y
+        };
+
+        this.#well_centroid_ux.set_uuid(this.#crystal_well_uuid, well_centroid);
 
         // Let the spreader calculate the available space for the image.
         // This will trigger a call to this.handle_spread_event().
         // This only needs to be here for the very first opening of this tab.
         this.image1_spreader.spread();
 
         // Resize the image to fit on the screen.
@@ -332,15 +439,16 @@
             y2: h
         })
 
         // Resize the displayed image according to the current screen size.
         this.resize_image()
 
         // Tell pixel_ux to render under the new transformer.
-        this.#pixel_ux.render()
+        this.#confirmed_target_ux.render()
+        this.#well_centroid_ux.render()
 
     } // end method
 
     // -----------------------------------------------------------------------
     // Resize the displayed image according to the current screen size.
 
     resize_image() {
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,17 @@
 // Class backing the actions ux.
 
 class echolocator__ImageListUx extends echolocator__UxAutoUpdate {
     COOKIE_NAME = "IMAGE_LIST_UX";
     FETCH_IMAGE_LIST = "echolocator_guis::commands::fetch_image_list";
+    EXPORT = "echolocator_guis::commands::export";
 
     #jquery_objects = {};
-    #name_pattern = "undefined";
+    #visit = "undefined";
+    #barcode_filter = "undefined";
     #should_show_only_undecided = "undefined";
 
     constructor(runtime, plugin_link_name, $interaction_parent) {
         super(runtime);
 
         this.plugin_link_name = plugin_link_name;
         this.$interaction_parent = $interaction_parent;
@@ -19,42 +21,53 @@
     // -------------------------------------------------------------
     // Activate things on the UX.
 
     activate() {
         super.activate()
 
         this.#jquery_objects.$div = $(".T_composed", this.$interaction_parent);
-        this.#jquery_objects.$name_pattern = $(".T_name_pattern", this.$interaction_parent);
+        this.#jquery_objects.$visit = $(".T_visit", this.$interaction_parent);
+        this.#jquery_objects.$barcode_filter = $(".T_barcode_filter", this.$interaction_parent);
         this.#jquery_objects.$should_show_only_undecided = $(".T_should_show_only_undecided", this.$interaction_parent);
+        this.#jquery_objects.$export_button = $(".T_export_button", this.$interaction_parent);
 
         var that = this;
-        this.#jquery_objects.$name_pattern.change(
+        this.#jquery_objects.$visit.change(
+            function(jquery_event_object) {
+                that._handle_filter_change(jquery_event_object);
+            });
+
+        this.#jquery_objects.$barcode_filter.change(
             function(jquery_event_object) {
                 that._handle_filter_change(jquery_event_object);
             });
 
         this.#jquery_objects.$should_show_only_undecided.change(
             function(jquery_event_object) {
                 that._handle_filter_change(jquery_event_object);
             });
 
-        // this.request_update();
+        this.#jquery_objects.$export_button.click(
+            function(jquery_event_object) {
+                that._handle_export_clicked(jquery_event_object);
+            });
 
     } // end method
 
     // -------------------------------------------------------------
     // Request update from database.
 
     request_update() {
 
         var json_object = {}
         json_object[this.COMMAND] = this.FETCH_IMAGE_LIST;
         json_object[this.ENABLE_COOKIES] = [this.COOKIE_NAME];
 
-        json_object["name_pattern"] = this.#name_pattern;
+        json_object["visit"] = this.#visit;
+        json_object["barcode_filter"] = this.#barcode_filter;
         json_object["should_show_only_undecided"] = this.#should_show_only_undecided;
 
         this.send(json_object);
 
     } // end method
 
     // -------------------------------------------------------------
@@ -65,18 +78,22 @@
 
         // Let the base class have a look at the response.
         super.handle_ajax_success(response, status, jqXHR);
 
         var filters = response.filters;
         if (filters !== undefined) {
             var t;
-            t = filters["name_pattern"];
+            t = filters["visit"];
+            if (t === undefined)
+                t = "";
+            this.#jquery_objects.$visit.val(t);
+            t = filters["barcode_filter"];
             if (t === undefined)
                 t = "";
-            this.#jquery_objects.$name_pattern.val(t);
+            this.#jquery_objects.$barcode_filter.val(t);
             t = filters["should_show_only_undecided"];
             if (t === undefined)
                 t = false;
             this.#jquery_objects.$should_show_only_undecided.prop("checked", t);
         }
 
         var html = response.html;
@@ -89,51 +106,73 @@
     }
 
     // -------------------------------------------------------------
 
     _handle_filter_change(jquery_event_object) {
         var F = "echolocator__ImageListUx::_handle_filter_change"
 
-        this.#name_pattern = this.#jquery_objects.$name_pattern.val()
+        this.#visit = this.#jquery_objects.$visit.val()
+        this.#barcode_filter = this.#jquery_objects.$barcode_filter.val()
         this.#should_show_only_undecided = this.#jquery_objects.$should_show_only_undecided.prop("checked")
         this.request_update()
 
     } // end method
 
     // -------------------------------------------------------------
 
+    _handle_export_clicked(jquery_event_object) {
+        var F = "echolocator__ImageListUx::_handle_export_clicked"
+
+        this.#visit = this.#jquery_objects.$visit.val()
+        this.#barcode_filter = this.#jquery_objects.$barcode_filter.val()
+
+        // Enable no cookie for this request.
+        var json_object = {}
+        json_object[this.COMMAND] = this.EXPORT;
+
+        json_object["visit"] = this.#visit;
+        json_object["barcode_filter"] = this.#barcode_filter;
+
+        this.send(json_object);
+
+    } // end method
+
+    // -------------------------------------------------------------
+
     _handle_filename_clicked(jquery_event_object) {
 
         var $filename_row = $(jquery_event_object.target);
 
+        // User clicked on a cell within the row?
         if ($filename_row.get(0).tagName == "TD")
             $filename_row = $filename_row.parent();
 
-        var autoid = $filename_row.attr("autoid");
+        // The row has the attribute holding the crystal well of this row.
+        var crystal_well_uuid = $filename_row.attr("crystal_well_uuid");
 
-        this._load_image(autoid);
+        this._load_image(crystal_well_uuid);
 
         this.set_and_render_auto_update(false);
 
     } // end method
 
     // -------------------------------------------------------------
 
-    _load_image(autoid) {
+    _load_image(crystal_well_uuid) {
         var F = "echolocator__ImageListUx::_load_image";
 
-        console.log(F + ": loading image " + autoid)
+        console.log(F + ": loading image for crystal_well_uuid " + crystal_well_uuid)
 
         //     this.$filename_rows.removeClass("T_picked");
         //     image_info.$filename_row.addClass("T_picked");
 
         // Trigger an event that the index.js will use to coordinate cross-widget changes.
         var custom_event = new CustomEvent(echolocator__Events_IMAGE_PICKED_EVENT, {
             detail: {
-                autoid: autoid
+                crystal_well_uuid: crystal_well_uuid
             }
         });
 
         this.dispatchEvent(custom_event);
 
     } // end method
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,28 @@
 var echolocator__PixelUx__UserMotionEvent = "echolocator__PixelUx__UserMotionEvent";
 var echolocator__PixelUx__UserChangeEvent = "echolocator__PixelUx__UserChangeEvent";
 
 class echolocator__PixelUx extends echolocator__UxBase {
-    SET_TARGET_POSITION = "echolocator_guis::commands::set_target_position";
+    UPDATE = "echolocator_guis::commands::update";
 
     #raphael = null;
+    #color = null;
+    #is_draggable = null;
     #transformer = null;
     #guide = null;
-    #autoid = null;
-    #target_position = null;
+    #uuid = null;
+    #target = null;
 
-    constructor(runtime, plugin_link_name, $interaction_parent, raphael) {
+    constructor(runtime, plugin_link_name, $interaction_parent, color, is_draggable) {
         super(runtime);
 
         this.plugin_link_name = plugin_link_name;
         this.$interaction_parent = $interaction_parent;
+        this.#color = color;
+        this.#is_draggable = is_draggable;
     }
 
     // -------------------------------------------------------------
     // Activate things on the UX.
 
     activate(raphael) {
         super.activate()
@@ -41,111 +45,104 @@
         // Guide stops.
         this.#guide.addEventListener(
             webviz__hair__Guide2__UserChangeEvent,
             function(event) {
                 that.handle_guide_change_event(event);
             });
 
-        this.#guide.activate(this.#raphael, "yellowgreen");
+        this.#guide.activate(this.#raphael, this.#color, this.#is_draggable);
 
         // Set box to appear guaranteed on-screen somewhere.
         this.#guide.set_box({
             position: {
                 x: 110,
-                y: 110
+                y: 220
             },
             visible: true
         });
 
     } // end method
 
     // -------------------------------------------------------------
     // When the selected image changes, we get notified.
     // We will move the guide to the image's target location.
     // We will update the x and y as the guid moves.
 
-    set_autoid(autoid, target_position) {
-        var F = "echolocator__PixelUx::set_autoid"
+    set_uuid(uuid, target) {
+        var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::set_uuid"
 
         // Remember the image info.
-        this.#autoid = autoid;
-        this.#target_position = target_position;
+        this.#uuid = uuid;
+        this.#target = target;
+
+        console.log(F + ": uuid " + this.#uuid + " is for target [" + this.#target.x + ", " + this.#target.y + "]")
 
         this.render();
 
     } // end method
 
     // -----------------------------------------------------------------------
     // Render the viewable things according to the current tranformer settings.
     render(event) {
-        var F = "echolocator__PixelUx::render"
+        var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::render"
+
+        console.log(F + ": rendering target [" + this.#target.x + ", " + this.#target.y + "]")
 
         // Everything we send or receive from the outside is data coordinates.
         // Convert it to view coordinates which is are used by the guide.
-        var view_position = this.#transformer.data_to_view(this.#target_position);
+        var view_position = this.#transformer.data_to_view(this.#target);
+
+        console.log(F + ": rendering to view position [" + view_position.x + ", " + view_position.y + "]")
 
         // Move the guide to the canvas view location.
         this.#guide.set_box({
             position: view_position
         })
 
     } // end method
 
     // -----------------------------------------------------------------------
     // Guide is moving (dragging).
     handle_guide_motion_event(event) {
-        var F = "echolocator__PixelUx::handle_guide_motion_event"
+        var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::handle_guide_motion_event"
 
-        // console.log(F + " guide moving")
+        // Trigger an event that image_edit.js will use to avoid handling the click on the paper.
+        var custom_event = new CustomEvent(echolocator__PixelUx__UserMotionEvent, {
+            detail: {}
+        });
+
+        this.dispatchEvent(custom_event);
 
     } // end method
 
 
     // -----------------------------------------------------------------------
     // Guide has changed (mouse up after dragging).
     // Also can be called by image_edit_ux after click on canvas.
     handle_guide_change_event(event) {
-        var F = "echolocator__PixelUx::handle_guide_change_event"
+        var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::handle_guide_change_event"
 
         console.log(F + " guide changed")
 
         // The guide gives view coordinates.
         var view_position = this.#guide.get().position;
 
         // Everything we send or receive from the outside is data coordinates.
-        this.#target_position = this.#transformer.view_to_data(view_position)
+        this.#target = this.#transformer.view_to_data(view_position)
 
-        console.log(F + ": dragged view_position" +
+        console.log(F + ": [INTERPI] dragged view_position" +
             " [" + view_position.x + ", " + view_position.y + "]" +
-            " transformed to target_position" +
-            " [" + this.#target_position.x + ", " + this.#target_position.y + "]");
-
-        this.update_database();
+            " transformed to target" +
+            " [" + this.#target.x + ", " + this.#target.y + "]");
 
-        // Trigger an event that image_edit.js will use to advance to the next image.
+        // Trigger an event that image_edit.js will use to save the target and advance to the next image.
         var custom_event = new CustomEvent(echolocator__PixelUx__UserChangeEvent, {
             detail: {
-                target_position: this.#target_position
+                target: this.#target
             }
         });
 
         this.dispatchEvent(custom_event);
 
     } // end method
 
-    // -----------------------------------------------------------------------
-    // Called after guide changed by a user action.
-    // Also can be called by image_edit_ux after click on canvas has set a new position.
-
-    update_database(event) {
-        var F = "echolocator__PixelUx::update_database"
-
-        var json_object = {}
-        json_object[this.COMMAND] = this.SET_TARGET_POSITION;
-        json_object["autoid"] = this.#autoid;
-        json_object["target_position"] = this.#target_position;
-
-        this.send(json_object);
-
-    } // end method
-
 }
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -22,14 +22,48 @@
     }
 
     // -------------------------------------------------------------
     // Activate things on the UX.
 
     activate() {
 
+        // Activate confirmation message display place on the UX.
+        this.activate_confirmation_message();
+
+        // Activate error message display place on the UX.
+        this.activate_error_message();
+
+    } // end method
+
+    // -------------------------------------------------------------
+    // Activate confirmation message display place on the UX.
+
+    activate_confirmation_message() {
+
+        var cm_class = "T_ajax_confirmation_message";
+        var $cm_container = $("." + cm_class + "_container", this.$interaction_parent);
+        var $cm = $("." + cm_class, this.$interaction_parent);
+
+        if ($cm_container.length == 0) {
+            this.$interaction_parent.prepend("<div class='" + cm_class + "_container'><div class='" + cm_class + "'></div></div>");
+            $cm_container = $("." + cm_class + "_container", this.$interaction_parent);
+            $cm = $("." + cm_class, this.$interaction_parent);
+        }
+
+        $cm_container.hide();
+        this.#jquery_objects.$confirmation_message_container = $cm_container;
+        this.#jquery_objects.$confirmation_message = $cm;
+
+    } // end method
+
+    // -------------------------------------------------------------
+    // Activate error message display place on the UX.
+
+    activate_error_message() {
+
         var em_class = "T_ajax_error_message";
         var $em_container = $("." + em_class + "_container", this.$interaction_parent);
         var $em = $("." + em_class, this.$interaction_parent);
 
         if ($em_container.length == 0) {
             this.$interaction_parent.prepend("<div class='" + em_class + "_container'><xmp class='" + em_class + "'></xmp></div>");
             $em_container = $("." + em_class + "_container", this.$interaction_parent);
@@ -45,64 +79,98 @@
     // -------------------------------------------------------------
     // Handle the response when it comes.
 
     handle_ajax_success(response, status, jqXHR) {
         var F = "echolocator__UxBase::handle_ajax_success[" + this.plugin_link_name + "]";
 
         var error_message = null;
+        var confirmation_message = null;
         var http_code = jqXHR.status;
 
-        // If not 200, then we don't likely have response as json.
-        if (http_code !== 200) {
-            error_message = "error " + http_code + " (" + status + ")" + "\n" + response;
-        }
-        // Presumably we got a cogent json response, so check if the content has an error field.
-        else {
+        // With 200, we presumably we probably got a cogent json response.
+        if (http_code === 200) {
+            // Check if the content has an error field.
             if (response.exception || response.error) {
                 error_message = "exception in server response\n" + JSON.stringify(response);
             }
+
+            // Check if the content has a confirmation field.
+            // We could, theoretically, have both an error and a confirmation.
+            if (response.confirmation) {
+                confirmation_message = response.confirmation;
+            }
+        }
+        // If not 200, then we don't likely have response as json.
+        else {
+            error_message = "error " + http_code + " (" + status + ")" + "\n" + response;
         }
 
+        this.display_ajax_confirmation(confirmation_message);
         this.display_ajax_error(error_message);
 
         return error_message;
     }
 
     // -------------------------------------------------------------
     // Handle the response failure if it comes.
     handle_ajax_failure(jqXHR, status, error_thrown) {
         var F = "echolocator__UxBase::handle_ajax_failure[" + this.plugin_link_name + "]";
+        console.log(F + ": status \"" + status + "\"");
+        console.log(F + ": error_thrown \"" + error_thrown + "\"");
+        console.log(F + ": jqXHR.responseText \"" + jqXHR.responseText + "\"");
+        console.log(F + ": jqXHR.statusText \"" + jqXHR.statusText + "\"");
+        console.log(F + ": jqXHR.status \"" + jqXHR.status + "\"");
+        console.log(F + ": jqXHR.getAllResponseHeaders() \"" + jqXHR.getAllResponseHeaders() + "\"");
 
+        if (status == "error" && jqXHR.status == 0) {
+            error_message = "the server is unreachable";
+        } else {
 
-        var http_code = jqXHR.status;
-        var error_message = null;
+            var http_code = jqXHR.status;
+            var error_message = null;
 
-        if (error_thrown.name != undefined)
-            error_message = error_thrown.name + ": " + error_thrown.message;
-        else
-            error_message = error_thrown;
+            if (error_thrown.name != undefined)
+                error_message = error_thrown.name + ": " + error_thrown.message;
+            else
+                error_message = error_thrown;
 
-        error_message = "error " + http_code + " " + error_message + "\n" + jqXHR.responseText;
+            error_message = "error " + http_code + " " + error_message + "\n" + jqXHR.responseText;
+        }
 
         console.log(F + ": " + error_message);
 
         this.display_ajax_error(error_message);
 
         return error_message;
     }
 
     // -------------------------------------------------------------
+    // Display any confirmation from ajax response.
+    display_ajax_confirmation(confirmation_message) {
+        var F = "echolocator__UxBase::display_ajax_confirmation[" + this.plugin_link_name + "]";
+
+        if (confirmation_message === null) {
+            this.#jquery_objects.$confirmation_message_container.hide();
+        } else {
+            console.log(F + ": displaying confirmation " + confirmation_message);
+
+            this.#jquery_objects.$confirmation_message.text(confirmation_message);
+            this.#jquery_objects.$confirmation_message_container.show();
+        }
+    }
+
+    // -------------------------------------------------------------
     // Display any error from ajax response.
     display_ajax_error(error_message) {
         var F = "echolocator__UxBase::display_ajax_error[" + this.plugin_link_name + "]";
 
         if (error_message === null) {
             this.#jquery_objects.$error_message_container.hide();
         } else {
-            console.log(F + ": displaying " + error_message);
+            console.log(F + ": displaying error " + error_message);
 
             this.#jquery_objects.$error_message.text(error_message);
             this.#jquery_objects.$error_message_container.show();
         }
     }
 
     // -------------------------------------------------------------
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -11,16 +11,16 @@
         this.name = name;
         this.debug_identifier = name;
         this.precisionLine = precisionLine;
     } // end constructor
 
     // -------------------------------------------------------------
 
-    activate(raphael, color) {
-        var F = "webviz__hair__Guide2::activate";
+    activate(raphael, color, is_draggable) {
+        var F = "webviz__hair__Guide2[" + this.name + "]::activate";
 
         this._raphael = raphael
 
         raphael.setStart();
 
         this._hline = this._raphael.path("M0,0:L1,0").attr({
             stroke: color,
@@ -58,22 +58,23 @@
 
         this._vline._group = this._group;
         this._vline._parent_object = this;
 
         this._ball._group = this._group;
         this._ball._parent_object = this;
 
-        this._group.drag(this._drag_move, this._drag_start, this._drag_stop);
+        if (is_draggable)
+            this._group.drag(this._drag_move, this._drag_start, this._drag_stop);
 
-        console.log(F + " activated")
+        console.log(F + ": activated")
     } // end method
 
     // -------------------------------------------------------------
     set_box(settings) {
-        var F = "webviz__hair__Guide2::set_box";
+        var F = "webviz__hair__Guide2[" + this.name + "]::set_box";
 
         for (var k in settings) {
             var setting = settings[k];
 
             if (k == "position") {
                 console.log(F + ": setting position [" + setting.x + ", " + setting.y + "]")
 
@@ -104,15 +105,15 @@
         }
     } // end method
 
     // -------------------------------------------------------------
     // Returns the currents settings in a JSON-serializable structure.
 
     get() {
-        var F = "webviz__hair__Guide2::get";
+        var F = "webviz__hair__Guide2[" + this.name + "]::get";
 
         var settings = {};
 
         // Position to where the group's anchor point has been moved.
         var x = this._ball.matrix.x(0, 0);
         var y = this._ball.matrix.y(0, 0);
 
@@ -132,17 +133,17 @@
 
         this._parent_object._trigger_change_event(webviz__hair__Guide2__UserMotionEvent);
 
     } // end method
 
     // -------------------------------------------------------------
     _drag_start() {
-        var F = "webviz__hair__Guide2::_drag_start";
+        var F = "webviz__hair__Guide2[" + this._parent_object.name + "]::_drag_start";
 
-        console.log(F + " drag start")
+        console.log(F + ": drag start")
 
         // var keys = new Array();
         // for (var k in this)
         // {
         //     keys.push(k);
         // }
         // console.log("this is " + this.toString() + "\n" + JSON.stringify(keys));
@@ -150,33 +151,33 @@
         this.ody = 0;
 
         this.timeout = undefined;
     }
 
     // -------------------------------------------------------------
     _drag_stop() {
-        var F = "webviz__hair__Guide2::_drag_stop";
+        var F = "webviz__hair__Guide2[" + this._parent_object.name + "]::_drag_stop";
 
         // Not yet started the timeout?
         if (this.timeout === undefined) {
-            console.log(F + " drag stop");
+            console.log(F + ": drag stop");
             var that = this;
             // Notify listeners in separate thread.
             this.timeout = setTimeout(function() {
                 that._parent_object._trigger_change_event(webviz__hair__Guide2__UserChangeEvent)
             }, 1);
         }
     }
 
     // -------------------------------------------------------------
     _trigger_change_event(event, detail) {
-        var F = "webviz__hair__Guide2::_trigger_change_event";
+        var F = "webviz__hair__Guide2[" + this.name + "]::_trigger_change_event";
 
         if (event == webviz__hair__Guide2__UserChangeEvent)
-            console.log(F + " triggering " + event);
+            console.log(F + ": triggering " + event);
 
         // Trigger an event that the index.js will use to coordinate cross-widget changes.
         var custom_event = new CustomEvent(event, {
             detail: detail
         });
 
         this.dispatchEvent(custom_event);
```

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/targeting.html` & `echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.html`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/guis/html/targeting.js` & `echolocator-1.0.1/src/echolocator_lib/guis/html/targeting.js`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/src/echolocator_lib/version.py` & `echolocator-1.0.1/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/configurations/laptop.yaml` & `echolocator-1.0.1/configurations/development.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,72 @@
 type: echolocator_lib.echolocator_contexts.classic
 
-visit:
-    beamline: b29
-    year: 2022
-    visit: cy29757-3
-    directory: /dls/b29/data/2022/cy29757-3
-    # Format to make actual data_filename using data_label as token.
-    data_path_pattern: "/dls/b29/data/2022/cy29757-3/Merlin/{data_label}_data.mib"
-
 logging_settings:
     console:
         enabled: True
         verbose: True
+        filters:
+            markers:
+                - "[RELCOOK]"
+                - "[COOKSEL]"
+                - "[COOKOFF]"
+                - "[GUITABS]"
+                - "[SETTINGVAL]"
     logfile:
         enabled: True
         directory: ${output_directory}/logfile.log
     graypy:
         enabled: False
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
-    dls_servbase_dataface_server: &DLS_BILLY_DATAFACE_SERVER http://*:27620
-    dls_servbase_dataface_client: &DLS_BILLY_DATAFACE_CLIENT http://localhost:27620
-    dataface_port: &DATAFACE_PORT 27621
+    dls_servbase_database_filename: &DLS_SERVBASE_DATABASE_FILENAME /scratch/${USER}/echolocator/databases/dls_servbase_dataface.sqlite
+    database_filename: &DATABASE_FILENAME /scratch/${USER}/echolocator/databases/runtime/echolocator.sqlite
+    dls_servbase_dataface_server: &DLS_SERVBASE_DATAFACE_SERVER http://*:27620
+    dls_servbase_dataface_client: &DLS_SERVBASE_DATAFACE_CLIENT http://localhost:27620
     echolocator_gui_server: &ECHOLOCATOR_GUI_SERVER http://*:27622
     echolocator_gui_client: &ECHOLOCATOR_GUI_CLIENT http://127.0.0.1:27622
 
 # The dls_servbase_dataface client/server composite.
-dls_servbase_dataface_specification: &DLS_BILLY_DATAFACE_SPECIFICATION
+dls_servbase_dataface_specification: &DLS_SERVBASE_DATAFACE_SPECIFICATION
     type: "dls_servbase_lib.datafaces.aiohttp"
     type_specific_tbd:
         # The remote dataface server access.
         aiohttp_specification:
-            server: *DLS_BILLY_DATAFACE_SERVER
-            client: *DLS_BILLY_DATAFACE_CLIENT
+            server: *DLS_SERVBASE_DATAFACE_SERVER
+            client: *DLS_SERVBASE_DATAFACE_CLIENT
         # The local implementation of the dataface.
         actual_dataface_specification:
             type: "dls_servbase_lib.datafaces.aiosqlite"
             database:
                 type: "dls_servbase_lib.databases.aiosqlite"
-                filename: "${output_directory}/dls_servbase_dataface.sqlite"
+                filename: *DLS_SERVBASE_DATABASE_FILENAME
                 log_level: "WARNING"
     context:
-        start_as: process
+        start_as: coro
 
-# The echolocator_dataface client/server composite.
-echolocator_dataface_specification: &ECHOLOCATOR_DATAFACE_SPECIFICATION
-    type: "echolocator_lib.echolocator_datafaces.aiohttp"
-    type_specific_tbd:
-        # The remote echolocator_dataface server access.
-        aiohttp_specification:
-            server_host: "*"
-            client_host: "127.0.0.1"
-            port: *DATAFACE_PORT
-        # The local implementation of the echolocator_dataface.
-        actual_echolocator_dataface_specification:
-            type: "echolocator_lib.echolocator_datafaces.aiosqlite"
-            database:
-                type: "echolocator_lib.echolocator_databases.aiosqlite"
-                filename: "${output_directory}/echolocator_dataface.sqlite"
-                log_level: "WARNING"
-    context:
-        start_as: process
+# The xchembku_dataface direct access.
+xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
+    type: "xchembku_lib.xchembku_datafaces.direct"
+    database:
+        type: "xchembku_lib.xchembku_databases.normsql"
+        filename: *DATABASE_FILENAME
+        log_level: "WARNING"
 
 # The echolocator_gui specification.
 echolocator_gui_specification:
-    type: "echolocator_lib.echolocator_guis.aiohttp"
+    type: "echolocator_lib.guis.aiohttp"
     type_specific_tbd:
         # The remote echolocator_gui server access.
         aiohttp_specification:
             server: *ECHOLOCATOR_GUI_SERVER
             client: *ECHOLOCATOR_GUI_CLIENT
             search_paths: ["examples/html"]
             cookie_specification:
                 type: "dls_servbase_lib.cookies.dataface"
                 type_specific_tbd:
-                    dataface_specification: *DLS_BILLY_DATAFACE_SPECIFICATION
-    # The dataface which the gui talks to.
-    echolocator_dataface_specification: *ECHOLOCATOR_DATAFACE_SPECIFICATION
+                    dataface_specification: *DLS_SERVBASE_DATAFACE_SPECIFICATION
     context:
-        start_as: process
+        start_as: coro
```

### Comparing `echolocator-0.0.1/tests/conftest.py` & `echolocator-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/example_images/1.jpg` & `echolocator-1.0.1/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/example_images/2.jpg` & `echolocator-1.0.1/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/example_images/3.jpg` & `echolocator-1.0.1/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/example_images/4.png` & `echolocator-1.0.1/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/images/1.jpg` & `echolocator-1.0.1/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/images/2.jpg` & `echolocator-1.0.1/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-0.0.1/tests/images/3.jpg` & `echolocator-1.0.1/tests/images/3.jpg`

 * *Files identical despite different names*

