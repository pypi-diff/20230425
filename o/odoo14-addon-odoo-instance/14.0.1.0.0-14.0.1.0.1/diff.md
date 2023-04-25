# Comparing `tmp/odoo14-addon-odoo_instance-14.0.1.0.0.tar.gz` & `tmp/odoo14-addon-odoo_instance-14.0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.0.0.tar", last modified: Mon Apr 24 20:48:04 2023, max compression
+gzip compressed data, was "odoo14-addon-odoo_instance-14.0.1.0.1.tar", last modified: Tue Apr 25 00:20:29 2023, max compression
```

## Comparing `odoo14-addon-odoo_instance-14.0.1.0.0.tar` & `odoo14-addon-odoo_instance-14.0.1.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4476 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.595107 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.595107 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.595107 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3353 2023-04-24 20:46:42.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/README.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1185 2023-04-24 20:42:10.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.595107 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/calendar_tags.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/ir_cron.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/odoo_version_data.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      246 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/calendar_event.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      488 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/import_requirements_wizard.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19126 2023-04-24 20:20:54.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1986 2023-04-24 19:30:19.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance_module.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      754 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance_process.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1790 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance_window.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      184 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_version.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      474 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/process_module_rel.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/project_project.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/res_partner.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/readme/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      221 2023-04-24 20:45:35.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/readme/HISTORY.rst
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/readme/newsfragments/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/security/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1555 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/security/ir.model.access.csv
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/security/security_groups.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.595107 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/description/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    12703 2023-04-24 20:46:43.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/description/index.html
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.595107 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/css/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/css/project_instance.css
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/img/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/img/icon.png
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/js/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/js/project_instance.js
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/tests/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/tests/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/tests/test_project_instance.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2182 2023-04-24 20:07:33.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      945 2023-04-24 20:06:02.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1187 2023-04-24 20:13:00.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)    20909 2023-04-24 20:38:11.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      750 2023-04-24 20:08:46.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_module_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1392 2023-04-24 20:11:17.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_process_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      896 2023-04-24 20:11:02.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_version_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/project_project_view.xml
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/res_partner_view.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/wizards/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/wizards/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2653 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4476 2023-04-24 20:48:04.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2666 2023-04-24 20:48:04.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-24 20:48:04.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-24 20:48:04.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 20:48:04.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-24 20:48:04.000000 odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-24 20:48:04.598440 odoo14-addon-odoo_instance-14.0.1.0.0/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-24 17:06:45.000000 odoo14-addon-odoo_instance-14.0.1.0.0/setup.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3777 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/PKG-INFO
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.526388 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.529722 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3365 2023-04-24 23:44:11.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/README.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1185 2023-04-24 23:39:21.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/__manifest__.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      217 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/calendar_tags.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1396 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/ir_cron.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    95199 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     9484 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      705 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo_version_data.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      246 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      208 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/calendar_event.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      488 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/import_requirements_wizard.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    19284 2023-04-25 00:12:04.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2469 2023-04-24 23:30:49.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_module.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1377 2023-04-24 22:28:12.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_process.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1790 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_window.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      184 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_version.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      474 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/process_module_rel.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/project_project.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      182 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/res_partner.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1254 2023-04-24 17:29:42.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      385 2023-04-24 23:44:06.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/HISTORY.rst
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/newsfragments/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       12 2023-04-24 18:45:09.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/newsfragments/.gitignore
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       24 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1555 2023-04-24 22:12:05.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/ir.model.access.csv
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      383 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/security_groups.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.529722 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    12978 2023-04-24 23:44:12.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/index.html
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.529722 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/css/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/css/project_instance.css
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/img/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    33659 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/img/icon.png
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/js/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/js/project_instance.js
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/tests/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/tests/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        0 2023-04-24 17:05:00.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/tests/test_project_instance.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1049 2023-04-24 19:27:51.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3034 2023-04-24 22:37:43.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1614 2023-04-25 00:16:27.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3947 2023-04-24 23:30:35.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_searches.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)    18726 2023-04-24 23:58:22.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      971 2023-04-24 19:32:46.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3029 2023-04-25 00:00:05.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_module_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1674 2023-04-24 23:58:59.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_process_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      896 2023-04-24 20:11:02.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_version_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      920 2023-04-24 18:27:56.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/project_project_view.xml
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     1083 2023-04-24 20:15:25.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/res_partner_view.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       94 2023-04-24 19:55:35.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2309 2023-04-24 23:39:11.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     3777 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2666 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/not-zip-safe
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       43 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/requires.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-04-25 00:20:29.000000 odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/top_level.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-04-25 00:20:29.533055 odoo14-addon-odoo_instance-14.0.1.0.1/setup.cfg
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-04-24 23:39:06.000000 odoo14-addon-odoo_instance-14.0.1.0.1/setup.py
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,107 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: odoo14-addon-odoo_instance
-Version: 14.0.1.0.0
+Version: 14.0.1.0.1
 Summary: Manage Odoo instances with relevant information
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: AGPL-3
-Description: =============
-        Odoo Instance
-        =============
-        
-        .. 
-           !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-           !! This file is generated by oca-gen-addon-readme !!
-           !! changes will be overwritten.                   !!
-           !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-           !! source digest: sha256:f2da2437719a5d8289e9efca6c8494107d561bdd55c7ccad6fc699a975331235
-           !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        
-        .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
-            :target: https://odoo-community.org/page/development-status
-            :alt: Beta
-        .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
-            :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
-            :alt: License: AGPL-3
-        .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
-            :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
-            :alt: coopdevs/odoo14-addons
-        
-        |badge1| |badge2| |badge3|
-        
-        This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
-        
-        **Features**
-        
-         - Create and manage project instances, classified by Odoo version, and organize them by stages.
-         - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
-         - Manage processes, associate them with project instances, and track related modules, all classified by Odoo version.
-         - Manage odoo modules, including their name, Odoo and own version, and associate them with processes.
-         - Get installed modules and their versions from a requirements file.
-         - Troubleshooting tab for storing helpful documentation, such as postmortems, specific configurations, and more.
-         - Assign users to different project roles within each project instance.
-         - Display server information for each project instance.
-         - Manage commercial data related to project instances.
-        
-        **Table of contents**
-        
-        .. contents::
-           :local:
-        
-        Changelog
-        =========
-        
-        14.0.1.0.0 (2023-04-24)
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        **Features**
-        
-        - Rename models and split logic in files
-        
-        
-        14.0.0.2.0 (2023-04-24)
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        **Features**
-        
-        - Add instance relations to project and res.partner
-        
-        Bug Tracker
-        ===========
-        
-        Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
-        In case of trouble, please check there if your issue has already been reported.
-        If you spotted it first, help us to smash it by providing a detailed and welcomed
-        `feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
-        
-        Do not contact contributors directly about support or help with technical issues.
-        
-        Credits
-        =======
-        
-        Authors
-        ~~~~~~~
-        
-        * Coopdevs
-        
-        Maintainers
-        ~~~~~~~~~~~
-        
-        This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
-        
-        You are welcome to contribute.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
+
+=============
+Odoo Instance
+=============
+
+.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+   !! This file is generated by oca-gen-addon-readme !!
+   !! changes will be overwritten.                   !!
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
+.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
+    :target: https://odoo-community.org/page/development-status
+    :alt: Beta
+.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
+    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+    :alt: License: AGPL-3
+.. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
+    :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
+    :alt: coopdevs/odoo14-addons
+
+|badge1| |badge2| |badge3| 
+
+This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
+
+**Features**
+
+ - Create and manage project instances, classified by Odoo version, and organize them by stages.
+ - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
+ - Manage processes, associate them with project instances, and track related modules, all classified by Odoo version.
+ - Manage odoo modules, including their name, Odoo and own version, and associate them with processes.
+ - Get installed modules and their versions from a requirements file.
+ - Troubleshooting tab for storing helpful documentation, such as postmortems, specific configurations, and more.
+ - Assign users to different project roles within each project instance.
+ - Display server information for each project instance.
+ - Manage commercial data related to project instances.
+
+**Table of contents**
+
+.. contents::
+   :local:
+
+Changelog
+=========
+
+14.0.1.0.1 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Improved UX: Searches, filters, grouping...
+
+**Bugfixes**
+
+- Removed forgotten debug statementes
+
+
+14.0.1.0.0 (2023-04-24)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Rename models and split logic in files
+
+
+14.0.0.2.0 (2023-04-24)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add instance relations to project and res.partner
+
+Bug Tracker
+===========
+
+Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
+In case of trouble, please check there if your issue has already been reported.
+If you spotted it first, help us smashing it by providing a detailed and welcomed
+`feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+
+Do not contact contributors directly about support or help with technical issues.
+
+Credits
+=======
+
+Authors
+~~~~~~~
+
+* Coopdevs
+
+Maintainers
+~~~~~~~~~~~
+
+This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
+
+You are welcome to contribute.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/README.rst` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+Metadata-Version: 2.1
+Name: odoo14-addon-odoo-instance
+Version: 14.0.1.0.1
+Summary: Manage Odoo instances with relevant information
+Home-page: https://www.coopdevs.org
+Author: Coopdevs
+License: AGPL-3
+Classifier: Programming Language :: Python
+Classifier: Framework :: Odoo
+Classifier: Framework :: Odoo :: 14.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Requires-Python: >=3.6
+
 =============
 Odoo Instance
 =============
 
-.. 
-   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:f2da2437719a5d8289e9efca6c8494107d561bdd55c7ccad6fc699a975331235
-   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
     :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
     :alt: coopdevs/odoo14-addons
 
-|badge1| |badge2| |badge3|
+|badge1| |badge2| |badge3| 
 
 This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
 
 **Features**
 
  - Create and manage project instances, classified by Odoo version, and organize them by stages.
  - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
@@ -40,14 +50,26 @@
 
 .. contents::
    :local:
 
 Changelog
 =========
 
+14.0.1.0.1 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Improved UX: Searches, filters, grouping...
+
+**Bugfixes**
+
+- Removed forgotten debug statementes
+
+
 14.0.1.0.0 (2023-04-24)
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 **Features**
 
 - Rename models and split logic in files
 
@@ -60,15 +82,15 @@
 - Add instance relations to project and res.partner
 
 Bug Tracker
 ===========
 
 Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
-If you spotted it first, help us to smash it by providing a detailed and welcomed
+If you spotted it first, help us smashing it by providing a detailed and welcomed
 `feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/__manifest__.py` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Odoo Instance',
-    'version': '14.0.1.0.0',
+    'version': '14.0.1.0.1',
     'category': 'Project',
     'summary': 'Manage Odoo instances with relevant information',
     'author': 'Coopdevs',
     'website': 'https://www.coopdevs.org',
     'depends': ['base', 'contract', 'project', 'calendar'],
     'data': [
         'security/security_groups.xml',
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/ir_cron.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo12_core_modules_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo14_core_modules_app_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/data/odoo_version_data.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/data/odoo_version_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance.py` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,14 @@
         'res.partner', string='Client Contact', domain=[('type', '=', 'contact')])
 
     technician_ids = fields.Many2many(
         'res.users', string='Technicians', relation='odoo_instance_technician_rel')
     functional_ids = fields.Many2many(
         'res.users', string='Functional Experts', relation='odoo_instance_functional_rel')
 
-    odoo_version = fields.Selection([
-        ('12.0', '12.0'),
-        ('13.0', '13.0'),
-        ('14.0', '14.0'),
-        ('15.0', '15.0'),
-        ('16.0', '16.0'),
-    ], string="Odoo Version")
-
     odoo_version_id = fields.Many2one('odoo.version', string="Odoo Version", required=True)
 
     state = fields.Selection([
         ('in_progress', 'In Progress'),
         ('running', 'Running'),
         ('paused', 'Paused'),
         ('cancelled', 'Terminated')
@@ -86,16 +78,20 @@
     deploy_duration = fields.Float(
         string='Deploy Duration', default=1.0, help="Duration in hours")
 
 
 
     # Functional Information
     process_ids = fields.Many2many(
-        'odoo.instance.process', string='Processes')
-
+        'odoo.instance.process',
+        'odoo_instance_process_rel',
+        'instance_id',
+        'process_id',
+        string='Processes'
+    )
     available_windows = fields.One2many(
         'odoo.instance.window', 'instance_id', string='Available Windows')
 
     functional_requirement_ids = fields.One2many(
         'odoo.instance.functional_requirement', 'odoo_instance_id', string='Functional Requirements')
 
 
@@ -169,31 +165,34 @@
             ], limit=1)
         for version in current_versions:
             # delete the instance in the version
             version.instance_ids = [(3, self.id)]
             # if the version is not used by any instance, delete it
             if not version.instance_ids:
                 version.unlink()
-        _logger.debug('current_versions: %s', current_versions)         
+        
         for line in file_content.splitlines():
             line = line.strip()
             if not line or '==' not in line:
                 continue
 
             module_name, version = line.split('==')
             module = Module.search(
                 [('technical_name', '=', module_name)], limit=1)
 
             if not module:
                 module_data = self.get_module_name_from_pypi(module_name)
+        
                 module = Module.create({
                     'technical_name': module_data['technical_name'],
                     'name': module_data['name'],
-                    'module_type': module_data['module_type'],
-                    'odoo_version_id': module_data['odoo_version_id'].id,
+                    'module_type': module_data['module_type'],                    
+                    #assign odoo_version_id only if odoo_version_id.d is a int
+                    'odoo_version_id': module_data['odoo_version_id'],
+                    #'odoo_version_id': module_data['odoo_version_id'].id,
                     'pypi_url': f'https://pypi.org/project/{module_name}/',
                     'is_odoo_module': module_data['is_odoo_module'],
                 })
 
             version_record = ModuleVersion.search([
                 ('name', '=', version),
                 ('module_id', '=', module.id),
@@ -214,37 +213,41 @@
 
     def get_module_name_from_pypi(self, technical_name):
         url = f'https://pypi.org/pypi/{technical_name}/json'
         response = requests.get(url)
         module_data = {
             'technical_name': technical_name,
             'name': technical_name,
-            'module_type': 'custom',
+            'module_type': 'dep',
+            'odoo_version_id': self.odoo_version_id.id,
         }
 
         if response.status_code == 200:
             data = response.json()
             module_data['technical_name'] = data['info']['name']
             module_data['name'] = data['info']['summary']
             module_data['home_page'] = data['info']['home_page']
             module_data['is_odoo_module'] = False
-            _logger.critical('technical_name: %s', technical_name)
+            _logger.debug('Importing technical_name: %s', technical_name)
 
-            # Check if the module is Odoo core or OCA
-            if 'oca' in module_data['home_page'].lower():
-                module_data['module_type'] = 'OCA'
             if 'odoo' in module_data['technical_name'].lower():
                 module_data['is_odoo_module'] = True
 
-            # extract odoo version from version key. Example: version	"14.0.1.0.3"
-            odoo_version_pattern = r"(\d{1,2}\.\d{1,2})"
-            match = re.search(odoo_version_pattern, data['info']['version'])
-            if match:
-                module_data['odoo_version'] = match.group(1)
-                module_data['odoo_version_id'] = self.env['odoo.version'].search([('name', '=', match.group(1))], limit=1)
+            if module_data['is_odoo_module']:
+                # Check if the module is Odoo core or OCA
+                if 'oca' in module_data['home_page'].lower():
+                    module_data['module_type'] = 'OCA'
+
+
+                # extract odoo version from version key. Example: version	"14.0.1.0.3"
+                odoo_version_pattern = r"(\d{1,2}\.\d{1,2})"
+                match = re.search(odoo_version_pattern, data['info']['version'])
+                if match:
+                    module_data['odoo_version'] = match.group(1)
+                    module_data['odoo_version_id'] = self.env['odoo.version'].search([('name', '=', match.group(1))], limit=1).id
 
         else:
             _logger.warning(
                 f'Error fetching module name from pypi.org for {technical_name}')
 
         return module_data
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance_module.py` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,36 @@
 
     name = fields.Char(string='Name', required=True)
     technical_name = fields.Char(string='Technical Name', required=True)
     is_odoo_module = fields.Boolean(string='Is Odoo Module', default=True)
     pypi_url = fields.Char(string='PyPI URL')
     version_ids = fields.One2many(
         'odoo.instance.module.version', 'module_id', string='Versions')
-    odoo_version = fields.Char(string='Odoo Version')
     odoo_version_id = fields.Many2one('odoo.version', string="Odoo Version")
     module_type = fields.Selection([
         ('core', 'Odoo Core'),
         ('OCA', 'OCA'),
-        ('custom', 'Custom'),
+        ('custom', 'Custom'),        
+        ('other', 'Other'),
+        ('dep', 'Dependency')
     ], string='Module Type', default='custom')
 
+    instance_ids = fields.Many2many(
+            'odoo.instance', string='Instances',
+            compute='_compute_instance_ids', readonly=True, store=True)
+
+    @api.depends('version_ids.instance_ids')
+    def _compute_instance_ids(self):
+        for record in self:
+            instance_ids = self.env['odoo.instance']
+            for version in record.version_ids:
+                instance_ids |= version.instance_ids
+            record.instance_ids = instance_ids
+
+
     def fetch_pypi_information(self):
         package_info_url = f'https://pypi.org/pypi/{self.name}/json'
         response = requests.get(package_info_url)
         if response.status_code == 200:
             package_data = response.json()
             self.display_name = package_data['info']['name']
             self.is_odoo_module = 'odoo' in package_data['info']['keywords'].lower(
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance_process.py` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_process.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from odoo import fields, models
+from odoo import fields, models, api
 import logging
 
 class OdooInstanceProcess(models.Model):
     _logger = logging.getLogger(__name__)
     _name = 'odoo.instance.process'
     _description = 'Instance Process'
 
@@ -15,7 +15,23 @@
         "module_id",
         string="Related Modules",
         search=['|', ('name', 'ilike', '%search%'),
                     ('technical_name', 'ilike', '%search%')]
     )
     handbook_url = fields.Char(string="Handbook URL")    
     odoo_version_id = fields.Many2one("odoo.version", string="Odoo Version", required=True)
+    instance_ids = fields.Many2many(
+            'odoo.instance', 
+            compute='compute_instance_ids', 
+            string='Instances',
+            search='search_instance_ids'
+        )
+    
+    def compute_instance_ids(self):
+        for record in self:
+            instance_ids = self.env['odoo.instance'].search([('process_ids', 'in', record.id)])
+            record.instance_ids = instance_ids.ids
+
+    @api.model
+    def search_instance_ids(self, operator, value):
+        instances = self.env['odoo.instance'].search([('name', operator, value)])
+        return [('id', 'in', instances.process_ids.ids)]
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/models/odoo_instance_window.py` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/models/odoo_instance_window.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/readme/DESCRIPTION.rst` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/readme/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/security/ir.model.access.csv` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/security/ir.model.access.csv`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 access_odoo_instance_process,odoo.instance.process,model_odoo_instance_process,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_schedule,odoo.instance.schedule,model_odoo_instance_schedule,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_unavailabe_schedule,odoo.instance.unavailable_schedule,model_odoo_instance_unavailable_schedule,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_functional_requirement,odoo.instance.functional.requirement,model_odoo_instance_functional_requirement,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window,odoo.instance.window,model_odoo_instance_window,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_window_wizard,odoo.instance.window.wizard,model_odoo_instance_window_wizard,odoo_instance.group_odoo_instance_user,1,1,1,1
 access_odoo_instance_troubleshooting,odoo.instance.troubleshooting,model_odoo_instance_troubleshooting,odoo_instance.group_odoo_instance_user,1,1,1,1
-access_odoo_version,odoo.version,model_odoo_version,odoo_instance.group_odoo_instance_user,1,1,1,1
+access_odoo_version,odoo.version,model_odoo_version,odoo_instance.group_odoo_instance_user,1,1,0,0
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/index.html`

 * *Files 3% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/description/index.html` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/description/index.html`

```diff
@@ -359,16 +359,14 @@
   </head>
   <body>
     <div class="document" id="odoo-instance">
       <h1 class="title">Odoo Instance</h1>
       <!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !! This file is generated by oca-gen-addon-readme !!
 !! changes will be overwritten.                   !!
-!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-!! source digest: sha256:f2da2437719a5d8289e9efca6c8494107d561bdd55c7ccad6fc699a975331235
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->
       <p>
         <a class="reference external" href="https://odoo-community.org/page/development-status">
           <img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png"/>
         </a>
         <a class="reference external" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html">
           <img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png"/>
@@ -396,97 +394,117 @@
       </blockquote>
       <p>
         <strong>Table of contents</strong>
       </p>
       <div class="contents local topic" id="contents">
         <ul class="simple">
           <li>
-            <a class="reference internal" href="#changelog" id="id3">Changelog</a>
+            <a class="reference internal" href="#changelog" id="id4">Changelog</a>
             <ul>
               <li>
-                <a class="reference internal" href="#id1" id="id4">14.0.1.0.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id1" id="id5">14.0.1.0.1 (2023-04-25)</a>
               </li>
               <li>
-                <a class="reference internal" href="#id2" id="id5">14.0.0.2.0 (2023-04-24)</a>
+                <a class="reference internal" href="#id2" id="id6">14.0.1.0.0 (2023-04-24)</a>
+              </li>
+              <li>
+                <a class="reference internal" href="#id3" id="id7">14.0.0.2.0 (2023-04-24)</a>
               </li>
             </ul>
           </li>
           <li>
-            <a class="reference internal" href="#bug-tracker" id="id6">Bug Tracker</a>
+            <a class="reference internal" href="#bug-tracker" id="id8">Bug Tracker</a>
           </li>
           <li>
-            <a class="reference internal" href="#credits" id="id7">Credits</a>
+            <a class="reference internal" href="#credits" id="id9">Credits</a>
             <ul>
               <li>
-                <a class="reference internal" href="#authors" id="id8">Authors</a>
+                <a class="reference internal" href="#authors" id="id10">Authors</a>
               </li>
               <li>
-                <a class="reference internal" href="#maintainers" id="id9">Maintainers</a>
+                <a class="reference internal" href="#maintainers" id="id11">Maintainers</a>
               </li>
             </ul>
           </li>
         </ul>
       </div>
       <div class="section" id="changelog">
         <h1>
-          <a class="toc-backref" href="#id3">Changelog</a>
+          <a class="toc-backref" href="#id4">Changelog</a>
         </h1>
         <div class="section" id="id1">
           <h2>
-            <a class="toc-backref" href="#id4">14.0.1.0.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id5">14.0.1.0.1 (2023-04-25)</a>
           </h2>
           <p>
             <strong>Features</strong>
           </p>
           <ul class="simple">
-            <li>Rename models and split logic in files</li>
+            <li>Improved UX: Searches, filters, grouping…</li>
+          </ul>
+          <p>
+            <strong>Bugfixes</strong>
+          </p>
+          <ul class="simple">
+            <li>Removed forgotten debug statementes</li>
           </ul>
         </div>
         <div class="section" id="id2">
           <h2>
-            <a class="toc-backref" href="#id5">14.0.0.2.0 (2023-04-24)</a>
+            <a class="toc-backref" href="#id6">14.0.1.0.0 (2023-04-24)</a>
+          </h2>
+          <p>
+            <strong>Features</strong>
+          </p>
+          <ul class="simple">
+            <li>Rename models and split logic in files</li>
+          </ul>
+        </div>
+        <div class="section" id="id3">
+          <h2>
+            <a class="toc-backref" href="#id7">14.0.0.2.0 (2023-04-24)</a>
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
-          <a class="toc-backref" href="#id6">Bug Tracker</a>
+          <a class="toc-backref" href="#id8">Bug Tracker</a>
         </h1>
         <p>
           Bugs are tracked on
           <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues">GitHub Issues</a>
           .
 In case of trouble, please check there if your issue has already been reported.
-If you spotted it first, help us to smash it by providing a detailed and welcomed
+If you spotted it first, help us smashing it by providing a detailed and welcomed
           <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>
           .
         </p>
         <p>Do not contact contributors directly about support or help with technical issues.</p>
       </div>
       <div class="section" id="credits">
         <h1>
-          <a class="toc-backref" href="#id7">Credits</a>
+          <a class="toc-backref" href="#id9">Credits</a>
         </h1>
         <div class="section" id="authors">
           <h2>
-            <a class="toc-backref" href="#id8">Authors</a>
+            <a class="toc-backref" href="#id10">Authors</a>
           </h2>
           <ul class="simple">
             <li>Coopdevs</li>
           </ul>
         </div>
         <div class="section" id="maintainers">
           <h2>
-            <a class="toc-backref" href="#id9">Maintainers</a>
+            <a class="toc-backref" href="#id11">Maintainers</a>
           </h2>
           <p>
             This module is part of the
             <a class="reference external" href="https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance">coopdevs/odoo14-addons</a>
             project on GitHub.
           </p>
           <p>You are welcome to contribute.</p>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/static/src/img/icon.png` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/static/src/img/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/import_requirements_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

 * *Files 6% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_actions.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_actions.xml`

```diff
@@ -11,22 +11,24 @@
     </record>
     <!-- Action for odoo.instance -->
     <record id="odoo_instance_action" model="ir.actions.act_window">
       <field name="name">Odoo Instances</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.instance</field>
       <field name="view_mode">tree,form,kanban</field>
+      <field name="context">{'search_default_my_instances': 1}</field>
     </record>
     <!-- Action for odoo.instance.module -->
     <record id="odoo_instance_module_action" model="ir.actions.act_window">
       <field name="name">Modules</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.instance.module</field>
       <field name="view_mode">tree,form</field>
       <field name="view_id" ref="odoo_instance_module_tree"/>
+      <field name="context">{'search_default_is_odoo_module': 1}</field>
     </record>
     <!-- Action for odoo.instance.process -->
     <record id="odoo_instance_process_action" model="ir.actions.act_window">
       <field name="name">Processes</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.instance.process</field>
       <field name="view_mode">tree,form</field>
@@ -36,9 +38,21 @@
     <record id="odoo_version_action" model="ir.actions.act_window">
       <field name="name">Odoo Versions</field>
       <field name="type">ir.actions.act_window</field>
       <field name="res_model">odoo.version</field>
       <field name="view_mode">tree,form,kanban</field>
       <field name="view_id" ref="odoo_version_tree"/>
     </record>
+    <record id="odoo_instance_v12_action" model="ir.actions.act_window">
+      <field name="name">Odoo 12.0 Instances</field>
+      <field name="res_model">odoo.instance</field>
+      <field name="view_mode">tree,form</field>
+      <field name="domain">[('odoo_version_id.name', '=', '12.0')]</field>
+    </record>
+    <record id="odoo_instance_v14_action" model="ir.actions.act_window">
+      <field name="name">Odoo 14.0 Instances</field>
+      <field name="res_model">odoo.instance</field>
+      <field name="view_mode">tree,form</field>
+      <field name="domain">[('odoo_version_id.name', '=', '14.0')]</field>
+    </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

 * *Files 20% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_menuitems.xml`

```diff
@@ -1,13 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <data>
     <!-- Menu item for odoo.instance -->
     <menuitem id="odoo_instance_menu" name="Odoo Instances" action="odoo_instance_action" web_icon="odoo_instance,static/src/img/icon.png"/>
+    <!-- Menu item for odoo.instance folded -->
+    <menuitem id="odoo_instances_menu_versions" name="Instances" parent="odoo_instance_menu" sequence="10"/>
+    <!-- Menu item for odoo.instance.process -->
+    <menuitem id="menu_odoo_instance_process" name="Processes" parent="odoo_instance_menu" sequence="20" action="odoo_instance_process_action"/>
     <!-- Menu item for odoo.instance.module -->
     <menuitem id="menu_odoo_instance_module" name="Modules" parent="odoo_instance_menu" sequence="30" action="odoo_instance_module_action"/>
     <!-- Menu item for odoo.instance.version -->
     <menuitem id="menu_odoo_version" name="Odoo Versions" parent="odoo_instance_menu" sequence="40" action="odoo_version_action"/>
-    <!-- Menu item for odoo.instance.process -->
-    <menuitem id="menu_odoo_instance_process" name="Processes" parent="odoo_instance_menu" sequence="30" action="odoo_instance_process_action"/>
+    <!-- Menu item for 12.0 instances -->
+    <menuitem id="odoo_instance_v12_menu" name="Odoo 12.0 Instances" parent="odoo_instances_menu_versions" action="odoo_instance_v12_action" sequence="10"/>
+    <!-- Menu item for 14.0 instances -->
+    <menuitem id="odoo_instance_v14_menu" name="Odoo 14.0 Instances" parent="odoo_instances_menu_versions" action="odoo_instance_v14_action" sequence="20"/>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/res_partner_view.xml`

 * *Files 24% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_searches.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/res_partner_view.xml`

```diff
@@ -1,27 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <data>
-    <record id="odoo_instance_search" model="ir.ui.view">
-      <field name="name">odoo.instance.search</field>
-      <field name="model">odoo.instance</field>
+    <!-- Inherit Res Partner Form View to add Instances -->
+    <record id="view_partner_form_inherit" model="ir.ui.view">
+      <field name="name">res.partner.form.inherit</field>
+      <field name="model">res.partner</field>
+      <field name="inherit_id" ref="base.view_partner_form"/>
       <field name="arch" type="xml">
-        <search>
-          <filter name="my_instances" string="My Instances" domain="[('technician_ids.user_id', '=', uid), ('functional_ids.user_id', '=', uid)]" help="Instances where I am a technician or functional"/>
-        </search>
-        <search>
-          <field name="odoo_version_id"/>
-        </search>
-      </field>
-    </record>
-    <record id="view_odoo_instance_module_search" model="ir.ui.view">
-      <field name="name">odoo.instance.module.search</field>
-      <field name="model">odoo.instance.module</field>
-      <field name="arch" type="xml">
-        <search>
-          <field name="name"/>
-          <field name="technical_name"/>
-        </search>
+        <xpath expr="//page[@name='sales_purchases']" position="after">
+          <page string="Odoo Instances">
+            <field name="instance_ids" context="{'default_partner_id': active_id}">
+              <tree action="odoo_instance.action_odoo_instance_form">
+                <field name="name"/>
+                <field name="odoo_version_id"/>
+                <field name="instance_type"/>
+              </tree>
+            </field>
+          </page>
+        </xpath>
       </field>
     </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

 * *Files 4% similar despite different names*

#### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_view.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_view.xml`

```diff
@@ -263,61 +263,14 @@
             <div class="o_kanban_card_partner_name">
               <t t-esc="record.partner_id.raw_value.name"/>
             </div>
           </xpath>
         </kanban>
       </field>
     </record>
-    <record id="view_odoo_instance_module_version_tree" model="ir.ui.view">
-      <field name="name">odoo.instance.module.version.tree</field>
-      <field name="model">odoo.instance.module.version</field>
-      <field name="arch" type="xml">
-        <tree string="Module Versions">
-          <field name="module_id"/>
-          <!-- <field name="version" /> -->
-        </tree>
-      </field>
-    </record>
-    <record id="view_odoo_instance_module_form" model="ir.ui.view">
-      <field name="name">odoo.instance.module.form</field>
-      <field name="model">odoo.instance.module</field>
-      <field name="arch" type="xml">
-        <form string="Module">
-          <sheet>
-            <div class="oe_title">
-              <label for="name" class="oe_edit_only"/>
-              <h1>
-                <field name="name"/>
-              </h1>
-            </div>
-            <group>
-              <field name="technical_name"/>
-              <group>
-                <field name="is_odoo_module"/>
-                <field name="module_type"/>
-              </group>
-              <group>
-                <field name="odoo_version_id"/>
-                <field name="pypi_url" widget="url"/>
-              </group>
-            </group>
-            <notebook>
-              <page string="Versions">
-                <field name="version_ids">
-                  <tree>
-                    <field name="name"/>
-                    <field name="instance_ids" widget="many2many_tags"/>
-                  </tree>
-                </field>
-              </page>
-            </notebook>
-          </sheet>
-        </form>
-      </field>
-    </record>
     <record id="view_functional_requirement_tree" model="ir.ui.view">
       <field name="name">odoo.instance.functional_requirement.tree</field>
       <field name="model">odoo.instance.functional_requirement</field>
       <field name="arch" type="xml">
         <tree string="Functional Requirements">
           <field name="name"/>
           <field name="status"/>
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_instance_window_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/odoo_version_view.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/odoo_version_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/views/project_project_view.xml` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/views/project_project_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/wizards/odoo_instance_window_wizard.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         CalendarEvent = self.env['calendar.event']
         event_name = f"[{self._context.get('instance_name', 'Instance')}] Deploy"
         
         # Agregar técnicos como participantes del evento
         attendee_ids = [(0, 0, {'partner_id': user.partner_id.id}) for user in self.attendee_ids]
         end_hour = self.start_time + timedelta(hours=self.duration)
         deploy_tag = self.env['calendar.event.type'].search([('name', '=', 'Deploy')], limit=1)
-
+        _logger.debug(f"Creating event with name: {event_name}")
         _logger.debug(f"Attendees: {attendee_ids}")
-        _logger.exception(f"Instance: {self.instance_id}")
+        _logger.debug(f"Instance: {self.instance_id}")
         vals = {
             'name': event_name,
             'start': self.start_time,
             'stop': end_hour,
             'description': self.description,
             'allday': False,
             'privacy': 'public',
@@ -46,17 +46,8 @@
             'type': 'ir.actions.act_window',
             'res_model': 'calendar.event',
             'res_id': event.id,
             'view_mode': 'form',
             'target': 'current',
             'flags': {'form': {'action_buttons': True, 'options': {'mode': 'edit'}}},
         }
-        def save_event(self):
-                self.ensure_one()
-                CalendarEvent = self.env['calendar.event']
-                attendees = [(4, technician_id.id) for technician_id in self.instance_id.technician_ids]
-              
-                event = CalendarEvent.create(vals)
-                return {'type': 'ir.actions.act_window_close'}
-        
-
-    #     event = CalendarEvent.create(vals)
+
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/PKG-INFO` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo/addons/odoo_instance/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,94 @@
-Metadata-Version: 1.2
-Name: odoo14-addon-odoo-instance
-Version: 14.0.1.0.0
-Summary: Manage Odoo instances with relevant information
-Home-page: https://www.coopdevs.org
-Author: Coopdevs
-License: AGPL-3
-Description: =============
-        Odoo Instance
-        =============
-        
-        .. 
-           !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-           !! This file is generated by oca-gen-addon-readme !!
-           !! changes will be overwritten.                   !!
-           !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-           !! source digest: sha256:f2da2437719a5d8289e9efca6c8494107d561bdd55c7ccad6fc699a975331235
-           !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        
-        .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
-            :target: https://odoo-community.org/page/development-status
-            :alt: Beta
-        .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
-            :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
-            :alt: License: AGPL-3
-        .. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
-            :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
-            :alt: coopdevs/odoo14-addons
-        
-        |badge1| |badge2| |badge3|
-        
-        This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
-        
-        **Features**
-        
-         - Create and manage project instances, classified by Odoo version, and organize them by stages.
-         - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
-         - Manage processes, associate them with project instances, and track related modules, all classified by Odoo version.
-         - Manage odoo modules, including their name, Odoo and own version, and associate them with processes.
-         - Get installed modules and their versions from a requirements file.
-         - Troubleshooting tab for storing helpful documentation, such as postmortems, specific configurations, and more.
-         - Assign users to different project roles within each project instance.
-         - Display server information for each project instance.
-         - Manage commercial data related to project instances.
-        
-        **Table of contents**
-        
-        .. contents::
-           :local:
-        
-        Changelog
-        =========
-        
-        14.0.1.0.0 (2023-04-24)
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        **Features**
-        
-        - Rename models and split logic in files
-        
-        
-        14.0.0.2.0 (2023-04-24)
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        **Features**
-        
-        - Add instance relations to project and res.partner
-        
-        Bug Tracker
-        ===========
-        
-        Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
-        In case of trouble, please check there if your issue has already been reported.
-        If you spotted it first, help us to smash it by providing a detailed and welcomed
-        `feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
-        
-        Do not contact contributors directly about support or help with technical issues.
-        
-        Credits
-        =======
-        
-        Authors
-        ~~~~~~~
-        
-        * Coopdevs
-        
-        Maintainers
-        ~~~~~~~~~~~
-        
-        This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
-        
-        You are welcome to contribute.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Framework :: Odoo
-Classifier: Framework :: Odoo :: 14.0
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.6
+=============
+Odoo Instance
+=============
+
+.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+   !! This file is generated by oca-gen-addon-readme !!
+   !! changes will be overwritten.                   !!
+   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
+.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
+    :target: https://odoo-community.org/page/development-status
+    :alt: Beta
+.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
+    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+    :alt: License: AGPL-3
+.. |badge3| image:: https://img.shields.io/badge/github-coopdevs%2Fodoo14--addons-lightgray.png?logo=github
+    :target: https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance
+    :alt: coopdevs/odoo14-addons
+
+|badge1| |badge2| |badge3| 
+
+This Odoo module provides a comprehensive solution for managing project instances, their deployment schedules, and associated components such as processes, modules, troubleshooting documentation, project roles, server information, and commercial data. All instances, processes, and modules are classified by the Odoo version.
+
+**Features**
+
+ - Create and manage project instances, classified by Odoo version, and organize them by stages.
+ - Schedule and manage deployment events for project instances, including the start time, duration, and description, with automatic calculation of the next available deployment window and a wizard to create calendar events.
+ - Manage processes, associate them with project instances, and track related modules, all classified by Odoo version.
+ - Manage odoo modules, including their name, Odoo and own version, and associate them with processes.
+ - Get installed modules and their versions from a requirements file.
+ - Troubleshooting tab for storing helpful documentation, such as postmortems, specific configurations, and more.
+ - Assign users to different project roles within each project instance.
+ - Display server information for each project instance.
+ - Manage commercial data related to project instances.
+
+**Table of contents**
+
+.. contents::
+   :local:
+
+Changelog
+=========
+
+14.0.1.0.1 (2023-04-25)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Improved UX: Searches, filters, grouping...
+
+**Bugfixes**
+
+- Removed forgotten debug statementes
+
+
+14.0.1.0.0 (2023-04-24)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Rename models and split logic in files
+
+
+14.0.0.2.0 (2023-04-24)
+~~~~~~~~~~~~~~~~~~~~~~~
+
+**Features**
+
+- Add instance relations to project and res.partner
+
+Bug Tracker
+===========
+
+Bugs are tracked on `GitHub Issues <https://github.com/coopdevs/odoo14-addons/issues>`_.
+In case of trouble, please check there if your issue has already been reported.
+If you spotted it first, help us smashing it by providing a detailed and welcomed
+`feedback <https://github.com/coopdevs/odoo14-addons/issues/new?body=module:%20odoo_instance%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+
+Do not contact contributors directly about support or help with technical issues.
+
+Credits
+=======
+
+Authors
+~~~~~~~
+
+* Coopdevs
+
+Maintainers
+~~~~~~~~~~~
+
+This module is part of the `coopdevs/odoo14-addons <https://github.com/coopdevs/odoo14-addons/tree/14.0/odoo_instance>`_ project on GitHub.
+
+You are welcome to contribute.
```

### Comparing `odoo14-addon-odoo_instance-14.0.1.0.0/odoo14_addon_odoo_instance.egg-info/SOURCES.txt` & `odoo14-addon-odoo_instance-14.0.1.0.1/odoo14_addon_odoo_instance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

