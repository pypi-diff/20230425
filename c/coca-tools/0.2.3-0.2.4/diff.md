# Comparing `tmp/coca_tools-0.2.3.tar.gz` & `tmp/coca_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coca_tools-0.2.3.tar", max compression
+gzip compressed data, was "coca_tools-0.2.4.tar", max compression
```

## Comparing `coca_tools-0.2.3.tar` & `coca_tools-0.2.4.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0      411 2023-04-25 04:42:42.991337 coca_tools-0.2.3/README.md
--rw-r--r--   0        0        0      792 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/__init__.py
--rw-r--r--   0        0        0      581 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/setup.py
--rw-r--r--   0        0        0      298 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0      199 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      104 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     6071 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2013 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      126 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.vscode/settings.json
--rw-r--r--   0        0        0     1270 2023-04-25 04:42:42.991337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile
--rw-r--r--   0        0        0     1926 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0     1007 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/__init__.py
--rw-r--r--   0        0        0     3314 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
--rw-r--r--   0        0        0       77 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/uvicorn.py
--rw-r--r--   0        0        0       73 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/postgres/.gitignore
--rw-r--r--   0        0        0       73 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/redis/.gitignore
--rw-r--r--   0        0        0      491 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/tutorials.md
--rw-r--r--   0        0        0       98 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/.gitignore
--rw-r--r--   0        0        0      968 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env
--rwxr-xr-x   0        0        0     1119 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py
--rw-r--r--   0        0        0     1288 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0      718 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      359 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/run.py
--rw-r--r--   0        0        0       71 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/__init__.py
--rw-r--r--   0        0        0       44 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/admin/__init__.py
--rw-r--r--   0        0        0      276 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/__init__.py
--rw-r--r--   0        0        0     1191 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py
--rw-r--r--   0        0        0       24 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/schemas/__init__.py
--rw-r--r--   0        0        0       24 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/utils/__init__.py
--rw-r--r--   0        0        0      179 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/apps.py
--rw-r--r--   0        0        0     7720 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/migrations/__init__.py
--rw-r--r--   0        0        0       44 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/serializers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tasks.py
--rw-r--r--   0        0        0       84 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tests.py
--rw-r--r--   0        0        0      158 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/urls.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/views/__init__.py
--rw-r--r--   0        0        0       54 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/__init__.py
--rw-r--r--   0        0        0      115 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/logger.py
--rw-r--r--   0        0        0      597 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py
--rw-r--r--   0        0        0      208 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/__init__.py
--rw-r--r--   0        0        0      394 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/api_router.py
--rw-r--r--   0        0        0      914 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py
--rw-r--r--   0        0        0     8484 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py
--rw-r--r--   0        0        0      883 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py
--rw-r--r--   0        0        0     2418 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py
--rw-r--r--   0        0        0      605 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py
--rw-r--r--   0        0        0     3108 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py
--rw-r--r--   0        0        0      377 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/elk_settings.py
--rw-r--r--   0        0        0      543 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py
--rw-r--r--   0        0        0      935 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py
--rw-r--r--   0        0        0     1288 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py
--rw-r--r--   0        0        0      570 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py
--rw-r--r--   0        0        0      773 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py
--rw-r--r--   0        0        0     1044 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py
--rw-r--r--   0        0        0     1096 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py
--rw-r--r--   0        0        0      126 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/security_settings.py
--rw-r--r--   0        0        0     1758 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py
--rw-r--r--   0        0        0      814 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py
--rw-r--r--   0        0        0      882 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py
--rw-r--r--   0        0        0     1556 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py
--rw-r--r--   0        0        0     1754 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/schema/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/staticfiles/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/static/.gitkeep
--rw-r--r--   0        0        0       37 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0      708 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/setup.py
--rw-r--r--   0        0        0      298 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0      199 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      103 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     6071 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2013 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.vscode/settings.json
--rw-r--r--   0        0        0     1270 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile
--rw-r--r--   0        0        0     1389 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0     1007 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/__init__.py
--rw-r--r--   0        0        0      216 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
--rw-r--r--   0        0        0       77 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/uvicorn.py
--rw-r--r--   0        0        0       74 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/mongo/.gitignore
--rw-r--r--   0        0        0       74 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/redis/.gitignore
--rw-r--r--   0        0        0      491 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/tutorials.md
--rw-r--r--   0        0        0       98 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/.gitignore
--rw-r--r--   0        0        0      761 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env
--rw-r--r--   0        0        0     1288 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0      640 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      359 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/run.py
--rw-r--r--   0        0        0        8 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/README.md
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/__init__.py
--rw-r--r--   0        0        0      550 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py
--rw-r--r--   0        0        0       34 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/__init__.py
--rw-r--r--   0        0        0      115 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/logger.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/__init__.py
--rw-r--r--   0        0        0      743 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py
--rw-r--r--   0        0        0     4172 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py
--rw-r--r--   0        0        0      178 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/__init__.py
--rw-r--r--   0        0        0      463 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/shutdown.py
--rw-r--r--   0        0        0      797 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py
--rw-r--r--   0        0        0      448 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/__init__.py
--rw-r--r--   0        0        0      644 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py
--rw-r--r--   0        0        0      638 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py
--rw-r--r--   0        0        0       75 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/__init__.py
--rw-r--r--   0        0        0      703 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py
--rw-r--r--   0        0        0     3613 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py
--rw-r--r--   0        0        0     1952 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/models/__init__.py
--rw-r--r--   0        0        0      241 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/__init__.py
--rw-r--r--   0        0        0      325 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/__init__.py
--rw-r--r--   0        0        0       61 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/__init__.py
--rw-r--r--   0        0        0      131 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/get_info.py
--rw-r--r--   0        0        0       70 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/__init__.py
--rw-r--r--   0        0        0      107 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/get_info.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/schemas/__init__.py
--rw-r--r--   0        0        0       64 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/__init__.py
--rw-r--r--   0        0        0      581 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py
--rw-r--r--   0        0        0     1032 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py
--rw-r--r--   0        0        0     2467 2023-04-25 04:42:42.995337 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py
--rw-r--r--   0        0        0      605 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py
--rw-r--r--   0        0        0     4228 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py
--rw-r--r--   0        0        0      378 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/elk_settings.py
--rw-r--r--   0        0        0      543 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py
--rw-r--r--   0        0        0      935 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py
--rw-r--r--   0        0        0     1288 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py
--rw-r--r--   0        0        0      575 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py
--rw-r--r--   0        0        0      773 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py
--rw-r--r--   0        0        0     1078 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py
--rw-r--r--   0        0        0      825 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py
--rw-r--r--   0        0        0      126 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/security_settings.py
--rw-r--r--   0        0        0     1758 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py
--rw-r--r--   0        0        0      814 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py
--rw-r--r--   0        0        0      882 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0      435 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/api_response.py
--rw-r--r--   0        0        0     6722 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py
--rw-r--r--   0        0        0      659 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py
--rw-r--r--   0        0        0      977 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py
--rw-r--r--   0        0        0      579 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py
--rw-r--r--   0        0        0      417 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/__init__.py
--rw-r--r--   0        0        0      114 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/client_events.py
--rw-r--r--   0        0        0      114 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/server_events.py
--rw-r--r--   0        0        0        0 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/static/.gitkeep
--rw-r--r--   0        0        0       37 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0      270 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_fastapi_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-25 04:42:42.999338 coca_tools-0.2.3/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0     1360 2023-04-25 04:42:42.999338 coca_tools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 coca_tools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      411 2023-04-25 05:01:29.395868 coca_tools-0.2.4/README.md
+-rw-r--r--   0        0        0      737 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/__init__.py
+-rw-r--r--   0        0        0      581 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/setup.py
+-rw-r--r--   0        0        0      298 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0      199 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      104 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     6071 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2013 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      126 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     1270 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile
+-rw-r--r--   0        0        0     1926 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1007 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/__init__.py
+-rw-r--r--   0        0        0     3314 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
+-rw-r--r--   0        0        0       77 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/uvicorn.py
+-rw-r--r--   0        0        0       73 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/postgres/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/redis/.gitignore
+-rw-r--r--   0        0        0      491 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/tutorials.md
+-rw-r--r--   0        0        0       98 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/.gitignore
+-rw-r--r--   0        0        0      968 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env
+-rwxr-xr-x   0        0        0     1119 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py
+-rw-r--r--   0        0        0     1288 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0      718 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      359 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/run.py
+-rw-r--r--   0        0        0       71 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/admin/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/__init__.py
+-rw-r--r--   0        0        0     1191 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py
+-rw-r--r--   0        0        0       24 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/schemas/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/utils/__init__.py
+-rw-r--r--   0        0        0      179 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/apps.py
+-rw-r--r--   0        0        0     7720 2023-04-25 05:01:29.395868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/migrations/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/serializers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tasks.py
+-rw-r--r--   0        0        0       84 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tests.py
+-rw-r--r--   0        0        0      158 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/urls.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/views/__init__.py
+-rw-r--r--   0        0        0       54 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/logger.py
+-rw-r--r--   0        0        0      597 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py
+-rw-r--r--   0        0        0      208 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/api_router.py
+-rw-r--r--   0        0        0      914 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py
+-rw-r--r--   0        0        0     8484 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py
+-rw-r--r--   0        0        0      883 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py
+-rw-r--r--   0        0        0     2418 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py
+-rw-r--r--   0        0        0      605 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py
+-rw-r--r--   0        0        0     3108 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py
+-rw-r--r--   0        0        0      377 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/elk_settings.py
+-rw-r--r--   0        0        0      543 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py
+-rw-r--r--   0        0        0      935 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py
+-rw-r--r--   0        0        0     1288 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py
+-rw-r--r--   0        0        0      570 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py
+-rw-r--r--   0        0        0      773 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py
+-rw-r--r--   0        0        0     1044 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py
+-rw-r--r--   0        0        0     1096 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py
+-rw-r--r--   0        0        0      126 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/security_settings.py
+-rw-r--r--   0        0        0     1265 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py
+-rw-r--r--   0        0        0      755 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py
+-rw-r--r--   0        0        0      882 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py
+-rw-r--r--   0        0        0     1556 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py
+-rw-r--r--   0        0        0     1754 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/schema/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/staticfiles/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/static/.gitkeep
+-rw-r--r--   0        0        0       37 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/setup.py
+-rw-r--r--   0        0        0      298 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0      199 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      103 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     6071 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2013 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     1270 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile
+-rw-r--r--   0        0        0     1389 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1007 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
+-rw-r--r--   0        0        0       77 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/uvicorn.py
+-rw-r--r--   0        0        0       74 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/mongo/.gitignore
+-rw-r--r--   0        0        0       74 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/redis/.gitignore
+-rw-r--r--   0        0        0      491 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/tutorials.md
+-rw-r--r--   0        0        0       98 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/.gitignore
+-rw-r--r--   0        0        0      761 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env
+-rw-r--r--   0        0        0     1288 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0      640 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      359 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/run.py
+-rw-r--r--   0        0        0        8 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/__init__.py
+-rw-r--r--   0        0        0      550 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py
+-rw-r--r--   0        0        0       34 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/logger.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py
+-rw-r--r--   0        0        0     4172 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py
+-rw-r--r--   0        0        0      178 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/shutdown.py
+-rw-r--r--   0        0        0      797 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py
+-rw-r--r--   0        0        0      448 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py
+-rw-r--r--   0        0        0      638 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py
+-rw-r--r--   0        0        0       75 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/__init__.py
+-rw-r--r--   0        0        0      703 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py
+-rw-r--r--   0        0        0     3613 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py
+-rw-r--r--   0        0        0     1952 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/models/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/get_info.py
+-rw-r--r--   0        0        0       70 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/get_info.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/schemas/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/__init__.py
+-rw-r--r--   0        0        0      581 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py
+-rw-r--r--   0        0        0     1032 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py
+-rw-r--r--   0        0        0     2467 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py
+-rw-r--r--   0        0        0      605 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py
+-rw-r--r--   0        0        0     4228 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py
+-rw-r--r--   0        0        0      378 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/elk_settings.py
+-rw-r--r--   0        0        0      543 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py
+-rw-r--r--   0        0        0      935 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py
+-rw-r--r--   0        0        0     1288 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py
+-rw-r--r--   0        0        0      575 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py
+-rw-r--r--   0        0        0      773 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py
+-rw-r--r--   0        0        0     1078 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py
+-rw-r--r--   0        0        0      825 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py
+-rw-r--r--   0        0        0      126 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/security_settings.py
+-rw-r--r--   0        0        0     1758 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py
+-rw-r--r--   0        0        0      814 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py
+-rw-r--r--   0        0        0      882 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0      435 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/api_response.py
+-rw-r--r--   0        0        0     6722 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py
+-rw-r--r--   0        0        0      659 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py
+-rw-r--r--   0        0        0      977 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py
+-rw-r--r--   0        0        0      579 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py
+-rw-r--r--   0        0        0      417 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/client_events.py
+-rw-r--r--   0        0        0      114 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/server_events.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/static/.gitkeep
+-rw-r--r--   0        0        0       37 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-25 05:01:29.399868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-25 05:01:29.403868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-25 05:01:29.403868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_fastapi_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-25 05:01:29.403868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-25 05:01:29.403868 coca_tools-0.2.4/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     1360 2023-04-25 05:01:29.403868 coca_tools-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 coca_tools-0.2.4/PKG-INFO
```

### Comparing `coca_tools-0.2.3/cocatools/__init__.py` & `coca_tools-0.2.4/cocatools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 
 """Entry point of my coca tools
 """
 import os
 
 from cookiecutter.main import cookiecutter
 
-<<<<<<< HEAD
-__version__ = '0.2.2'
-=======
-__version__ = '0.2.3'
->>>>>>> dev
+__version__ = '0.2.4'
 BASE_PATH = os.path.dirname(os.path.abspath(__file__))
 TEMPLATE_PATH = os.path.join(BASE_PATH, 'cookiecutter_templates')
 
 
 def welcome():
     """Say welcome to users"""
     print('welcome to coca tools')
```

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/cookiecutter.json` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 class AppSocketIoSetting(BaseSettingMixin):
     WS_SERVER_ENABLE: bool = False
     WS_SERVER_ENABLE_DEBUGGING: bool = False
     # ``'*'`` to allow all origins, or to ``[]`` to disable CORS handling, tested
     WS_SERVER_CORS_ORIGINS: Union[str, List] = '*'
-    WS_SERVER_MOUNT_LOCATION: str = '{{ cookiecutter.ws_app_mount_path }}'
-    WS_SERVER_SOCKETIO_PATH: str = '{{ cookiecutter.ws_socketio_path }}'
+    WS_SERVER_MOUNT_LOCATION: str = '/ws'
+    WS_SERVER_SOCKETIO_PATH: str = 'socket.io'
     WS_SERVER_KEEP_ALIVE: int = 120
     WS_SERVER_MAX_FILE_SIZE: int = 90 * (10**6)  # bytes  -> 10 Mb
     WS_SERVER_PING_TIMEOUT: int = 5  # s        -> 30 s
     WS_SERVER_PING_INTERVAL: int = 25  # s        -> 30 s
 
     class Config:
         case_sensitive = True
```

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,30 +26,14 @@
     PROJECT_DESCRIPTION: str = '{{ cookiecutter.project_short_description }}'
 
     # Service proxy
     SERVICE_USE_PROXY: Optional[bool] = False
     SERVICE_PROXY_ADDR: Optional[str] = ''
     SERVICE_NO_PROXY: Optional[str] = ''
 
-    {% if cookiecutter.enable_api_app == 'yes' %}
-    SERVICE_ENABLE_API: bool = True
-    {% else %}
-    SERVICE_ENABLE_API: bool = False
-    {% endif %}
-    SERVICE_API_MOUNT_PATH: Optional[str] = '{{ cookiecutter.api_app_mount_path }}'
-
-
-    {% if cookiecutter.enable_ws_app == 'yes' %}
-    SERVICE_SOCKETIO_ENABLE: bool = True
-    {% else %}
-    SERVICE_SOCKETIO_ENABLE: bool = False
-    {% endif %}
-    SERVICE_SOCKETIO_MOUNT_PATH: Optional[str] = '{{ cookiecutter.ws_app_mount_path }}'
-
-
     def get_service_info(self) -> Dict:
         return {
             'name': self.PROJECT_NAME,
             'port': self.SERVICE_PORT,
             'code': self.SERVICE_CODE
         }
```

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py` & `coca_tools-0.2.4/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.3/pyproject.toml` & `coca_tools-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Coca-tools"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["NhanDD <hp.duongducnhan@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cocatools"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `coca_tools-0.2.3/PKG-INFO` & `coca_tools-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coca-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: NhanDD
 Author-email: hp.duongducnhan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

