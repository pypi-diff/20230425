# Comparing `tmp/feed-archiver-2.0.0b1.tar.gz` & `tmp/feed-archiver-2.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.0b1.tar", last modified: Sun Apr 16 17:35:48 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.1b0.tar", last modified: Mon Apr 24 21:06:18 2023, max compression
```

## Comparing `feed-archiver-2.0.0b1.tar` & `feed-archiver-2.0.1b0.tar`

### file list

```diff
@@ -1,250 +1,253 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4472 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      779 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2482 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2747 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/LICENSE
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    61244 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      180 2023-04-16 17:24:44.000000 feed-archiver-2.0.0b1/NEWS-VERSION.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3567 2023-04-16 17:24:46.000000 feed-archiver-2.0.0b1/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    21849 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2792 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py310.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py311.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py37.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py38.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5687 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      927 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/gitlab-runner/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/gitlab-runner/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-16 17:24:46.000000 feed-archiver-2.0.0b1/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      578 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py310/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6384 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py310/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py311/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6135 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py311/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2645 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py37/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7097 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py37/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2515 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py38/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6424 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py38/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2412 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py39/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6411 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py39/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2136 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7309 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      360 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3362 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1613 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1613 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4347 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/LICENSE
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60299 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       82 2023-04-24 06:43:54.000000 feed-archiver-2.0.1b0/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3743 2023-04-24 06:43:56.000000 feed-archiver-2.0.1b0/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25645 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    24557 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6108 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/gitlab-runner/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/gitlab-runner/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-24 06:43:56.000000 feed-archiver-2.0.1b0/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/requirements/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/requirements/py310/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6246 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/requirements/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/requirements/py311/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6020 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/requirements/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/requirements/py37/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6936 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/requirements/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/requirements/py38/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6286 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/requirements/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/requirements/py39/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6273 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-24 06:43:57.000000 feed-archiver-2.0.1b0/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25645 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7383 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.706425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-24 21:06:18.000000 feed-archiver-2.0.1b0/src/feedarchiver/version.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.702425 feed-archiver-2.0.1b0/src/pythonprojectstructure/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-24 21:06:18.710425 feed-archiver-2.0.1b0/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       87 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/src/pythonprojectstructure/newsfragments/+upgrade-requirements.bugfix.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.1b0/tox.ini
```

### Comparing `feed-archiver-2.0.0b1/.dir-locals.el.in` & `feed-archiver-2.0.1b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/.dockerignore` & `feed-archiver-2.0.1b0/.dockerignore`

 * *Files 8% similar despite different names*

```diff
@@ -50,22 +50,19 @@
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
 .coverage
 .coverage.*
-coverage.*
 .cache
 **/.cache
 nosetests.xml
-pytest-junit.xml
 *,cover
 **/,cover
-pylint.*
 .hypothesis/
 .mypy_cache
 **/.mypy_cache
 
 # Translations
 *.mo
 **/.mo
@@ -112,15 +109,14 @@
 # Rope project settings
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific build artifacts
-/README.md
 # Local, development `$ docker compose ...` end-to-end stack
 /src/feedarchiver/tests/archives/end-to-end/*
 !/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
 /sonarr
 /server/.htpasswd
 
 # Explicit ignores for the Docker build context.
```

### Comparing `feed-archiver-2.0.0b1/.env.in` & `feed-archiver-2.0.1b0/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/.github/workflows/build-test.yml` & `feed-archiver-2.0.1b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/.gitignore` & `feed-archiver-2.0.1b0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -50,22 +50,19 @@
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
 .coverage
 .coverage.*
-coverage.*
 .cache
 **/.cache
 nosetests.xml
-pytest-junit.xml
 *,cover
 **/,cover
-pylint.*
 .hypothesis/
 .mypy_cache
 **/.mypy_cache
 
 # Translations
 *.mo
 **/.mo
@@ -112,15 +109,14 @@
 # Rope project settings
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific build artifacts
-/README.md
 # Local, development `$ docker compose ...` end-to-end stack
 /src/feedarchiver/tests/archives/end-to-end/*
 !/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
 /sonarr
 /server/.htpasswd
 
 # Explicit ignores for the Docker build context.
```

### Comparing `feed-archiver-2.0.0b1/.gitlab-ci.yml` & `feed-archiver-2.0.1b0/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,14 @@
     - "chown -R $PUID:$PGID ./"
   # TODO: Debug stale venv issues and restore cache once fixed
 
 variables:
   # Variables controlling behavior:
   PUID: "1001"
   PGID: "1001"
-  DOCKER_IMAGE: "$CI_REGISTRY_IMAGE"
-  # Different variable name needed by the GitHub CLI:
-  GH_TOKEN: "$PROJECT_GITHUB_PAT"
   # Uncomment to get more debugging output:
   # DEBUG: "true"
 
 stages:
   - "build-test"
   - "release"
   - "release-bump"
```

### Comparing `feed-archiver-2.0.0b1/.pre-commit-config.yaml` & `feed-archiver-2.0.1b0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Run all test, linters and other code checks before committing and pushing.
 fail_fast: true
 repos:
 # Check commit message format and style before pushing to a remote
   - repo: "https://github.com/commitizen-tools/commitizen"
-    rev: "v2.42.1"
+    rev: "3.0.1"
     hooks:
       - id: "commitizen"
 # Checks defined in the `./Makefile`
   - repo: "local"
     hooks:
 # Fail fast, run quicker checks first
     - id: "test-push"
```

### Comparing `feed-archiver-2.0.0b1/.prospector.yaml` & `feed-archiver-2.0.1b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/CONTRIBUTING.rst` & `feed-archiver-2.0.1b0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ########################################################################################
-CONTRIBUTING
+Contributing
 ########################################################################################
 
 Development requires fairly standard development tools, but ``git`` and ``make`` to
 bootstrap the local development environment.  Once installed, clone the repository::
 
   $ git clone "https://gitlab.com/rpatterson/feed-archiver"
```

### Comparing `feed-archiver-2.0.0b1/Dockerfile` & `feed-archiver-2.0.1b0/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 ## Container image for use by end users
 
 # Stay as close to a vanilla Python environment as possible
 ARG PYTHON_MINOR=3.10
 FROM python:${PYTHON_MINOR}
 
-ARG PYTHON_ENV=py310
-ARG VERSION=
-ARG PYTHON_WHEEL
-
 RUN \
     rm -f /etc/apt/apt.conf.d/docker-clean && \
     echo 'Binary::apt::APT::Keep-Downloaded-Packages "true";' \
     >"/etc/apt/apt.conf.d/keep-cache"
 RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
     --mount=type=cache,target=/var/lib/apt,sharing=locked \
     apt-get update && \
     apt-get install --no-install-recommends -y gosu=1.12-1+b6
 # Put the `ENTRYPOINT` on the `$PATH`
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 
 WORKDIR "/usr/local/src/feed-archiver/"
 # Install dependencies with fixed versions in a separate layer to optimize build times
 # because this step takes the most time and changes the least frequently.
+ARG PYTHON_ENV=py310
 COPY [ "./requirements/${PYTHON_ENV}/user.txt", "./requirements/${PYTHON_ENV}/" ]
 # hadolint ignore=DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
     pip install -r "./requirements/${PYTHON_ENV}/user.txt"
 # Install this package in the most common/standard Python way while still being able to
 # build the image locally.
+ARG PYTHON_WHEEL
 COPY [ "${PYTHON_WHEEL}", "${PYTHON_WHEEL}" ]
 # hadolint ignore=DL3013,DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
     pip install "${PYTHON_WHEEL}" && \
     rm -rfv "./dist/"
 
 # Find the same home directory even when run as another user, e.g. `root`.
@@ -47,8 +45,9 @@
 LABEL org.opencontainers.image.title="Feed Archiver"
 LABEL org.opencontainers.image.description="Archive the full contents of RSS/Atom syndication feeds including enclosures and assets."
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
 LABEL org.opencontainers.image.base.name="docker.io/library/python:${PYTHON_MINOR}"
 # Build-time `LABEL`s
+ARG VERSION=
 LABEL org.opencontainers.image.version=${VERSION}
```

### Comparing `feed-archiver-2.0.0b1/Dockerfile.devel` & `feed-archiver-2.0.1b0/Dockerfile.devel`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 ## Container image for use by developers
 
 # Stay as close to the end user image as possible for build cache efficiency.
 # Then add everything that might contribute to efficient development
 ARG PYTHON_MINOR=3.10
 FROM python:${PYTHON_MINOR}
 
-ARG PYTHON_ENV=py310
-ENV PYTHON_ENV="${PYTHON_ENV}"
-ARG VERSION=
-
 RUN \
     rm -f /etc/apt/apt.conf.d/docker-clean && \
     echo 'Binary::apt::APT::Keep-Downloaded-Packages "true";' \
     >"/etc/apt/apt.conf.d/keep-cache"
 RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
     --mount=type=cache,target=/var/lib/apt,sharing=locked \
     apt-get update && \
     apt-get install --no-install-recommends -y gosu=1.12-1+b6
 # Put the `ENTRYPOINT` on the `$PATH`
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 
 WORKDIR "/usr/local/src/feed-archiver/"
+# Install dependencies with fixed versions in a separate layer to optimize build times
+# because this step takes the most time and changes the least frequently.
+ARG PYTHON_ENV=py310
+COPY [ "./requirements/${PYTHON_ENV}/user.txt", "./requirements/${PYTHON_ENV}/" ]
+# hadolint ignore=DL3042
+RUN --mount=type=cache,target=/root/.cache,sharing=locked \
+    pip install -r "./requirements/${PYTHON_ENV}/user.txt"
+# End of layers shared with the end-user `./Dockerfile` image.
+
 # Match local development tool chain and avoid time consuming redundant package
 # installs.  Initialize the `$ tox -e py3##` Python virtual environment to install this
 # package and all the development tools into the image.
+ARG PYTHON_ENV=py310
 COPY [ "./build-host/requirements-${PYTHON_ENV}.txt", "./build-host/" ]
 # hadolint ignore=DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
     pip install -r "./build-host/requirements-${PYTHON_ENV}.txt"
 COPY [ "./requirements/${PYTHON_ENV}/devel.txt", "./requirements/${PYTHON_ENV}/" ]
 COPY [ "./tox.ini", "./" ]
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
@@ -35,14 +41,15 @@
 # Activate the Python virtual environment
 ENV VIRTUAL_ENV="/usr/local/src/feed-archiver/.tox/${PYTHON_ENV}"
 ENV PATH="${VIRTUAL_ENV}/bin:${PATH}"
 
 # Remain in the checkout `WORKDIR` and make the primary testing tool for the default
 # command to run.
 ENV HOME="/home/feed-archiver"
+ENV PYTHON_ENV="${PYTHON_ENV}"
 ENTRYPOINT [ "entrypoint" ]
 # Have to use the shell form of `CMD` because we need variable substitution:
 # hadolint ignore=DL3025
 CMD tox -e "${PYTHON_ENV}"
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
 LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/feed-archiver"
@@ -51,8 +58,9 @@
 LABEL org.opencontainers.image.title="Feed Archiver Development"
 LABEL org.opencontainers.image.description="Feed Archiver development image"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
 LABEL org.opencontainers.image.base.name="docker.io/library/python:${PYTHON_MINOR}"
 # Build-time `LABEL`s
+ARG VERSION=
 LABEL org.opencontainers.image.version=${VERSION}
```

### Comparing `feed-archiver-2.0.0b1/LICENSE` & `feed-archiver-2.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/Makefile` & `feed-archiver-2.0.1b0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 export TZ
 export DOCKER_GID=$(shell getent group "docker" | cut -d ":" -f 3)
 
 # Values concerning supported Python versions:
 # Use the same Python version tox would as a default.
 # https://tox.wiki/en/latest/config.html#base_python
 PYTHON_HOST_MINOR:=$(shell \
-    pip --version | sed -nE 's|.* \(python ([0-9]+.[0-9]+)\)$$|\1|p')
+    pip --version | sed -nE 's|.* \(python ([0-9]+.[0-9]+)\)$$|\1|p;q')
 export PYTHON_HOST_ENV=py$(subst .,,$(PYTHON_HOST_MINOR))
 # Determine the latest installed Python version of the supported versions
 PYTHON_BASENAMES=$(PYTHON_SUPPORTED_MINORS:%=python%)
 PYTHON_AVAIL_EXECS:=$(foreach \
     PYTHON_BASENAME,$(PYTHON_BASENAMES),$(shell which $(PYTHON_BASENAME)))
 PYTHON_LATEST_EXEC=$(firstword $(PYTHON_AVAIL_EXECS))
 PYTHON_LATEST_BASENAME=$(notdir $(PYTHON_LATEST_EXEC))
@@ -215,56 +215,62 @@
 export TOX_RUN_ARGS
 # The options that allow for rapid execution of arbitrary commands in the venvs managed
 # by tox
 TOX_EXEC_OPTS=--no-recreate-pkg --skip-pkg-install
 TOX_EXEC_ARGS=tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" --
 TOX_EXEC_BUILD_ARGS=tox exec $(TOX_EXEC_OPTS) -e "build" --
 
-# Values used to build Docker images and run containers:
+# Values used to build Docker images:
+DOCKER_FILE=./Dockerfile
+export DOCKER_BUILD_ARGS=
+export DOCKER_BUILD_PULL=false
+# Values used to tag built images:
+export DOCKER_VARIANT=
+DOCKER_VARIANT_PREFIX=
+ifneq ($(DOCKER_VARIANT),)
+DOCKER_VARIANT_PREFIX=$(DOCKER_VARIANT)-
+endif
+export DOCKER_BRANCH_TAG=$(subst /,-,$(VCS_BRANCH))
 GITLAB_CI=false
 GITHUB_ACTIONS=false
 CI_PROJECT_NAMESPACE=$(CI_UPSTREAM_NAMESPACE)
 CI_TEMPLATE_REGISTRY_HOST=registry.gitlab.com
+ifeq ($(GITHUB_ACTIONS),true)
+DOCKER_REGISTRY_HOST=ghcr.io
+else
+DOCKER_REGISTRY_HOST=$(CI_TEMPLATE_REGISTRY_HOST)
+endif
+export DOCKER_REGISTRY_HOST
 CI_REGISTRY=$(CI_TEMPLATE_REGISTRY_HOST)/$(CI_PROJECT_NAMESPACE)
 CI_REGISTRY_IMAGE=$(CI_REGISTRY)/$(CI_PROJECT_NAME)
-DOCKER_COMPOSE_RUN_ARGS=
-DOCKER_COMPOSE_RUN_ARGS+= --rm
-ifneq ($(CI),true)
-DOCKER_COMPOSE_RUN_ARGS+= --quiet-pull
-endif
-ifeq ($(shell tty),not a tty)
-DOCKER_COMPOSE_RUN_ARGS+= -T
-endif
-DOCKER_BUILD_ARGS=
 DOCKER_REGISTRIES=DOCKER GITLAB GITHUB
 export DOCKER_REGISTRY=$(firstword $(DOCKER_REGISTRIES))
 DOCKER_IMAGE_DOCKER=$(DOCKER_USER)/$(CI_PROJECT_NAME)
 DOCKER_IMAGE_GITLAB=$(CI_REGISTRY_IMAGE)
 DOCKER_IMAGE_GITHUB=ghcr.io/$(CI_PROJECT_NAMESPACE)/$(CI_PROJECT_NAME)
 DOCKER_IMAGE=$(DOCKER_IMAGE_$(DOCKER_REGISTRY))
 DOCKER_IMAGES=
 ifeq ($(GITLAB_CI),true)
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITLAB)
 else ifeq ($(GITHUB_ACTIONS),true)
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITHUB)
 else
 DOCKER_IMAGES+=$(DOCKER_IMAGE_DOCKER)
 endif
-export DOCKER_VARIANT=
-DOCKER_VARIANT_PREFIX=
-ifneq ($(DOCKER_VARIANT),)
-DOCKER_VARIANT_PREFIX=$(DOCKER_VARIANT)-
-endif
-export DOCKER_BRANCH_TAG=$(subst /,-,$(VCS_BRANCH))
+# Values used to run built images in containers:
 DOCKER_VOLUMES=\
 ./var/docker/$(PYTHON_ENV)/ \
 ./src/feed_archiver.egg-info/ \
 ./var/docker/$(PYTHON_ENV)/feed_archiver.egg-info/ \
 ./.tox/ ./var/docker/$(PYTHON_ENV)/.tox/
-export DOCKER_BUILD_PULL=false
+DOCKER_COMPOSE_RUN_ARGS=
+DOCKER_COMPOSE_RUN_ARGS+= --rm
+ifeq ($(shell tty),not a tty)
+DOCKER_COMPOSE_RUN_ARGS+= -T
+endif
 
 # Values derived from or overridden by CI environments:
 GITHUB_REPOSITORY_OWNER=$(CI_UPSTREAM_NAMESPACE)
 # Determine if this checkout is a fork of the upstream project:
 CI_IS_FORK=false
 ifeq ($(GITLAB_CI),true)
 USER_EMAIL=$(USER_NAME)@runners-manager.gitlab.com
@@ -272,15 +278,15 @@
 ifneq ($(VCS_BRANCH),main)
 DOCKER_REGISTRIES=GITLAB
 endif
 endif
 ifneq ($(CI_PROJECT_NAMESPACE),$(CI_UPSTREAM_NAMESPACE))
 CI_IS_FORK=true
 DOCKER_REGISTRIES=GITLAB
-DOCKER_IMAGES+=$(CI_TEMPLATE_REGISTRY_HOST)/$(CI_UPSTREAM_NAMESPACE)/$(CI_PROJECT_NAME)
+DOCKER_IMAGES+=$(DOCKER_REGISTRY_HOST)/$(CI_UPSTREAM_NAMESPACE)/$(CI_PROJECT_NAME)
 endif
 else ifeq ($(GITHUB_ACTIONS),true)
 USER_EMAIL=$(USER_NAME)@actions.github.com
 ifneq ($(VCS_BRANCH),develop)
 ifneq ($(VCS_BRANCH),main)
 DOCKER_REGISTRIES=GITHUB
 endif
@@ -321,25 +327,29 @@
 endif
 GITHUB_RELEASE_ARGS=--prerelease
 # Only publish releases from the `main` or `develop` branches and only under the
 # canonical CI/CD platform:
 ifeq ($(GITLAB_CI),true)
 ifeq ($(VCS_BRANCH),main)
 RELEASE_PUBLISH=true
-PYPI_REPO=pypi
-PYPI_HOSTNAME=pypi.org
 GITHUB_RELEASE_ARGS=
 else ifeq ($(VCS_BRANCH),develop)
 # Publish pre-releases from the `develop` branch:
 RELEASE_PUBLISH=true
+endif
+ifeq ($(RELEASE_PUBLISH),true)
 PYPI_REPO=pypi
+PYPI_HOSTNAME=pypi.org
+ifeq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
+# Only build and publish multi-platform images for the canonical Python version:
+DOCKER_PLATFORMS=linux/amd64 linux/arm64 linux/arm/v7
+endif
 endif
 endif
 CI_REGISTRY_USER=$(CI_PROJECT_NAMESPACE)
-CI_REGISTRY_IMAGE=$(CI_REGISTRY)/$(CI_PROJECT_NAME)
 # Address undefined variables warnings when running under local development
 PYPI_PASSWORD=
 export PYPI_PASSWORD
 TEST_PYPI_PASSWORD=
 export TEST_PYPI_PASSWORD
 VCS_REMOTE_PUSH_URL=
 CODECOV_TOKEN=
@@ -454,15 +464,15 @@
 # development container.  Top level targets, like `test`, should run as much as possible
 # inside the development container.
 
 .PHONY: build-docker
 ### Set up for development in Docker containers.
 build-docker: build-pkgs ./var/log/tox/build/build.log
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
-	    DOCKER_BUILD_ARGS="--progress plain" \
+	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    $(PYTHON_MINORS:%=build-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-%)
 ### Set up for development in a Docker container for one Python version.
 $(PYTHON_MINORS:%=build-docker-%):
 	$(MAKE) -e \
 	    PYTHON_MINORS="$(@:build-docker-%=%)" \
@@ -485,32 +495,77 @@
 ifeq ($(VCS_BRANCH),main)
 # Only update tags end users may depend on to be stable from the `main` branch
 	VERSION=$$(./.tox/build/bin/cz version --project)
 	major_version=$$(echo $${VERSION} | sed -nE 's|([0-9]+).*|\1|p')
 	minor_version=$$(
 	    echo $${VERSION} | sed -nE 's|([0-9]+\.[0-9]+).*|\1|p'
 	)
-	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${minor_version}
-	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${major_version}
+	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-v$${minor_version}
+	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-v$${major_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)
 endif
 # This variant is the default used for tags such as `latest`
 ifeq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(DOCKER_BRANCH_TAG)
 ifeq ($(VCS_BRANCH),main)
-	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$${minor_version}
-	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$${major_version}
+	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)v$${minor_version}
+	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)v$${major_version}
 ifeq ($(DOCKER_VARIANT),)
 	echo $${docker_image}:latest
 else
 	echo $${docker_image}:$(DOCKER_VARIANT)
 endif
 endif
 endif
 
+.PHONY: build-docker-build
+### Run the actual commands used to build the Docker container image.
+build-docker-build: $(HOME)/.local/var/log/docker-multi-platform-host-install.log \
+		./var/log/tox/build/build.log \
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
+		./var/log/docker-login-DOCKER.log
+# Workaround broken interactive session detection:
+	docker pull "python:$(PYTHON_MINOR)"
+	docker_build_caches=""
+ifeq ($(GITLAB_CI),true)
+# Don't cache when building final releases on `main`
+	$(MAKE) -e "./var/log/docker-login-GITLAB.log" || true
+ifneq ($(VCS_BRANCH),main)
+	if $(MAKE) -e pull-docker
+	then
+	    docker_build_caches+=" --cache-from $(DOCKER_IMAGE_GITLAB):\
+	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
+	fi
+endif
+endif
+ifeq ($(GITHUB_ACTIONS),true)
+	$(MAKE) -e "./var/log/docker-login-GITHUB.log" || true
+ifneq ($(VCS_BRANCH),main)
+	if $(MAKE) -e pull-docker
+	then
+	    docker_build_caches+=" --cache-from $(DOCKER_IMAGE_GITHUB):\
+	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
+	fi
+endif
+endif
+	docker_image_tags=""
+	for image_tag in $$(
+	    $(MAKE) -e --no-print-directory build-docker-tags
+	)
+	do
+	    docker_image_tags+="--tag $${image_tag} "
+	done
+# https://github.com/moby/moby/issues/39003#issuecomment-879441675
+	docker buildx build $(DOCKER_BUILD_ARGS) \
+	    --build-arg BUILDKIT_INLINE_CACHE="1" \
+	    --build-arg PYTHON_MINOR="$(PYTHON_MINOR)" \
+	    --build-arg PYTHON_ENV="$(PYTHON_ENV)" \
+	    --build-arg VERSION="$$(./.tox/build/bin/cz version --project)" \
+	    $${docker_image_tags} $${docker_build_caches} --file "$(DOCKER_FILE)" "./"
+
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
 $(PYTHON_MINORS:%=build-docker-requirements-%): ./.env
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
 	$(MAKE) -e build-docker-volumes-$${PYTHON_ENV} \
 	    "./var/docker/$${PYTHON_ENV}/log/build-devel.log"
@@ -548,15 +603,15 @@
 test-debug: ./var/log/tox/$(PYTHON_ENV)/editable.log
 	$(TOX_EXEC_ARGS) pytest --pdb
 
 .PHONY: test-docker
 ### Run the full suite of tests, coverage checks, and code linters in containers.
 test-docker: build-pkgs ./var/log/tox/build/build.log ./var/log/codecov-install.log
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
-	    DOCKER_BUILD_ARGS="--progress plain" \
+	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=test-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=test-docker-%)
 ### Run the full suite of tests inside a docker container for one Python version.
 $(PYTHON_MINORS:%=test-docker-%):
 	$(MAKE) -e \
@@ -598,15 +653,15 @@
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
 test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV) \
 		./var/log/docker-login-DOCKER.log
-	docker compose pull hadolint
+	docker compose pull --quiet hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./Dockerfile.devel"
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
@@ -628,18 +683,20 @@
 	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
 	if ! git fetch "$(VCS_COMPARE_REMOTE)" "$(VCS_COMPARE_BRANCH)"
 	then
 # Compare with the pre-release branch if this branch hasn't been pushed yet:
 	    vcs_compare_rev="$(VCS_COMPARE_REMOTE)/develop"
 	fi
 endif
-	$(TOX_EXEC_BUILD_ARGS) cz check --rev-range "$${vcs_compare_rev}..HEAD"
 	exit_code=0
-	$(TOX_EXEC_BUILD_ARGS) python ./bin/cz-check-bump --compare-ref \
-	    "$${vcs_compare_rev}" || exit_code=$$?
+	(
+	    $(TOX_EXEC_BUILD_ARGS) cz check --rev-range "$${vcs_compare_rev}..HEAD" &&
+	    $(TOX_EXEC_BUILD_ARGS) python ./bin/cz-check-bump --compare-ref \
+	        "$${vcs_compare_rev}"
+	) || exit_code=$$?
 	if (( $$exit_code == 3 || $$exit_code == 21 ))
 	then
 	    exit
 	elif (( $$exit_code != 0 ))
 	then
 	    exit $$exit_code
 	else
@@ -722,47 +779,44 @@
 ### Publish all container images to all container registries.
 release-docker: build-docker-volumes-$(PYTHON_ENV) build-docker \
 		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	$(MAKE) -e -j DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=release-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
-### Publish the container images for one Python version to all container registry.
-$(PYTHON_MINORS:%=release-docker-%): $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
+### Publish the container images for one Python version to all container registries.
+$(PYTHON_MINORS:%=release-docker-%): \
+		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log) \
+		$(HOME)/.local/var/log/docker-multi-platform-host-install.log
 	export PYTHON_ENV="py$(subst .,,$(@:release-docker-%=%))"
-	$(MAKE) -e -j DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
-	    $(DOCKER_REGISTRIES:%=release-docker-registry-%)
-ifeq ($(VCS_BRANCH),main)
-ifeq ($${PYTHON_ENV},$(PYTHON_HOST_ENV))
-	$(MAKE) -e "./var/log/docker-login-DOCKER.log"
-	docker compose pull pandoc docker-pushrm
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
+# Build other platforms in emulation and rely on the layer cache for bundling the
+# previously built native images into the manifests.
+	DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --push"
+ifneq ($(DOCKER_PLATFORMS),)
+	DOCKER_BUILD_ARGS+=" --platform $(subst $(EMPTY) ,$(COMMA),$(DOCKER_PLATFORMS))"
+else
 endif
+	export DOCKER_BUILD_ARGS
+# Push the development manifest and images:
+	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
+	    build-docker-build
+# Push the end-user manifest and images:
+	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
+	$(MAKE) -e DOCKER_BUILD_ARGS="$${DOCKER_BUILD_ARGS}\
+	    --build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build
+# Update Docker Hub `README.md` from the official/canonical Python version:
+ifeq ($(VCS_BRANCH),main)
+	if [ "$${PYTHON_ENV}" == "$(PYTHON_HOST_ENV)" ]
+	then
+	    $(MAKE) -e "./var/log/docker-login-DOCKER.log"
+	    docker compose pull --quiet pandoc docker-pushrm
+	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
+	fi
 endif
 
-.PHONY: $(DOCKER_REGISTRIES:%=release-docker-registry-%)
-### Publish all container images to one container registry.
-$(DOCKER_REGISTRIES:%=release-docker-registry-%):
-# https://docs.docker.com/docker-hub/#step-5-build-and-push-a-container-image-to-docker-hub-from-your-computer
-	$(MAKE) -e "./var/log/docker-login-$(@:release-docker-registry-%=%).log"
-	for user_tag in $$(
-	    $(MAKE) -e --no-print-directory \
-	        build-docker-tags-$(@:release-docker-registry-%=%)
-	)
-	do
-	    docker push "$${user_tag}"
-	done
-	for devel_tag in $$(
-	    $(MAKE) -e DOCKER_VARIANT="devel" --no-print-directory \
-	        build-docker-tags-$(@:release-docker-registry-%=%)
-	)
-	do
-	    docker push "$${devel_tag}"
-	done
-
 .PHONY: release-bump
 ### Bump the package version if on a branch that should trigger a release.
 release-bump: ~/.gitconfig $(VCS_RELEASE_FETCH_TARGETS) \
 		./var/log/git-remotes.log ./var/log/tox/build/build.log \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
 		./.env build-docker-volumes-$(PYTHON_ENV)
 	if ! git diff --cached --exit-code
@@ -805,15 +859,15 @@
 	$(MAKE) -e ./var/log/gpg-import.log
 endif
 # Capture the release notes for *just this* release for creating the GitHub release.
 # Have to run before the real `$ towncrier build` run without the `--draft` option
 # because after that the `newsfragments` will have been deleted.
 	next_version=$$(
 	    $(TOX_EXEC_BUILD_ARGS) cz bump $${cz_bump_args} --yes --dry-run |
-	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p'
+	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p;q'
 	) || true
 # Build and stage the release notes to be commited by `$ cz bump`
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
 	    tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" -qq -- \
 	    towncrier build --version "$${next_version}" --draft --yes \
 	    >"./NEWS-VERSION.rst"
 	git add -- "./NEWS-VERSION.rst"
@@ -823,19 +877,16 @@
 	$(TOX_EXEC_BUILD_ARGS) cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
 	    $(PYTHON_ENVS:%=./requirements/%/devel.txt) \
 	    $(PYTHON_ENVS:%=./build-host/requirements-%.txt)
-ifneq ($(CI),true)
-# If running under CI/CD then the image will be updated in the next pipeline stage.
-# For testing locally, however, ensure the image is up-to-date for subsequent recipes.
+# Ensure the image is up-to-date for subsequent recipes.
 	$(MAKE) -e "./var/docker/$(PYTHON_ENV)/log/build-user.log"
-endif
 ifeq ($(VCS_BRANCH),main)
 # Merge the bumped version back into `develop`:
 	bump_rev="$$(git rev-parse HEAD)"
 	git switch -C "develop" --track "$(VCS_COMPARE_REMOTE)/develop" --
 	git merge --ff --gpg-sign \
 	    -m "Merge branch 'main' release back into develop" "$${bump_rev}"
 ifeq ($(CI),true)
@@ -1011,108 +1062,51 @@
 # created and can be used directly to save time on Tox's overhead when we don't need
 # Tox's logic about when to update/recreate them, e.g.:
 #     $ ./.tox/build/bin/cz --help
 # Mostly useful for build/release tools.
 $(PYTHON_ALL_ENVS:%=./var/log/tox/%/build.log):
 	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
 	mkdir -pv "$(dir $(@))"
-	tox run $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/build.log=%)" --notest |
+	tox run $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/build.log=%)" --notest |&
 	    tee -a "$(@)"
 # Workaround tox's `usedevelop = true` not working with `./pyproject.toml`.  Use as a
 # prerequisite when using Tox-managed virtual environments directly and changes to code
 # need to take effect immediately.
 $(PYTHON_ENVS:%=./var/log/tox/%/editable.log):
 	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
 	mkdir -pv "$(dir $(@))"
 	tox exec $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/editable.log=%)" -- \
-	    pip install -e "./" | tee -a "$(@)"
+	    pip install -e "./" |& tee -a "$(@)"
 
 ## Docker real targets:
 
 # Build the development image:
 ./var/docker/$(PYTHON_ENV)/log/build-devel.log: \
 		./Dockerfile.devel ./.dockerignore ./bin/entrypoint \
 		./pyproject.toml ./setup.cfg ./tox.ini \
 		./build-host/requirements.txt.in ./docker-compose.yml \
 		./docker-compose.override.yml ./.env \
 		./var/docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)" \
-	    build-docker-volumes-$(PYTHON_ENV) "./var/log/tox/build/build.log" \
-	    "./var/log/docker-login-DOCKER.log"
+	$(MAKE) -e build-docker-volumes-$(PYTHON_ENV)
 	mkdir -pv "$(dir $(@))"
-# Workaround issues with local images and the development image depending on the end
-# user image.  It seems that `depends_on` isn't sufficient.
-	$(MAKE) -e $(HOME)/.local/var/log/feed-archiver-host-install.log
-	export VERSION=$$(./.tox/build/bin/cz version --project)
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    touch "$(@)" "./var/docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
 	        feed-archiver-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
 	        "./var/log/tox/$(PYTHON_ENV)/build.log"
 	    exit
 	fi
 endif
-# https://github.com/moby/moby/issues/39003#issuecomment-879441675
-	docker_build_args="$(DOCKER_BUILD_ARGS) \
-	    --build-arg BUILDKIT_INLINE_CACHE=1 \
-	    --build-arg PYTHON_MINOR=$(PYTHON_MINOR) \
-	    --build-arg PYTHON_ENV=$(PYTHON_ENV) \
-	    --build-arg VERSION=$${VERSION}"
-	docker_build_devel_tags=""
-	for devel_tag in $$(
-	    $(MAKE) -e DOCKER_VARIANT="devel" --no-print-directory build-docker-tags
-	)
-	do
-	    docker_build_devel_tags+="--tag $${devel_tag} "
-	done
-	docker_build_caches=""
-ifeq ($(GITLAB_CI),true)
-# Don't cache when building final releases on `main`
-	$(MAKE) -e "./var/log/docker-login-GITLAB.log" || true
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
-	then
-	    docker_build_caches+=" --cache-from \
-	$(DOCKER_IMAGE_GITLAB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-	$(MAKE) -e "./var/log/docker-login-GITHUB.log" || true
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
-	then
-	    docker_build_caches+=" --cache-from \
-	$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-ifeq ($(CI),true)
-# Workaround broken interactive session detection
-	docker pull "python:${PYTHON_MINOR}"
-endif
-	docker buildx build $${docker_build_args} $${docker_build_devel_tags} \
-	    $${docker_build_caches} --file "./Dockerfile.devel" "./"
-# Ensure any subsequent builds have optimal caches
-ifeq ($(GITLAB_CI),true)
-	docker push \
-	    "$(DOCKER_IMAGE_GITLAB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-ifneq ($(CI_IS_FORK),true)
-	docker push \
-	    "$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-endif
-	date >>"$(@)"
+	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
+	    DOCKER_BUILD_ARGS="--load" build-docker-build >>"$(@)"
 # Update the pinned/frozen versions, if needed, using the container.  If changed, then
 # we may need to re-build the container image again to ensure it's current and correct.
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
 	    make -e PYTHON_MINORS="$(PYTHON_MINOR)" build-requirements-$(PYTHON_ENV)
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
@@ -1122,67 +1116,24 @@
 endif
 
 # Build the end-user image:
 ./var/docker/$(PYTHON_ENV)/log/build-user.log: \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
 		./var/docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)" \
-	    "./var/log/tox/build/build.log"
-	mkdir -pv "$(dir $(@))"
-	export VERSION=$$(./.tox/build/bin/cz version --project)
-# https://github.com/moby/moby/issues/39003#issuecomment-879441675
-	docker_build_args="$(DOCKER_BUILD_ARGS) \
-	    --build-arg BUILDKIT_INLINE_CACHE=1 \
-	    --build-arg PYTHON_MINOR=$(PYTHON_MINOR) \
-	    --build-arg PYTHON_ENV=$(PYTHON_ENV) \
-	    --build-arg VERSION=$${VERSION}"
-# Build the end-user image now that all required artifacts are built"
 ifeq ($(PYTHON_WHEEL),)
 	$(MAKE) -e "build-pkgs"
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 endif
-	docker_build_user_tags=""
-	for user_tag in $$($(MAKE) -e --no-print-directory build-docker-tags)
-	do
-	    docker_build_user_tags+="--tag $${user_tag} "
-	done
-	docker_build_caches=""
-ifeq ($(GITLAB_CI),true)
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e pull-docker
-	then
-	    docker_build_caches+=" \
-	--cache-from $(DOCKER_IMAGE_GITLAB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-ifneq ($(VCS_BRANCH),main)
-	if $(MAKE) -e pull-docker
-	then
-	    docker_build_caches+=" \
-	--cache-from $(DOCKER_IMAGE_GITHUB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-	fi
-endif
-endif
-	docker buildx build $${docker_build_args} $${docker_build_user_tags} \
-	    --build-arg PYTHON_WHEEL="$${PYTHON_WHEEL}" $${docker_build_caches} "./"
-# Ensure any subsequent builds have optimal caches
-ifeq ($(GITLAB_CI),true)
-	docker push "$(DOCKER_IMAGE_GITLAB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-ifeq ($(GITHUB_ACTIONS),true)
-ifneq ($(CI_IS_FORK),true)
-	docker push "$(DOCKER_IMAGE_GITHUB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
-endif
-endif
-	date >>"$(@)"
-# The images install the host requirements, reflect that in the bind mount volumes
-	date >>"$(@:%/build.log=%/host-install.log)"
+# Build the end-user image now that all required artifacts are built"
+	mkdir -pv "$(dir $(@))"
+	$(MAKE) -e DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --load \
+	--build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build >>"$(@)"
+# The image installs the host requirements, reflect that in the bind mount volumes
+	date >>"$(@:%/build-user.log=%/host-install.log)"
 
 ./var/ $(PYTHON_ENVS:%=./var/docker/%/) \
 ./src/feed_archiver.egg-info/ \
 $(PYTHON_ENVS:%=./var/docker/%/feed_archiver.egg-info/) \
 ./.tox/ $(PYTHON_ENVS:%=./var/docker/%/.tox/):
 	mkdir -pv "$(@)"
 
@@ -1253,15 +1204,30 @@
 	    fi
 	    if [ -e ./build-host/requirements-$(PYTHON_HOST_ENV).txt ]
 	    then
 	        pip install -r "./build-host/requirements-$(PYTHON_HOST_ENV).txt"
 	    else
 	        pip install -r "./build-host/requirements.txt.in"
 	    fi
-	) | tee -a "$(@)"
+	) |& tee -a "$(@)"
+
+# https://docs.docker.com/build/building/multi-platform/#building-multi-platform-images
+$(HOME)/.local/var/log/docker-multi-platform-host-install.log:
+	mkdir -pv "$(dir $(@))"
+	if ! docker context inspect "multi-platform" |& tee -a "$(@)"
+	then
+	    docker context create "multi-platform" |& tee -a "$(@)"
+	fi
+	if ! docker buildx inspect |& tee -a "$(@)" |
+	    grep -q '^ *Endpoint: *multi-platform *'
+	then
+	    (
+	        docker buildx create --use "multi-platform" || true
+	    ) |& tee -a "$(@)"
+	fi
 
 ./var/log/codecov-install.log:
 	mkdir -pv "$(dir $(@))"
 # Install the code test coverage publishing tool
 	(
 	    if ! which codecov
 	    then
```

### Comparing `feed-archiver-2.0.0b1/NEWS.rst` & `feed-archiver-2.0.1b0/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+feed-archiver  (2023-04-24)
+===========================
+
+No significant changes.
+
+
+feed-archiver 2.0.0 (2023-04-16)
+================================
+
+No significant changes.
+
+
 feed-archiver 2.0.0b1 (2023-04-16)
 ==================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Sun Apr 16 03:54:21 PM UTC 2023.
```

### Comparing `feed-archiver-2.0.0b1/PKG-INFO` & `feed-archiver-2.0.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.0b1
+Version: 2.0.1b0
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
-Keywords: template,structure
+Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -83,14 +83,27 @@
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
 	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
 	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
+     - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
+          :alt: KeyBase PGP key ID
+          :target: https://keybase.io/rpatterson
+       .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
+          :alt: GitHub followers count
+          :target: https://github.com/rpatterson
+       .. figure:: https://img.shields.io/liberapay/receives/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay donated per week
+          :target: https://liberapay.com/rpatterson/donate
+       .. figure:: https://img.shields.io/liberapay/patrons/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay patrons count
+          :target: https://liberapay.com/rpatterson/donate
+
 The ``$ feed-archiver`` command aims to archive RSS/Atom feeds as fully as possible in
 such a way that the archive can serve (at least) 2 use cases:
 
 #. `Mirror of Feed Enclosures and Assets`_
 
     A mirror of the archived feeds that can be in turn served onto onto feed
     clients/subscribers (such as podcatchers).  For example, you can subscribe to the
@@ -103,14 +116,16 @@
 
 #. `Ingest Feed Enclosures Into Media Libraries`_
 
     An alternate hierarchy of feed item enclosures better suited for ingestion into
     other media software, such as media library servers.  For example, your podcast
     episodes can also be made available in your `Jellyfin`_/Emby/Plex library.
 
+.. contents:: Table of Contents
+
 ********************
 Detailed Description
 ********************
 
 Mirror of Feed Enclosures and Assets
 ====================================
 
@@ -171,22 +186,59 @@
 re-using example configurations known to work by others.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
+Install and use either via a local, native installation or a Docker container image:
+
+Local/Native Installation
+========================================================================================
+
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
-  $ sudo pip3 install feed-archiver
+  $ pip3 install --user feed-archiver
 
 Optional shell tab completion is available via `argcomplete`_.
 
-Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
-details.
+Docker Container Image Installation
+========================================================================================
+
+The recommended way to use the Docker container image is via `Docker Compose`_.  See
+`the example ./docker-compose.yml file`_ for an example configuration.  Once you have
+your configuration, you can create and run the container::
+
+  $ docker compose up
+
+Alternatively, you make use the image directly.  Pull `the Docker image`_::
+
+  $ docker pull "registry.gitlab.org/rpatterson/feed-archiver"
+
+And then use the image to create and run a container::
+
+  $ docker run --rm -it "registry.gitlab.org/rpatterson/feed-archiver" ...
+
+Images variant tags are published for the Python version, branch, and major/minor
+versions so that users can control when they get new images over time,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-main``.  The canonical
+Python version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:main``.  Pre-releases are from
+``develop`` and final releases are from ``main`` which is also the default for tags
+without a branch, e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310``. The
+major/minor version tags are only applied to the final release images and without the
+corresponding ``main`` branch tag,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-v0.8``.
+
+Multi-platform Docker images are published containing images for the following
+platforms or architectures in the Python 3.10 ``py310`` variant:
+
+- ``linux/amd64``
+- ``linux/arm64``
+- ``linux/arm/v7``
 
 
 ****************************************************************************************
 Usage
 ****************************************************************************************
 
 Create a ``./.feed-archiver.yml`` YAML file in a directory to serve as the root
@@ -237,14 +289,20 @@
     -h, --help            show this help message and exit
     --log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
 			  Select logging verbosity. (default: INFO)
     --archive-dir [ARCHIVE_DIR], -a [ARCHIVE_DIR]
 			  the archive root directory into which all feeds, their enclosures and assets
 			  will be downloaded (default: .)
 
+If using the Docker container image, the container can be run from the command-line as
+well::
+
+  $ docker compose run "feed-archiver" feed-archiver --help
+  usage: feed-archiver [-h]
+
 To link feed item enclosures into an `alternate hierarchy`_, such as in a media library,
 add a ``enclosures`` key to the feed configuration whose value is an list/array of
 objects each defining one alternative path to link to the feed item enclosure.  Any
 ``enclosures`` defined in the top-level ``defaults`` key will be used for all feeds.
 Configuration to be shared across multiple ``enclosures`` configurations may be placed
 in the corresponding ``defaults`` / ``plugins`` / ``enclosures`` / ``{plugin_name}``
 object.  The actual linking of enclosures is delegated to `plugins`_.
@@ -406,15 +464,15 @@
 They may also include:
 
 - ``stem-append`` containing a string to append to the episode file stem before the
   enclosure suffix/extension
 
 
 ****************************************************************************************
-CONTRIBUTING
+Contributing
 ****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
@@ -451,14 +509,15 @@
    https://jellyfin.org/docs/general/server/media/external-audio-files.html
 .. _Sonarr: https://sonarr.tv
 .. _connect to the Sonarr API: https://github.com/Sonarr/Sonarr/wiki/API#url
 .. _look up the TV show/series: https://github.com/Sonarr/Sonarr/wiki/Series#getid
 .. _lookup the episode file: https://github.com/Sonarr/Sonarr/wiki/Episode#get
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/feed-archiver
+.. _`Docker Compose`: https://docs.docker.com/compose/
 .. _`the example ./docker-compose.yml file`:
    https://gitlab.com/rpatterson/feed-archiver/blob/main/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
```

### Comparing `feed-archiver-2.0.0b1/README.rst` & `feed-archiver-2.0.1b0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,27 @@
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
 	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
 	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
+     - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
+          :alt: KeyBase PGP key ID
+          :target: https://keybase.io/rpatterson
+       .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
+          :alt: GitHub followers count
+          :target: https://github.com/rpatterson
+       .. figure:: https://img.shields.io/liberapay/receives/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay donated per week
+          :target: https://liberapay.com/rpatterson/donate
+       .. figure:: https://img.shields.io/liberapay/patrons/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay patrons count
+          :target: https://liberapay.com/rpatterson/donate
+
 The ``$ feed-archiver`` command aims to archive RSS/Atom feeds as fully as possible in
 such a way that the archive can serve (at least) 2 use cases:
 
 #. `Mirror of Feed Enclosures and Assets`_
 
     A mirror of the archived feeds that can be in turn served onto onto feed
     clients/subscribers (such as podcatchers).  For example, you can subscribe to the
@@ -75,14 +88,16 @@
 
 #. `Ingest Feed Enclosures Into Media Libraries`_
 
     An alternate hierarchy of feed item enclosures better suited for ingestion into
     other media software, such as media library servers.  For example, your podcast
     episodes can also be made available in your `Jellyfin`_/Emby/Plex library.
 
+.. contents:: Table of Contents
+
 ********************
 Detailed Description
 ********************
 
 Mirror of Feed Enclosures and Assets
 ====================================
 
@@ -143,22 +158,59 @@
 re-using example configurations known to work by others.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
+Install and use either via a local, native installation or a Docker container image:
+
+Local/Native Installation
+========================================================================================
+
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
-  $ sudo pip3 install feed-archiver
+  $ pip3 install --user feed-archiver
 
 Optional shell tab completion is available via `argcomplete`_.
 
-Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
-details.
+Docker Container Image Installation
+========================================================================================
+
+The recommended way to use the Docker container image is via `Docker Compose`_.  See
+`the example ./docker-compose.yml file`_ for an example configuration.  Once you have
+your configuration, you can create and run the container::
+
+  $ docker compose up
+
+Alternatively, you make use the image directly.  Pull `the Docker image`_::
+
+  $ docker pull "registry.gitlab.org/rpatterson/feed-archiver"
+
+And then use the image to create and run a container::
+
+  $ docker run --rm -it "registry.gitlab.org/rpatterson/feed-archiver" ...
+
+Images variant tags are published for the Python version, branch, and major/minor
+versions so that users can control when they get new images over time,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-main``.  The canonical
+Python version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:main``.  Pre-releases are from
+``develop`` and final releases are from ``main`` which is also the default for tags
+without a branch, e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310``. The
+major/minor version tags are only applied to the final release images and without the
+corresponding ``main`` branch tag,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-v0.8``.
+
+Multi-platform Docker images are published containing images for the following
+platforms or architectures in the Python 3.10 ``py310`` variant:
+
+- ``linux/amd64``
+- ``linux/arm64``
+- ``linux/arm/v7``
 
 
 ****************************************************************************************
 Usage
 ****************************************************************************************
 
 Create a ``./.feed-archiver.yml`` YAML file in a directory to serve as the root
@@ -209,14 +261,20 @@
     -h, --help            show this help message and exit
     --log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
 			  Select logging verbosity. (default: INFO)
     --archive-dir [ARCHIVE_DIR], -a [ARCHIVE_DIR]
 			  the archive root directory into which all feeds, their enclosures and assets
 			  will be downloaded (default: .)
 
+If using the Docker container image, the container can be run from the command-line as
+well::
+
+  $ docker compose run "feed-archiver" feed-archiver --help
+  usage: feed-archiver [-h]
+
 To link feed item enclosures into an `alternate hierarchy`_, such as in a media library,
 add a ``enclosures`` key to the feed configuration whose value is an list/array of
 objects each defining one alternative path to link to the feed item enclosure.  Any
 ``enclosures`` defined in the top-level ``defaults`` key will be used for all feeds.
 Configuration to be shared across multiple ``enclosures`` configurations may be placed
 in the corresponding ``defaults`` / ``plugins`` / ``enclosures`` / ``{plugin_name}``
 object.  The actual linking of enclosures is delegated to `plugins`_.
@@ -378,15 +436,15 @@
 They may also include:
 
 - ``stem-append`` containing a string to append to the episode file stem before the
   enclosure suffix/extension
 
 
 ****************************************************************************************
-CONTRIBUTING
+Contributing
 ****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
@@ -423,14 +481,15 @@
    https://jellyfin.org/docs/general/server/media/external-audio-files.html
 .. _Sonarr: https://sonarr.tv
 .. _connect to the Sonarr API: https://github.com/Sonarr/Sonarr/wiki/API#url
 .. _look up the TV show/series: https://github.com/Sonarr/Sonarr/wiki/Series#getid
 .. _lookup the episode file: https://github.com/Sonarr/Sonarr/wiki/Episode#get
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/feed-archiver
+.. _`Docker Compose`: https://docs.docker.com/compose/
 .. _`the example ./docker-compose.yml file`:
    https://gitlab.com/rpatterson/feed-archiver/blob/main/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
```

### Comparing `feed-archiver-2.0.0b1/TODO.rst` & `feed-archiver-2.0.1b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/bin/cz-check-bump` & `feed-archiver-2.0.1b0/bin/cz-check-bump`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         (arg, False)
         for arg in (
             "changelog",
             "changelog_to_stdout",
             "no_verify",
             "check_consistency",
             "retry",
-            "pre_bump_hooks",
-            "post_bump_hooks",
+            "version_type",
         )
     )
     bump_cmd = commands.Bump(config=conf, arguments=arguments)
 
     compare_ref = parsed_args.compare_ref
     if compare_ref is None:
         # Reproduce last version lookup from `commitizen.commands.bump.Bump.__call__()`:
```

### Comparing `feed-archiver-2.0.0b1/bin/entrypoint` & `feed-archiver-2.0.1b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/bin/get-base-version` & `feed-archiver-2.0.1b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/build-host/Dockerfile` & `feed-archiver-2.0.1b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/build-host/Makefile` & `feed-archiver-2.0.1b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/build-host/README.rst` & `feed-archiver-2.0.1b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/build-host/bin/entrypoint` & `feed-archiver-2.0.1b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/build-host/requirements-py310.txt` & `feed-archiver-2.0.1b0/build-host/requirements-py310.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.0b1/build-host/requirements-py311.txt` & `feed-archiver-2.0.1b0/build-host/requirements-py39.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py311.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
@@ -24,11 +24,15 @@
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
+tomli==2.0.1
+    # via
+    #   pyproject-api
+    #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.0b1/build-host/requirements-py37.txt` & `feed-archiver-2.0.1b0/build-host/requirements-py37.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.4.1
+importlib-metadata==6.6.0
     # via
     #   pluggy
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
@@ -40,11 +40,11 @@
 tox==4.4.12
     # via -r build-host/requirements.txt.in
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
     #   tox
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via tox
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.0b1/build-host/requirements-py38.txt` & `feed-archiver-2.0.1b0/build-host/requirements-py38.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.0b1/build-host/requirements-py39.txt` & `feed-archiver-2.0.1b0/build-host/requirements-py311.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py311.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
@@ -24,15 +24,11 @@
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
-tomli==2.0.1
-    # via
-    #   pyproject-api
-    #   tox
 tox==4.4.12
     # via -r build-host/requirements.txt.in
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.0b1/docker-compose-servarr.yml` & `feed-archiver-2.0.1b0/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/docker-compose.override.yml` & `feed-archiver-2.0.1b0/docker-compose.override.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # `./docker-compose.yml`.
 version: "3.8"
 
 services:
 
   # Configuration specific to development:
   feed-archiver:
-    image: "merpatterson/feed-archiver:${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    image: "\
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/feed-archiver\
+      :${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "feed-archiver-checkout"
     build:
       context: "${CHECKOUT_DIR}/"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
@@ -41,15 +43,17 @@
   ofelia:
     container_name: "feed-archiver-devel-ofelia"
 
   ## Contianers used for development and release:
 
   # Container for use by developers:
   feed-archiver-devel:
-    image: "merpatterson/feed-archiver:devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    image: "\
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/feed-archiver\
+      :devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "feed-archiver-devel"
     profiles:
       - "test"
     build:
       context: "${CHECKOUT_DIR}/"
       dockerfile: "${CHECKOUT_DIR}/Dockerfile.devel"
       args:
@@ -68,17 +72,21 @@
       # Ensure local changes are reflected inside the container.
       - "${CHECKOUT_DIR}/bin/entrypoint:/usr/local/bin/entrypoint"
       - "${CHECKOUT_DIR}/:/usr/local/src/feed-archiver/"
       # Preserve caches caches between container runs
       - "${CHECKOUT_DIR}/home/:/home/feed-archiver/"
       # Avoid any clashes between image variants and/or the local host at both build and
       # run-time.
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/:/usr/local/src/feed-archiver/var/"
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/:/usr/local/src/feed-archiver/.tox/"
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/feed_archiver.egg-info/:/usr/local/src/feed-archiver/src/feed_archiver.egg-info/"
+      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/\
+        :/usr/local/src/feed-archiver/var/"
+      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/\
+        :/usr/local/src/feed-archiver/.tox/"
+      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}\
+        /feed_archiver.egg-info/\
+        :/usr/local/src/feed-archiver/src/feed_archiver.egg-info/"
 
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
     image: "ghcr.io/hadolint/hadolint"
     profiles:
       - "test"
     environment:
@@ -94,16 +102,21 @@
     profiles:
       - "release"
     user: "${PUID:-1000}:${PGID:-${PUID:-1000}}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
       - "${CHECKOUT_DIR}/:/data/"
+    entrypoint: "ash"
+    # Strip reStructuredText directives unsupported in Markdown:
     command: >-
-      "./README.rst" -f "rst" -t "markdown" -o "./README.md"
+      -xeu -c '
+        grep -Ev "^ *\.\. +(contents)::.*" "./README.rst" |
+        pandoc -f "rst" -t "markdown" -o "./var/README.md"
+      '
 
   docker-pushrm:
     image: "chko/docker-pushrm"
     depends_on:
       pandoc:
         condition: "service_completed_successfully"
     profiles:
@@ -111,32 +124,35 @@
     environment:
       TZ: "${TZ:-Etc/UTC}"
       DOCKER_USER: "${DOCKER_USER:-merpatterson}"
       DOCKER_PASS: "${DOCKER_PASS}"
     volumes:
       - "${CHECKOUT_DIR}/:/data/"
     command: >-
-      --file "/data/README.md" --short "feed archiver foundation or template"
+      --file "/data/var/README.md"
+      --short "feed archiver foundation or template"
       --debug "merpatterson/feed-archiver"
 
   gitlab-release-cli:
-    image: "registry.gitlab.com/gitlab-org/release-cli:latest"
+    image: "${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/gitlab-org/release-cli:latest"
     profiles:
       - "release"
     environment:
       CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
     volumes:
       - "./:/usr/local/src/feed-archiver/"
     working_dir: "/usr/local/src/feed-archiver/"
 
   ## Containers related to CI/CD:
 
   # The container in which CI/CD is run:
   build-host:
-    image: "merpatterson/feed-archiver:build-host"
+    image: "\
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/feed-archiver\
+      :build-host"
     profiles:
       - "ci"
     build: "${CHECKOUT_DIR}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
       - "${CHECKOUT_DIR}/:${CHECKOUT_DIR}"
```

### Comparing `feed-archiver-2.0.0b1/docker-compose.yml` & `feed-archiver-2.0.1b0/docker-compose.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 version: "3.8"
 
 services:
 
   ## Container for use by end users:
   feed-archiver:
-    image: "merpatterson/feed-archiver"
+    image: "registry.gitlab.com/rpatterson/feed-archiver"
     container_name: "feed-archiver"
     # Needed because we expect the container to run once and exit and to be run by
     # ofelia from then on.
     restart: "no"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env` to match permissions inside and
```

### Comparing `feed-archiver-2.0.0b1/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.1b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/nginx/templates/default.conf.template` & `feed-archiver-2.0.1b0/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/pyproject.toml` & `feed-archiver-2.0.1b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "2.0.0b1"
+version = "2.0.1b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-2.0.0b1/requirements/build.txt.in` & `feed-archiver-2.0.1b0/requirements/build.txt.in`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Build, release and development tools that can operate totally independently and are
 # used outside the Docker container in the developer's localhost environment.
 
+# Get the Python dist/package version from VCS `v#.#.#` tags dynamically.
+setuptools_scm
+
 # VCS hooks to enforce passint tests, test coverage, style and linting
 pre-commit
 
 # Release libraries and tools.
 # Parse commit messages according to conventional commits to decide wether the next
 # version tag should be a major, minor or patch bump and create the VCS tag.  Also VCS
 # hooks to enforce that commit messages comply with conventional commits
```

### Comparing `feed-archiver-2.0.0b1/requirements/py310/build.txt` & `feed-archiver-2.0.1b0/requirements/py38/build.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.6
+argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==2.42.1
+commitizen==3.0.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==4.13.0
     # via
+    #   commitizen
     #   keyring
     #   twine
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -57,26 +60,28 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via commitizen
+    # via
+    #   commitizen
+    #   setuptools-scm
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -92,32 +97,40 @@
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
+setuptools-scm==7.1.0
+    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
-termcolor==2.2.0
+termcolor==2.3.0
     # via commitizen
+tomli==2.0.1
+    # via setuptools-scm
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via commitizen
+    # via
+    #   rich
+    #   setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `feed-archiver-2.0.0b1/requirements/py310/devel.txt` & `feed-archiver-2.0.1b0/requirements/py38/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==23.1.0
     # via pytest-subtests
@@ -67,15 +67,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -137,15 +137,14 @@
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
-    #   setuptools-scm
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -155,16 +154,14 @@
 platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
-poetry-semver==0.1.0
-    # via requirements-detector
 pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
@@ -174,15 +171,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -224,30 +221,30 @@
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
-requirements-detector==1.1.0
+requirements-detector==1.2.1
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
     # via rstcheck
+semver==3.0.0
+    # via requirements-detector
 setoptconf-tmp==0.3.1
     # via prospector
-setuptools-scm==7.1.0
-    # via feed-archiver (pyproject.toml)
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
@@ -277,43 +274,44 @@
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
-    #   setuptools-scm
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.22
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
 types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
 types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
+    #   black
     #   mypy
     #   pydantic
-    #   setuptools-scm
+    #   pylint
+    #   rich
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.0b1/requirements/py310/user.txt` & `feed-archiver-2.0.1b0/requirements/py310/user.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
```

### Comparing `feed-archiver-2.0.0b1/requirements/py311/build.txt` & `feed-archiver-2.0.1b0/requirements/py311/build.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.6
+argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==2.42.1
+commitizen==3.0.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==4.13.0
     # via
+    #   commitizen
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -57,26 +58,28 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via commitizen
+    # via
+    #   commitizen
+    #   setuptools-scm
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -92,29 +95,31 @@
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
+setuptools-scm==7.1.0
+    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
-termcolor==2.2.0
+termcolor==2.3.0
     # via commitizen
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via commitizen
+    # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.0b1/requirements/py311/devel.txt` & `feed-archiver-2.0.1b0/requirements/py311/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==23.1.0
     # via pytest-subtests
@@ -65,15 +65,15 @@
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -135,15 +135,14 @@
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
-    #   setuptools-scm
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -153,16 +152,14 @@
 platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
-poetry-semver==0.1.0
-    # via requirements-detector
 pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
@@ -172,15 +169,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -222,30 +219,30 @@
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
-requirements-detector==1.1.0
+requirements-detector==1.2.1
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
     # via rstcheck
+semver==3.0.0
+    # via requirements-detector
 setoptconf-tmp==0.3.1
     # via prospector
-setuptools-scm==7.1.0
-    # via feed-archiver (pyproject.toml)
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
@@ -269,15 +266,15 @@
     #   prospector
     #   requirements-detector
     #   vulture
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.22
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
@@ -285,20 +282,19 @@
     # via feed-archiver (pyproject.toml)
 types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   mypy
     #   pydantic
-    #   setuptools-scm
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.0b1/requirements/py311/user.txt` & `feed-archiver-2.0.1b0/requirements/py311/user.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py311/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
```

### Comparing `feed-archiver-2.0.0b1/requirements/py37/build.txt` & `feed-archiver-2.0.1b0/requirements/py37/build.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.6
+argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==2.42.1
+commitizen==3.0.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==5.2.0
+importlib-metadata==4.13.0
     # via
     #   argcomplete
+    #   commitizen
     #   keyring
     #   pre-commit
+    #   setuptools-scm
     #   twine
     #   virtualenv
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
@@ -62,26 +64,28 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via commitizen
+    # via
+    #   commitizen
+    #   setuptools-scm
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -97,34 +101,39 @@
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
+setuptools-scm==7.1.0
+    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
-termcolor==2.2.0
+termcolor==2.3.0
     # via commitizen
+tomli==2.0.1
+    # via setuptools-scm
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   commitizen
     #   importlib-metadata
     #   markdown-it-py
     #   platformdirs
     #   rich
+    #   setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via
```

### Comparing `feed-archiver-2.0.0b1/requirements/py37/devel.txt` & `feed-archiver-2.0.1b0/requirements/py37/devel.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==23.1.0
     # via pytest-subtests
@@ -69,15 +69,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -113,15 +113,14 @@
     #   feed-archiver (pyproject.toml)
     #   pluggy
     #   pre-commit
     #   pydocstyle
     #   pytest
     #   rstcheck
     #   rstcheck-core
-    #   setuptools-scm
     #   stevedore
     #   virtualenv
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.11.5
@@ -155,15 +154,14 @@
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
-    #   setuptools-scm
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -173,16 +171,14 @@
 platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
-poetry-semver==0.1.0
-    # via requirements-detector
 pre-commit==2.21.0
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
@@ -192,15 +188,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -242,30 +238,30 @@
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
-requirements-detector==1.1.0
+requirements-detector==1.2.1
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
     # via rstcheck
+semver==3.0.0
+    # via requirements-detector
 setoptconf-tmp==0.3.1
     # via prospector
-setuptools-scm==7.1.0
-    # via feed-archiver (pyproject.toml)
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
@@ -295,21 +291,20 @@
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
-    #   setuptools-scm
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.22
     # via pyroma
 typed-ast==1.5.4
     # via
     #   astroid
     #   black
     #   mypy
 typer[all]==0.7.0
@@ -333,20 +328,19 @@
     #   mypy
     #   platformdirs
     #   pydantic
     #   pylint
     #   rich
     #   rstcheck
     #   rstcheck-core
-    #   setuptools-scm
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.21.0
+virtualenv==20.21.1
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.0b1/requirements/py37/user.txt` & `feed-archiver-2.0.1b0/requirements/py37/user.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py37/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 backports-cached-property==1.0.2 ; python_version < "3.8"
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
@@ -28,15 +28,15 @@
 httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
-importlib-metadata==5.2.0 ; python_version < "3.8"
+importlib-metadata==6.6.0 ; python_version < "3.8"
     # via
     #   argcomplete
     #   feed-archiver (pyproject.toml)
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.0b1/requirements/py38/build.txt` & `feed-archiver-2.0.1b0/requirements/py39/build.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.6
+argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==2.42.1
+commitizen==3.0.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==4.13.0
     # via
+    #   commitizen
     #   keyring
     #   twine
-importlib-resources==5.12.0
-    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -59,26 +58,28 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via commitizen
+    # via
+    #   commitizen
+    #   setuptools-scm
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -94,36 +95,36 @@
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
+setuptools-scm==7.1.0
+    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
-termcolor==2.2.0
+termcolor==2.3.0
     # via commitizen
+tomli==2.0.1
+    # via setuptools-scm
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via
-    #   commitizen
-    #   rich
+    # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `feed-archiver-2.0.0b1/requirements/py38/devel.txt` & `feed-archiver-2.0.1b0/requirements/py310/devel.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==23.1.0
     # via pytest-subtests
@@ -67,15 +67,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -137,15 +137,14 @@
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
-    #   setuptools-scm
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -155,16 +154,14 @@
 platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
-poetry-semver==0.1.0
-    # via requirements-detector
 pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
@@ -174,15 +171,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -224,30 +221,30 @@
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
-requirements-detector==1.1.0
+requirements-detector==1.2.1
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
     # via rstcheck
+semver==3.0.0
+    # via requirements-detector
 setoptconf-tmp==0.3.1
     # via prospector
-setuptools-scm==7.1.0
-    # via feed-archiver (pyproject.toml)
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
@@ -277,46 +274,41 @@
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
-    #   setuptools-scm
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.22
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
 types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
 types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
-    #   black
     #   mypy
     #   pydantic
-    #   pylint
-    #   rich
-    #   setuptools-scm
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.0b1/requirements/py38/user.txt` & `feed-archiver-2.0.1b0/requirements/py38/user.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
```

### Comparing `feed-archiver-2.0.0b1/requirements/py39/build.txt` & `feed-archiver-2.0.1b0/requirements/py310/build.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.6
+argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==2.42.1
+commitizen==3.0.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.4.1
+importlib-metadata==4.13.0
     # via
+    #   commitizen
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -57,26 +58,28 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via commitizen
+    # via
+    #   commitizen
+    #   setuptools-scm
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
@@ -92,29 +95,33 @@
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
+setuptools-scm==7.1.0
+    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
-termcolor==2.2.0
+termcolor==2.3.0
     # via commitizen
+tomli==2.0.1
+    # via setuptools-scm
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via commitizen
+    # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.0b1/requirements/py39/devel.txt` & `feed-archiver-2.0.1b0/requirements/py39/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.2
+astroid==2.15.3
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==23.1.0
     # via pytest-subtests
@@ -67,15 +67,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -137,15 +137,14 @@
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
-    #   setuptools-scm
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
@@ -155,16 +154,14 @@
 platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
-poetry-semver==0.1.0
-    # via requirements-detector
 pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
@@ -174,15 +171,15 @@
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.15.0
+pygments==2.15.1
     # via
     #   pyroma
     #   rich
 pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
@@ -224,30 +221,30 @@
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
-requirements-detector==1.1.0
+requirements-detector==1.2.1
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
     # via rstcheck
+semver==3.0.0
+    # via requirements-detector
 setoptconf-tmp==0.3.1
     # via prospector
-setuptools-scm==7.1.0
-    # via feed-archiver (pyproject.toml)
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
@@ -277,21 +274,20 @@
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
-    #   setuptools-scm
     #   towncrier
 tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.22
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.7
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
@@ -302,20 +298,19 @@
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
-    #   setuptools-scm
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.0b1/requirements/py39/user.txt` & `feed-archiver-2.0.1b0/requirements/py39/user.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
```

### Comparing `feed-archiver-2.0.0b1/server/docker-compose.yml` & `feed-archiver-2.0.1b0/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/setup.cfg` & `feed-archiver-2.0.1b0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = feed-archiver
 version = attr: src.feedarchiver.version
 description = Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 url = https://gitlab.com/rpatterson/feed-archiver
 long_description = file: README.rst
 long_description_content_type = text/x-rst
-keywords = template, structure
+keywords = feeds, syndication, rss, atom, podcasts, enclosures
 author = Ross Patterson
 author_email = me@rpatterson.net
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
@@ -64,15 +64,14 @@
 	prospector[with_everything]
 	xenon
 	rstcheck
 	black
 	autoflake
 	autopep8
 	pip-tools
-	setuptools_scm
 	towncrier
 	build
 	lxml-stubs
 	types-requests
 	types-PyYAML
 
 [tool:pytest]
```

### Comparing `feed-archiver-2.0.0b1/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.1b0/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.0b1
+Version: 2.0.1b0
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
-Keywords: template,structure
+Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -83,14 +83,27 @@
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
 	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
 	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
+     - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
+          :alt: KeyBase PGP key ID
+          :target: https://keybase.io/rpatterson
+       .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
+          :alt: GitHub followers count
+          :target: https://github.com/rpatterson
+       .. figure:: https://img.shields.io/liberapay/receives/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay donated per week
+          :target: https://liberapay.com/rpatterson/donate
+       .. figure:: https://img.shields.io/liberapay/patrons/rpatterson.svg?logo=liberapay
+          :alt: LiberaPay patrons count
+          :target: https://liberapay.com/rpatterson/donate
+
 The ``$ feed-archiver`` command aims to archive RSS/Atom feeds as fully as possible in
 such a way that the archive can serve (at least) 2 use cases:
 
 #. `Mirror of Feed Enclosures and Assets`_
 
     A mirror of the archived feeds that can be in turn served onto onto feed
     clients/subscribers (such as podcatchers).  For example, you can subscribe to the
@@ -103,14 +116,16 @@
 
 #. `Ingest Feed Enclosures Into Media Libraries`_
 
     An alternate hierarchy of feed item enclosures better suited for ingestion into
     other media software, such as media library servers.  For example, your podcast
     episodes can also be made available in your `Jellyfin`_/Emby/Plex library.
 
+.. contents:: Table of Contents
+
 ********************
 Detailed Description
 ********************
 
 Mirror of Feed Enclosures and Assets
 ====================================
 
@@ -171,22 +186,59 @@
 re-using example configurations known to work by others.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
+Install and use either via a local, native installation or a Docker container image:
+
+Local/Native Installation
+========================================================================================
+
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
-  $ sudo pip3 install feed-archiver
+  $ pip3 install --user feed-archiver
 
 Optional shell tab completion is available via `argcomplete`_.
 
-Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
-details.
+Docker Container Image Installation
+========================================================================================
+
+The recommended way to use the Docker container image is via `Docker Compose`_.  See
+`the example ./docker-compose.yml file`_ for an example configuration.  Once you have
+your configuration, you can create and run the container::
+
+  $ docker compose up
+
+Alternatively, you make use the image directly.  Pull `the Docker image`_::
+
+  $ docker pull "registry.gitlab.org/rpatterson/feed-archiver"
+
+And then use the image to create and run a container::
+
+  $ docker run --rm -it "registry.gitlab.org/rpatterson/feed-archiver" ...
+
+Images variant tags are published for the Python version, branch, and major/minor
+versions so that users can control when they get new images over time,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-main``.  The canonical
+Python version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:main``.  Pre-releases are from
+``develop`` and final releases are from ``main`` which is also the default for tags
+without a branch, e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310``. The
+major/minor version tags are only applied to the final release images and without the
+corresponding ``main`` branch tag,
+e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-v0.8``.
+
+Multi-platform Docker images are published containing images for the following
+platforms or architectures in the Python 3.10 ``py310`` variant:
+
+- ``linux/amd64``
+- ``linux/arm64``
+- ``linux/arm/v7``
 
 
 ****************************************************************************************
 Usage
 ****************************************************************************************
 
 Create a ``./.feed-archiver.yml`` YAML file in a directory to serve as the root
@@ -237,14 +289,20 @@
     -h, --help            show this help message and exit
     --log-level {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
 			  Select logging verbosity. (default: INFO)
     --archive-dir [ARCHIVE_DIR], -a [ARCHIVE_DIR]
 			  the archive root directory into which all feeds, their enclosures and assets
 			  will be downloaded (default: .)
 
+If using the Docker container image, the container can be run from the command-line as
+well::
+
+  $ docker compose run "feed-archiver" feed-archiver --help
+  usage: feed-archiver [-h]
+
 To link feed item enclosures into an `alternate hierarchy`_, such as in a media library,
 add a ``enclosures`` key to the feed configuration whose value is an list/array of
 objects each defining one alternative path to link to the feed item enclosure.  Any
 ``enclosures`` defined in the top-level ``defaults`` key will be used for all feeds.
 Configuration to be shared across multiple ``enclosures`` configurations may be placed
 in the corresponding ``defaults`` / ``plugins`` / ``enclosures`` / ``{plugin_name}``
 object.  The actual linking of enclosures is delegated to `plugins`_.
@@ -406,15 +464,15 @@
 They may also include:
 
 - ``stem-append`` containing a string to append to the episode file stem before the
   enclosure suffix/extension
 
 
 ****************************************************************************************
-CONTRIBUTING
+Contributing
 ****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
@@ -451,14 +509,15 @@
    https://jellyfin.org/docs/general/server/media/external-audio-files.html
 .. _Sonarr: https://sonarr.tv
 .. _connect to the Sonarr API: https://github.com/Sonarr/Sonarr/wiki/API#url
 .. _look up the TV show/series: https://github.com/Sonarr/Sonarr/wiki/Series#getid
 .. _lookup the episode file: https://github.com/Sonarr/Sonarr/wiki/Episode#get
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/feed-archiver
+.. _`Docker Compose`: https://docs.docker.com/compose/
 .. _`the example ./docker-compose.yml file`:
    https://gitlab.com/rpatterson/feed-archiver/blob/main/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
```

### Comparing `feed-archiver-2.0.0b1/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.1b0/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -134,8 +134,9 @@
 src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
 src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
 src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+src/pythonprojectstructure/newsfragments/+upgrade-requirements.bugfix.rst
```

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/__init__.py` & `feed-archiver-2.0.1b0/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/archive.py` & `feed-archiver-2.0.1b0/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.1b0/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.1b0/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.1b0/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/feed.py` & `feed-archiver-2.0.1b0/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/formats.py` & `feed-archiver-2.0.1b0/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.1b0/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/src/feedarchiver/utils.py` & `feed-archiver-2.0.1b0/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b1/tox.ini` & `feed-archiver-2.0.1b0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -64,12 +64,12 @@
 
 [testenv:build]
 description = Independent build, release, devel tools (requires PYTHON_HOST_ENV)
 skip_install = true
 # Workaround an issue with `skip_install` and passing in the `--installpkg` CLI option:
 # https://github.com/tox-dev/tox/issues/2442#issuecomment-1347549575
 package_env =
-deps = -rrequirements/{env:PYTHON_HOST_ENV}/build.txt
+deps = -rrequirements/{env:PYTHON_HOST_ENV:py310}/build.txt
 commands =
 
 [testenv:.pkg]
 deps = build
```

