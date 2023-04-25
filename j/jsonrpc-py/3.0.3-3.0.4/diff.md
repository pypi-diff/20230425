# Comparing `tmp/jsonrpc-py-3.0.3.tar.gz` & `tmp/jsonrpc-py-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.3.tar", last modified: Sun Apr 23 01:43:27 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.4.tar", last modified: Tue Apr 25 08:02:31 2023, max compression
```

## Comparing `jsonrpc-py-3.0.3.tar` & `jsonrpc-py-3.0.4.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.436999 jsonrpc-py-3.0.3/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:43:27.436999 jsonrpc-py-3.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.416000 jsonrpc-py-3.0.3/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.409000 jsonrpc-py-3.0.3/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.419000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.426999 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.429000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.431999 jsonrpc-py-3.0.3/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.433999 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1856 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 01:43:27.000000 jsonrpc-py-3.0.3/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 01:43:27.436999 jsonrpc-py-3.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:43:27.435999 jsonrpc-py-3.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-23 01:43:05.000000 jsonrpc-py-3.0.3/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.054547 jsonrpc-py-3.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-25 08:02:31.054547 jsonrpc-py-3.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.032545 jsonrpc-py-3.0.4/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.025544 jsonrpc-py-3.0.4/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.035545 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.043546 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.045546 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1602 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.049546 jsonrpc-py-3.0.4/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.050547 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-25 08:02:30.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-04-25 08:02:31.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:02:30.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 08:02:30.000000 jsonrpc-py-3.0.4/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 08:02:31.054547 jsonrpc-py-3.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:02:31.053547 jsonrpc-py-3.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-25 08:02:08.000000 jsonrpc-py-3.0.4/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.3/.gitlab-ci.yml` & `jsonrpc-py-3.0.4/.gitlab-ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -21,51 +21,49 @@
 before_script:
   - python -VV
   - python -m venv --copies .venv
   - source .venv/bin/activate
 
 code quality:
   stage: testing
-  script:
-    - time make install
-    - time make linting
-    - time make coverage
+  script: make install linting coverage
   coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     name: ${CI_JOB_NAME}-${CI_COMMIT_REF_NAME}-${CI_COMMIT_SHA}
     expire_in: 1 day
     reports:
+      junit: pytest.xml
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
 
 build package:
   stage: building
-  script: time make build
+  script: make build
   artifacts:
     paths:
       - dist
     expire_in: 1 day
   only:
     - tags
 
 deployment:
   stage: publishing
   dependencies:
     - build package
-  script: time make release
+  script: make release
   environment:
     name: PyPI
     url: https://pypi.org/project/jsonrpc-py
   only:
     - tags
 
 pages:
   stage: publishing
-  script: time make docs
+  script: make docs
   environment:
     name: GitLab Pages
     url: https://docs.jsonrpc.ru
   artifacts:
     paths:
       - public
     expire_in: 1 day
```

### Comparing `jsonrpc-py-3.0.3/LICENSE` & `jsonrpc-py-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/Makefile` & `jsonrpc-py-3.0.4/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 flake8: ## Run the flake8 utility
 	@flake8 jsonrpc tests
 
 linting: isort black mypy flake8 ## Lint a whole project
 
 test: ## Run the unit tests
-	@coverage run -m pytest -xv
+	@coverage run -m pytest -xv --junit-xml=pytest.xml
 
 coverage: test ## Report a coverage statistics
 	@coverage report
-	@coverage xml -q
+	@coverage xml -qo coverage.xml
 
 clean: ## Delete all temporary files
 	@find jsonrpc tests -type f -name '*.py[cod]' -delete
 	@find jsonrpc tests -type d -name '__pycache__' -delete
 	@rm -rf *.egg *.egg-info build dist public
```

### Comparing `jsonrpc-py-3.0.3/PKG-INFO` & `jsonrpc-py-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.3
+Version: 3.0.4
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.3/README.md` & `jsonrpc-py-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.4/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.4/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.4/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/changelog.rst` & `jsonrpc-py-3.0.4/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/conf.py` & `jsonrpc-py-3.0.4/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 # A list of strings that are module names of extensions:
 extensions: Final[tuple[str, ...]] = (
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
 )
 
 # Highlighting of the code blocks:
-pygments_style: Final[str] = "stata-light"
+pygments_style: Final[str] = "trac"
 
 # This variable is Furo-specific at this time:
-pygments_dark_style: Final[str] = "stata-dark"
+pygments_dark_style: Final[str] = "monokai"
 
 # Options for HTML Output
 # -----------------------
 
 # The "theme" that the HTML output should use:
 html_theme: Final[str] = "furo"
```

### Comparing `jsonrpc-py-3.0.3/docs/deployment.rst` & `jsonrpc-py-3.0.4/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/index.rst` & `jsonrpc-py-3.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/quickstart.rst` & `jsonrpc-py-3.0.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/docs/reference.rst` & `jsonrpc-py-3.0.4/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/__init__.py` & `jsonrpc-py-3.0.4/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/asgi.py` & `jsonrpc-py-3.0.4/jsonrpc/asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.4/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/errors.py` & `jsonrpc-py-3.0.4/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/request.py` & `jsonrpc-py-3.0.4/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/response.py` & `jsonrpc-py-3.0.4/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/serializer.py` & `jsonrpc-py-3.0.4/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.4/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc/utilities.py` & `jsonrpc-py-3.0.4/jsonrpc/utilities.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.4/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.3
+Version: 3.0.4
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.3/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.4/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 docs/changelog/v2.x.x/v2.5.0.rst
 docs/changelog/v2.x.x/v2.5.1.rst
 docs/changelog/v3.x.x/index.rst
 docs/changelog/v3.x.x/v3.0.0.rst
 docs/changelog/v3.x.x/v3.0.1.rst
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
+docs/changelog/v3.x.x/v3.0.4.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
```

### Comparing `jsonrpc-py-3.0.3/pyproject.toml` & `jsonrpc-py-3.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_asgi.py` & `jsonrpc-py-3.0.4/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_dispatcher.py` & `jsonrpc-py-3.0.4/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_errors.py` & `jsonrpc-py-3.0.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_request.py` & `jsonrpc-py-3.0.4/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_response.py` & `jsonrpc-py-3.0.4/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_serializer.py` & `jsonrpc-py-3.0.4/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.3/tests/test_utilities.py` & `jsonrpc-py-3.0.4/tests/test_utilities.py`

 * *Files identical despite different names*

