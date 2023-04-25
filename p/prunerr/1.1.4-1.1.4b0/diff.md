# Comparing `tmp/prunerr-1.1.4.tar.gz` & `tmp/prunerr-1.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prunerr-1.1.4.tar", last modified: Tue Apr 25 07:10:17 2023, max compression
+gzip compressed data, was "prunerr-1.1.4b0.tar", last modified: Tue Apr 25 05:09:45 2023, max compression
```

## Comparing `prunerr-1.1.4.tar` & `prunerr-1.1.4b0.tar`

### file list

```diff
@@ -1,1377 +1,1377 @@
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-25 04:48:04.000000 prunerr-1.1.4/.dir-locals.el.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.4/.dockerignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1261 2023-04-25 04:48:04.000000 prunerr-1.1.4/.env.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/.github/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/.github/workflows/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-25 04:48:04.000000 prunerr-1.1.4/.github/workflows/build-test.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.4/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4341 2023-04-25 04:48:04.000000 prunerr-1.1.4/.gitlab-ci.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      777 2023-04-25 04:48:04.000000 prunerr-1.1.4/.pre-commit-config.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-25 04:48:04.000000 prunerr-1.1.4/.prospector.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-25 04:48:04.000000 prunerr-1.1.4/CONTRIBUTING.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2429 2023-04-25 04:48:04.000000 prunerr-1.1.4/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3224 2023-04-25 04:48:04.000000 prunerr-1.1.4/Dockerfile.devel
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-25 04:48:04.000000 prunerr-1.1.4/LICENSE
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    58261 2023-04-25 04:48:04.000000 prunerr-1.1.4/Makefile
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       70 2023-04-25 06:48:17.000000 prunerr-1.1.4/NEWS-VERSION.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     4770 2023-04-25 06:48:17.000000 prunerr-1.1.4/NEWS.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17773 2023-04-25 07:10:17.241116 prunerr-1.1.4/PKG-INFO
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16788 2023-04-25 06:38:28.000000 prunerr-1.1.4/README.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5038 2023-04-25 04:48:04.000000 prunerr-1.1.4/TODO.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2759 2023-04-25 04:48:04.000000 prunerr-1.1.4/bin/cz-check-bump
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-25 04:48:04.000000 prunerr-1.1.4/bin/entrypoint
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-25 04:48:04.000000 prunerr-1.1.4/bin/get-base-version
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-25 04:48:04.000000 prunerr-1.1.4/bin/hadolint
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/build-host/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-25 04:48:04.000000 prunerr-1.1.4/build-host/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-25 04:48:04.000000 prunerr-1.1.4/build-host/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-25 04:48:04.000000 prunerr-1.1.4/build-host/README.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/build-host/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-25 04:48:04.000000 prunerr-1.1.4/build-host/bin/entrypoint
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      730 2023-04-25 06:47:20.000000 prunerr-1.1.4/build-host/requirements-py310.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      673 2023-04-25 06:47:20.000000 prunerr-1.1.4/build-host/requirements-py311.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      947 2023-04-25 06:47:20.000000 prunerr-1.1.4/build-host/requirements-py37.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-25 06:47:20.000000 prunerr-1.1.4/build-host/requirements-py38.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-25 06:47:20.000000 prunerr-1.1.4/build-host/requirements-py39.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-25 04:48:04.000000 prunerr-1.1.4/build-host/requirements.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/dist/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.4/dist/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-25 04:48:04.000000 prunerr-1.1.4/docker-compose-servarr.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5132 2023-04-25 04:48:04.000000 prunerr-1.1.4/docker-compose.override.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4047 2023-04-25 04:48:04.000000 prunerr-1.1.4/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/gitlab-runner/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/gitlab-runner/config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-25 04:48:04.000000 prunerr-1.1.4/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      566 2023-04-25 04:48:04.000000 prunerr-1.1.4/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/home/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-25 04:48:04.000000 prunerr-1.1.4/home/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-25 04:48:04.000000 prunerr-1.1.4/home/.pypirc.in
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     3005 2023-04-25 06:48:17.000000 prunerr-1.1.4/pyproject.toml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/requirements/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      668 2023-04-25 04:48:04.000000 prunerr-1.1.4/requirements/build.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/requirements/py310/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2567 2023-04-25 04:48:04.000000 prunerr-1.1.4/requirements/py310/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5141 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py310/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py310/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/requirements/py311/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2529 2023-04-25 04:48:04.000000 prunerr-1.1.4/requirements/py311/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4915 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py311/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py311/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/requirements/py37/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2840 2023-04-25 04:48:04.000000 prunerr-1.1.4/requirements/py37/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5960 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py37/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py37/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/requirements/py38/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2668 2023-04-25 04:48:04.000000 prunerr-1.1.4/requirements/py38/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5459 2023-04-25 06:54:29.000000 prunerr-1.1.4/requirements/py38/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-25 06:54:16.000000 prunerr-1.1.4/requirements/py38/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/requirements/py39/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2565 2023-04-25 04:48:04.000000 prunerr-1.1.4/requirements/py39/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5446 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py39/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-25 06:47:20.000000 prunerr-1.1.4/requirements/py39/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/s6/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/s6/etc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/s6/etc/s6-overlay/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/s6/etc/s6-overlay/s6-rc.d/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-25 04:48:04.000000 prunerr-1.1.4/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1748 2023-04-25 07:10:17.241116 prunerr-1.1.4/setup.cfg
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/src/prunerr/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/__main__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/downloaditem.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/src/prunerr/home/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/home/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/src/prunerr/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/newsfragments/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/servarr.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/src/prunerr/tests/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/example-5s.mkv
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/daemon/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/daemon/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/download-client-only/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/download-clients/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/download-clients/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/download-items/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/download-items/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/empty/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/empty/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/empty/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/move-exec/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/move-exec/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/move-exec/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/home/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/home/review-edge-cases/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:08:55.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:08:55.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.193115 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.221116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.197116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.225116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.201115 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.229116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.205115 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.233116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:08:55.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.209116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:08:55.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:08:55.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.237116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_cli.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_daemon.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_downloaditem.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_free_space.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_move.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_review.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_servarr.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/tests/test_verify.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/prunerr/utils.py
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      160 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr/version.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.217116 prunerr-1.1.4/src/prunerr.egg-info/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17773 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr.egg-info/PKG-INFO
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64730 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr.egg-info/SOURCES.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr.egg-info/dependency_links.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr.egg-info/entry_points.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      312 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr.egg-info/requires.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-25 07:10:17.000000 prunerr-1.1.4/src/prunerr.egg-info/top_level.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.213116 prunerr-1.1.4/src/pythonprojectstructure/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 07:10:17.241116 prunerr-1.1.4/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       87 2023-04-25 04:48:04.000000 prunerr-1.1.4/src/pythonprojectstructure/newsfragments/+upgrade-requirements.bugfix.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3327 2023-04-25 04:48:04.000000 prunerr-1.1.4/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.dir-locals.el.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.dockerignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1261 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.env.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/.github/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/.github/workflows/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4341 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.gitlab-ci.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      777 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/.prospector.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2429 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3224 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/Dockerfile.devel
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/LICENSE
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    58261 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      166 2023-04-25 04:49:00.000000 prunerr-1.1.4b0/NEWS-VERSION.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4699 2023-04-25 04:49:02.000000 prunerr-1.1.4b0/NEWS.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17607 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/PKG-INFO
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16620 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/README.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5038 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/TODO.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2759 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/bin/cz-check-bump
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/bin/entrypoint
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/bin/get-base-version
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/bin/hadolint
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/build-host/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/build-host/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/build-host/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/build-host/README.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/build-host/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      730 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      673 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      947 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/build-host/requirements.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/dist/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/dist/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/docker-compose-servarr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5132 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/docker-compose.override.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4047 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/gitlab-runner/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/gitlab-runner/config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      566 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/home/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/home/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/home/.pypirc.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3007 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/pyproject.toml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/requirements/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      668 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/requirements/build.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/requirements/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2567 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/requirements/py310/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5141 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py310/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/requirements/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2529 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/requirements/py311/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4915 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py311/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/requirements/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2840 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/requirements/py37/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5960 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py37/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/requirements/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2668 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/requirements/py38/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5459 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py38/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/requirements/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2565 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/requirements/py39/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5446 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-25 04:49:03.000000 prunerr-1.1.4b0/requirements/py39/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/s6/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/s6/etc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/s6/etc/s6-overlay/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/s6/etc/s6-overlay/s6-rc.d/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.888635 prunerr-1.1.4b0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1748 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/setup.cfg
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/__main__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/downloaditem.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/home/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/home/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/newsfragments/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/servarr.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/example-5s.mkv
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/daemon/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/daemon/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/download-client-only/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/download-clients/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/download-clients/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/download-items/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/download-items/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/empty/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/empty/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/empty/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/move-exec/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/move-exec/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/move-exec/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/home/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/home/review-edge-cases/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:08:18.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.844634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:08:18.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.896635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.848634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.852634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.900635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.856634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.904635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.860634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.908635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.864634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.912635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.868634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.872634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.916635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:08:18.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.876634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.920635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:08:18.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:08:18.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.880634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.924635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_cli.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_daemon.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_downloaditem.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_free_space.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_move.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_review.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_servarr.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/tests/test_verify.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/prunerr/utils.py
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      162 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr/version.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.892634 prunerr-1.1.4b0/src/prunerr.egg-info/
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    17607 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr.egg-info/PKG-INFO
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64730 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr.egg-info/SOURCES.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr.egg-info/dependency_links.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr.egg-info/entry_points.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      312 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr.egg-info/requires.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-25 05:09:45.000000 prunerr-1.1.4b0/src/prunerr.egg-info/top_level.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.884634 prunerr-1.1.4b0/src/pythonprojectstructure/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-25 05:09:45.928635 prunerr-1.1.4b0/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       87 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/src/pythonprojectstructure/newsfragments/+upgrade-requirements.bugfix.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3327 2023-04-25 04:48:04.000000 prunerr-1.1.4b0/tox.ini
```

### Comparing `prunerr-1.1.4/.dir-locals.el.in` & `prunerr-1.1.4b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.dockerignore` & `prunerr-1.1.4b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.env.in` & `prunerr-1.1.4b0/.env.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.github/workflows/build-test.yml` & `prunerr-1.1.4b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.gitignore` & `prunerr-1.1.4b0/.gitignore`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.gitlab-ci.yml` & `prunerr-1.1.4b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.pre-commit-config.yaml` & `prunerr-1.1.4b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/.prospector.yaml` & `prunerr-1.1.4b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/CONTRIBUTING.rst` & `prunerr-1.1.4b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/Dockerfile` & `prunerr-1.1.4b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/Dockerfile.devel` & `prunerr-1.1.4b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/LICENSE` & `prunerr-1.1.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/Makefile` & `prunerr-1.1.4b0/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/NEWS.rst` & `prunerr-1.1.4b0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 prunerr  (2023-04-25)
 =====================
 
-No significant changes.
-
-
-prunerr  (2023-04-25)
-=====================
-
 Improved Documentation
 ----------------------
 
 - Link important use cases to their corresponding example configuration.
 
 
 prunerr  (2023-04-24)
```

### Comparing `prunerr-1.1.4/PKG-INFO` & `prunerr-1.1.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.4
+Version: 1.1.4b0
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
@@ -62,17 +62,17 @@
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/prunerr?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/prunerr/releases
        .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
           :target: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml
-       .. figure:: https://app.codecov.io/github/rpatterson/prunerr/branch/main/graph/badge.svg?token=GNKVQ8VYOU
+       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
-	  :target: https://app.codecov.io/github/rpatterson/prunerr
+	  :target: https://codecov.io/github/rpatterson/prunerr
        .. figure:: https://img.shields.io/github/stars/rpatterson/prunerr?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/prunerr/
 
      - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr/main?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
@@ -111,17 +111,14 @@
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L145-177>`_.
 - Delete `public items first
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L142-144>`_.
 - Delete private items in `an order to maximize tracker ratio and/or bonuses
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L188-209>`_.
 - Delete `stalled items
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L188-209>`_
-  , and `items containing archives such as *.rar
-  releases
-  <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L78-97>`_
   and `blacklist them
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L77>`_,
   AKA mark them as failed, in Servarr.
 - And more...
 
 .. contents:: Table of Contents
```

### Comparing `prunerr-1.1.4/README.rst` & `prunerr-1.1.4b0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/prunerr?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/prunerr/releases
        .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
           :target: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml
-       .. figure:: https://app.codecov.io/github/rpatterson/prunerr/branch/main/graph/badge.svg?token=GNKVQ8VYOU
+       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
-	  :target: https://app.codecov.io/github/rpatterson/prunerr
+	  :target: https://codecov.io/github/rpatterson/prunerr
        .. figure:: https://img.shields.io/github/stars/rpatterson/prunerr?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/prunerr/
 
      - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr/main?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
@@ -84,17 +84,14 @@
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L145-177>`_.
 - Delete `public items first
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L142-144>`_.
 - Delete private items in `an order to maximize tracker ratio and/or bonuses
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L188-209>`_.
 - Delete `stalled items
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L188-209>`_
-  , and `items containing archives such as *.rar
-  releases
-  <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L78-97>`_
   and `blacklist them
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L77>`_,
   AKA mark them as failed, in Servarr.
 - And more...
 
 .. contents:: Table of Contents
```

### Comparing `prunerr-1.1.4/TODO.rst` & `prunerr-1.1.4b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/bin/cz-check-bump` & `prunerr-1.1.4b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/bin/entrypoint` & `prunerr-1.1.4b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/bin/get-base-version` & `prunerr-1.1.4b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/Dockerfile` & `prunerr-1.1.4b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/Makefile` & `prunerr-1.1.4b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/README.rst` & `prunerr-1.1.4b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/bin/entrypoint` & `prunerr-1.1.4b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/requirements-py310.txt` & `prunerr-1.1.4b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/requirements-py311.txt` & `prunerr-1.1.4b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/requirements-py37.txt` & `prunerr-1.1.4b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/requirements-py38.txt` & `prunerr-1.1.4b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/build-host/requirements-py39.txt` & `prunerr-1.1.4b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/docker-compose-servarr.yml` & `prunerr-1.1.4b0/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/docker-compose.override.yml` & `prunerr-1.1.4b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/docker-compose.yml` & `prunerr-1.1.4b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/gitlab-runner/config/config.toml.in` & `prunerr-1.1.4b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/gitlab-runner/docker-compose.yml` & `prunerr-1.1.4b0/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/pyproject.toml` & `prunerr-1.1.4b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "1.1.4"
+version = "1.1.4b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `prunerr-1.1.4/requirements/build.txt.in` & `prunerr-1.1.4b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py310/build.txt` & `prunerr-1.1.4b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py310/devel.txt` & `prunerr-1.1.4b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py310/user.txt` & `prunerr-1.1.4b0/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py311/build.txt` & `prunerr-1.1.4b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py311/devel.txt` & `prunerr-1.1.4b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py311/user.txt` & `prunerr-1.1.4b0/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py37/build.txt` & `prunerr-1.1.4b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py37/devel.txt` & `prunerr-1.1.4b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py37/user.txt` & `prunerr-1.1.4b0/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py38/build.txt` & `prunerr-1.1.4b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py38/devel.txt` & `prunerr-1.1.4b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py38/user.txt` & `prunerr-1.1.4b0/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py39/build.txt` & `prunerr-1.1.4b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py39/devel.txt` & `prunerr-1.1.4b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/requirements/py39/user.txt` & `prunerr-1.1.4b0/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/setup.cfg` & `prunerr-1.1.4b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/__init__.py` & `prunerr-1.1.4b0/src/prunerr/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/downloadclient.py` & `prunerr-1.1.4b0/src/prunerr/downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/downloaditem.py` & `prunerr-1.1.4b0/src/prunerr/downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/home/.config/prunerr.yml` & `prunerr-1.1.4b0/src/prunerr/home/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/operations.py` & `prunerr-1.1.4b0/src/prunerr/operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/runner.py` & `prunerr-1.1.4b0/src/prunerr/runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/servarr.py` & `prunerr-1.1.4b0/src/prunerr/servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/Makefile` & `prunerr-1.1.4b0/src/prunerr/tests/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/__init__.py` & `prunerr-1.1.4b0/src/prunerr/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/example-5s.mkv` & `prunerr-1.1.4b0/src/prunerr/tests/example-5s.mkv`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/home/daemon/.config/prunerr.yml` & `prunerr-1.1.4b0/src/prunerr/tests/home/daemon/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/home/download-clients/.config/prunerr.yml` & `prunerr-1.1.4b0/src/prunerr/tests/home/download-clients/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml` & `prunerr-1.1.4b0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json` & `prunerr-1.1.4b0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_cli.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_daemon.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_downloadclient.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_downloaditem.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_free_space.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_free_space.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_move.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_move.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_operations.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_review.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_runner.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_servarr.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/tests/test_verify.py` & `prunerr-1.1.4b0/src/prunerr/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr/utils.py` & `prunerr-1.1.4b0/src/prunerr/utils.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/src/prunerr.egg-info/PKG-INFO` & `prunerr-1.1.4b0/src/prunerr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.4
+Version: 1.1.4b0
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
@@ -62,17 +62,17 @@
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/prunerr?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/prunerr/releases
        .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
           :target: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml
-       .. figure:: https://app.codecov.io/github/rpatterson/prunerr/branch/main/graph/badge.svg?token=GNKVQ8VYOU
+       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
-	  :target: https://app.codecov.io/github/rpatterson/prunerr
+	  :target: https://codecov.io/github/rpatterson/prunerr
        .. figure:: https://img.shields.io/github/stars/rpatterson/prunerr?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/prunerr/
 
      - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr/main?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
@@ -111,17 +111,14 @@
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L145-177>`_.
 - Delete `public items first
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L142-144>`_.
 - Delete private items in `an order to maximize tracker ratio and/or bonuses
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L188-209>`_.
 - Delete `stalled items
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L188-209>`_
-  , and `items containing archives such as *.rar
-  releases
-  <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L78-97>`_
   and `blacklist them
   <https://gitlab.com/rpatterson/prunerr/-/blob/main/src/prunerr/home/.config/prunerr.yml#L77>`_,
   AKA mark them as failed, in Servarr.
 - And more...
 
 .. contents:: Table of Contents
```

### Comparing `prunerr-1.1.4/src/prunerr.egg-info/SOURCES.txt` & `prunerr-1.1.4b0/src/prunerr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.4/tox.ini` & `prunerr-1.1.4b0/tox.ini`

 * *Files identical despite different names*

