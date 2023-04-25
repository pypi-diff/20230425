# Comparing `tmp/govuk-frontend-jinja-2.5.0.tar.gz` & `tmp/govuk-frontend-jinja-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk-frontend-jinja-2.5.0.tar", last modified: Tue Feb 14 14:54:54 2023, max compression
+gzip compressed data, was "govuk-frontend-jinja-2.6.0.tar", last modified: Tue Apr 25 13:15:42 2023, max compression
```

## Comparing `govuk-frontend-jinja-2.5.0.tar` & `govuk-frontend-jinja-2.6.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.908641 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.908641 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.908641 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.908641 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/accordion/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/back-link/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/back-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/breadcrumbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/button/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/button/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/character-count/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/character-count/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/checkboxes/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/cookie-banner/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/date-input/
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/date-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/details/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/details/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/error-message/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/error-message/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/error-summary/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/fieldset/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/file-upload/
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/footer/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/footer/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.912642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/header/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/header/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/hint/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/hint/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/input/
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/inset-text/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/label/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/label/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/notification-banner/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/pagination/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/panel/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/phase-banner/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/radios/
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/select/
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/skip-link/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/summary-list/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/table/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/table/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/tabs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/tag/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/tag/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/textarea/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/textarea/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/warning-text/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.916642 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/macros/i18n.html
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:54:54.908641 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-02-14 14:54:54.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-02-14 14:54:54.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 14:54:54.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-14 14:54:54.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-14 14:54:54.000000 govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-14 14:54:54.920642 govuk-frontend-jinja-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-02-14 14:54:41.000000 govuk-frontend-jinja-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.613981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.613981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/accordion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/back-link/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/back-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/breadcrumbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/button/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/button/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/character-count/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/character-count/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/date-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/date-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/details/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/details/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-message/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-summary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/fieldset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/file-upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/hint/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/hint/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/inset-text/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/label/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/label/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/notification-banner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/panel/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/phase-banner/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/radios/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/skip-link/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/summary-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/table/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tabs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tag/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tag/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/textarea/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/textarea/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/warning-text/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/macros/i18n.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/setup.py
```

### Comparing `govuk-frontend-jinja-2.5.0/LICENSE` & `govuk-frontend-jinja-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/PKG-INFO` & `govuk-frontend-jinja-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-jinja
-Version: 2.5.0
+Version: 2.6.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/LandRegistry/govuk-frontend-jinja
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,29 +21,31 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 4.4.1](https://img.shields.io/badge/govuk--frontend%20version-4.4.1-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/surevine/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
+| [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
 | [1.5.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.5.1) | [3.14.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.14.0) |
 | [1.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.4.0) | [3.13.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.13.0) |
@@ -128,14 +130,16 @@
 9. [GitHub Actions](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-publish.yml) will run on the new tag to build the package and publish it to PyPI. Verify that the package has been updated with the latest release tag by checking [the project page](https://pypi.org/project/govuk-frontend-jinja/)
 
 ## Contributors
 
 - [Matt Shaw](https://github.com/matthew-shaw) (Primary maintainer)
 - [Andy Mantell](https://github.com/andymantell) (Original author)
 
+See the full list of [contributors on GitHub](https://github.com/LandRegistry/govuk-frontend-jinja/graphs/contributors)
+
 ## Support
 
 This software is provided _"as-is"_ without warranty. Support is provided on a _"best endeavours"_ basis by the maintainers and open source community.
 
 If you are a civil servant you can sign up to the [UK Government Digital Slack](https://ukgovernmentdigital.slack.com/signup) workspace to contact the maintainers listed [above](#contributors) and the community of people using this project in the [#govuk-design-system](https://ukgovernmentdigital.slack.com/archives/C6DMEH5R6) channel.
 
 Otherwise, please see the [contribution guidelines](CONTRIBUTING.md) for how to raise a bug report or feature request.
```

### Comparing `govuk-frontend-jinja-2.5.0/README.md` & `govuk-frontend-jinja-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 4.4.1](https://img.shields.io/badge/govuk--frontend%20version-4.4.1-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/surevine/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
+| [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
 | [1.5.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.5.1) | [3.14.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.14.0) |
 | [1.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.4.0) | [3.13.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.13.0) |
@@ -104,14 +106,16 @@
 9. [GitHub Actions](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-publish.yml) will run on the new tag to build the package and publish it to PyPI. Verify that the package has been updated with the latest release tag by checking [the project page](https://pypi.org/project/govuk-frontend-jinja/)
 
 ## Contributors
 
 - [Matt Shaw](https://github.com/matthew-shaw) (Primary maintainer)
 - [Andy Mantell](https://github.com/andymantell) (Original author)
 
+See the full list of [contributors on GitHub](https://github.com/LandRegistry/govuk-frontend-jinja/graphs/contributors)
+
 ## Support
 
 This software is provided _"as-is"_ without warranty. Support is provided on a _"best endeavours"_ basis by the maintainers and open source community.
 
 If you are a civil servant you can sign up to the [UK Government Digital Slack](https://ukgovernmentdigital.slack.com/signup) workspace to contact the maintainers listed [above](#contributors) and the community of people using this project in the [#govuk-design-system](https://ukgovernmentdigital.slack.com/archives/C6DMEH5R6) channel.
 
 Otherwise, please see the [contribution guidelines](CONTRIBUTING.md) for how to raise a bug report or feature request.
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/accordion/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/accordion/macro.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 {% set id = params.id %}
 {% set headingLevel = params.headingLevel if params.headingLevel else 2 %}
 
 <div class="govuk-accordion {%- if params.classes %} {{ params.classes }}{% endif -%}" data-module="govuk-accordion" id="{{ id }}"
   {%- if params.hideAllSectionsText %} data-i18n.hide-all-sections="{{ params.hideAllSectionsText | escape }}"{% endif %}
   {%- if params.hideSectionText %} data-i18n.hide-section="{{ params.hideSectionText | escape }}"{% endif %}
   {%- if params.hideSectionAriaLabelText %} data-i18n.hide-section-aria-label="{{ params.hideSectionAriaLabelText | escape }}"{% endif %}
+  {%- if params.rememberExpanded is not undefined %} data-remember-expanded="{{ params.rememberExpanded | escape | lower }}"{% endif %}
   {%- if params.showAllSectionsText %} data-i18n.show-all-sections="{{ params.showAllSectionsText | escape }}"{% endif %}
   {%- if params.showSectionText %} data-i18n.show-section="{{ params.showSectionText | escape }}"{% endif %}
   {%- if params.showSectionAriaLabelText %} data-i18n.show-section-aria-label="{{ params.showSectionAriaLabelText | escape }}"{% endif %}
   {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor %}>
   {% for item in params['items'] %}
     {% if item %}
       <div class="govuk-accordion__section {%- if item.expanded %} govuk-accordion__section--expanded{% endif %}">
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/button/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/button/macro.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 </svg>
   {% endset %}
   {% set classNames = classNames + " govuk-button--start" %}
 {% endif %}
 
 {#- Define common attributes that we can use across all element types #}
 
-{%- set commonAttributes %} class="{{ classNames }}" data-module="govuk-button"{% for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor %}{% endset %}
+{%- set commonAttributes %} class="{{ classNames }}" data-module="govuk-button"{% for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor %}{% if params.id %} id="{{ params.id }}"{% endif %}{% endset %}
 
 {#- Define common attributes we can use for both button and input types #}
 
 {%- set buttonAttributes %}{% if params.name %} name="{{ params.name }}"{% endif %}{% if params.disabled %} disabled="disabled" aria-disabled="true"{% endif %}{% if params.preventDoubleClick is not undefined %} data-prevent-double-click="{{params.preventDoubleClick | lower}}"{% endif %}{% endset %}
 
 {#- Actually create a button... or a link! #}
```

#### html2text {}

```diff
@@ -9,21 +9,22 @@
 The SVG needs `focusable="false"` so that Internet Explorer does not treat it
 as an interactive element - without this it will be 'focusable' when using the
 keyboard to navigate. #}    {% endset %} {% set classNames = classNames + "
 govuk-button--start" %} {% endif %} {#- Define common attributes that we can
 use across all element types #} {%- set commonAttributes %} class="{
 { classNames }}" data-module="govuk-button"{% for attribute, value in
 (params.attributes.items() if params.attributes else {}.items()) %} {
-{attribute}}="{{value}}"{% endfor %}{% endset %} {#- Define common attributes
-we can use for both button and input types #} {%- set buttonAttributes %}{% if
-params.name %} name="{{ params.name }}"{% endif %}{% if params.disabled %}
-disabled="disabled" aria-disabled="true"{% endif %}{% if
-params.preventDoubleClick is not undefined %} data-prevent-double-click="{
-{params.preventDoubleClick | lower}}"{% endif %}{% endset %} {#- Actually
-create a button... or a link! #} {%- if element == 'a' %}
+{attribute}}="{{value}}"{% endfor %}{% if params.id %} id="{{ params.id }}"{%
+endif %}{% endset %} {#- Define common attributes we can use for both button
+and input types #} {%- set buttonAttributes %}{% if params.name %} name="{
+{ params.name }}"{% endif %}{% if params.disabled %} disabled="disabled" aria-
+disabled="true"{% endif %}{% if params.preventDoubleClick is not undefined %}
+data-prevent-double-click="{{params.preventDoubleClick | lower}}"{% endif %}{%
+endset %} {#- Actually create a button... or a link! #} {%- if element == 'a'
+%}
 {- commonAttributes | safe }}> {{ params.html | safe if params.html else
 params.text }} {# Indentation is intentional to output HTML nicely #} {{-
 iconHtml | safe | trim if iconHtml -}}
  {%- elif element == 'button' %}
 %- if params.value %} value="{{ params.value }}"{% endif %}{%- if params.type
 %} type="{{ params.type }}"{% endif %} {{- buttonAttributes | safe }} {{-
 commonAttributes | safe }}> {{ params.html | safe if params.html else
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/character-count/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/character-count/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/date-input/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/date-input/macro.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% macro govukDateInput(params) %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage -%}
 {% from "govuk_frontend_jinja/components/fieldset/macro.html" import govukFieldset %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/input/macro.html" import govukInput %}
 
 {#- a record of other elements that we need to associate with the input using
-   aria-describedby – for example hints or error messages -#}
+  aria-describedby – for example hints or error messages -#}
 {% set ns = namespace() %}
 {% set ns.describedBy = params.fieldset.describedBy if params.fieldset and params.fieldset.describedBy else "" %}
 
 {% if 'items' in params and params['items'] | length %}
   {% set dateInputItems = params['items'] %}
 {% else %}
   {% set dateInputItems = [
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/details/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/details/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/error-message/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-message/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/error-summary/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-summary/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/fieldset/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/fieldset/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/file-upload/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/file-upload/macro.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% macro govukFileUpload(params) %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage -%}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
-   aria-describedby – for example hints or error messages -#}
+  aria-describedby – for example hints or error messages -#}
 {% set describedBy = params.describedBy if params.describedBy else "" %}
 <div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}">
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
     'isPageHeading': params.label.isPageHeading,
@@ -36,12 +36,13 @@
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim }}
 {% endif %}
   <input class="govuk-file-upload {%- if params.classes %} {{ params.classes }}{% endif %} {%- if params.errorMessage %} govuk-file-upload--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}" type="file"
   {%- if params.value %} value="{{ params.value }}"{% endif %}
+  {%- if params.disabled %} disabled{% endif %}
   {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
   {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor %}>
 </div>
 
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/footer/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/footer/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/header/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/header/macro.html`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             <path
               fill="currentColor" fill-rule="evenodd"
               d="M25 30.2c3.5 1.5 7.7-.2 9.1-3.7 1.5-3.6-.2-7.8-3.9-9.2-3.6-1.4-7.6.3-9.1 3.9-1.4 3.5.3 7.5 3.9 9zM9 39.5c3.6 1.5 7.8-.2 9.2-3.7 1.5-3.6-.2-7.8-3.9-9.1-3.6-1.5-7.6.2-9.1 3.8-1.4 3.5.3 7.5 3.8 9zM4.4 57.2c3.5 1.5 7.7-.2 9.1-3.8 1.5-3.6-.2-7.7-3.9-9.1-3.5-1.5-7.6.3-9.1 3.8-1.4 3.5.3 7.6 3.9 9.1zm38.3-21.4c3.5 1.5 7.7-.2 9.1-3.8 1.5-3.6-.2-7.7-3.9-9.1-3.6-1.5-7.6.3-9.1 3.8-1.3 3.6.4 7.7 3.9 9.1zm64.4-5.6c-3.6 1.5-7.8-.2-9.1-3.7-1.5-3.6.2-7.8 3.8-9.2 3.6-1.4 7.7.3 9.2 3.9 1.3 3.5-.4 7.5-3.9 9zm15.9 9.3c-3.6 1.5-7.7-.2-9.1-3.7-1.5-3.6.2-7.8 3.7-9.1 3.6-1.5 7.7.2 9.2 3.8 1.5 3.5-.3 7.5-3.8 9zm4.7 17.7c-3.6 1.5-7.8-.2-9.2-3.8-1.5-3.6.2-7.7 3.9-9.1 3.6-1.5 7.7.3 9.2 3.8 1.3 3.5-.4 7.6-3.9 9.1zM89.3 35.8c-3.6 1.5-7.8-.2-9.2-3.8-1.4-3.6.2-7.7 3.9-9.1 3.6-1.5 7.7.3 9.2 3.8 1.4 3.6-.3 7.7-3.9 9.1zM69.7 17.7l8.9 4.7V9.3l-8.9 2.8c-.2-.3-.5-.6-.9-.9L72.4 0H59.6l3.5 11.2c-.3.3-.6.5-.9.9l-8.8-2.8v13.1l8.8-4.7c.3.3.6.7.9.9l-5 15.4v.1c-.2.8-.4 1.6-.4 2.4 0 4.1 3.1 7.5 7 8.1h.2c.3 0 .7.1 1 .1.4 0 .7 0 1-.1h.2c4-.6 7.1-4.1 7.1-8.1 0-.8-.1-1.7-.4-2.4V34l-5.1-15.4c.4-.2.7-.6 1-.9zM66 92.8c16.9 0 32.8 1.1 47.1 3.2 4-16.9 8.9-26.7 14-33.5l-9.6-3.4c1 4.9 1.1 7.2 0 10.2-1.5-1.4-3-4.3-4.2-8.7L108.6 76c2.8-2 5-3.2 7.5-3.3-4.4 9.4-10 11.9-13.6 11.2-4.3-.8-6.3-4.6-5.6-7.9 1-4.7 5.7-5.9 8-.5 4.3-8.7-3-11.4-7.6-8.8 7.1-7.2 7.9-13.5 2.1-21.1-8 6.1-8.1 12.3-4.5 20.8-4.7-5.4-12.1-2.5-9.5 6.2 3.4-5.2 7.9-2 7.2 3.1-.6 4.3-6.4 7.8-13.5 7.2-10.3-.9-10.9-8-11.2-13.8 2.5-.5 7.1 1.8 11 7.3L80.2 60c-4.1 4.4-8 5.3-12.3 5.4 1.4-4.4 8-11.6 8-11.6H55.5s6.4 7.2 7.9 11.6c-4.2-.1-8-1-12.3-5.4l1.4 16.4c3.9-5.5 8.5-7.7 10.9-7.3-.3 5.8-.9 12.8-11.1 13.8-7.2.6-12.9-2.9-13.5-7.2-.7-5 3.8-8.3 7.1-3.1 2.7-8.7-4.6-11.6-9.4-6.2 3.7-8.5 3.6-14.7-4.6-20.8-5.8 7.6-5 13.9 2.2 21.1-4.7-2.6-11.9.1-7.7 8.8 2.3-5.5 7.1-4.2 8.1.5.7 3.3-1.3 7.1-5.7 7.9-3.5.7-9-1.8-13.5-11.2 2.5.1 4.7 1.3 7.5 3.3l-4.7-15.4c-1.2 4.4-2.7 7.2-4.3 8.7-1.1-3-.9-5.3 0-10.2l-9.5 3.4c5 6.9 9.9 16.7 14 33.5 14.8-2.1 30.8-3.2 47.7-3.2z"
             ></path>
           </svg>
           <!--<![endif]-->
           <!--[if IE 8]>
-          <img src="{{ params.assetsPath | default('/assets/images') }}/govuk-logotype-crown.png" class="govuk-header__logotype-crown-fallback-image" width="36" height="32">
+          <img src="{{ params.assetsPath | default('/assets/images') }}/govuk-logotype-crown.png" class="govuk-header__logotype-crown-fallback-image" width="36" height="32" alt="">
           <![endif]-->
           <span class="govuk-header__logotype-text">
             GOV.UK
           </span>
         </span>
         {% if (params.productName) %}
         <span class="govuk-header__product-name">
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/input/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/input/macro.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% macro govukInput(params) %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage -%}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
-   aria-describedby – for example hints or error messages -#}
+  aria-describedby – for example hints or error messages -#}
 {% set describedBy = params.describedBy if params.describedBy else "" %}
 <div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}">
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
     'isPageHeading': params.label.isPageHeading,
@@ -46,14 +46,15 @@
       {{- params.prefix.html | safe if params.prefix.html else params.prefix.text -}}
     </div>
   {% endif -%}
 
   <input class="govuk-input {%- if params.classes %} {{ params.classes }}{% endif %} {%- if params.errorMessage %} govuk-input--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}" type="{{ params.type | default('text') }}"
   {%- if (params.spellcheck == false) or (params.spellcheck == true) %} spellcheck="{{ params.spellcheck | lower }}"{% endif %}
   {%- if params.value %} value="{{ params.value}}"{% endif %}
+  {%- if params.disabled %} disabled{% endif %}
   {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
   {%- if params.autocomplete %} autocomplete="{{ params.autocomplete}}"{% endif %}
   {%- if params.pattern %} pattern="{{ params.pattern }}"{% endif %}
   {%- if params.inputmode %} inputmode="{{ params.inputmode }}"{% endif %}
   {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor -%}>
 
   {%- if params.suffix and (params.suffix.text or params.suffix.html) %}
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/label/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/label/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/pagination/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/pagination/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/panel/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/panel/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/radios/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/radios/macro.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% macro govukRadios(params) %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage -%}
 {% from "govuk_frontend_jinja/components/fieldset/macro.html" import govukFieldset %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- If an id 'prefix' is not passed, fall back to using the name attribute
-   instead. We need this for error messages and hints as well -#}
+  instead. We need this for error messages and hints as well -#}
 {% set idPrefix = params.idPrefix if params.idPrefix else params.name %}
 
 {% set ns = namespace() %}
 
 {#- a record of other elements that we need to associate with the input using
-   aria-describedby – for example hints or error messages -#}
+  aria-describedby – for example hints or error messages -#}
 {% set ns.describedBy = params.fieldset.describedBy if params.fieldset and params.fieldset.describedBy else "" %}
 
 {#- Capture the HTML so we can optionally nest it in a fieldset -#}
 {% set innerHtml %}
 {% if params.hint %}
   {% set hintId = idPrefix + '-hint' %}
   {% set ns.describedBy = ns.describedBy + ' ' + hintId if ns.describedBy else hintId %}
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/select/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/select/macro.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% macro govukSelect(params) %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage -%}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
-   aria-describedby – for example hints or error messages -#}
+  aria-describedby – for example hints or error messages -#}
 {% set describedBy = params.describedBy if params.describedBy else "" %}
 <div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}">
 {% if params.label %}
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
@@ -37,15 +37,18 @@
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | indent(2) | trim }}
 {% endif %}
   <select class="govuk-select
-    {%- if params.classes %} {{ params.classes }}{% endif %}{%- if params.errorMessage %} govuk-select--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}" {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %} {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+    {%- if params.classes %} {{ params.classes }}{% endif %}{%- if params.errorMessage %} govuk-select--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}"
+    {%- if params.disabled %} disabled{% endif %}
+    {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
+    {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
     {% if 'items' in params and params['items'] | length %}
       {% for item in params['items'] %}
         {% if item %}
           <option value="{{ item.value }}"
             {{-" selected" if item.selected | default(params.value and item.value == params.value) }}
             {{-" disabled" if item.disabled }}
             {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor -%}>{{ item.text }}</option>
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/summary-list/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/summary-list/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/table/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/table/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/tabs/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tabs/macro.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% macro govukTabs(params) %}
 {#- If an id 'prefix' is not passed, fall back to using the name attribute
-   instead. We need this for error messages and hints as well -#}
+  instead. We need this for error messages and hints as well -#}
 {% set idPrefix = params.idPrefix if params.idPrefix -%}
 
 <div {%- if params.id %} id="{{params.id}}"{% endif %} class="govuk-tabs {%- if params.classes %} {{ params.classes }}{% endif %}" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor %} data-module="govuk-tabs">
   <h2 class="govuk-tabs__title">
     {{ params.title | default ("Contents") }}
   </h2>
   {% if 'items' in params and params['items'] | length %}
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/textarea/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/textarea/macro.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% macro govukTextarea(params) %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage -%}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
-   aria-describedby – for example hints or error messages -#}
+  aria-describedby – for example hints or error messages -#}
 {% set describedBy = params.describedBy if params.describedBy else "" %}
 <div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}">
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
     'isPageHeading': params.label.isPageHeading,
@@ -36,13 +36,14 @@
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim }}
 {% endif %}
   <textarea class="govuk-textarea {{- ' govuk-textarea--error' if params.errorMessage else '' }} {{- ' ' + params.classes if params.classes else ''}}" id="{{ params.id }}" name="{{ params.name }}" rows="{%if params.rows %} {{- params.rows -}} {% else %}5{%endif %}"
   {%- if (params.spellcheck == false) or (params.spellcheck == true) %} spellcheck="{{ params.spellcheck | lower }}"{% endif %}
+  {%- if params.disabled %} disabled{% endif %}
   {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
   {%- if params.autocomplete %} autocomplete="{{ params.autocomplete}}"{% endif %}
   {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor %}>{{ params.value }}</textarea>
 </div>
 
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/components/warning-text/macro.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/warning-text/macro.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% macro govukWarningText(params) %}
   <div class="govuk-warning-text {{- ' ' + params.classes if params.classes else ''}}"
   {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{attribute}}="{{value}}"{% endfor -%}
   >
   <span class="govuk-warning-text__icon" aria-hidden="true">!</span>
   <strong class="govuk-warning-text__text">
-    <span class="govuk-warning-text__assistive">{{ params.iconFallbackText }}</span>
+    <span class="govuk-warning-text__assistive">{{ params.iconFallbackText | default("Warning") }}</span>
     {{ params.html | safe if params.html else params.text }}
   </strong>
 </div>
 
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/macros/i18n.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/macros/i18n.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja/templates/template.html` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/template.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/PKG-INFO` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-jinja
-Version: 2.5.0
+Version: 2.6.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/LandRegistry/govuk-frontend-jinja
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,29 +21,31 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 4.4.1](https://img.shields.io/badge/govuk--frontend%20version-4.4.1-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/surevine/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
+| [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
 | [1.5.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.5.1) | [3.14.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.14.0) |
 | [1.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.4.0) | [3.13.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.13.0) |
@@ -128,14 +130,16 @@
 9. [GitHub Actions](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-publish.yml) will run on the new tag to build the package and publish it to PyPI. Verify that the package has been updated with the latest release tag by checking [the project page](https://pypi.org/project/govuk-frontend-jinja/)
 
 ## Contributors
 
 - [Matt Shaw](https://github.com/matthew-shaw) (Primary maintainer)
 - [Andy Mantell](https://github.com/andymantell) (Original author)
 
+See the full list of [contributors on GitHub](https://github.com/LandRegistry/govuk-frontend-jinja/graphs/contributors)
+
 ## Support
 
 This software is provided _"as-is"_ without warranty. Support is provided on a _"best endeavours"_ basis by the maintainers and open source community.
 
 If you are a civil servant you can sign up to the [UK Government Digital Slack](https://ukgovernmentdigital.slack.com/signup) workspace to contact the maintainers listed [above](#contributors) and the community of people using this project in the [#govuk-design-system](https://ukgovernmentdigital.slack.com/archives/C6DMEH5R6) channel.
 
 Otherwise, please see the [contribution guidelines](CONTRIBUTING.md) for how to raise a bug report or feature request.
```

### Comparing `govuk-frontend-jinja-2.5.0/govuk_frontend_jinja.egg-info/SOURCES.txt` & `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.5.0/setup.py` & `govuk-frontend-jinja-2.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 components = []
 directories = glob.glob("govuk_frontend_jinja/**/**/*.html", recursive=True)
 for directory in directories:
     components.append(os.path.relpath(os.path.dirname(directory), "govuk_frontend_jinja") + "/*.html")
 
 setuptools.setup(
     name="govuk-frontend-jinja",
-    version="2.5.0",
+    version="2.6.0",
     author="Matt Shaw",
     author_email="matthew.shaw@landregistry.gov.uk",
     description="GOV.UK Frontend Jinja Macros",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LandRegistry/govuk-frontend-jinja",
     packages=setuptools.find_packages(exclude=["tests"]),
```

