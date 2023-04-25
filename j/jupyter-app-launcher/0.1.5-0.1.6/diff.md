# Comparing `tmp/jupyter_app_launcher-0.1.5.tar.gz` & `tmp/jupyter_app_launcher-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_app_launcher-0.1.5.tar", last modified: Thu Oct 13 19:28:42 2022, max compression
+gzip compressed data, was "jupyter_app_launcher-0.1.6.tar", last modified: Tue Apr 25 13:31:44 2023, max compression
```

## Comparing `jupyter_app_launcher-0.1.5.tar` & `jupyter_app_launcher-0.1.6.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     4434 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3896 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-13 19:26:21.000000 jupyter_app_launcher-0.1.5/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/install.json
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jest.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.312398 jupyter_app_launcher-0.1.5/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter-config/nb-config/jupyter_app_launcher.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter-config/server-config/jupyter_app_launcher.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher/
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/base_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/notebook_voila_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/url_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/handler_factory_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)    15569 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/185.82fac5cc1c6565bd7ef8.js
--rw-r--r--   0 runner    (1001) docker     (121)    16646 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/928.0c42755f6c12a4749474.js
--rw-r--r--   0 runner    (1001) docker     (121)    73231 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8250 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/remoteEntry.124741e093a93bb3edd8.js
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-13 19:28:39.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/schema/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/script.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3896 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 19:26:38.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-13 19:28:42.000000 jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-10-13 19:27:06.000000 jupyter_app_launcher-0.1.5/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.316398 jupyter_app_launcher-0.1.5/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/__tests__/jupyter_app_launcher.spec.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/app_tracker.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/documents/
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/documents/factory.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/documents/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/documents/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.312398 jupyter_app_launcher-0.1.5/src/factories/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/factories/local_server/
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/local_server/local_server_factory.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/factories/markdown/
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/markdown/custom_context.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/markdown/markdown_factory.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/factories/notebook/
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook/notebook_factory.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/app_model.ts
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/app_widget.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/create_notebook_panel.ts
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/custom_context.ts
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/item.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_grid/notebook_grid_factory.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/factories/notebook_voila/
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/notebook_voila/notebook_voila_factory.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/src/factories/url/
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factories/url/url_factory.ts
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/factory_manager.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (121)     4576 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/manager_plugin.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/running_launcher_app.ts
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/schema.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/token.ts
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/style/
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/style/base.css
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/style/index.css
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/style/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/ui-tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/ui-tests/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/ui-tests/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/ui-tests/playwright.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 19:28:42.320398 jupyter_app_launcher-0.1.5/ui-tests/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/ui-tests/tests/jupyter_app_launcher.spec.ts
--rw-r--r--   0 runner    (1001) docker     (121)   452195 2022-10-13 19:26:22.000000 jupyter_app_launcher-0.1.5/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jest.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.397894 jupyter_app_launcher-0.1.6/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.401894 jupyter_app_launcher-0.1.6/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter-config/nb-config/jupyter_app_launcher.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.401894 jupyter_app_launcher-0.1.6/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter-config/server-config/jupyter_app_launcher.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.401894 jupyter_app_launcher-0.1.6/jupyter_app_launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/base_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/notebook_voila_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/url_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/handler_factory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/185.82fac5cc1c6565bd7ef8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16646 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/928.8a7a4cbe74d3e7e248e6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73231 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/remoteEntry.7f954df4c15496d19670.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 13:31:41.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/jupyter_app_launcher/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/schema/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/jupyter_app_launcher/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:29:20.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 13:31:44.000000 jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-25 13:30:04.000000 jupyter_app_launcher-0.1.6/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.405894 jupyter_app_launcher-0.1.6/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/__tests__/jupyter_app_launcher.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/app_tracker.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/documents/factory.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/documents/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/documents/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.401894 jupyter_app_launcher-0.1.6/src/factories/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/factories/local_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/local_server/local_server_factory.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/factories/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/markdown/custom_context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/markdown/markdown_factory.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/factories/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook/notebook_factory.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/app_model.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/app_widget.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/create_notebook_panel.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/custom_context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/item.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_grid/notebook_grid_factory.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/factories/notebook_voila/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/notebook_voila/notebook_voila_factory.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/src/factories/url/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factories/url/url_factory.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/factory_manager.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/manager_plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/running_launcher_app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/schema.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/token.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/src/tools.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/ui-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/ui-tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/ui-tests/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/ui-tests/playwright.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:44.409894 jupyter_app_launcher-0.1.6/ui-tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/ui-tests/tests/jupyter_app_launcher.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   452195 2023-04-25 13:28:58.000000 jupyter_app_launcher-0.1.6/yarn.lock
```

### Comparing `jupyter_app_launcher-0.1.5/CHANGELOG.md` & `jupyter_app_launcher-0.1.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.6
+
+([Full Changelog](https://github.com/trungleduc/jupyter_app_launcher/compare/v0.1.5...1633002852cafdc3bd97165e86bab9967f3474c4))
+
+### Merged PRs
+
+- Substitute environment variables in URL source [#28](https://github.com/trungleduc/jupyter_app_launcher/pull/28) ([@sinkuladis](https://github.com/sinkuladis))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/trungleduc/jupyter_app_launcher/graphs/contributors?from=2022-10-13&to=2023-04-25&type=c))
+
+[@sinkuladis](https://github.com/search?q=repo%3Atrungleduc%2Fjupyter_app_launcher+involves%3Asinkuladis+updated%3A2022-10-13..2023-04-25&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.5
 
 ([Full Changelog](https://github.com/trungleduc/jupyter_app_launcher/compare/v0.1.4...7040059d7c75904332f7d08a1f1e374e2ef3c117))
 
 ### Merged PRs
 
 - Fix missing session of grid app [#14](https://github.com/trungleduc/jupyter_app_launcher/pull/14) ([@trungleduc](https://github.com/trungleduc))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/trungleduc/jupyter_app_launcher/graphs/contributors?from=2022-10-10&to=2022-10-13&type=c))
 
 [@trungleduc](https://github.com/search?q=repo%3Atrungleduc%2Fjupyter_app_launcher+involves%3Atrungleduc+updated%3A2022-10-10..2022-10-13&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.4
 
 ([Full Changelog](https://github.com/trungleduc/jupyter_app_launcher/compare/v0.1.3...905393074b86d038ec2d82b5ade81158a2f7d44f))
 
 ### Enhancements made
 
 - Add notebook gridstack document [#11](https://github.com/trungleduc/jupyter_app_launcher/pull/11) ([@trungleduc](https://github.com/trungleduc))
```

### Comparing `jupyter_app_launcher-0.1.5/LICENSE` & `jupyter_app_launcher-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/MANIFEST.in` & `jupyter_app_launcher-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/PKG-INFO` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyter_app_launcher
-Version: 0.1.5
+Name: jupyter-app-launcher
+Version: 0.1.6
 Summary: A JupyterLab extension to create custom launcher entries.
 Home-page: https://github.com/trungleduc/jupyter_app_launcher
 Author: Trung Le
 Author-email: leductrungxf@gmail.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -25,15 +25,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <h1 align="center">jupyter_app_launcher</h1>
 
-[![Github Actions Status](https://github.com/trungleduc/jupyter_app_launcher/workflows/Build/badge.svg)](https://github.com/trungleduc/jupyter_app_launcher/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/jupyter-app-launcher/badge/?version=latest)](https://jupyter-app-launcher.readthedocs.io/en/latest/?badge=latest) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trungleduc/jupyter_app_launcher/main?urlpath=lab) [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://trungleduc.github.io/jupyter_app_launcher/lab/index.html) [![GitHub license](https://badgen.net/github/license/trungleduc/jupyter_app_launcher)](https://github.com/trungleduc/jupyter_app_launcher/blob/master/LICENSE)
+[![Github Actions Status](https://github.com/trungleduc/jupyter_app_launcher/workflows/Build/badge.svg)](https://github.com/trungleduc/jupyter_app_launcher/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/jupyter-app-launcher/badge/?version=latest)](https://jupyter-app-launcher.readthedocs.io/en/latest/?badge=latest) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trungleduc/jupyter_app_launcher/main?urlpath=lab) [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://trungleduc.github.io/jupyter_app_launcher/lab/index.html)
 
 <h2 align="center"> A JupyterLab extension to create custom launcher entries </h2>
 
 **jupyter_app_launcher** helps users customize the JupyterLab launcher with a simple YAML file. Users can add custom entries to the launcher to:
 
 - Open a predefined notebook or markdown file.
 - Render a notebook in dashboard mode
```

### Comparing `jupyter_app_launcher-0.1.5/README.md` & `jupyter_app_launcher-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">jupyter_app_launcher</h1>
 
-[![Github Actions Status](https://github.com/trungleduc/jupyter_app_launcher/workflows/Build/badge.svg)](https://github.com/trungleduc/jupyter_app_launcher/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/jupyter-app-launcher/badge/?version=latest)](https://jupyter-app-launcher.readthedocs.io/en/latest/?badge=latest) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trungleduc/jupyter_app_launcher/main?urlpath=lab) [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://trungleduc.github.io/jupyter_app_launcher/lab/index.html) [![GitHub license](https://badgen.net/github/license/trungleduc/jupyter_app_launcher)](https://github.com/trungleduc/jupyter_app_launcher/blob/master/LICENSE)
+[![Github Actions Status](https://github.com/trungleduc/jupyter_app_launcher/workflows/Build/badge.svg)](https://github.com/trungleduc/jupyter_app_launcher/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/jupyter-app-launcher/badge/?version=latest)](https://jupyter-app-launcher.readthedocs.io/en/latest/?badge=latest) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trungleduc/jupyter_app_launcher/main?urlpath=lab) [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://trungleduc.github.io/jupyter_app_launcher/lab/index.html)
 
 <h2 align="center"> A JupyterLab extension to create custom launcher entries </h2>
 
 **jupyter_app_launcher** helps users customize the JupyterLab launcher with a simple YAML file. Users can add custom entries to the launcher to:
 
 - Open a predefined notebook or markdown file.
 - Render a notebook in dashboard mode
```

### Comparing `jupyter_app_launcher-0.1.5/RELEASE.md` & `jupyter_app_launcher-0.1.6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jest.config.js` & `jupyter_app_launcher-0.1.6/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/__init__.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/_version.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/base_factory.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/base_factory.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/notebook_voila_factory.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/notebook_voila_factory.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/factories/url_factory.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/factories/url_factory.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/handler_factory_manager.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/handler_factory_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/handlers.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/package.json` & `jupyter_app_launcher-0.1.6/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.1.6'"}*

```diff
@@ -55,19 +55,14 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.124741e093a93bb3edd8.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_app_launcher"
                 },
                 "managers": [
                     "pip"
@@ -122,9 +117,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/185.82fac5cc1c6565bd7ef8.js` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/185.82fac5cc1c6565bd7ef8.js`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/928.0c42755f6c12a4749474.js` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/928.8a7a4cbe74d3e7e248e6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunkjupyter_app_launcher = self.webpackChunkjupyter_app_launcher || []).push([
     [928], {
         928: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => Y
             });
-            var o = n(12),
-                i = n(61),
-                s = n(512),
-                r = n(132),
+            var o = n(142),
+                i = n(33),
+                s = n(467),
+                r = n(154),
                 a = n(840),
-                d = n(322);
+                d = n(820);
             async function c(e = {}, t = "") {
                 const n = d.ServerConnection.makeSettings(),
                     i = o.URLExt.join(n.baseUrl, "jupyterlab-app-launcher", t);
                 let s;
                 try {
                     s = await d.ServerConnection.makeRequest(i, e, n)
                 } catch (e) {
@@ -92,17 +92,17 @@
                         a.url = d + e, l.resolve()
                     })), {
                         panel: a,
                         ready: l.promise
                     }
                 }
             }
-            var h = n(906),
-                g = n(613),
-                m = n(377);
+            var h = n(486),
+                g = n(123),
+                m = n(86);
             class y {
                 constructor(e) {
                     this.options = e
                 }
                 async create(e, t) {
                     if (!e.sourceCode) return;
                     const n = t.cwd,
@@ -122,30 +122,30 @@
                         await s.context.rename(`${e.title}${0===a?"":"-"+a}.ipynb`), r = !0
                     } catch (e) {
                         a += 1
                     }
                     await s.context.save(), await s.sessionContext.ready, s.content.activeCellIndex = 1
                 }
             }
-            var w = n(861),
-                v = n(891),
-                f = n(177),
-                _ = n(527);
+            var w = n(191),
+                v = n(135),
+                f = n(413),
+                _ = n(819);
             class b extends _.Context {
                 async save() {
                     await this.ready
                 }
                 async saveAs() {
                     await this.ready
                 }
                 async revert() {
                     await this.ready
                 }
             }
-            var k, C = n(992);
+            var k, C = n(832);
             class x extends C.Panel {
                 constructor(e, t, n) {
                     super(), this.removeClass("lm-Widget"), this.removeClass("p-Widget"), this.addClass("grid-stack-item");
                     const o = new C.Panel;
                     o.addClass("grid-stack-item-content"), t.addClass("grid-item-widget"), o.addWidget(t), this.addWidget(o), this._cellOutput = t, this._info = n, this.cellIdentity = e
                 }
                 get cellOutput() {
@@ -512,15 +512,15 @@
                 get ready() {
                     return this._customReadyPromise.promise
                 }
                 resolveReady() {
                     this._customReadyPromise.resolve(void 0)
                 }
             }
-            var j = n(586);
+            var j = n(161);
             class A {
                 constructor(e) {
                     this.options = e
                 }
                 async create(e, t) {
                     if (!e.sourceCode) return void console.error("Missing source code!");
                     await this.options.manager.ready;
@@ -571,15 +571,15 @@
                         manager: e.serviceManager,
                         rendermime: t
                     });
                     return s.registerFactory("markdown", p), s
                 },
                 provides: T
             };
-            var J = n(655);
+            var J = n(502);
 
             function L(e) {
                 const t = p.UUID.uuid4(),
                     n = e.split(" ");
                 let o;
                 o = 1 === n.length ? n[0].substring(0, 2) : `${n[0].substring(0,1)}${n[1].substring(0,1)}`;
                 const i = `<svg class="jp-al-app-icon" width="16" viewBox="0 0 24 24" role="img" xmlns="http://www.w3.org/2000/svg"><text x="0" y="16" fill="#000" style="font-size: 14px">${o.toUpperCase()}</text></svg>`;
```

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/remoteEntry.124741e093a93bb3edd8.js` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/remoteEntry.7f954df4c15496d19670.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, u, i, l, f, s, d, p, c, h, v, b, y, m, g, j, w, _ = {
+    var e, r, t, n, a, o, u, i, l, s, d, f, p, c, h, v, b, y, m, g, j, w, _ = {
             299: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(928).then((() => () => t(928))),
                         "./extension": () => t.e(928).then((() => () => t(928))),
                         "./style": () => t.e(185).then((() => () => t(185)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,50 +44,50 @@
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         185: "82fac5cc1c6565bd7ef8",
-        928: "0c42755f6c12a4749474",
+        928: "8a7a4cbe74d3e7e248e6",
         929: "e93d30d17e899a596fd8"
     } [e] + ".js?v=" + {
         185: "82fac5cc1c6565bd7ef8",
-        928: "0c42755f6c12a4749474",
+        928: "8a7a4cbe74d3e7e248e6",
         929: "e93d30d17e899a596fd8"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter_app_launcher:", S.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var u, i;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        u = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
+                        u = d;
                         break
                     }
                 }
             u || (i = !0, (u = document.createElement("script")).charset = "utf-8", u.timeout = 120, S.nc && u.setAttribute("nonce", S.nc), u.setAttribute("data-webpack", r + a), u.src = t), e[t] = [n];
-            var d = (r, n) => {
+            var f = (r, n) => {
                     u.onerror = u.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], u.parentNode && u.parentNode.removeChild(u), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: u
                 }), 12e4);
-            u.onerror = d.bind(null, u.onerror), u.onload = d.bind(null, u.onload), i && document.head.appendChild(u)
+            u.onerror = f.bind(null, u.onerror), u.onload = f.bind(null, u.onload), i && document.head.appendChild(u)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -109,15 +109,15 @@
                         (!i || !i.loaded && (!n != !i.eager ? n : u > i.from)) && (a[r] = {
                             get: t,
                             from: u,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (i("gridstack", "6.0.2", (() => S.e(929).then((() => () => S(929))))), i("jupyter_app_launcher", "0.1.5", (() => S.e(928).then((() => () => S(928)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("gridstack", "6.0.2", (() => S.e(929).then((() => () => S(929))))), i("jupyter_app_launcher", "0.1.6", (() => S.e(928).then((() => () => S(928)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -166,33 +166,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var u = 0, i = 1, l = !0;; i++, u++) {
-                var f, s, d = i < e.length ? (typeof e[i])[0] : "";
-                if (u >= r.length || "o" == (s = (typeof(f = r[u]))[0])) return !l || ("u" == d ? i > n && !a : "" == d != a);
-                if ("u" == s) {
-                    if (!l || "u" != d) return !1
+                var s, d, f = i < e.length ? (typeof e[i])[0] : "";
+                if (u >= r.length || "o" == (d = (typeof(s = r[u]))[0])) return !l || ("u" == f ? i > n && !a : "" == f != a);
+                if ("u" == d) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == s)
+                    if (f == d)
                         if (i <= n) {
-                            if (f != e[i]) return !1
+                            if (s != e[i]) return !1
                         } else {
-                            if (a ? f > e[i] : f < e[i]) return !1;
-                            f != e[i] && (l = !1)
+                            if (a ? s > e[i] : s < e[i]) return !1;
+                            s != e[i] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (a || i <= n) return !1;
                     l = !1, i--
                 } else {
-                    if (i <= n || s < d != a) return !1;
+                    if (i <= n || d < f != a) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, i--)
+                } else "s" != f && "n" != f && (l = !1, i--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (u = 1; u < e.length; u++) {
             var h = e[u];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -204,54 +204,54 @@
         return t
     }, i = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = l(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(f(e, t, a, n)), h(e[t][a])
-    }, d = (e, r, t) => {
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(s(e, t, a, n)), h(e[t][a])
+    }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, p = (e, r, t, n) => {
         var o = e[t];
         return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = (e, r, t, n) => {
         "undefined" != typeof console && console.warn && console.warn(p(e, r, t, n))
     }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, a) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
-    })(((e, r, t, n) => (u(e, t), h(d(r, t, n) || c(r, e, t, n) || i(r, t))))), y = v(((e, r, t, n) => (u(e, t), s(r, 0, t, n)))), m = v(((e, r, t, n, a) => {
-        var o = r && S.o(r, t) && d(r, t, n);
+    })(((e, r, t, n) => (u(e, t), h(f(r, t, n) || c(r, e, t, n) || i(r, t))))), y = v(((e, r, t, n) => (u(e, t), d(r, 0, t, n)))), m = v(((e, r, t, n, a) => {
+        var o = r && S.o(r, t) && f(r, t, n);
         return o ? h(o) : a()
     })), g = {}, j = {
-        12: () => y("default", "@jupyterlab/coreutils", [1, 5, 4, 8]),
-        61: () => y("default", "@jupyterlab/apputils", [1, 3, 4, 8]),
-        132: () => b("default", "@jupyterlab/running", [1, 3, 4, 8]),
-        177: () => y("default", "@jupyterlab/codemirror", [1, 3, 4, 8]),
-        322: () => y("default", "@jupyterlab/services", [1, 6, 4, 8]),
-        377: () => y("default", "@jupyterlab/rendermime", [1, 3, 4, 8]),
-        512: () => y("default", "@jupyterlab/launcher", [1, 3, 4, 8]),
+        33: () => y("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        86: () => y("default", "@jupyterlab/rendermime", [1, 3, 6, 3]),
+        123: () => y("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        135: () => b("default", "@jupyterlab/outputarea", [1, 3, 6, 3]),
+        142: () => y("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        154: () => b("default", "@jupyterlab/running", [1, 3, 6, 3]),
+        161: () => y("default", "@jupyterlab/markdownviewer", [1, 3, 6, 3]),
+        191: () => b("default", "@jupyterlab/cells", [1, 3, 6, 3]),
+        413: () => y("default", "@jupyterlab/codemirror", [1, 3, 6, 3]),
+        467: () => y("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
+        486: () => y("default", "@jupyterlab/codeeditor", [1, 3, 6, 3]),
+        502: () => y("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
         526: () => y("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        527: () => b("default", "@jupyterlab/docregistry", [1, 3, 4, 8]),
-        586: () => y("default", "@jupyterlab/markdownviewer", [1, 3, 4, 8]),
-        613: () => y("default", "@jupyterlab/notebook", [1, 3, 4, 8]),
-        655: () => y("default", "@jupyterlab/ui-components", [1, 3, 4, 8]),
         720: () => y("default", "@lumino/messaging", [1, 1, 10, 0]),
         784: () => m("default", "gridstack", [1, 6, 0, 1], (() => S.e(929).then((() => () => S(929))))),
+        819: () => b("default", "@jupyterlab/docregistry", [1, 3, 6, 3]),
+        820: () => y("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        832: () => y("default", "@lumino/widgets", [1, 1, 37, 2]),
         840: () => y("default", "@lumino/signaling", [1, 1, 10, 0]),
-        861: () => b("default", "@jupyterlab/cells", [1, 3, 4, 8]),
-        891: () => b("default", "@jupyterlab/outputarea", [1, 3, 4, 8]),
-        906: () => y("default", "@jupyterlab/codeeditor", [1, 3, 4, 8]),
-        918: () => y("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        992: () => y("default", "@lumino/widgets", [1, 1, 33, 0])
+        918: () => y("default", "@lumino/algorithm", [1, 1, 9, 0])
     }, w = {
-        928: [12, 61, 132, 177, 322, 377, 512, 526, 527, 586, 613, 655, 720, 784, 840, 861, 891, 906, 918, 992]
+        928: [33, 86, 123, 135, 142, 154, 161, 191, 413, 467, 486, 502, 526, 720, 784, 819, 820, 832, 840, 918]
     }, S.f.consumes = (e, r) => {
         S.o(w, e) && w[e].forEach((e => {
             if (S.o(g, e)) return r.push(g[e]);
             var t = r => {
                     g[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
```

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/labextension/static/third-party-licenses.json` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/schema/config.schema.json` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/schema/config.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/script.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/script.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher/utils.py` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         validate(data, SCHEMA)
         source_config = data.get('source', None)
         type_config = data.get('type')
         if source_config is not None:
             data['sourceCode'] = path_to_res(source_config, cwd)
         if type_config not in ['url', 'local-server']:
             data['source'] = create_abs_path(source_config, cwd)
+        if type_config == 'url':
+            data['source'] = os.path.expandvars(source_config)
         if data.get('icon', None) is not None:
             data['icon'] = path_to_res(data['icon'], cwd)
         cwd_config = data.get('cwd', None)
         if cwd_config is not None:
             data['cwd'] = create_abs_path(cwd_config, cwd)
         return True
     except Exception:
```

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/PKG-INFO` & `jupyter_app_launcher-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyter-app-launcher
-Version: 0.1.5
+Name: jupyter_app_launcher
+Version: 0.1.6
 Summary: A JupyterLab extension to create custom launcher entries.
 Home-page: https://github.com/trungleduc/jupyter_app_launcher
 Author: Trung Le
 Author-email: leductrungxf@gmail.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -25,15 +25,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <h1 align="center">jupyter_app_launcher</h1>
 
-[![Github Actions Status](https://github.com/trungleduc/jupyter_app_launcher/workflows/Build/badge.svg)](https://github.com/trungleduc/jupyter_app_launcher/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/jupyter-app-launcher/badge/?version=latest)](https://jupyter-app-launcher.readthedocs.io/en/latest/?badge=latest) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trungleduc/jupyter_app_launcher/main?urlpath=lab) [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://trungleduc.github.io/jupyter_app_launcher/lab/index.html) [![GitHub license](https://badgen.net/github/license/trungleduc/jupyter_app_launcher)](https://github.com/trungleduc/jupyter_app_launcher/blob/master/LICENSE)
+[![Github Actions Status](https://github.com/trungleduc/jupyter_app_launcher/workflows/Build/badge.svg)](https://github.com/trungleduc/jupyter_app_launcher/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/jupyter-app-launcher/badge/?version=latest)](https://jupyter-app-launcher.readthedocs.io/en/latest/?badge=latest) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/trungleduc/jupyter_app_launcher/main?urlpath=lab) [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://trungleduc.github.io/jupyter_app_launcher/lab/index.html)
 
 <h2 align="center"> A JupyterLab extension to create custom launcher entries </h2>
 
 **jupyter_app_launcher** helps users customize the JupyterLab launcher with a simple YAML file. Users can add custom entries to the launcher to:
 
 - Open a predefined notebook or markdown file.
 - Render a notebook in dashboard mode
```

### Comparing `jupyter_app_launcher-0.1.5/jupyter_app_launcher.egg-info/SOURCES.txt` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 jupyter_app_launcher.egg-info/top_level.txt
 jupyter_app_launcher/factories/__init__.py
 jupyter_app_launcher/factories/base_factory.py
 jupyter_app_launcher/factories/notebook_voila_factory.py
 jupyter_app_launcher/factories/url_factory.py
 jupyter_app_launcher/labextension/package.json
 jupyter_app_launcher/labextension/static/185.82fac5cc1c6565bd7ef8.js
-jupyter_app_launcher/labextension/static/928.0c42755f6c12a4749474.js
+jupyter_app_launcher/labextension/static/928.8a7a4cbe74d3e7e248e6.js
 jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js
 jupyter_app_launcher/labextension/static/929.e93d30d17e899a596fd8.js.LICENSE.txt
-jupyter_app_launcher/labextension/static/remoteEntry.124741e093a93bb3edd8.js
+jupyter_app_launcher/labextension/static/remoteEntry.7f954df4c15496d19670.js
 jupyter_app_launcher/labextension/static/style.js
 jupyter_app_launcher/labextension/static/third-party-licenses.json
 jupyter_app_launcher/schema/config.schema.json
 jupyter_app_launcher/tests/__init__.py
 jupyter_app_launcher/tests/test_handlers.py
 src/app_tracker.ts
 src/factory_manager.ts
```

### Comparing `jupyter_app_launcher-0.1.5/package.json` & `jupyter_app_launcher-0.1.6/jupyter_app_launcher/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.7f954df4c15496d19670.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -55,14 +55,19 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.7f954df4c15496d19670.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_app_launcher"
                 },
                 "managers": [
                     "pip"
@@ -117,9 +122,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `jupyter_app_launcher-0.1.5/pyproject.toml` & `jupyter_app_launcher-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/setup.py` & `jupyter_app_launcher-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/app_tracker.ts` & `jupyter_app_launcher-0.1.6/src/app_tracker.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/documents/factory.ts` & `jupyter_app_launcher-0.1.6/src/documents/factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/documents/plugin.ts` & `jupyter_app_launcher-0.1.6/src/documents/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/documents/widget.ts` & `jupyter_app_launcher-0.1.6/src/documents/widget.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/local_server/local_server_factory.ts` & `jupyter_app_launcher-0.1.6/src/factories/local_server/local_server_factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/markdown/custom_context.ts` & `jupyter_app_launcher-0.1.6/src/factories/markdown/custom_context.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/markdown/markdown_factory.ts` & `jupyter_app_launcher-0.1.6/src/factories/markdown/markdown_factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook/notebook_factory.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook/notebook_factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook_grid/app_model.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook_grid/app_model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook_grid/app_widget.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook_grid/app_widget.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook_grid/create_notebook_panel.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook_grid/create_notebook_panel.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook_grid/item.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook_grid/item.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook_grid/notebook_grid_factory.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook_grid/notebook_grid_factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/notebook_voila/notebook_voila_factory.ts` & `jupyter_app_launcher-0.1.6/src/factories/notebook_voila/notebook_voila_factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factories/url/url_factory.ts` & `jupyter_app_launcher-0.1.6/src/factories/url/url_factory.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/factory_manager.ts` & `jupyter_app_launcher-0.1.6/src/factory_manager.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/handler.ts` & `jupyter_app_launcher-0.1.6/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/index.ts` & `jupyter_app_launcher-0.1.6/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/manager_plugin.ts` & `jupyter_app_launcher-0.1.6/src/manager_plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/running_launcher_app.ts` & `jupyter_app_launcher-0.1.6/src/running_launcher_app.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/schema.ts` & `jupyter_app_launcher-0.1.6/src/schema.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/token.ts` & `jupyter_app_launcher-0.1.6/src/token.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/src/tools.ts` & `jupyter_app_launcher-0.1.6/src/tools.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/style/base.css` & `jupyter_app_launcher-0.1.6/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/tsconfig.json` & `jupyter_app_launcher-0.1.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/ui-tests/README.md` & `jupyter_app_launcher-0.1.6/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/ui-tests/jupyter_server_test_config.py` & `jupyter_app_launcher-0.1.6/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/ui-tests/tests/jupyter_app_launcher.spec.ts` & `jupyter_app_launcher-0.1.6/ui-tests/tests/jupyter_app_launcher.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_app_launcher-0.1.5/yarn.lock` & `jupyter_app_launcher-0.1.6/yarn.lock`

 * *Files identical despite different names*

