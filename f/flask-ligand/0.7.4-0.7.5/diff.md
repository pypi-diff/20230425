# Comparing `tmp/flask-ligand-0.7.4.tar.gz` & `tmp/flask-ligand-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-ligand-0.7.4.tar", last modified: Mon Apr 24 22:47:20 2023, max compression
+gzip compressed data, was "flask-ligand-0.7.5.tar", last modified: Mon Apr 24 23:21:27 2023, max compression
```

## Comparing `flask-ligand-0.7.4.tar` & `flask-ligand-0.7.5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.flaskenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.077338 flask-ligand-0.7.4/.github/
--rw-r--r--   0 root         (0) root         (0)      528 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      625 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.github/workflows/bump_and_publish_release.yml
--rw-r--r--   0 root         (0) root         (0)      797 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.github/workflows/coverage.yml
--rw-r--r--   0 root         (0) root         (0)      622 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.github/workflows/pull_request.yml
--rw-r--r--   0 root         (0) root         (0)     1096 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      371 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.readthedocs.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/.run/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Flask - Debug.run.xml
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Flask.run.xml
--rw-r--r--   0 root         (0) root         (0)      459 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Integration Test Environment.run.xml
--rw-r--r--   0 root         (0) root         (0)     1473 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Integration.run.xml
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit (tox).run.xml
--rw-r--r--   0 root         (0) root         (0)      856 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit (tox-fast).run.xml
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit - Database.run.xml
--rw-r--r--   0 root         (0) root         (0)     1045 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit - JWT.run.xml
--rw-r--r--   0 root         (0) root         (0)     1047 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit - OpenAPI.run.xml
--rw-r--r--   0 root         (0) root         (0)     1506 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit - Settings.run.xml
--rw-r--r--   0 root         (0) root         (0)     1459 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/Unit.run.xml
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/develop-venv.run.xml
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/gen-admin-access-token.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/gen-docs.run.xml
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/lint.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/setup-db.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/.run/test-all.run.xml
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    15588 2023-04-24 22:47:16.000000 flask-ligand-0.7.4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     3615 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    34523 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8962 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/Makefile
--rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3683 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/README.rst
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.077338 flask-ligand-0.7.4/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/docker/env_files/
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docker/env_files/integration.env
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/docker/kc-data/
--rw-r--r--   0 root         (0) root         (0)    78994 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docker/kc-data/flask-ligand-realm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/docker/postgres-data/
--rw-r--r--   0 root         (0) root         (0)      589 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docker/postgres-data/create-multiple-postgresql-databases.sh
--rw-r--r--   0 root         (0) root         (0)      799 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/docs/
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.081338 flask-ligand-0.7.4/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     7352 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/_static/small_logo.jpg
--rw-r--r--   0 root         (0) root         (0)     2704 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/api_reference.rst
--rw-r--r--   0 root         (0) root         (0)     6093 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/auth0.rst
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6080 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)     2571 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/database_configuration.rst
--rw-r--r--   0 root         (0) root         (0)     3885 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/developer_guide.rst
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/development.rst
--rw-r--r--   0 root         (0) root         (0)    12374 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/flask_environments.rst
--rw-r--r--   0 root         (0) root         (0)     2411 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1139 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/integration_testing.rst
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)      765 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1304 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/oidc_configuration.rst
--rw-r--r--   0 root         (0) root         (0)     2546 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/openapi.rst
--rw-r--r--   0 root         (0) root         (0)    25967 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/quickstart.rst
--rw-r--r--   0 root         (0) root         (0)     1637 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/release_process.rst
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/flask_ligand/
--rw-r--r--   0 root         (0) root         (0)     3715 2023-04-24 22:47:16.000000 flask-ligand-0.7.4/flask_ligand/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/cli.py
--rw-r--r--   0 root         (0) root         (0)     5441 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/controllers.py
--rw-r--r--   0 root         (0) root         (0)    12650 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/flask_ligand/extensions/
--rw-r--r--   0 root         (0) root         (0)     1514 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6979 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/extensions/api.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/extensions/database.py
--rw-r--r--   0 root         (0) root         (0)     5210 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/extensions/jwt.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/py.typed
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/flask_ligand/views/
--rw-r--r--   0 root         (0) root         (0)     1552 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/flask_ligand/views/common/
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/views/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/views/common/openapi_doc.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/flask_ligand/views/openapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/flask_ligand.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2670 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      276 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 22:47:20.000000 flask-ligand-0.7.4/flask_ligand.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1112 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      329 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      737 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8190 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/tests/integration/migrations/
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/README
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     2736 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/tests/integration/migrations/versions/
--rw-r--r--   0 root         (0) root         (0)      691 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/versions/47f10265b5d7_.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/migrations/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/integration/test_basic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 22:47:20.085338 flask-ligand-0.7.4/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/test_api_extension.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/test_database_extension.py
--rw-r--r--   0 root         (0) root         (0)     6791 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/test_jwt_extension.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/test_openapi_api.py
--rw-r--r--   0 root         (0) root         (0)    21947 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tests/unit/test_settings.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 22:47:15.000000 flask-ligand-0.7.4/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.476063 flask-ligand-0.7.5/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.flaskenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.456062 flask-ligand-0.7.5/.github/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.456062 flask-ligand-0.7.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.github/workflows/bump_and_publish_release.yml
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.github/workflows/coverage.yml
+-rw-r--r--   0 root         (0) root         (0)      622 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.github/workflows/pull_request.yml
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      371 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.readthedocs.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.460062 flask-ligand-0.7.5/.run/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Flask - Debug.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Flask.run.xml
+-rw-r--r--   0 root         (0) root         (0)      459 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Integration Test Environment.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Integration.run.xml
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit (tox).run.xml
+-rw-r--r--   0 root         (0) root         (0)      856 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit (tox-fast).run.xml
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit - Database.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit - JWT.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit - OpenAPI.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit - Settings.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/Unit.run.xml
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/develop-venv.run.xml
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/gen-admin-access-token.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/gen-docs.run.xml
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/lint.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/setup-db.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/.run/test-all.run.xml
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    15799 2023-04-24 23:21:23.000000 flask-ligand-0.7.5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3615 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 23:21:27.476063 flask-ligand-0.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3683 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/README.rst
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.448062 flask-ligand-0.7.5/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.460062 flask-ligand-0.7.5/docker/env_files/
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docker/env_files/integration.env
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.460062 flask-ligand-0.7.5/docker/kc-data/
+-rw-r--r--   0 root         (0) root         (0)    78994 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docker/kc-data/flask-ligand-realm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.460062 flask-ligand-0.7.5/docker/postgres-data/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docker/postgres-data/create-multiple-postgresql-databases.sh
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.464062 flask-ligand-0.7.5/docs/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.464062 flask-ligand-0.7.5/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     7352 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/_static/small_logo.jpg
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/api_reference.rst
+-rw-r--r--   0 root         (0) root         (0)     6093 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/auth0.rst
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/database_configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/developer_guide.rst
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/development.rst
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/flask_environments.rst
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/integration_testing.rst
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)      765 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/oidc_configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/openapi.rst
+-rw-r--r--   0 root         (0) root         (0)    25967 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/quickstart.rst
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/release_process.rst
+-rw-r--r--   0 root         (0) root         (0)      130 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.468062 flask-ligand-0.7.5/flask_ligand/
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-04-24 23:21:23.000000 flask-ligand-0.7.5/flask_ligand/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5441 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/controllers.py
+-rw-r--r--   0 root         (0) root         (0)    12650 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.468062 flask-ligand-0.7.5/flask_ligand/extensions/
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6979 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/extensions/api.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/extensions/database.py
+-rw-r--r--   0 root         (0) root         (0)     5210 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/extensions/jwt.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.468062 flask-ligand-0.7.5/flask_ligand/views/
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.468062 flask-ligand-0.7.5/flask_ligand/views/common/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/views/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/views/common/openapi_doc.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/flask_ligand/views/openapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.468062 flask-ligand-0.7.5/flask_ligand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      276 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 23:21:27.000000 flask-ligand-0.7.5/flask_ligand.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      329 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-24 23:21:27.476063 flask-ligand-0.7.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      737 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.472063 flask-ligand-0.7.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.472063 flask-ligand-0.7.5/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.472063 flask-ligand-0.7.5/tests/integration/migrations/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/README
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.472063 flask-ligand-0.7.5/tests/integration/migrations/versions/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/versions/47f10265b5d7_.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/migrations/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/integration/test_basic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 23:21:27.472063 flask-ligand-0.7.5/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/test_api_extension.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/test_database_extension.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/test_jwt_extension.py
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/test_openapi_api.py
+-rw-r--r--   0 root         (0) root         (0)    21947 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tests/unit/test_settings.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 23:21:22.000000 flask-ligand-0.7.5/tox.ini
```

### Comparing `flask-ligand-0.7.4/.github/dependabot.yml` & `flask-ligand-0.7.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.github/workflows/bump_and_publish_release.yml` & `flask-ligand-0.7.5/.github/workflows/bump_and_publish_release.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.github/workflows/coverage.yml` & `flask-ligand-0.7.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.github/workflows/pull_request.yml` & `flask-ligand-0.7.5/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.pre-commit-config.yaml` & `flask-ligand-0.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Flask - Debug.run.xml` & `flask-ligand-0.7.5/.run/Flask - Debug.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Flask.run.xml` & `flask-ligand-0.7.5/.run/Flask.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Integration.run.xml` & `flask-ligand-0.7.5/.run/Integration.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit (tox).run.xml` & `flask-ligand-0.7.5/.run/Unit (tox).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit (tox-fast).run.xml` & `flask-ligand-0.7.5/.run/Unit (tox-fast).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit - Database.run.xml` & `flask-ligand-0.7.5/.run/Unit - Database.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit - JWT.run.xml` & `flask-ligand-0.7.5/.run/Unit - JWT.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit - OpenAPI.run.xml` & `flask-ligand-0.7.5/.run/Unit - OpenAPI.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit - Settings.run.xml` & `flask-ligand-0.7.5/.run/Unit - Settings.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/.run/Unit.run.xml` & `flask-ligand-0.7.5/.run/Unit.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/CHANGELOG.md` & `flask-ligand-0.7.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Changelog
 =========
 
 <!--next-version-placeholder-->
 
+## v0.7.5 (2023-04-24)
+### Fix
+* :arrow_up: Update myst-parser[linkify] requirement from ~=0.18 to ~=1.0 ([`e66965b`](https://github.com/cowofevil/flask-ligand/commit/e66965b52a226369b1e816e279b40ef4af1bc574))
+
 ## v0.7.4 (2023-04-24)
 ### Fix
 * :arrow_up: Update mypy requirement from ~=1.0 to ~=1.2 ([`a9f8d63`](https://github.com/cowofevil/flask-ligand/commit/a9f8d6324f162e8fddbae05fb2ada70448f899b7))
 
 ## v0.7.3 (2023-04-24)
 ### Fix
 * :arrow_up: Update python-semantic-release requirement ([`65190bc`](https://github.com/cowofevil/flask-ligand/commit/65190bc8295f4442e7ecd7ab4291d9fffcfede4f))
```

### Comparing `flask-ligand-0.7.4/CONTRIBUTING.rst` & `flask-ligand-0.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/LICENSE` & `flask-ligand-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/Makefile` & `flask-ligand-0.7.5/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/PKG-INFO` & `flask-ligand-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand
-Version: 0.7.4
+Version: 0.7.5
 Summary: A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand/issues
```

### Comparing `flask-ligand-0.7.4/README.rst` & `flask-ligand-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/app.py` & `flask-ligand-0.7.5/app.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docker/env_files/integration.env` & `flask-ligand-0.7.5/docker/env_files/integration.env`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docker/kc-data/flask-ligand-realm.json` & `flask-ligand-0.7.5/docker/kc-data/flask-ligand-realm.json`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docker/postgres-data/create-multiple-postgresql-databases.sh` & `flask-ligand-0.7.5/docker/postgres-data/create-multiple-postgresql-databases.sh`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docker-compose.yml` & `flask-ligand-0.7.5/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/Makefile` & `flask-ligand-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/_static/small_logo.jpg` & `flask-ligand-0.7.5/docs/_static/small_logo.jpg`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/api_reference.rst` & `flask-ligand-0.7.5/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/auth0.rst` & `flask-ligand-0.7.5/docs/auth0.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/conf.py` & `flask-ligand-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/database_configuration.rst` & `flask-ligand-0.7.5/docs/database_configuration.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/developer_guide.rst` & `flask-ligand-0.7.5/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/flask_environments.rst` & `flask-ligand-0.7.5/docs/flask_environments.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/index.rst` & `flask-ligand-0.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/integration_testing.rst` & `flask-ligand-0.7.5/docs/integration_testing.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/make.bat` & `flask-ligand-0.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/oidc_configuration.rst` & `flask-ligand-0.7.5/docs/oidc_configuration.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/openapi.rst` & `flask-ligand-0.7.5/docs/openapi.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/quickstart.rst` & `flask-ligand-0.7.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/docs/release_process.rst` & `flask-ligand-0.7.5/docs/release_process.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/__init__.py` & `flask-ligand-0.7.5/flask_ligand/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from typing import Any, Tuple
     from flask_ligand.extensions.api import Api
 
 
 # ======================================================================================================================
 # Globals
 # ======================================================================================================================
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 
 # ======================================================================================================================
 # Functions: Public
 # ======================================================================================================================
 def create_app(
     flask_app_name: str,
```

### Comparing `flask-ligand-0.7.4/flask_ligand/cli.py` & `flask-ligand-0.7.5/flask_ligand/cli.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/controllers.py` & `flask-ligand-0.7.5/flask_ligand/controllers.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/default_settings.py` & `flask-ligand-0.7.5/flask_ligand/default_settings.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/extensions/__init__.py` & `flask-ligand-0.7.5/flask_ligand/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/extensions/api.py` & `flask-ligand-0.7.5/flask_ligand/extensions/api.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/extensions/database.py` & `flask-ligand-0.7.5/flask_ligand/extensions/database.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/extensions/jwt.py` & `flask-ligand-0.7.5/flask_ligand/extensions/jwt.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/schemas.py` & `flask-ligand-0.7.5/flask_ligand/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/views/__init__.py` & `flask-ligand-0.7.5/flask_ligand/views/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/views/common/openapi_doc.py` & `flask-ligand-0.7.5/flask_ligand/views/common/openapi_doc.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand/views/openapi.py` & `flask-ligand-0.7.5/flask_ligand/views/openapi.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/flask_ligand.egg-info/PKG-INFO` & `flask-ligand-0.7.5/flask_ligand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand
-Version: 0.7.4
+Version: 0.7.5
 Summary: A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand/issues
```

### Comparing `flask-ligand-0.7.4/flask_ligand.egg-info/SOURCES.txt` & `flask-ligand-0.7.5/flask_ligand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/pyproject.toml` & `flask-ligand-0.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/requirements-dev.txt` & `flask-ligand-0.7.5/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/setup.cfg` & `flask-ligand-0.7.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flask-ligand
-version = 0.7.4
+version = 0.7.5
 summary = A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 description_file = README.rst
 description_content_type = text/x-rst; charset=UTF-8
 author = Ryan Gard
 author_email = ryan@gardiancapitol.com
 keywords = flask
 license = GNU Affero General Public License v3
```

### Comparing `flask-ligand-0.7.4/setup.py` & `flask-ligand-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/integration/conftest.py` & `flask-ligand-0.7.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/integration/migrations/alembic.ini` & `flask-ligand-0.7.5/tests/integration/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/integration/migrations/env.py` & `flask-ligand-0.7.5/tests/integration/migrations/env.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/integration/migrations/versions/47f10265b5d7_.py` & `flask-ligand-0.7.5/tests/integration/migrations/versions/47f10265b5d7_.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/integration/test_basic.py` & `flask-ligand-0.7.5/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/unit/conftest.py` & `flask-ligand-0.7.5/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/unit/test_api_extension.py` & `flask-ligand-0.7.5/tests/unit/test_api_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/unit/test_database_extension.py` & `flask-ligand-0.7.5/tests/unit/test_database_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/unit/test_jwt_extension.py` & `flask-ligand-0.7.5/tests/unit/test_jwt_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/unit/test_openapi_api.py` & `flask-ligand-0.7.5/tests/unit/test_openapi_api.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.4/tests/unit/test_settings.py` & `flask-ligand-0.7.5/tests/unit/test_settings.py`

 * *Files identical despite different names*

