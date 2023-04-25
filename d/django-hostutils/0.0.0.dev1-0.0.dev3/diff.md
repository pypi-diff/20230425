# Comparing `tmp/django-hostutils-0.0.0.dev1.tar.gz` & `tmp/django-hostutils-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hostutils-0.0.0.dev1.tar", last modified: Thu Apr 20 05:38:20 2023, max compression
+gzip compressed data, was "django-hostutils-0.0.dev3.tar", last modified: Tue Apr 25 00:40:22 2023, max compression
```

## Comparing `django-hostutils-0.0.0.dev1.tar` & `django-hostutils-0.0.dev3.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/.github/workflows/bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/django_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   133744 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/cpu.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/cpu.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/disk.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/host.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/memory.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/network.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/_static/process.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/images/cpu.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/images/disk.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/images/host.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/images/memory.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/images/network.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/images/process.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/internals.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/docs/source/version_history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-20 05:38:20.000000 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-20 05:38:20.000000 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:38:20.000000 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 05:38:20.000000 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 05:38:20.000000 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:38:20.000000 django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.918427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/ajax.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/htmx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.914427 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/core/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:20.922427 django-hostutils-0.0.0.dev1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/unit/test_ajax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/unit/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-20 05:38:06.000000 django-hostutils-0.0.0.dev1/tests/unit/test_htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   133744 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/version_history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_htmx.py
```

### Comparing `django-hostutils-0.0.0.dev1/.github/workflows/python-publish.yml` & `django-hostutils-0.0.dev3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/.gitignore` & `django-hostutils-0.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/LICENSE` & `django-hostutils-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/PKG-INFO` & `django-hostutils-0.0.dev3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hostutils
-Version: 0.0.0.dev1
+Version: 0.0.dev3
 Summary: host utilities for django projects
 Home-page: https://github.com/davidslusser/django-hostutils
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: any
 Description-Content-Type: text/markdown
@@ -32,16 +32,17 @@
 <br/>
 
 ## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
+|Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
-
+|Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
 ## License
 django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
```

### Comparing `django-hostutils-0.0.0.dev1/README.md` & `django-hostutils-0.0.dev3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 <br/>
 
 ## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
+|Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
-
+|Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
 ## License
 django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
```

### Comparing `django-hostutils-0.0.0.dev1/docs/Makefile` & `django-hostutils-0.0.dev3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/make.bat` & `django-hostutils-0.0.dev3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/cpu.PNG` & `django-hostutils-0.0.dev3/docs/source/_static/cpu.PNG`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/cpu.jpg` & `django-hostutils-0.0.dev3/docs/source/_static/cpu.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/disk.jpg` & `django-hostutils-0.0.dev3/docs/source/_static/disk.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/host.jpg` & `django-hostutils-0.0.dev3/docs/source/_static/host.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/memory.jpg` & `django-hostutils-0.0.dev3/docs/source/_static/memory.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/network.jpg` & `django-hostutils-0.0.dev3/docs/source/_static/network.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/_static/process.jpg` & `django-hostutils-0.0.dev3/docs/source/_static/process.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/about.rst` & `django-hostutils-0.0.dev3/docs/source/about.rst`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/conf.py` & `django-hostutils-0.0.dev3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/features.rst` & `django-hostutils-0.0.dev3/docs/source/features.rst`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/images/cpu.jpg` & `django-hostutils-0.0.dev3/docs/source/images/cpu.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/images/disk.jpg` & `django-hostutils-0.0.dev3/docs/source/images/disk.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/images/host.jpg` & `django-hostutils-0.0.dev3/docs/source/images/host.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/images/memory.jpg` & `django-hostutils-0.0.dev3/docs/source/images/memory.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/images/network.jpg` & `django-hostutils-0.0.dev3/docs/source/images/network.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/images/process.jpg` & `django-hostutils-0.0.dev3/docs/source/images/process.jpg`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/index.rst` & `django-hostutils-0.0.dev3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/docs/source/installation.rst` & `django-hostutils-0.0.dev3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/setup.cfg` & `django-hostutils-0.0.dev3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,21 @@
 
 [options.extras_require]
 dev = 
 	bandit
 	black
 	build
 	mypy
+	mypy-extensions
 	pylint
 	pytest
 	pytest-cov
 	pytest-django
+	types-python-dateutil
+	typing_extensions
 
 [options.packages.find]
 where = src
 exclude = 
 	__pycache__
 	*.pyc
 	test
```

### Comparing `django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/PKG-INFO` & `django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hostutils
-Version: 0.0.0.dev1
+Version: 0.0.dev3
 Summary: host utilities for django projects
 Home-page: https://github.com/davidslusser/django-hostutils
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: any
 Description-Content-Type: text/markdown
@@ -32,16 +32,17 @@
 <br/>
 
 ## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
+|Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
-
+|Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
 ## License
 django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
```

### Comparing `django-hostutils-0.0.0.dev1/src/django_hostutils.egg-info/SOURCES.txt` & `django-hostutils-0.0.dev3/src/django_hostutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/bandit.yaml
 .github/workflows/black.yaml
+.github/workflows/mypy.yaml
 .github/workflows/pylint.yaml
 .github/workflows/pytest.yaml
 .github/workflows/python-publish.yml
 docs/Makefile
 docs/django_settings.py
 docs/make.bat
 docs/source/about.rst
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/forms.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %}
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
         .card .card-header {
@@ -25,15 +25,14 @@
             flex-wrap: wrap;
         }
         .titlecard-container > * {
             flex: 1;
         }
         .titlecard {
             height: 8rem;
-            background-color: var(--light);
         }
         .titlecard .stat {
             color: var(--primary);
             font-size: 2.5rem;
             font-weight: bold;
             text-align: center;
             margin-top: -.75rem;
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %} {%
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
 load static %} {% load handyhelper_tags %} {% block local_head %} {% include
 'handyhelpers/component/chartjs_components.htm' %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{ physical_count }}
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %}
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     <style>
         .titlecard-container {
             display: flex;
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %} {%
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
 load static %} {% load handyhelper_tags %} {% block local_head %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{_cpu_count_}}
 CPU_Count
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %}
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
         .card .card-header {
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %} {%
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
 load static %} {% load handyhelper_tags %} {% block local_head %} {% include
 'handyhelpers/component/chartjs_components.htm' %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{ io_counters.read_count|byte_size }}
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %}
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
         .card .card-header {
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %} {%
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
 load static %} {% load handyhelper_tags %} {% block local_head %} {% include
 'handyhelpers/component/chartjs_components.htm' %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{virtual.total|byte_size}}
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %}
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     <style>
         .card .card-header {
             color: var(--primary);
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %} {%
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
 load static %} {% load handyhelper_tags %} {% block local_head %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{ counters.bytes_sent|byte_size }}
 Bytes Sent
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %}
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     <style>
         .card .card-header {
             color: var(--primary);
@@ -73,55 +73,55 @@
     {% endif %}
 </section>
 
 <section class="mb-5 animated fadeIn" style="animation-delay: .25s;">
     <div id="id_title_card_wrapper" class="container-fluid mt-5">
         <div class="titlecard-container">
             <div class="card titlecard shadow hvr-grow"
-                 hx-get="{% url 'hostutils:get_process_stats' %}?source=card&status=running" hx-target='#id_process_list_container'
+                 hx-get="{% url 'hostutils:get_host_processes' %}?source=card&status=running" hx-target='#id_process_list_container'
                  onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                 <div class="card-body">
                     <div class="stat">{{ counts.running }}</div>
                     <div class="description">Running</div>
                 </div>
             </div>
             <div class="card titlecard shadow hvr-grow"
-                 hx-get="{% url 'hostutils:get_process_stats' %}?source=card&status=idle" hx-target='#id_process_list_container'
+                 hx-get="{% url 'hostutils:get_host_processes' %}?source=card&status=idle" hx-target='#id_process_list_container'
                  onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                 <div class="card-body">
                     <div class="stat">{{ counts.idle }}</div>
                     <div class="description">Idle</div>
                 </div>
             </div>
             <div class="card titlecard shadow hvr-grow"
-                 hx-get="{% url 'hostutils:get_process_stats' %}?source=card&status=sleeping" hx-target='#id_process_list_container'
+                 hx-get="{% url 'hostutils:get_host_processes' %}?source=card&status=sleeping" hx-target='#id_process_list_container'
                  onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                 <div class="card-body">
                     <div class="stat">{{ counts.sleeping }}</div>
                     <div class="description">Sleeping</div>
                 </div>
             </div>
             <div class="card titlecard shadow hvr-grow"
-                 hx-get="{% url 'hostutils:get_process_stats' %}?source=card&status=stopped" hx-target='#id_process_list_container'
+                 hx-get="{% url 'hostutils:get_host_processes' %}?source=card&status=stopped" hx-target='#id_process_list_container'
                  onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                 <div class="card-body">
                     <div class="stat">{{ counts.stopped }}</div>
                     <div class="description">Stopped</div>
                 </div>
             </div>
             <div class="card titlecard shadow hvr-grow"
-                 hx-get="{% url 'hostutils:get_process_stats' %}?source=card&status=zombie" hx-target='#id_process_list_container'
+                 hx-get="{% url 'hostutils:get_host_processes' %}?source=card&status=zombie" hx-target='#id_process_list_container'
                  onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                 <div class="card-body">
                     <div class="stat">{{ counts.zombie }}</div>
                     <div class="description">Zombie</div>
                 </div>
             </div>
             <div class="card titlecard shadow hvr-grow"
-                 hx-get="{% url 'hostutils:get_process_stats' %}?source=card&status=dead" hx-target='#id_process_list_container'
+                 hx-get="{% url 'hostutils:get_host_processes' %}?source=card&status=dead" hx-target='#id_process_list_container'
                  onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                 <div class="card-body">
                     <div class="stat">{{ counts.dead }}</div>
                     <div class="description">Dead</div>
                 </div>
             </div>
         </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends base_template|default:"handyhelpers/handyhelpers_base.htm" %} {%
+{% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
 load static %} {% load handyhelper_tags %} {% block local_head %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% include 'hostutils/bs5/snippets/processes_results_timestamp.htm' %}
 {% endif %}
 {{ counts.running }}
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/urls.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     path("host_memory/", gui.ShowHostMemory.as_view(), name="host_memory"),
     path("host_network/", gui.ShowHostNetwork.as_view(), name="host_network"),
     path("host_process/", gui.ShowHostProcesses.as_view(), name="host_process"),
     # ajax views
     path("get_cpu_stats/", ajax.GetHostCpuStats.as_view(), name="get_cpu_stats"),
     path("get_interface_stats/", ajax.GetHostNetworkStats.as_view(), name="get_interface_stats"),
     path("get_partition_stats/", ajax.GetHostParitionStats.as_view(), name="get_partition_stats"),
-    path("get_process_stats/", ajax.GetHostProcessStats.as_view(), name="get_process_stats"),   
+    path("get_process_stats/", ajax.GetHostProcessStats.as_view(), name="get_process_stats"),
     # htmx views
     path("get_host_processes/", htmx.GetHostProcesses.as_view(), name="get_host_processes"),
 ]
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/__init__.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/ajax.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 import psutil
 
 from django.http import HttpResponse
 from django.template import loader
 
 from handyhelpers.views.ajax import AjaxGetView
+from typing import Union
 
 
 class GetHostCpuStats(AjaxGetView):
     """
     Description:
         Get CPU status for a given cpu on the host machine.
     Args:
         request: AJAX request object.
     Returns:
         HttpResponse: JSON formatted response.
     """
 
     template = loader.get_template("hostutils/bs5/ajax/get_cpu_stats.htm")
 
-    def get(self, request, *args, **kwargs):
+    def get(self, request, *args, **kwargs) -> HttpResponse:
         try:
             cpu = int(request.GET["client_response"])
             self.data = {
                 "time": psutil.cpu_times(percpu=True)[cpu],
                 "time_percent": psutil.cpu_times_percent(percpu=True)[cpu],
                 "frequency": psutil.cpu_freq(percpu=True)[cpu],
             }
             return super().get(request, *args, **kwargs)
-        except Exception as err:
-            return HttpResponse('Invalid request inputs', status=400)
+        except Exception:
+            return HttpResponse("Invalid request inputs", status=400)
 
 
 class GetHostNetworkStats(AjaxGetView):
     """
     Description:
         Get network statistics for a given network interface on the host machine.
     Args:
         request: AJAX request object.
     Returns:
         HttpResponse: JSON formatted response.
     """
 
     template = loader.get_template("hostutils/bs5/ajax/get_interface_stats.htm")
 
-    def get(self, request, *args, **kwargs):
+    def get(self, request, *args, **kwargs) -> HttpResponse:
         try:
             interface = self.request.GET["client_response"]
             self.data = psutil.net_if_stats()[interface]
             return super().get(request, *args, **kwargs)
-        except Exception as err:
-            return HttpResponse('Invalid request inputs', status=400)
+        except Exception:
+            return HttpResponse("Invalid request inputs", status=400)
 
 
 class GetHostParitionStats(AjaxGetView):
     """
     Description:
         Get disk usage for a given partition on the host machine.
     Args:
         request: AJAX request object.
     Returns:
         HttpResponse: JSON formatted response.
     """
 
     template = loader.get_template("hostutils/bs5/ajax/get_partition_stats.htm")
 
-    def get(self, request, *args, **kwargs):
+    def get(self, request, *args, **kwargs) -> HttpResponse:
         try:
             part = request.GET["client_response"]
             self.data = psutil.disk_usage(part)
             return super().get(request, *args, **kwargs)
-        except Exception as err:
-            return HttpResponse('Invalid request inputs', status=400)
+        except Exception:
+            return HttpResponse("Invalid request inputs", status=400)
 
 
 class GetHostProcessStats(AjaxGetView):
     """
     Description:
         Get process details for a given process on the host machine.
     Args:
         request: AJAX request object.
     Returns:
         HttpResponse: JSON formatted response.
     """
 
     template = loader.get_template("hostutils/bs5/ajax/get_process_stats.htm")
 
-    def get(self, request, *args, **kwargs):
+    def get(self, request, *args, **kwargs) -> HttpResponse:
+        self.data: Union[dict, psutil.Process] 
         try:
             proc = request.GET["client_response"]
             self.data = psutil.Process(int(proc))
-        except Exception as err:
-            return HttpResponse('Invalid request inputs', status=400)
         except psutil.AccessDenied:
             self.data = {}
+        except Exception:
+            return HttpResponse("Invalid request inputs", status=400)
         return super().get(request, *args, **kwargs)
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/gui.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/hostutils/views/htmx.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 from django.views.generic import View
 
 # import forms
 from djangoaddicts.hostutils.forms import HostProcessFilterForm
 
 
 class GetHostProcesses(View):
-    
     @staticmethod
-    def get_process_count(process_list: list , status: str) -> int:
+    def get_process_count(process_list: list, status: str) -> int:
         """get a count of processes for a given status
 
         Args:
             process_list (list): list of processes as returned from psutil.process_iter(
             status (str): name of process status to count
 
         Returns:
             int: number of processes of 'status'
         """
         count = 0
         for process in process_list:
             try:
                 if process.status() == status:
-                    count +=1 
+                    count += 1
             except psutil.NoSuchProcess:
                 continue
         return count
-    
+
     def get(self, request):
         """Get host prcesses"""
         context = {}
         process_list = list(psutil.process_iter())
         filter_form = HostProcessFilterForm(request.GET or None)
         context["counts"] = {
             "running": self.get_process_count(process_list, "running"),
@@ -45,15 +44,15 @@
 
         if request.GET.dict().get("clear", None):
             context["clear_filter"] = False
 
         else:
             if filter_form.is_valid():
                 context["clear_filter"] = True
-                
+
                 if filter_form.cleaned_data.get("status", None):
                     filtered_process_list = []
                     for i in process_list:
                         if i.status() in filter_form.cleaned_data["status"]:
                             filtered_process_list.append(i)
                     process_list = filtered_process_list
```

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/tests/core/settings.py` & `django-hostutils-0.0.dev3/tests/core/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # INSTALLED_APPS with these apps is necessary for Sphinx to build
 # without warnings & errors
 # Depending on your package, the list of apps may be different
 INSTALLED_APPS = [
     "django.contrib.auth",
     "django.contrib.contenttypes",
-    "auditlog",
     "handyhelpers",
     "djangoaddicts.hostutils",
 ]
 
 ROOT_URLCONF = "tests.core.urls"
 
 DATABASES = {
```

### Comparing `django-hostutils-0.0.0.dev1/tests/unit/test_ajax.py` & `django-hostutils-0.0.dev3/tests/unit/test_ajax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import psutil
+
 from django.test import TestCase
 from django.shortcuts import reverse
 
+from unittest.mock import patch
+
 
 class GetHostCpuStatsTests(TestCase):
     """test GetHostCpuStats ajax view"""
     def setUp(self):
         super(GetHostCpuStatsTests, self).setUp()
         self.url = reverse("hostutils:get_cpu_stats")
         self.headers = dict(HTTP_X_REQUESTED_WITH="XMLHttpRequest")
@@ -73,14 +77,22 @@
         self.headers = dict(HTTP_X_REQUESTED_WITH="XMLHttpRequest")
 
     def test_get(self):
         response = self.client.get(self.url, data={"client_response": "1"}, **self.headers)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, "hostutils/bs5/ajax/get_process_stats.htm")
 
+    def test_access_denied(self):
+        with patch("psutil.Process") as mocked_process:
+            mocked_process.side_effect = psutil.AccessDenied
+            response = self.client.get(self.url, data={"client_response": "838"}, **self.headers)
+            self.assertEqual(response.status_code, 200)
+            self.assertTemplateUsed(response, "hostutils/bs5/ajax/get_process_stats.htm")
+            self.assertIn("data not available for this process", response.content.decode("utf8"))
+
     def test_get_with_invalid_data(self):
         response = self.client.get(self.url, data={"blah": 0}, **self.headers)
         self.assertEqual(response.status_code, 400)
 
     def test_get_with_invalid_request(self):
         response = self.client.get(self.url, data={"client_response": "999"})
         self.assertEqual(response.status_code, 400)
```

### Comparing `django-hostutils-0.0.0.dev1/tests/unit/test_gui.py` & `django-hostutils-0.0.dev3/tests/unit/test_gui.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.0.dev1/tests/unit/test_htmx.py` & `django-hostutils-0.0.dev3/tests/unit/test_htmx.py`

 * *Files identical despite different names*

