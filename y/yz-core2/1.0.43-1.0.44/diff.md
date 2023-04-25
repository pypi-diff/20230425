# Comparing `tmp/yz-core2-1.0.43.tar.gz` & `tmp/yz-core2-1.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.43.tar", last modified: Mon Apr 24 09:43:10 2023, max compression
+gzip compressed data, was "yz-core2-1.0.44.tar", last modified: Tue Apr 25 07:36:58 2023, max compression
```

## Comparing `yz-core2-1.0.43.tar` & `yz-core2-1.0.44.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.739972 yz-core2-1.0.43/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.43/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-04-24 09:43:10.739830 yz-core2-1.0.43/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.43/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-04-24 09:43:10.740008 yz-core2-1.0.43/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-04-24 09:42:23.000000 yz-core2-1.0.43/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.726398 yz-core2-1.0.43/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.43/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.43/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.43/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.727294 yz-core2-1.0.43/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-04-24 09:43:10.000000 yz-core2-1.0.43/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3360 2023-04-24 09:43:10.000000 yz-core2-1.0.43/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-04-24 09:43:10.000000 yz-core2-1.0.43/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-04-24 09:43:10.000000 yz-core2-1.0.43/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-04-24 09:43:10.000000 yz-core2-1.0.43/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-04-24 09:43:10.000000 yz-core2-1.0.43/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.728120 yz-core2-1.0.43/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.728919 yz-core2-1.0.43/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.729518 yz-core2-1.0.43/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.729936 yz-core2-1.0.43/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6253 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.730483 yz-core2-1.0.43/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2248 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.730773 yz-core2-1.0.43/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.731711 yz-core2-1.0.43/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.732055 yz-core2-1.0.43/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6726 2023-04-24 09:03:30.000000 yz-core2-1.0.43/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10503 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.732259 yz-core2-1.0.43/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7522 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/extensions/storage/minio/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.732967 yz-core2-1.0.43/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7810 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.43/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2948 2023-04-21 02:05:49.000000 yz-core2-1.0.43/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      402 2023-04-21 02:05:49.000000 yz-core2-1.0.43/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.733318 yz-core2-1.0.43/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    12746 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.43/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.43/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.43/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.733952 yz-core2-1.0.43/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.734232 yz-core2-1.0.43/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.734702 yz-core2-1.0.43/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.734936 yz-core2-1.0.43/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.735766 yz-core2-1.0.43/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.736228 yz-core2-1.0.43/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.736474 yz-core2-1.0.43/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.736614 yz-core2-1.0.43/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.736992 yz-core2-1.0.43/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.737147 yz-core2-1.0.43/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.737733 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.738092 yz-core2-1.0.43/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.738373 yz-core2-1.0.43/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.738496 yz-core2-1.0.43/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-24 09:43:10.739612 yz-core2-1.0.43/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.43/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1834 2023-04-21 07:30:35.000000 yz-core2-1.0.43/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.112462 yz-core2-1.0.44/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.44/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-04-25 07:36:58.112291 yz-core2-1.0.44/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.44/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-04-25 07:36:58.112501 yz-core2-1.0.44/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-04-25 07:34:31.000000 yz-core2-1.0.44/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.097059 yz-core2-1.0.44/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.44/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.44/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.44/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.097772 yz-core2-1.0.44/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-04-25 07:36:58.000000 yz-core2-1.0.44/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3382 2023-04-25 07:36:58.000000 yz-core2-1.0.44/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-04-25 07:36:58.000000 yz-core2-1.0.44/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-04-25 07:36:58.000000 yz-core2-1.0.44/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-04-25 07:36:58.000000 yz-core2-1.0.44/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-04-25 07:36:58.000000 yz-core2-1.0.44/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.098624 yz-core2-1.0.44/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.099503 yz-core2-1.0.44/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.100049 yz-core2-1.0.44/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.100465 yz-core2-1.0.44/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6349 2023-04-25 07:35:32.000000 yz-core2-1.0.44/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.101005 yz-core2-1.0.44/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.44/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.101253 yz-core2-1.0.44/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.102513 yz-core2-1.0.44/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.44/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.102825 yz-core2-1.0.44/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6726 2023-04-24 09:03:30.000000 yz-core2-1.0.44/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10503 2023-04-21 07:30:35.000000 yz-core2-1.0.44/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.44/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.103062 yz-core2-1.0.44/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7522 2023-04-21 07:30:35.000000 yz-core2-1.0.44/yzcore/extensions/storage/minio/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.103993 yz-core2-1.0.44/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8370 2023-04-25 06:05:51.000000 yz-core2-1.0.44/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.44/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2948 2023-04-21 02:05:49.000000 yz-core2-1.0.44/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.44/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.104477 yz-core2-1.0.44/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    12066 2023-04-24 10:39:38.000000 yz-core2-1.0.44/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.44/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.44/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.44/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.105061 yz-core2-1.0.44/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.105314 yz-core2-1.0.44/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.105703 yz-core2-1.0.44/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.105888 yz-core2-1.0.44/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.106632 yz-core2-1.0.44/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.107011 yz-core2-1.0.44/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.107231 yz-core2-1.0.44/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.107370 yz-core2-1.0.44/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.107859 yz-core2-1.0.44/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.107998 yz-core2-1.0.44/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.108594 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.109999 yz-core2-1.0.44/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.110256 yz-core2-1.0.44/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.110388 yz-core2-1.0.44/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-25 07:36:58.112040 yz-core2-1.0.44/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1393 2023-04-25 07:36:53.000000 yz-core2-1.0.44/yzcore/utils/cache.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.44/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1834 2023-04-21 07:30:35.000000 yz-core2-1.0.44/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.43/LICENSE` & `yz-core2-1.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/PKG-INFO` & `yz-core2-1.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.43
+Version: 1.0.44
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.43/README.md` & `yz-core2-1.0.44/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/setup.py` & `yz-core2-1.0.44/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.43",
+    version="1.0.44",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.43/tests/test_setting_reload.py` & `yz-core2-1.0.44/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/tests/test_uid.py` & `yz-core2-1.0.44/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.44/yz_core2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.43
+Version: 1.0.44
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.43/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.44/yz_core2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,13 +81,14 @@
 yzcore/templates/project_template/src/const/__init__.py
 yzcore/templates/project_template/src/const/_job.py
 yzcore/templates/project_template/src/const/_task.py
 yzcore/templates/project_template/src/tests/__init__.py
 yzcore/templates/project_template/src/tests/test_xxx.py
 yzcore/templates/project_template/src/utils/__init__.py
 yzcore/utils/__init__.py
+yzcore/utils/cache.py
 yzcore/utils/check_path.py
 yzcore/utils/check_sys.py
 yzcore/utils/crypto.py
 yzcore/utils/encoding.py
 yzcore/utils/nacos.py
 yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.43/yzcore/core/datastructures.py` & `yz-core2-1.0.44/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/core/encoders.py` & `yz-core2-1.0.44/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/core/management/__init__.py` & `yz-core2-1.0.44/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.44/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.44/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/core/management/templates.py` & `yz-core2-1.0.44/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/core/storage.py` & `yz-core2-1.0.44/yzcore/core/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from yzcore.extensions.storage import StorageManage, StorageRequestError
 from yzcore.default_settings import default_setting as settings
 from abc import ABCMeta, abstractmethod
-from functools import cached_property
+try:
+    # python3.8
+    from functools import cached_property
+except ImportError:
+    from yzcore.utils.cache import cached_property
 
 
 __all__ = [
     'StorageRequestError',
     'StorageController',
     'StorageManage',
 ]
```

### Comparing `yz-core2-1.0.43/yzcore/db/db_session.py` & `yz-core2-1.0.44/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.44/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.44/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/decorators.py` & `yz-core2-1.0.44/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/default_settings.py` & `yz-core2-1.0.44/yzcore/default_settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/exceptions.py` & `yz-core2-1.0.44/yzcore/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 
 
 class NoPermission(HTTPException):
     def __init__(self, detail: Any = 'Insufficient permissions', headers: dict = None):
         super().__init__(status_code=401, detail=detail, headers=headers)
 
 
+class Forbidden(HTTPException):
+    def __init__(self, detail: Any = 'Access Denied', headers: dict = None):
+        super().__init__(status_code=403, detail=detail, headers=headers)
+
+
 class UnknownError(HTTPException):
     def __init__(self, detail: Any = 'Unknown error', headers: dict = None):
         super().__init__(status_code=500, detail=detail, headers=headers)
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.44/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.44/yzcore/extensions/storage/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/base.py` & `yz-core2-1.0.44/yzcore/extensions/storage/base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/const.py` & `yz-core2-1.0.44/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.44/yzcore/extensions/storage/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.44/yzcore/extensions/storage/obs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,24 +48,28 @@
             except OSError:
                 pass
 
     @wrap_request_return_bool
     def create_bucket(self, bucket_name=None, location='cn-south-1'):
         """创建bucket，并且作为当前操作bucket"""
         resp = self.obsClient.createBucket(bucket_name, location=location)
-        self.bucket_name = bucket_name
-        return resp
+        if resp.status < 300:
+            self.bucket_name = bucket_name
+            return resp
+        else:
+            raise StorageRequestError(
+                f"static_code: {resp.status}, errorCode: {resp.errorCode}. Message: {resp.errorMessage}.")
 
     def list_buckets(self):
         resp = self.obsClient.listBuckets(isQueryLocation=True)
         if resp.status < 300:
             return resp.body.buckets
         else:
             raise StorageRequestError(
-                f"errorCode: {resp.errorCode}. Message: {resp.errorMessage}.")
+                f"static_code: {resp.status}, errorCode: {resp.errorCode}. Message: {resp.errorMessage}.")
 
     @wrap_request_return_bool
     def is_exist_bucket(self, bucket_name=None):
         if bucket_name is None:
             bucket_name = self.bucket_name
         return self.obsClient.headBucket(bucket_name)
 
@@ -96,14 +100,17 @@
         :param delimiter:
         :param max_keys:
         :return: dict
         """
         _result = []
         resp = self.obsClient.listObjects(self.bucket_name, prefix=prefix, marker=marker, delimiter=delimiter,
                                           max_keys=max_keys)
+        if resp.status >= 300:
+            raise StorageRequestError(
+                f"static_code: {resp.status}, errorCode: {resp.errorCode}. Message: {resp.errorMessage}.")
         for obj in resp.body.contents:
             _result.append({
                 'key': obj['key'],
                 'url': self.get_file_url(key=obj['key']),
                 'size': obj['size']
             })
         return _result
@@ -188,15 +195,15 @@
         obs_headers = SetObjectMetadataHeader()
         obs_headers.contentType = headers.get('Content-Type')  # oss 和 obs的参数名称不相同
         self.obsClient.setObjectMetadata(self.bucket_name, key, obs_headers)
         return True
 
     def file_exists(self, key):
         """检查文件是否存在"""
-        resp = self.obsClient.getObjectMetadata(self.bucket_name, key)
+        resp = self.obsClient.headObject(self.bucket_name, key)
         if resp.get('status') == 200:
             return True
         elif resp.get('status') == 404:
             return False
 
     def get_object_meta(self, key: str):
         """获取文件基本元信息，包括该Object的ETag、Size（文件大小）、LastModified，Content-Type，并不返回其内容"""
@@ -216,8 +223,11 @@
         }
         resp = self.obsClient.getBucketCors(self.bucket_name)
         if resp.status < 300:
             for rule in resp.body:
                 cors_dict['allowed_origins'] = rule.allowedOrigin
                 cors_dict['allowed_headers'] = rule.allowedHeader
                 cors_dict['allowed_methods'] = rule.allowedMethod
-        return cors_dict
+            return cors_dict
+        else:
+            raise StorageRequestError(
+                f"static_code: {resp.status}, errorCode: {resp.errorCode}. Message: {resp.errorMessage}.")
```

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.44/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.44/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.44/yzcore/extensions/storage/oss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,29 +90,14 @@
                 cors_dict['allowed_origins'] = rule.allowed_origins
                 cors_dict['allowed_headers'] = rule.allowed_headers
                 cors_dict['allowed_methods'] = rule.allowed_methods
         except oss2.exceptions.NoSuchCors:
             pass
         return cors_dict
 
-    def iter_buckets(self, prefix='', marker='', max_keys=100, max_retries=None):
-        """
-        :param prefix: 只列举匹配该前缀的Bucket
-        :param marker: 分页符。只列举Bucket名字典序在此之后的Bucket
-        :param max_keys: 每次调用 `list_buckets` 时的max_keys参数。注意迭代器返回的数目可能会大于该值。
-        :param max_retries:
-        :return:
-        """
-        if not hasattr(self, 'service'):
-            self.service = oss2.Service(self.auth, self.endpoint)
-
-        return oss2.BucketIterator(
-            self.service, prefix=prefix, marker=marker,
-            max_keys=max_keys, max_retries=max_retries)
-
     def list_buckets(self, prefix='', marker='', max_keys=100, params=None):
         """根据前缀罗列用户的Bucket。
 
         :param str prefix: 只罗列Bucket名为该前缀的Bucket，空串表示罗列所有的Bucket
         :param str marker: 分页标志。首次调用传空串，后续使用返回值中的next_marker
         :param int max_keys: 每次调用最多返回的Bucket数目
         :param dict params: list操作参数，传入'tag-key','tag-value'对结果进行过滤
```

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.44/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.44/yzcore/extensions/storage/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/extensions/uid.py` & `yz-core2-1.0.44/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/logger/__init__.py` & `yz-core2-1.0.44/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/logger/config.py` & `yz-core2-1.0.44/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/logger/filters.py` & `yz-core2-1.0.44/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/logger/handlers.py` & `yz-core2-1.0.44/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/request/aio_http.py` & `yz-core2-1.0.44/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/response/response.py` & `yz-core2-1.0.44/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/response/response_code.py` & `yz-core2-1.0.44/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.44/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.44/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/app_template/views.py` & `yz-core2-1.0.44/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.44/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/project_template/README.md` & `yz-core2-1.0.44/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.44/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.44/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.44/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.44/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/utils/check_sys.py` & `yz-core2-1.0.44/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/utils/crypto.py` & `yz-core2-1.0.44/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/utils/encoding.py` & `yz-core2-1.0.44/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/utils/nacos.py` & `yz-core2-1.0.44/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.43/yzcore/utils/time_utils.py` & `yz-core2-1.0.44/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

