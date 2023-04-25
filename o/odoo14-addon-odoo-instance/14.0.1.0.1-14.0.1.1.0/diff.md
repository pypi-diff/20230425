# Comparing `tmp/odoo14-addon-odoo_instance-14.0.1.0.1.tar.gz` & `tmp/odoo14-addon-odoo_instance-14.0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.0.1.tar", last modified: Tue Apr 25 00:20:29 2023, max compression
+gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.1.0.tar", last modified: Tue Apr 25 10:26:32 2023, max compression
```

## Comparing `odoo14-addon-odoo_instance-14.0.1.0.1.tar` & `odoo14-addon-odoo_instance-14.0.1.1.0.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3777 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.526388 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.529722 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3365 2023-04-24 23:44:11.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/README.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1185 2023-04-24 23:39:21.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/calendar_tags.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/ir_cron.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo_version_data.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      246 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/calendar_event.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      488 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/import_requirements_wizard.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19284 2023-04-25 00:12:04.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2469 2023-04-24 23:30:49.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_module.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1377 2023-04-24 22:28:12.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_process.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1790 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_window.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      184 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_version.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      474 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/process_module_rel.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/project_project.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/res_partner.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      385 2023-04-24 23:44:06.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/HISTORY.rst
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/newsfragments/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1555 2023-04-24 22:12:05.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/ir.model.access.csv
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/security_groups.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.529722 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    12978 2023-04-24 23:44:12.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/index.html
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.529722 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/css/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/css/project_instance.css
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/img/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/img/icon.png
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/js/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/js/project_instance.js
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/tests/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/tests/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/tests/test_project_instance.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3034 2023-04-24 22:37:43.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1614 2023-04-25 00:16:27.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3947 2023-04-24 23:30:35.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    18726 2023-04-24 23:58:22.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3029 2023-04-25 00:00:05.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_module_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1674 2023-04-24 23:58:59.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_process_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      896 2023-04-24 20:11:02.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_version_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/project_project_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/res_partner_view.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2309 2023-04-24 23:39:11.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3777 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2666 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-24 23:39:06.000000 odoo14-addon-odoo_instance-14.0.1.0.1/setup.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3865 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/PKG-INFO
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.219030 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.219030 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3453 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/README.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1277 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/__manifest__.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/calendar_tags.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/ir_cron.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo_version_data.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      273 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/calendar_event.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      488 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/import_requirements_wizard.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    21016 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2469 2023-04-24 23:30:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_module.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1377 2023-04-24 22:28:12.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_process.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1790 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_window.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      456 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_release.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      282 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_version.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      474 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/process_module_rel.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/project_project.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/res_partner.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      473 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/HISTORY.rst
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/newsfragments/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1654 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/ir.model.access.csv
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/security_groups.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    13269 2023-04-25 10:24:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/index.html
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.222364 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/css/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/css/project_instance.css
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/img/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/img/icon.png
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/js/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/js/project_instance.js
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/tests/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/tests/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/tests/test_project_instance.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3034 2023-04-24 22:37:43.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1964 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4622 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19080 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3029 2023-04-25 00:00:05.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_module_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1674 2023-04-24 23:58:59.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_process_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2254 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_release_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1113 2023-04-25 10:24:49.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_version_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/project_project_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/res_partner_view.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2309 2023-04-24 23:39:11.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3865 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2769 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/not-zip-safe
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       50 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/requires.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-25 10:26:32.000000 odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/top_level.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-25 10:26:32.225697 odoo14-addon-odoo_instance-14.0.1.1.0/setup.cfg
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-25 08:47:29.000000 odoo14-addon-odoo_instance-14.0.1.1.0/setup.py
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo_instance
-Version: 14.0.1.0.1
+Version: 14.0.1.1.0
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -50,14 +50,22 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.1.0 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Handle odoo releases
+
+
 14.0.1.0.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Improved UX: Searches, filters, grouping...
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/README.rst` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,22 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.1.0 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Handle odoo releases
+
+
 14.0.1.0.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Improved UX: Searches, filters, grouping...
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/__manifest__.py` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/__manifest__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 {
     'name': 'Odoo Instance',
-    'version': '14.0.1.0.1',
+    'version': '14.0.1.1.0',
     'category': 'Project',
     'summary': 'Manage Odoo instances with relevant information',
     'author': 'Coopdevs',
     'website': 'https://www.coopdevs.org',
     'depends': ['base', 'contract', 'project', 'calendar'],
     'data': [
         'security/security_groups.xml',
         'security/ir.model.access.csv',
         'views/odoo_instance_view.xml',        
         'views/odoo_module_view.xml',
         'views/odoo_instance_window_wizard_view.xml',
         'views/odoo_version_view.xml',
         'views/odoo_process_view.xml',
+        'views/odoo_release_view.xml',
         'views/res_partner_view.xml',
         'views/project_project_view.xml',
         'views/odoo_instance_actions.xml',
         'views/odoo_instance_menuitems.xml',
         'views/odoo_instance_searches.xml',
         'data/ir_cron.xml',
         'data/calendar_tags.xml',
         'data/odoo_version_data.xml',
         'data/odoo14_core_modules_app_data.xml',
         'data/odoo12_core_modules_data.xml',
     ],
-    # set icon
+    'external_dependencies': {
+        'python': ['pyyaml'],
+    },
     'images': ['static/src/img/icon.png'],
     'demo': [],
     'installable': True,
     'application': True,
     'auto_install': False,
     'license': 'AGPL-3',
 }
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo_version_data.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/data/odoo_version_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance.py` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime, time, timedelta
 from odoo import api, fields, models
 from odoo.exceptions import UserError
 import requests
 import logging
+import yaml
 import pytz
 import re
 _logger = logging.getLogger(__name__)
 
 
 class OdooInstance(models.Model):
     _name = 'odoo.instance'
@@ -39,14 +40,16 @@
         ('paused', 'Paused'),
         ('cancelled', 'Terminated')
     ], string='State', default='in_progress')
 
     # Technical Information
     
     inventory_url = fields.Char(string='Inventory URL')
+    branch = fields.Char(string='Branch', required=True)
+    odoo_release_id = fields.Many2one('odoo.release', string='Odoo Release')
     instance_type = fields.Selection([
         ('test', 'Test'),
         ('production', 'Production'),
     ], string="Instance Type", required=True)
 
     deploy_schedule = fields.One2many(
         'odoo.instance.schedule', 'instance_id', string="Deploy Schedule")
@@ -378,15 +381,44 @@
             if not self.instance_url:
                 raise UserError(("No hay URL para esta instancia."))
             return {
                 'type': 'ir.actions.act_url',
                 'url': self.instance_url,
                 'target': 'new',
             }
+    def update_odoo_release(self):
+            for instance in self:
+                inventory_url = instance.inventory_url
+                branch = instance.branch
+                raw_inventory_url = f"{inventory_url}/-/raw/{branch}/inventory/group_vars/all.yml"
+                response = requests.get(raw_inventory_url)
+
+                if response.status_code == 200:
+                    inventory_data = yaml.safe_load(response.text)
+                    odoo_release_str = inventory_data.get('odoo_role_odoo_release')
+
+                    if odoo_release_str:
+                        odoo_version, release_date_str = odoo_release_str.split('_')
+                        release_date = fields.Date.from_string(release_date_str)
+
+                        odoo_version_id = self.env['odoo.version'].search([('name', '=', odoo_version)], limit=1)
+                        if odoo_version_id:
+                            odoo_release = self.env['odoo.release'].search([
+                                ('name', '=', odoo_release_str),
+                                ('odoo_version_id', '=', odoo_version_id.id)
+                            ], limit=1)
+
+                            if not odoo_release:
+                                odoo_release = self.env['odoo.release'].create({
+                                    'name': odoo_release_str,
+                                    'release_date': release_date,
+                                    'odoo_version_id': odoo_version_id.id,
+                                })
 
+                            instance.odoo_release_id = odoo_release
 
 class OdooInstanceSchedule(models.Model):
     _name = 'odoo.instance.schedule'
     _description = 'Deploy Schedule'
 
     instance_id = fields.Many2one('odoo.instance', string="Instance")
     day_of_week = fields.Selection([
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_module.py` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_module.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_process.py` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_process.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_window.py` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/models/odoo_instance_window.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/ir.model.access.csv` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/security/ir.model.access.csv`

 * *Files 8% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 access_odoo_instance_schedule,odoo.instance.schedule,model_odoo_instance_schedule,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_unavailabe_schedule,odoo.instance.unavailable_schedule,model_odoo_instance_unavailable_schedule,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_functional_requirement,odoo.instance.functional.requirement,model_odoo_instance_functional_requirement,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window,odoo.instance.window,model_odoo_instance_window,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window_wizard,odoo.instance.window.wizard,model_odoo_instance_window_wizard,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_troubleshooting,odoo.instance.troubleshooting,model_odoo_instance_troubleshooting,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_version,odoo.version,model_odoo_version,odoo_instance.group_odoo_instance_user,1,1,0,0
+access_odoo_release,odoo.release,model_odoo_release,odoo_instance.group_odoo_instance_user,1,1,1,1
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/index.html`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/description/index.html`

```diff
@@ -394,117 +394,131 @@
       </blockquote>
       <p>
         <strong>Table of contents</strong>
       </p>
       <div class="contents local topic" id="contents">
         <ul class="simple">
           <li>
-            <a class="reference internal" href="#changelog" id="id4">Changelog</a>
+            <a class="reference internal" href="#changelog" id="id5">Changelog</a>
             <ul>
               <li>
-                <a class="reference internal" href="#id1" id="id5">14.0.1.0.1 (2023-04-25)</a>
+                <a class="reference internal" href="#id1" id="id6">14.0.1.1.0 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id2" id="id6">14.0.1.0.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id2" id="id7">14.0.1.0.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id3" id="id7">14.0.0.2.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id3" id="id8">14.0.1.0.0 (2023-04-24)</a>
+              </li>
+              <li>
+                <a class="reference internal" href="#id4" id="id9">14.0.0.2.0 (2023-04-24)</a>
               </li>
             </ul>
           </li>
           <li>
-            <a class="reference internal" href="#bug-tracker" id="id8">Bug Tracker</a>
+            <a class="reference internal" href="#bug-tracker" id="id10">Bug Tracker</a>
           </li>
           <li>
-            <a class="reference internal" href="#credits" id="id9">Credits</a>
+            <a class="reference internal" href="#credits" id="id11">Credits</a>
             <ul>
               <li>
-                <a class="reference internal" href="#authors" id="id10">Authors</a>
+                <a class="reference internal" href="#authors" id="id12">Authors</a>
               </li>
               <li>
-                <a class="reference internal" href="#maintainers" id="id11">Maintainers</a>
+                <a class="reference internal" href="#maintainers" id="id13">Maintainers</a>
               </li>
             </ul>
           </li>
         </ul>
       </div>
       <div class="section" id="changelog">
         <h1>
-          <a class="toc-backref" href="#id4">Changelog</a>
+          <a class="toc-backref" href="#id5">Changelog</a>
         </h1>
         <div class="section" id="id1">
           <h2>
-            <a class="toc-backref" href="#id5">14.0.1.0.1 (2023-04-25)</a>
+            <a class="toc-backref" href="#id6">14.0.1.1.0 (2023-04-25)</a>
+          </h2>
+          <p>
+            <strong>Features</strong>
+          </p>
+          <ul class="simple">
+            <li>Handle odoo releases</li>
+          </ul>
+        </div>
+        <div class="section" id="id2">
+          <h2>
+            <a class="toc-backref" href="#id7">14.0.1.0.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Improved UX: Searches, filters, grouping…</li>
           </ul>
           <p>
             <strong>Bugfixes</strong>
           </p>
           <ul class="simple">
             <li>Removed forgotten debug statementes</li>
           </ul>
         </div>
-        <div class="section" id="id2">
+        <div class="section" id="id3">
           <h2>
-            <a class="toc-backref" href="#id6">14.0.1.0.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id8">14.0.1.0.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Rename models and split logic in files</li>
           </ul>
         </div>
-        <div class="section" id="id3">
+        <div class="section" id="id4">
           <h2>
-            <a class="toc-backref" href="#id7">14.0.0.2.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id9">14.0.0.2.0 (2023-04-24)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
             <li>Add instance relations to project and res.partner</li>
           </ul>
         </div>
       </div>
       <div class="section" id="bug-tracker">
         <h1>
-          <a class="toc-backref" href="#id8">Bug Tracker</a>
+          <a class="toc-backref" href="#id10">Bug Tracker</a>
         </h1>
         <p>
           Bugs are tracked on
           <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues">GitHub Issues</a>
           .
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us smashing it by providing a detailed and welcomed
           <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>
           .
         </p>
         <p>Do not contact contributors directly about support or help with technical issues.</p>
       </div>
       <div class="section" id="credits">
         <h1>
-          <a class="toc-backref" href="#id9">Credits</a>
+          <a class="toc-backref" href="#id11">Credits</a>
         </h1>
         <div class="section" id="authors">
           <h2>
-            <a class="toc-backref" href="#id10">Authors</a>
+            <a class="toc-backref" href="#id12">Authors</a>
           </h2>
           <ul class="simple">
             <li>Coopdevs</li>
           </ul>
         </div>
         <div class="section" id="maintainers">
           <h2>
-            <a class="toc-backref" href="#id11">Maintainers</a>
+            <a class="toc-backref" href="#id13">Maintainers</a>
           </h2>
           <p>
             This module is part of the
             <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance">coopdevs/odoo14-addons</a>
             project on GitHub.
           </p>
           <p>You are welcome to contribute.</p>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/img/icon.png` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/static/src/img/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

 * *Files 14% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

```diff
@@ -11,9 +11,16 @@
     <menuitem id="menu_odoo_instance_module" name="Modules" parent="odoo_instance_menu" sequence="30" action="odoo_instance_module_action"/>
     <!-- Menu item for odoo.instance.version -->
     <menuitem id="menu_odoo_version" name="Odoo Versions" parent="odoo_instance_menu" sequence="40" action="odoo_version_action"/>
     <!-- Menu item for 12.0 instances -->
     <menuitem id="odoo_instance_v12_menu" name="Odoo 12.0 Instances" parent="odoo_instances_menu_versions" action="odoo_instance_v12_action" sequence="10"/>
     <!-- Menu item for 14.0 instances -->
     <menuitem id="odoo_instance_v14_menu" name="Odoo 14.0 Instances" parent="odoo_instances_menu_versions" action="odoo_instance_v14_action" sequence="20"/>
+    <!-- Odoo Release menu item -->
+    <record id="menu_odoo_release" model="ir.ui.menu">
+      <field name="name">Odoo Releases</field>
+      <field name="parent_id" ref="odoo_instance_menu"/>
+      <field name="action" ref="action_odoo_release"/>
+      <field name="sequence" eval="50"/>
+    </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml`

 * *Files 13% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml`

```diff
@@ -47,9 +47,24 @@
           <field name="instance_ids"/>
           <filter name="odoo_version_id" string="Odoo Version" domain="[]" context="{'group_by':'odoo_version_id'}"/>
           <filter name="odoo_12_0" string="Odoo 12.0" domain="[('odoo_version_id.name', '=', '12.0')]"/>
           <filter name="odoo_14_0" string="Odoo 14.0" domain="[('odoo_version_id.name', '=', '14.0')]"/>
         </search>
       </field>
     </record>
+    <!-- Odoo Release search view -->
+    <record id="view_odoo_release_search" model="ir.ui.view">
+      <field name="name">odoo.release.search</field>
+      <field name="model">odoo.release</field>
+      <field name="arch" type="xml">
+        <search>
+          <field name="name"/>
+          <field name="odoo_version_id"/>
+          <field name="release_date"/>
+          <group expand="0" string="Group By">
+            <filter name="odoo_version_id" string="Odoo Version" domain="[]" context="{'group_by': 'odoo_version_id'}"/>
+          </group>
+        </search>
+      </field>
+    </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

```diff
@@ -93,14 +93,19 @@
                     </tree>
                   </field>
                 </group>
               </page>
               <page string="Technic">
                 <group>
                   <field name="inventory_url" widget="url"/>
+                  <field name="branch"/>
+                  <field name="odoo_release_id"/>
+                  <button name="update_odoo_release" type="object" string="Import YAML" class="btn-secondary oe_edit_only"/>
+                </group>
+                <group>
                   <field name="server_information"/>
                   <field name="server_type"/>
                 </group>
                 <group string="Planned Deploys">
                   <field name="deploy_duration" widget="float_time"/>
                   <field name="deploy_event_ids" domain="[('start', '&gt;', current_date)]">
                     <tree string="Planned Deploys">
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_module_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_module_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_process_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_process_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_version_view.xml`

 * *Files 19% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/odoo_version_view.xml`

```diff
@@ -2,26 +2,30 @@
 <odoo>
   <record id="odoo_version_tree" model="ir.ui.view">
     <field name="name">odoo.version.tree</field>
     <field name="model">odoo.version</field>
     <field name="arch" type="xml">
       <tree string="Odoo Versions">
         <field name="name"/>
+        <field name="odoo_release_ids" widget="many2many_tags"/>
       </tree>
     </field>
   </record>
   <odoo>
     <record id="odoo_version_form" model="ir.ui.view">
       <field name="name">odoo.version.form</field>
       <field name="model">odoo.version</field>
       <field name="arch" type="xml">
         <form string="Odoo Version">
           <sheet>
             <group>
               <field name="name"/>
             </group>
+            <group>
+              <field name="odoo_release_ids" widget="table"/>
+            </group>
           </sheet>
         </form>
       </field>
     </record>
   </odoo>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/project_project_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/project_project_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/res_partner_view.xml` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-odoo-instance
-Version: 14.0.1.0.1
+Version: 14.0.1.1.0
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -50,14 +50,22 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.1.0 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Handle odoo releases
+
+
 14.0.1.0.1 (2023-04-25)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Improved UX: Searches, filters, grouping...
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt` & `odoo14-addon-odoo_instance-14.0.1.1.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 odoo/addons/odoo_instance/models/__init__.py
 odoo/addons/odoo_instance/models/calendar_event.py
 odoo/addons/odoo_instance/models/import_requirements_wizard.py
 odoo/addons/odoo_instance/models/odoo_instance.py
 odoo/addons/odoo_instance/models/odoo_instance_module.py
 odoo/addons/odoo_instance/models/odoo_instance_process.py
 odoo/addons/odoo_instance/models/odoo_instance_window.py
+odoo/addons/odoo_instance/models/odoo_release.py
 odoo/addons/odoo_instance/models/odoo_version.py
 odoo/addons/odoo_instance/models/process_module_rel.py
 odoo/addons/odoo_instance/models/project_project.py
 odoo/addons/odoo_instance/models/res_partner.py
 odoo/addons/odoo_instance/readme/DESCRIPTION.rst
 odoo/addons/odoo_instance/readme/HISTORY.rst
 odoo/addons/odoo_instance/readme/newsfragments/.gitignore
@@ -34,14 +35,15 @@
 odoo/addons/odoo_instance/views/odoo_instance_actions.xml
 odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
 odoo/addons/odoo_instance/views/odoo_instance_searches.xml
 odoo/addons/odoo_instance/views/odoo_instance_view.xml
 odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
 odoo/addons/odoo_instance/views/odoo_module_view.xml
 odoo/addons/odoo_instance/views/odoo_process_view.xml
+odoo/addons/odoo_instance/views/odoo_release_view.xml
 odoo/addons/odoo_instance/views/odoo_version_view.xml
 odoo/addons/odoo_instance/views/project_project_view.xml
 odoo/addons/odoo_instance/views/res_partner_view.xml
 odoo/addons/odoo_instance/wizards/__init__.py
 odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
 odoo14_addon_odoo_instance.egg-info/PKG-INFO
 odoo14_addon_odoo_instance.egg-info/SOURCES.txt
```

