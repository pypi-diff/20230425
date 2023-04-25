# Comparing `tmp/coca_tools-0.2.1.tar.gz` & `tmp/coca_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coca_tools-0.2.1.tar", max compression
+gzip compressed data, was "coca_tools-0.2.2.tar", max compression
```

## Comparing `coca_tools-0.2.1.tar` & `coca_tools-0.2.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0      875 2023-04-24 10:27:39.886117 coca_tools-0.2.1/README.md
--rw-r--r--   0        0        0      737 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/__init__.py
--rw-r--r--   0        0        0      760 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/setup.py
--rw-r--r--   0        0        0      298 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0      199 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      104 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     6071 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2013 2023-04-24 10:27:39.886117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      126 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.vscode/settings.json
--rw-r--r--   0        0        0     1270 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile
--rw-r--r--   0        0        0     1926 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0        8 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/__init__.py
--rw-r--r--   0        0        0     3314 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
--rw-r--r--   0        0        0       77 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/uvicorn.py
--rw-r--r--   0        0        0       73 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/postgres/.gitignore
--rw-r--r--   0        0        0       73 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/redis/.gitignore
--rw-r--r--   0        0        0      491 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/tutorials.md
--rw-r--r--   0        0        0       98 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/.gitignore
--rw-r--r--   0        0        0      968 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env
--rwxr-xr-x   0        0        0     1119 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py
--rw-r--r--   0        0        0     1288 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0      718 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      359 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/run.py
--rw-r--r--   0        0        0       71 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/__init__.py
--rw-r--r--   0        0        0       44 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/admin/__init__.py
--rw-r--r--   0        0        0      276 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/__init__.py
--rw-r--r--   0        0        0     1191 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py
--rw-r--r--   0        0        0       24 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/schemas/__init__.py
--rw-r--r--   0        0        0       24 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/utils/__init__.py
--rw-r--r--   0        0        0      179 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/apps.py
--rw-r--r--   0        0        0     7720 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/migrations/__init__.py
--rw-r--r--   0        0        0       44 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/serializers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tasks.py
--rw-r--r--   0        0        0       84 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tests.py
--rw-r--r--   0        0        0      158 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/urls.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/views/__init__.py
--rw-r--r--   0        0        0       54 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/__init__.py
--rw-r--r--   0        0        0      115 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/logger.py
--rw-r--r--   0        0        0      597 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py
--rw-r--r--   0        0        0      208 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/__init__.py
--rw-r--r--   0        0        0      394 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/api_router.py
--rw-r--r--   0        0        0      914 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py
--rw-r--r--   0        0        0     8484 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py
--rw-r--r--   0        0        0      883 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py
--rw-r--r--   0        0        0     2418 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py
--rw-r--r--   0        0        0      605 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py
--rw-r--r--   0        0        0     3108 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py
--rw-r--r--   0        0        0      377 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/elk_settings.py
--rw-r--r--   0        0        0      543 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py
--rw-r--r--   0        0        0      935 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py
--rw-r--r--   0        0        0     1288 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py
--rw-r--r--   0        0        0      570 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py
--rw-r--r--   0        0        0      773 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py
--rw-r--r--   0        0        0     1044 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py
--rw-r--r--   0        0        0     1096 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py
--rw-r--r--   0        0        0      126 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/security_settings.py
--rw-r--r--   0        0        0     1758 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py
--rw-r--r--   0        0        0      814 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py
--rw-r--r--   0        0        0      882 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py
--rw-r--r--   0        0        0     1556 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py
--rw-r--r--   0        0        0     1754 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/schema/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/staticfiles/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/static/.gitkeep
--rw-r--r--   0        0        0       37 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0      708 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/setup.py
--rw-r--r--   0        0        0      298 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.bumpversion.cfg
--rw-r--r--   0        0        0      199 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      103 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     6071 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2013 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.vscode/settings.json
--rw-r--r--   0        0        0     1270 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile
--rw-r--r--   0        0        0     1379 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0        8 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/__init__.py
--rw-r--r--   0        0        0      216 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
--rw-r--r--   0        0        0       77 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/uvicorn.py
--rw-r--r--   0        0        0       74 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/mongo/.gitignore
--rw-r--r--   0        0        0       74 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/redis/.gitignore
--rw-r--r--   0        0        0      491 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/tutorials.md
--rw-r--r--   0        0        0       98 2023-04-24 10:27:39.890117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/.gitignore
--rw-r--r--   0        0        0      761 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env
--rw-r--r--   0        0        0     1288 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml
--rw-r--r--   0        0        0      640 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      359 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/run.py
--rw-r--r--   0        0        0        8 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/README.md
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/__init__.py
--rw-r--r--   0        0        0      550 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py
--rw-r--r--   0        0        0       34 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/__init__.py
--rw-r--r--   0        0        0      115 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/logger.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/__init__.py
--rw-r--r--   0        0        0      743 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py
--rw-r--r--   0        0        0     4172 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py
--rw-r--r--   0        0        0      178 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/__init__.py
--rw-r--r--   0        0        0      463 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/shutdown.py
--rw-r--r--   0        0        0      797 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py
--rw-r--r--   0        0        0      448 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/__init__.py
--rw-r--r--   0        0        0      644 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py
--rw-r--r--   0        0        0      638 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py
--rw-r--r--   0        0        0       75 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/__init__.py
--rw-r--r--   0        0        0      703 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py
--rw-r--r--   0        0        0     3613 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py
--rw-r--r--   0        0        0     1952 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/models/__init__.py
--rw-r--r--   0        0        0      241 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/__init__.py
--rw-r--r--   0        0        0      325 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/__init__.py
--rw-r--r--   0        0        0       61 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/__init__.py
--rw-r--r--   0        0        0      131 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/get_info.py
--rw-r--r--   0        0        0       70 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/__init__.py
--rw-r--r--   0        0        0      107 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/get_info.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/schemas/__init__.py
--rw-r--r--   0        0        0       64 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/__init__.py
--rw-r--r--   0        0        0      581 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py
--rw-r--r--   0        0        0     1032 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py
--rw-r--r--   0        0        0     2467 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py
--rw-r--r--   0        0        0      605 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py
--rw-r--r--   0        0        0     4228 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py
--rw-r--r--   0        0        0      378 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/elk_settings.py
--rw-r--r--   0        0        0      543 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py
--rw-r--r--   0        0        0      935 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py
--rw-r--r--   0        0        0     1288 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py
--rw-r--r--   0        0        0      575 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py
--rw-r--r--   0        0        0      773 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py
--rw-r--r--   0        0        0     1078 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py
--rw-r--r--   0        0        0      825 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py
--rw-r--r--   0        0        0      126 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/security_settings.py
--rw-r--r--   0        0        0     1758 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py
--rw-r--r--   0        0        0      814 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py
--rw-r--r--   0        0        0      882 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0      435 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/api_response.py
--rw-r--r--   0        0        0     6722 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py
--rw-r--r--   0        0        0      659 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py
--rw-r--r--   0        0        0      977 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py
--rw-r--r--   0        0        0      579 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py
--rw-r--r--   0        0        0      417 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/__init__.py
--rw-r--r--   0        0        0      114 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/client_events.py
--rw-r--r--   0        0        0      114 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/server_events.py
--rw-r--r--   0        0        0        0 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/static/.gitkeep
--rw-r--r--   0        0        0       37 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0      270 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      270 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_fastapi_template/cookiecutter.json
--rw-r--r--   0        0        0      328 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_fastapi_template/setup.py
--rw-r--r--   0        0        0        8 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      340 2023-04-24 10:27:39.894117 coca_tools-0.2.1/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0     1360 2023-04-24 10:27:39.894117 coca_tools-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 coca_tools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2023-04-24 15:46:36.775037 coca_tools-0.2.2/README.md
+-rw-r--r--   0        0        0      737 2023-04-24 15:46:36.775037 coca_tools-0.2.2/cocatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.775037 coca_tools-0.2.2/cocatools/cookiecutter_templates/__init__.py
+-rw-r--r--   0        0        0      760 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/setup.py
+-rw-r--r--   0        0        0      298 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0      199 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      104 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     6071 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2013 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      126 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     1270 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile
+-rw-r--r--   0        0        0     1926 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1007 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/__init__.py
+-rw-r--r--   0        0        0     3314 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
+-rw-r--r--   0        0        0       77 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/uvicorn.py
+-rw-r--r--   0        0        0       73 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/postgres/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/data/redis/.gitignore
+-rw-r--r--   0        0        0      491 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/docs/tutorials.md
+-rw-r--r--   0        0        0       98 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/.gitignore
+-rw-r--r--   0        0        0      968 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env
+-rwxr-xr-x   0        0        0     1119 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py
+-rw-r--r--   0        0        0     1288 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0      718 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      359 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/run.py
+-rw-r--r--   0        0        0       71 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/admin/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/__init__.py
+-rw-r--r--   0        0        0     1191 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py
+-rw-r--r--   0        0        0       24 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/schemas/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/utils/__init__.py
+-rw-r--r--   0        0        0      179 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/apps.py
+-rw-r--r--   0        0        0     7720 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/migrations/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/serializers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tasks.py
+-rw-r--r--   0        0        0       84 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/tests.py
+-rw-r--r--   0        0        0      158 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/urls.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/views/__init__.py
+-rw-r--r--   0        0        0       54 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/constants/logger.py
+-rw-r--r--   0        0        0      597 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py
+-rw-r--r--   0        0        0      208 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/api_router.py
+-rw-r--r--   0        0        0      914 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py
+-rw-r--r--   0        0        0     8484 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py
+-rw-r--r--   0        0        0      883 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py
+-rw-r--r--   0        0        0     2418 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py
+-rw-r--r--   0        0        0      605 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py
+-rw-r--r--   0        0        0     3108 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py
+-rw-r--r--   0        0        0      377 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/elk_settings.py
+-rw-r--r--   0        0        0      543 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py
+-rw-r--r--   0        0        0      935 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py
+-rw-r--r--   0        0        0     1288 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py
+-rw-r--r--   0        0        0      570 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py
+-rw-r--r--   0        0        0      773 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py
+-rw-r--r--   0        0        0     1044 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py
+-rw-r--r--   0        0        0     1096 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py
+-rw-r--r--   0        0        0      126 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/security_settings.py
+-rw-r--r--   0        0        0     1758 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py
+-rw-r--r--   0        0        0      814 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py
+-rw-r--r--   0        0        0      882 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py
+-rw-r--r--   0        0        0     1556 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py
+-rw-r--r--   0        0        0     1754 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/schema/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/staticfiles/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/static/.gitkeep
+-rw-r--r--   0        0        0       37 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/setup.py
+-rw-r--r--   0        0        0      298 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.bumpversion.cfg
+-rw-r--r--   0        0        0      199 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      103 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     6071 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2013 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     1270 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile
+-rw-r--r--   0        0        0     1389 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0     1007 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py
+-rw-r--r--   0        0        0       77 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/configs/uvicorn.py
+-rw-r--r--   0        0        0       74 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/mongo/.gitignore
+-rw-r--r--   0        0        0       74 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/data/redis/.gitignore
+-rw-r--r--   0        0        0      491 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/docs/tutorials.md
+-rw-r--r--   0        0        0       98 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/.gitignore
+-rw-r--r--   0        0        0      761 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env
+-rw-r--r--   0        0        0     1288 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml
+-rw-r--r--   0        0        0      640 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      359 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/run.py
+-rw-r--r--   0        0        0        8 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/__init__.py
+-rw-r--r--   0        0        0      550 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py
+-rw-r--r--   0        0        0       34 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/constants/logger.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.779037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py
+-rw-r--r--   0        0        0     4172 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py
+-rw-r--r--   0        0        0      178 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/shutdown.py
+-rw-r--r--   0        0        0      797 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py
+-rw-r--r--   0        0        0      448 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py
+-rw-r--r--   0        0        0      638 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py
+-rw-r--r--   0        0        0       75 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/__init__.py
+-rw-r--r--   0        0        0      703 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py
+-rw-r--r--   0        0        0     3613 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py
+-rw-r--r--   0        0        0     1952 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/models/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/schema/get_info.py
+-rw-r--r--   0        0        0       70 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/routers/example/utils/get_info.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/schemas/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/__init__.py
+-rw-r--r--   0        0        0      581 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py
+-rw-r--r--   0        0        0     1032 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py
+-rw-r--r--   0        0        0     2467 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py
+-rw-r--r--   0        0        0      605 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py
+-rw-r--r--   0        0        0     4228 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py
+-rw-r--r--   0        0        0      378 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/elk_settings.py
+-rw-r--r--   0        0        0      543 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py
+-rw-r--r--   0        0        0      935 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py
+-rw-r--r--   0        0        0     1288 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py
+-rw-r--r--   0        0        0      575 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py
+-rw-r--r--   0        0        0      773 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py
+-rw-r--r--   0        0        0     1078 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py
+-rw-r--r--   0        0        0      825 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py
+-rw-r--r--   0        0        0      126 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/security_settings.py
+-rw-r--r--   0        0        0     1758 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py
+-rw-r--r--   0        0        0      814 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py
+-rw-r--r--   0        0        0      882 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0      435 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/api_response.py
+-rw-r--r--   0        0        0     6722 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py
+-rw-r--r--   0        0        0      659 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py
+-rw-r--r--   0        0        0      977 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py
+-rw-r--r--   0        0        0      579 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py
+-rw-r--r--   0        0        0      417 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/client_events.py
+-rw-r--r--   0        0        0      114 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws_events/server_events.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/static/.gitkeep
+-rw-r--r--   0        0        0       37 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_django_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_fastapi_template/cookiecutter.json
+-rw-r--r--   0        0        0      328 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_fastapi_template/setup.py
+-rw-r--r--   0        0        0        8 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      340 2023-04-24 15:46:36.783037 coca_tools-0.2.2/cocatools/cookiecutter_templates/monorepo_fastapi_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     1360 2023-04-24 15:46:36.783037 coca_tools-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 coca_tools-0.2.2/PKG-INFO
```

### Comparing `coca_tools-0.2.1/cocatools/__init__.py` & `coca_tools-0.2.2/cocatools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Entry point of my coca tools
 """
 import os
 
 from cookiecutter.main import cookiecutter
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 BASE_PATH = os.path.dirname(os.path.abspath(__file__))
 TEMPLATE_PATH = os.path.join(BASE_PATH, 'cookiecutter_templates')
 
 
 def welcome():
     """Say welcome to users"""
     print('welcome to coca tools')
```

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/cookiecutter.json` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/Makefile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/configs/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/envs/example.env`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/manage.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/api/example.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/apps/example/db_initializers.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/db_initializer.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/env_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/base_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/celery_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/db_mongo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/django_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/example_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/facebook_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/gunicorn_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/minio_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/nats_setting.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/redis_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/service_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/socketio_app_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/templates/zalo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/urls.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/django_template/{{cookiecutter.project_name}}/src/project/wsgi.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -42,10 +42,10 @@
 	if [ -z $(shell docker ps -aq -f name={{cookiecutter.project_slug}}-app) ]; then \
 		echo "not found container"; \
 	else \
 		docker rm -f {{cookiecutter.project_slug}}-app;  \
 	fi
 
 docker-up:
-	docker-down
-	docker-build
+	make docker-down
+	make docker-build
 	docker run --name {{cookiecutter.project_slug}}-app -p {{cookiecutter.port}}:{{cookiecutter.port}} -d {{cookiecutter.project_slug}}-app-image
```

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/envs/example.env`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/api.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/dbs/redis_cache/client_manager.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/events/startup.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/error_response_handler.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exc_handlers/request_validation_error_handler.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/exceptions/error_response.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/all.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/__init__.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/base_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/celery_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/db_mongo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/django_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/example_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/facebook_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/gunicorn_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/minio_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/nats_setting.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/redis_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/service_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/socketio_app_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/settings/teamplates/zalo_settings.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/app_creators.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py` & `coca_tools-0.2.2/cocatools/cookiecutter_templates/fastapi_template/{{cookiecutter.project_name}}/src/ws.py`

 * *Files identical despite different names*

### Comparing `coca_tools-0.2.1/pyproject.toml` & `coca_tools-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Coca-tools"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["NhanDD <hp.duongducnhan@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cocatools"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `coca_tools-0.2.1/PKG-INFO` & `coca_tools-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coca-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: NhanDD
 Author-email: hp.duongducnhan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,43 +26,30 @@
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: pylint[spelling] (>=2.17.2,<3.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
 
-# Attention
-- First things to do when clone this monorepo , require python version >= 3.11 and < 4.0
+# Installation
+- Require python >= 3.10
+- using pip
     ```
-    $ make init
+    $ pip install coca-tools
     ```
-- Open vs-code by "Open workspace from file" -> select "backend.code-workspace"
-- Before working with any services
+- using poetry
     ```
-    # go to service source directory
-
-    $ poetry install
+    $ poetry add coca-tools
     ```
 
 
-# Create docs guides
-- detail instruction to setup mkdocs
-    ```
-    https://realpython.com/python-project-documentation-with-mkdocs/
-    ```
-- for monorepo
+# Guide
+- Require: using in global environment
+- create fastapi template with command then fill the questions
     ```
-    https://github.com/backstage/mkdocs-monorepo-plugin
-    ```
-- install packages
-    ```
-    $ poetry add mkdocs "mkdocstrings[python]" mkdocs-material mkdocs-autorefs mkdocs-monorepo-plugin
-
-    run command bellow to init mkdocs for project
-    $ poetry run mkdocs new .
+    $ create-fastapi-app
     ```
-- with vscode install "docstring" extension
-- Run docs server
+- create django template with command then fill the questions
     ```
-    $ make mkdocs-serve
+    $ create-django-app
     ```
```

