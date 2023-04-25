# Comparing `tmp/oarepo-model-builder-files-3.1.4.tar.gz` & `tmp/oarepo-model-builder-files-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-files-3.1.4.tar", last modified: Wed Mar 22 14:28:50 2023, max compression
+gzip compressed data, was "oarepo-model-builder-files-3.1.5.tar", last modified: Tue Apr 25 08:23:00 2023, max compression
```

## Comparing `oarepo-model-builder-files-3.1.4.tar` & `oarepo-model-builder-files-3.1.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.432509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.432509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/builtin_models/invenio_files.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.432509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.432509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_record_service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_schema.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/invenio_files_parent_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/invenio_files_schema.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/invenio_files_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/invenio_files_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/invenio_files_before.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/profiles/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/invenio_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/invenio_files_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/invenio_files_test_file_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/templates/invenio_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/templates/invenio_files_test_file_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:28:50.432509 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-22 14:28:50.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-22 14:28:50.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:28:50.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-22 14:28:50.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-22 14:28:50.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-22 14:28:50.000000 oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-03-22 14:28:50.436509 oarepo-model-builder-files-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:26:23.000000 oarepo-model-builder-files-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.909293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.913293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/invenio_files.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.913293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.917292 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_schema.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.917292 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.921293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_schema.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.921293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_before.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.921293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/invenio_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/invenio_files_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/invenio_files_test_file_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_test_file_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.913293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/setup.py
```

### Comparing `oarepo-model-builder-files-3.1.4/PKG-INFO` & `oarepo-model-builder-files-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 3.1.4
+Version: 3.1.5
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-3.1.4/README.md` & `oarepo-model-builder-files-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/builtin_models/invenio_files.json` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/invenio_files.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/__init__.py` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/invenio_files.py` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_record_permissions.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_record_service_config.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_service_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio/templates/invenio_files_schema.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_schema.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_service_config.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_service_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/invenio_parent/templates/invenio_files_schema.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_schema.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/invenio_files_base_classes.py` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_base_classes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/model_preprocessors/invenio_files_before.py` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_before.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/profiles/file.py` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/file.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files/tests/templates/invenio_files_test_file_resources.py.jinja2` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_test_file_resources.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/PKG-INFO` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 3.1.4
+Version: 3.1.5
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/SOURCES.txt` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-3.1.4/oarepo_model_builder_files.egg-info/entry_points.txt` & `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/entry_points.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [oarepo.models]
 invenio_files = oarepo_model_builder_files.builtin_models:invenio_files.json
 
 [oarepo_model_builder.builders.files]
 0100-invenio_record_metadata = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 0100-invenio_record_resource_config = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
+0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 0110-invenio_record = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 0130-invenio_record_schema = oarepo_model_builder.invenio.invenio_record_schema:InvenioRecordSchemaBuilder
 0140-invenio_record_ui_schema = oarepo_model_builder.invenio.invenio_record_ui_schema:InvenioRecordUISchemaBuilder
 0310-invenio_record_service_config = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 0320-invenio_record_service = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 0410-invenio_record_resource = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
```

### Comparing `oarepo-model-builder-files-3.1.4/setup.cfg` & `oarepo-model-builder-files-3.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-files
-version = 3.1.4
+version = 3.1.5
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -21,14 +21,15 @@
 	invenio_files = oarepo_model_builder_files.builtin_models:invenio_files.json
 oarepo_model_builder.validation = 
 	files-validation = oarepo_model_builder_files.validation:validators
 oarepo_model_builder.builders.files = 
 	0110-invenio_record  = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 	0100-invenio_record_metadata  = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 	0100-invenio_record_resource_config  = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
+	0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 	0130-invenio_record_schema  = oarepo_model_builder.invenio.invenio_record_schema:InvenioRecordSchemaBuilder
 	0140-invenio_record_ui_schema  = oarepo_model_builder.invenio.invenio_record_ui_schema:InvenioRecordUISchemaBuilder
 	0310-invenio_record_service_config  = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 	0320-invenio_record_service  = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 	0410-invenio_record_resource  = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
 	0420-invenio_views  = oarepo_model_builder.invenio.invenio_views:InvenioViewsBuilder
```

