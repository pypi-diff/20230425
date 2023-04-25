# Comparing `tmp/qontract_development_cli-0.8.1.tar.gz` & `tmp/qontract_development_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qontract_development_cli-0.8.1.tar", max compression
+gzip compressed data, was "qontract_development_cli-0.9.0.tar", max compression
```

## Comparing `qontract_development_cli-0.8.1.tar` & `qontract_development_cli-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-03-17 08:56:23.329713 qontract_development_cli-0.8.1/LICENSE
--rw-r--r--   0        0        0    11689 2023-03-17 08:56:23.329713 qontract_development_cli-0.8.1/README.md
--rw-r--r--   0        0        0     1560 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/qontract_development_cli/__init__.py
--rw-r--r--   0        0        0      125 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/qontract_development_cli/__main__.py
--rw-r--r--   0        0        0     1313 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/qontract_development_cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/qontract_development_cli/commands/__init__.py
--rw-r--r--   0        0        0     2175 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/qontract_development_cli/commands/config.py
--rw-r--r--   0        0        0     1367 2023-03-17 08:56:23.332713 qontract_development_cli-0.8.1/qontract_development_cli/commands/env.py
--rw-r--r--   0        0        0    10908 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/commands/profile.py
--rw-r--r--   0        0        0      186 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/completions.py
--rw-r--r--   0        0        0     2028 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/config.py
--rw-r--r--   0        0        0     5229 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/models.py
--rw-r--r--   0        0        0     5212 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/shell.py
--rw-r--r--   0        0        0     3198 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/templates/compose.yml.j2
--rw-r--r--   0        0        0      505 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/templates/prep-worktree.sh.j2
--rw-r--r--   0        0        0      339 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/templates.py
--rw-r--r--   0        0        0      637 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/utils.py
--rw-r--r--   0        0        0     1448 2023-03-17 08:56:23.333713 qontract_development_cli-0.8.1/qontract_development_cli/watchdog.py
--rw-r--r--   0        0        0    13036 1970-01-01 00:00:00.000000 qontract_development_cli-0.8.1/setup.py
--rw-r--r--   0        0        0    12702 1970-01-01 00:00:00.000000 qontract_development_cli-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-21 14:16:50.707378 qontract_development_cli-0.9.0/LICENSE
+-rw-r--r--   0        0        0    14301 2023-03-21 14:16:50.707378 qontract_development_cli-0.9.0/README.md
+-rw-r--r--   0        0        0     1560 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/__init__.py
+-rw-r--r--   0        0        0      125 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/__main__.py
+-rw-r--r--   0        0        0     1313 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/commands/__init__.py
+-rw-r--r--   0        0        0     2175 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/commands/config.py
+-rw-r--r--   0        0        0     1367 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/commands/env.py
+-rw-r--r--   0        0        0    10908 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/commands/profile.py
+-rw-r--r--   0        0        0      186 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/completions.py
+-rw-r--r--   0        0        0     2028 2023-03-21 14:16:50.710378 qontract_development_cli-0.9.0/qontract_development_cli/config.py
+-rw-r--r--   0        0        0     5298 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/models.py
+-rw-r--r--   0        0        0     5212 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/shell.py
+-rw-r--r--   0        0        0     4084 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/templates/compose.yml.j2
+-rw-r--r--   0        0        0      505 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/templates/prep-worktree.sh.j2
+-rw-r--r--   0        0        0      339 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/templates.py
+-rw-r--r--   0        0        0      637 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/utils.py
+-rw-r--r--   0        0        0     1448 2023-03-21 14:16:50.711378 qontract_development_cli-0.9.0/qontract_development_cli/watchdog.py
+-rw-r--r--   0        0        0    15652 1970-01-01 00:00:00.000000 qontract_development_cli-0.9.0/setup.py
+-rw-r--r--   0        0        0    15314 1970-01-01 00:00:00.000000 qontract_development_cli-0.9.0/PKG-INFO
```

### Comparing `qontract_development_cli-0.8.1/LICENSE` & `qontract_development_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/README.md` & `qontract_development_cli-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -122,39 +122,41 @@
 * **rm**: Remove profile.
 * **run**: Run a profile.
 * **show**: Display profile.
 
 
 #### Settings
 
-| **Key**                        | **Description**                                                                            | **Default**                               |
-| ------------------------------ | ------------------------------------------------------------------------------------------ | ----------------------------------------- |
-| additional_environment         | Dictionary of additional environment variables to pass to the qontract-reconcile container | `{}`                                      |
-| container_uid                  | Change ownership of /recconcile files in container to this user id                         | current UID                               |
-| debugger                       | Python debugger                                                                            | debugpy                                   |
-| dry_run                        | Run --dry-run mode                                                                         | true                                      |
-| **integration_name**           | Intergration name                                                                          |                                           |
-| **integration_extra_args**     | Intergration extra arguments                                                               |                                           |
-| log_level                      | Log level                                                                                  | info                                      |
-| app_interface_path             | App-interface instance path. (Overrides *env.app_interface_path*)                          |                                           |
-| app_interface_pr               | App-interface PR/MR number                                                                 |                                           |
-| app_interface_upstream         | Upstream remote name                                                                       | upstream                                  |
-| qontract_reconcile_build_image | Build qontract-reconcile image                                                             | true                                      |
-| qontract_reconcile_image       | Qontract-reconcile image                                                                   | quay.io/app-sre/qontract-reconcile:latest |
-| qontract_reconcile_path        | Qontract-reconcile path                                                                    | ~/workspace/qontract-reconcile            |
-| qontract_reconcile_pr          | Qontract-reconcile PR/MR number                                                            |                                           |
-| qontract_reconcile_upstream    | Upstream remote name                                                                       | upstream                                  |
-| qontract_server_build_image    | Build qontract-server image                                                                | true                                      |
-| qontract_server_image          | Qontract-server image                                                                      | quay.io/app-sre/qontract-server:latest    |
-| qontract_server_path           | Qontract-server path                                                                       | ~/workspace/qontract-server               |
-| qontract_schemas_path          | Qontract-schemas path                                                                      | ~/workspace/qontract-schemas              |
-| qontract_schemas_pr            | Qontract-schemas PR/MR number                                                              |                                           |
-| qontract_schemas_upstream      | Upstream remote name                                                                       | upstream                                  |
-| run_once                       | If 'true', execute the integration once and exit                                           | true                                      |
-| sleep_duration_secs            | If not *run_once*, sleep duration until integration runs again                             | 10                                        |
+| **Key**                        | **Description**                                                                                                                                                              | **Default**                                 |
+| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
+| additional_environment         | Dictionary of additional environment variables to pass to the qontract-reconcile container                                                                                   | `{}`                                        |
+| container_uid                  | Change ownership of /recconcile files in container to this user id                                                                                                           | current UID                                 |
+| debugger                       | Python debugger                                                                                                                                                              | `debugpy`                                   |
+| dry_run                        | Run --dry-run mode                                                                                                                                                           | `true`                                      |
+| extra_hosts                    | List of 'HOSTNAME:IP' mapping entries for qontract-reconcile `/etc/hosts`. See [extra_hosts](https://docs.docker.com/compose/compose-file/#extra_hosts) docker compose file. | `[]`                                        |
+| **integration_name**           | Intergration name                                                                                                                                                            |                                             |
+| **integration_extra_args**     | Intergration extra arguments                                                                                                                                                 |                                             |
+| **internal_redhat_ca**         | Inject Red Hat internal CAs and `REQUESTS_CA_BUNDLE` environment variable                                                                                                    | `false`                                     |
+| log_level                      | Log level                                                                                                                                                                    | `info`                                      |
+| app_interface_path             | App-interface instance path. (Overrides *env.app_interface_path*)                                                                                                            |                                             |
+| app_interface_pr               | App-interface PR/MR number                                                                                                                                                   |                                             |
+| app_interface_upstream         | Upstream remote name                                                                                                                                                         | `upstream`                                  |
+| qontract_reconcile_build_image | Build qontract-reconcile image                                                                                                                                               | `true`                                      |
+| qontract_reconcile_image       | Qontract-reconcile image                                                                                                                                                     | `quay.io/app-sre/qontract-reconcile:latest` |
+| qontract_reconcile_path        | Qontract-reconcile path                                                                                                                                                      | `~/workspace/qontract-reconcile`            |
+| qontract_reconcile_pr          | Qontract-reconcile PR/MR number                                                                                                                                              |                                             |
+| qontract_reconcile_upstream    | Upstream remote name                                                                                                                                                         | `upstream`                                  |
+| qontract_server_build_image    | Build qontract-server image                                                                                                                                                  | `true`                                      |
+| qontract_server_image          | Qontract-server image                                                                                                                                                        | `quay.io/app-sre/qontract-server:lates`t    |
+| qontract_server_path           | Qontract-server path                                                                                                                                                         | `~/workspace/qontract-server`               |
+| qontract_schemas_path          | Qontract-schemas path                                                                                                                                                        | `~/workspace/qontract-schemas`              |
+| qontract_schemas_pr            | Qontract-schemas PR/MR number                                                                                                                                                |                                             |
+| qontract_schemas_upstream      | Upstream remote name                                                                                                                                                         | `upstream`                                  |
+| run_once                       | If 'true', execute the integration once and exit                                                                                                                             | `true`                                      |
+| sleep_duration_secs            | If not *run_once*, sleep duration until integration runs again                                                                                                               | `10`                                        |
 
 > :point_right: **Bold keys** are mandatory or should be customized.
 
 ### PR/MR support
 
 It's a pretty handy feature to create a profile from a pull request (merge request). E.g.:
```

### Comparing `qontract_development_cli-0.8.1/pyproject.toml` & `qontract_development_cli-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qontract-development-cli"
-version = "0.8.1"
+version = "0.9.0"
 description = "Helper tool for qontract-reconcile development"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/chassing/qontract-development-cli"
 homepage = "http://github.com/chassing/qontract-development-cli"
 
@@ -49,15 +49,15 @@
 
 [[tool.mypy.overrides]]
 module = ["getkey.*"]
 ignore_missing_imports = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.1"
+version = "0.9.0"
 version_files = ["pyproject.toml:version"]
 update_changelog_on_bump = true
 major_version_zero = true
 change_type_map = { "feat" = "Features", "fix" = "Bug Fixes" }
 tag_format = "v$version"
 
 [tool.isort]
```

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/cli.py` & `qontract_development_cli-0.9.0/qontract_development_cli/cli.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/commands/config.py` & `qontract_development_cli-0.9.0/qontract_development_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/commands/env.py` & `qontract_development_cli-0.9.0/qontract_development_cli/commands/env.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/commands/profile.py` & `qontract_development_cli-0.9.0/qontract_development_cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/config.py` & `qontract_development_cli-0.9.0/qontract_development_cli/config.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/models.py` & `qontract_development_cli-0.9.0/qontract_development_cli/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     qontract_server_path: Path = Path("~/workspace/qontract-server")
     qontract_schemas_path: Path = Path("~/workspace/qontract-schemas")
     qontract_schemas_pr: Optional[int] = None
     qontract_schemas_upstream: str = "upstream"
     run_once: bool = True
     sleep_duration_secs: int = 10
     additional_environment: dict[str, Any] = {}
+    internal_redhat_ca: bool = False
+    extra_hosts: list[str] = []
 
 
 class Base(BaseModel):
     name: str
     default: bool = False
     _root: Path
```

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/shell.py` & `qontract_development_cli-0.9.0/qontract_development_cli/shell.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/templates/compose.yml.j2` & `qontract_development_cli-0.9.0/qontract_development_cli/templates/compose.yml.j2`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 ---
 name: {{ config.docker_compose_project_name }}
 services:
 
+{% if profile.settings.internal_redhat_ca %}
+  internal-certificates:
+    image: quay.io/app-sre/internal-redhat-ca:latest
+    container_name: internal-certificates
+    command: |
+      sh -c 'cp -r /etc/pki/. /tmp/'
+    volumes:
+    - pki-volume:/tmp
+{% endif %}
 {% if env.settings.run_qontract_reconcile %}
   qontract-reconcile:
     container_name: qontract-reconcile-{{ profile.settings.integration_name }}
     stop_grace_period: 1s
     stop_signal: SIGKILL
     tty: true
     restart: unless-stopped
@@ -24,40 +33,57 @@
     - INTEGRATION_EXTRA_ARGS={{ profile.settings.integration_extra_args }}
     - DRY_RUN={% if profile.settings.dry_run %}--dry-run{% else %}--no-dry-run{%endif%}
     - SLEEP_DURATION_SECS={{ profile.settings.sleep_duration_secs }}
     - DEBUGGER={{ profile.settings.debugger }}
     - CONFIG=/config/{{ env.settings.config.name }}
     - APP_INTERFACE_STATE_BUCKET={{ env.settings.app_interface_state_bucket }}
     - APP_INTERFACE_STATE_BUCKET_ACCOUNT={{ env.settings.app_interface_state_bucket_account }}
+{% if profile.settings.internal_redhat_ca %}
+    - REQUESTS_CA_BUNDLE=/etc/pki/tls/cert.pem
+{% endif %}
 {% if  profile.settings.run_once %}
     - RUN_ONCE=1
 {% endif %}
     - gitlab_pr_submitter_queue_url={{ env.settings.gitlab_pr_submitter_queue_url }}
     - LOG_LEVEL={{ profile.settings.log_level.upper() }}
     {% for key, value in profile.settings.additional_environment.items() %}
     - {{ key }}={{ value }}
     {% endfor %}
     volumes:
     - {{ profile.settings.qontract_reconcile_path.expanduser().absolute() }}:/work
     - {{ env.settings.config.expanduser().absolute().parent }}:/config
     - tmp-volume:/tmp
+{% if profile.settings.internal_redhat_ca %}
+    - pki-volume:/etc/pki
+{% endif %}
 {% if env.settings.run_qontract_server or env.settings.run_vault %}
     links:
 {% endif %}
 {% if env.settings.run_qontract_server %}
     - qontract-server
 {% endif %}
 {% if env.settings.run_vault %}
     - vault
 {% endif %}
     ports:
     - 9090:9090 # Metrics Exporter
     - 5678:5678 # Debugger Port
     networks:
     - qontract-development
+{% if profile.settings.extra_hosts %}
+    extra_hosts:
+    {% for entry in profile.settings.extra_hosts %}
+    - "{{ entry }}"
+    {% endfor %}
+{% endif %}
+{% if profile.settings.internal_redhat_ca %}
+    depends_on:
+      internal-certificates:
+        condition: service_completed_successfully # Let the init container create the pki directory first
+{% endif %}
 {% endif %}
 
 {% if env.settings.run_qontract_server %}
   qontract-server:
     {% if profile.settings.qontract_server_build_image %}
     build:
       context: {{ profile.settings.qontract_server_path.expanduser().absolute() }}
@@ -90,11 +116,14 @@
     - 8200:8200
     networks:
     - qontract-development
 {% endif %}
 
 volumes:
   tmp-volume:
+{% if profile.settings.internal_redhat_ca %}
+  pki-volume:
+{% endif %}
 
 networks:
   qontract-development:
     name: qontract-development
```

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/utils.py` & `qontract_development_cli-0.9.0/qontract_development_cli/utils.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/qontract_development_cli/watchdog.py` & `qontract_development_cli-0.9.0/qontract_development_cli/watchdog.py`

 * *Files identical despite different names*

### Comparing `qontract_development_cli-0.8.1/setup.py` & `qontract_development_cli-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'watchfiles>=0.18.0,<0.19.0']
 
 entry_points = \
 {'console_scripts': ['qd = qontract_development_cli.__main__:app']}
 
 setup_kwargs = {
     'name': 'qontract-development-cli',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Helper tool for qontract-reconcile development',
-    'long_description': '# Qontract Development CLI\n\n[![PyPI](https://img.shields.io/pypi/v/qontract-development-cli)][pypi-link]\n[![PyPI platforms][pypi-platforms]][pypi-link]\n![PyPI - License](https://img.shields.io/pypi/l/qontract-development-cli)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)\n\nQontract Development CLI supports your daily [qontract-reconcile][qontract-reconcile] development work.\n\n## Installation\n\nYou can install this library from [PyPI][pypi-link] with `pip`:\n\n```shell\n$ python3 -m pip install qontract-development-cli\n```\n\nOr install it with `pipx`:\n```shell\n$ pipx install qontract-development-cli\n```\n\nYou can also use `pipx` to run the library without installing it:\n\n```shell\n$ pipx run qontract-development-cli\n```\n\n## Quickstart\n\n* Create initial configuration\n  ```shell\n  $ qd config init\n  ```\n  <img src="demo/qd_config_init.gif" />\n\n* Create a profile `sql-query` to run the `sql-query` integration\n  ```shell\n  $ qd profile create sql-query\n  ```\n  <img src="demo/qd_profile_create.gif" />\n\n* Run `sql-query` profile\n  ```shell\n  $ profile run dev sql-query\n  ```\n  <img src="images/profile_run_sql_query.svg" />\n\n## Features\n\nQontract Development CLI currently provides the following features (get help with `-h` or `--help`):\n\n- Run `qontract-reconcile` and `qontract-server` as docker containers on your local machine\n- Support for different environments (dev, prod, ...) via the `env` command\n- Configure your [qontract-reconcile integration][qontract-reconcile] with the `profile` command\n- Support pull request reviews (see `profile create`)\n- Bootstrap your initial configurations with the `config` command\n- Shell autocompletion (see `qd --help`)\n\n## Commands\n\n### Config\n\nManage global qontract-development CLI configuration.\n\n`qd config [sub-cmd] --help`\n\n* **edit**: open the configuration file in your favorite editor\n* **init**: create a default configuration\n\n#### Settings\n| **Key**                     | **Description**                       | **Default**                          |\n| --------------------------- | ------------------------------------- | ------------------------------------ |\n| debug                       | Enable/disable debug mode             | false                                |\n| defaults_profile            | Name of defaults profile              | defaults                             |\n| docker_compose_project_name | Docker compose project name           | qontract-development                 |\n| editor                      | Your favorite editor                  | $EDITOR or vim                       |\n| environments_dir            | Directory to store environment files  | User config directory / environments |\n| profiles_dir                | Directory to store profile files      | User config directory / profiles     |\n| worktrees_dir               | Directory to store git repo worktrees | User cache directory / worktrees     |\n\n\n## Environments\n\nAn environment specifies app-interface instance settings, e.g., **dev** vs. **prod** config and path to the actual app-interface instance.\n\n`qd env [sub-cmd] --help`\n\n* **edit**: Create/edit an environment file in your editor.\n* **ls**: List all available environments.\n* **rm**: Remove environment.\n* **show**: Display environment.\n\n\n#### Settings\n\n| **Key**                            | **Description**                      | **Default**                                    |\n| ---------------------------------- | ------------------------------------ | ---------------------------------------------- |\n| **app_interface_path**             | Path to local app-interface instance | ~/workspace/app-interface                      |\n| app_interface_state_bucket         | S3 bucket                            | empty                                          |\n| app_interface_state_bucket_account | AWS S3 account                       | empty                                          |\n| **config**                         | app-interface config                 | ~/workspace/qontract-reconcile/config.dev.toml |\n| gitlab_pr_submitter_queue_url      | Gitlab pr submitter queue url        |                                                |\n| run_qontract_reconcile             | Run qontract-reconcile container     | true                                           |\n| run_qontract_server                | Run qontract-server container        | true                                           |\n| run_vault                          | Run vault container                  | false                                          |\n\n> :point_right: **Bold keys** are mandatory or should be customized.\n\n## Profiles\n\nA profile specifies all settings to run a qontract-reconcile integration (e.g., *sql-query*).\n\n`qd profile [sub-cmd] --help`\n\n* **create**: Create a new profile to run an integration.\n\n  Supports the creation of a new profile from an open PR/MR. See `qd profile create --help` for all available options.\n\n* **edit**: Edit a profile in your editor.\n* **ls**: List all available profiles.\n* **rm**: Remove profile.\n* **run**: Run a profile.\n* **show**: Display profile.\n\n\n#### Settings\n\n| **Key**                        | **Description**                                                                            | **Default**                               |\n| ------------------------------ | ------------------------------------------------------------------------------------------ | ----------------------------------------- |\n| additional_environment         | Dictionary of additional environment variables to pass to the qontract-reconcile container | `{}`                                      |\n| container_uid                  | Change ownership of /recconcile files in container to this user id                         | current UID                               |\n| debugger                       | Python debugger                                                                            | debugpy                                   |\n| dry_run                        | Run --dry-run mode                                                                         | true                                      |\n| **integration_name**           | Intergration name                                                                          |                                           |\n| **integration_extra_args**     | Intergration extra arguments                                                               |                                           |\n| log_level                      | Log level                                                                                  | info                                      |\n| app_interface_path             | App-interface instance path. (Overrides *env.app_interface_path*)                          |                                           |\n| app_interface_pr               | App-interface PR/MR number                                                                 |                                           |\n| app_interface_upstream         | Upstream remote name                                                                       | upstream                                  |\n| qontract_reconcile_build_image | Build qontract-reconcile image                                                             | true                                      |\n| qontract_reconcile_image       | Qontract-reconcile image                                                                   | quay.io/app-sre/qontract-reconcile:latest |\n| qontract_reconcile_path        | Qontract-reconcile path                                                                    | ~/workspace/qontract-reconcile            |\n| qontract_reconcile_pr          | Qontract-reconcile PR/MR number                                                            |                                           |\n| qontract_reconcile_upstream    | Upstream remote name                                                                       | upstream                                  |\n| qontract_server_build_image    | Build qontract-server image                                                                | true                                      |\n| qontract_server_image          | Qontract-server image                                                                      | quay.io/app-sre/qontract-server:latest    |\n| qontract_server_path           | Qontract-server path                                                                       | ~/workspace/qontract-server               |\n| qontract_schemas_path          | Qontract-schemas path                                                                      | ~/workspace/qontract-schemas              |\n| qontract_schemas_pr            | Qontract-schemas PR/MR number                                                              |                                           |\n| qontract_schemas_upstream      | Upstream remote name                                                                       | upstream                                  |\n| run_once                       | If \'true\', execute the integration once and exit                                           | true                                      |\n| sleep_duration_secs            | If not *run_once*, sleep duration until integration runs again                             | 10                                        |\n\n> :point_right: **Bold keys** are mandatory or should be customized.\n\n### PR/MR support\n\nIt\'s a pretty handy feature to create a profile from a pull request (merge request). E.g.:\n\n```shell\n$ qd profile create --app-interface PATH_TO_YOUR_LOCAL/app-interface-dev-data --app-interface-pr NUMBER --qontract-schemas-pr NUMBER --qontract-reconcile-pr NUMBER --integration-name glitchtip --integration-extra-args \'\' glitchtip-pr-check\n```\n\nWhich results into this profile:\n\n```shell\n$ qd profile show glitchtip-pr-check\n---\napp_interface_path: PATH_TO_YOUR_LOCAL/app-interface-dev-data\napp_interface_pr: NUMBER\nintegration_name: glitchtip\nqontract_reconcile_pr: NUMBER\nqontract_schemas_pr: NUMBER\n```\n\nRunning this profile will:\n* Create new git worktrees (see `config.worktrees_dir`) for app-interface-dev-data, qontract-schema, and qontract-reconcile PRs\n* Start the containers with the adapted path to these worktrees\n* Restarting the profile will fetch PR updates\n\n> :point_right: A git worktree cleanup isn\'t implemented yet\n\n## Development\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n\n### Commits\n\nUse [Conventional Commit messages](https://www.conventionalcommits.org).\nThe most important prefixes you should have in mind are:\n\n* `fix:` which represents bug fixes and correlates to a [SemVer](https://semver.org/) patch.\n* `feat` represents a new feature and correlates to a SemVer minor.\n* `feat!:`,  or `fix!:`, `refactor!:`, etc., which represent a breaking change\n  (indicated by the `!`) and will result in a SemVer major.\n\n### Release\n\nTo release a new version, run:\n\n```shell\n$ make release\n```\n\nThis will:\n* Bump the version in `pyproject.toml`\n* Update the `CHANGELOG.md`\n* Commit the changes\n\n\n[pypi-link]:                https://pypi.org/project/qontract-development-cli/\n[pypi-platforms]:           https://img.shields.io/pypi/pyversions/qontract-development-cli\n[pypi-version]:             https://badge.fury.io/py/qontract-development-cli.svg\n[qontract-reconcile]:       https://github.com/app-sre/qontract-reconcile\n',
+    'long_description': '# Qontract Development CLI\n\n[![PyPI](https://img.shields.io/pypi/v/qontract-development-cli)][pypi-link]\n[![PyPI platforms][pypi-platforms]][pypi-link]\n![PyPI - License](https://img.shields.io/pypi/l/qontract-development-cli)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)\n\nQontract Development CLI supports your daily [qontract-reconcile][qontract-reconcile] development work.\n\n## Installation\n\nYou can install this library from [PyPI][pypi-link] with `pip`:\n\n```shell\n$ python3 -m pip install qontract-development-cli\n```\n\nOr install it with `pipx`:\n```shell\n$ pipx install qontract-development-cli\n```\n\nYou can also use `pipx` to run the library without installing it:\n\n```shell\n$ pipx run qontract-development-cli\n```\n\n## Quickstart\n\n* Create initial configuration\n  ```shell\n  $ qd config init\n  ```\n  <img src="demo/qd_config_init.gif" />\n\n* Create a profile `sql-query` to run the `sql-query` integration\n  ```shell\n  $ qd profile create sql-query\n  ```\n  <img src="demo/qd_profile_create.gif" />\n\n* Run `sql-query` profile\n  ```shell\n  $ profile run dev sql-query\n  ```\n  <img src="images/profile_run_sql_query.svg" />\n\n## Features\n\nQontract Development CLI currently provides the following features (get help with `-h` or `--help`):\n\n- Run `qontract-reconcile` and `qontract-server` as docker containers on your local machine\n- Support for different environments (dev, prod, ...) via the `env` command\n- Configure your [qontract-reconcile integration][qontract-reconcile] with the `profile` command\n- Support pull request reviews (see `profile create`)\n- Bootstrap your initial configurations with the `config` command\n- Shell autocompletion (see `qd --help`)\n\n## Commands\n\n### Config\n\nManage global qontract-development CLI configuration.\n\n`qd config [sub-cmd] --help`\n\n* **edit**: open the configuration file in your favorite editor\n* **init**: create a default configuration\n\n#### Settings\n| **Key**                     | **Description**                       | **Default**                          |\n| --------------------------- | ------------------------------------- | ------------------------------------ |\n| debug                       | Enable/disable debug mode             | false                                |\n| defaults_profile            | Name of defaults profile              | defaults                             |\n| docker_compose_project_name | Docker compose project name           | qontract-development                 |\n| editor                      | Your favorite editor                  | $EDITOR or vim                       |\n| environments_dir            | Directory to store environment files  | User config directory / environments |\n| profiles_dir                | Directory to store profile files      | User config directory / profiles     |\n| worktrees_dir               | Directory to store git repo worktrees | User cache directory / worktrees     |\n\n\n## Environments\n\nAn environment specifies app-interface instance settings, e.g., **dev** vs. **prod** config and path to the actual app-interface instance.\n\n`qd env [sub-cmd] --help`\n\n* **edit**: Create/edit an environment file in your editor.\n* **ls**: List all available environments.\n* **rm**: Remove environment.\n* **show**: Display environment.\n\n\n#### Settings\n\n| **Key**                            | **Description**                      | **Default**                                    |\n| ---------------------------------- | ------------------------------------ | ---------------------------------------------- |\n| **app_interface_path**             | Path to local app-interface instance | ~/workspace/app-interface                      |\n| app_interface_state_bucket         | S3 bucket                            | empty                                          |\n| app_interface_state_bucket_account | AWS S3 account                       | empty                                          |\n| **config**                         | app-interface config                 | ~/workspace/qontract-reconcile/config.dev.toml |\n| gitlab_pr_submitter_queue_url      | Gitlab pr submitter queue url        |                                                |\n| run_qontract_reconcile             | Run qontract-reconcile container     | true                                           |\n| run_qontract_server                | Run qontract-server container        | true                                           |\n| run_vault                          | Run vault container                  | false                                          |\n\n> :point_right: **Bold keys** are mandatory or should be customized.\n\n## Profiles\n\nA profile specifies all settings to run a qontract-reconcile integration (e.g., *sql-query*).\n\n`qd profile [sub-cmd] --help`\n\n* **create**: Create a new profile to run an integration.\n\n  Supports the creation of a new profile from an open PR/MR. See `qd profile create --help` for all available options.\n\n* **edit**: Edit a profile in your editor.\n* **ls**: List all available profiles.\n* **rm**: Remove profile.\n* **run**: Run a profile.\n* **show**: Display profile.\n\n\n#### Settings\n\n| **Key**                        | **Description**                                                                                                                                                              | **Default**                                 |\n| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |\n| additional_environment         | Dictionary of additional environment variables to pass to the qontract-reconcile container                                                                                   | `{}`                                        |\n| container_uid                  | Change ownership of /recconcile files in container to this user id                                                                                                           | current UID                                 |\n| debugger                       | Python debugger                                                                                                                                                              | `debugpy`                                   |\n| dry_run                        | Run --dry-run mode                                                                                                                                                           | `true`                                      |\n| extra_hosts                    | List of \'HOSTNAME:IP\' mapping entries for qontract-reconcile `/etc/hosts`. See [extra_hosts](https://docs.docker.com/compose/compose-file/#extra_hosts) docker compose file. | `[]`                                        |\n| **integration_name**           | Intergration name                                                                                                                                                            |                                             |\n| **integration_extra_args**     | Intergration extra arguments                                                                                                                                                 |                                             |\n| **internal_redhat_ca**         | Inject Red Hat internal CAs and `REQUESTS_CA_BUNDLE` environment variable                                                                                                    | `false`                                     |\n| log_level                      | Log level                                                                                                                                                                    | `info`                                      |\n| app_interface_path             | App-interface instance path. (Overrides *env.app_interface_path*)                                                                                                            |                                             |\n| app_interface_pr               | App-interface PR/MR number                                                                                                                                                   |                                             |\n| app_interface_upstream         | Upstream remote name                                                                                                                                                         | `upstream`                                  |\n| qontract_reconcile_build_image | Build qontract-reconcile image                                                                                                                                               | `true`                                      |\n| qontract_reconcile_image       | Qontract-reconcile image                                                                                                                                                     | `quay.io/app-sre/qontract-reconcile:latest` |\n| qontract_reconcile_path        | Qontract-reconcile path                                                                                                                                                      | `~/workspace/qontract-reconcile`            |\n| qontract_reconcile_pr          | Qontract-reconcile PR/MR number                                                                                                                                              |                                             |\n| qontract_reconcile_upstream    | Upstream remote name                                                                                                                                                         | `upstream`                                  |\n| qontract_server_build_image    | Build qontract-server image                                                                                                                                                  | `true`                                      |\n| qontract_server_image          | Qontract-server image                                                                                                                                                        | `quay.io/app-sre/qontract-server:lates`t    |\n| qontract_server_path           | Qontract-server path                                                                                                                                                         | `~/workspace/qontract-server`               |\n| qontract_schemas_path          | Qontract-schemas path                                                                                                                                                        | `~/workspace/qontract-schemas`              |\n| qontract_schemas_pr            | Qontract-schemas PR/MR number                                                                                                                                                |                                             |\n| qontract_schemas_upstream      | Upstream remote name                                                                                                                                                         | `upstream`                                  |\n| run_once                       | If \'true\', execute the integration once and exit                                                                                                                             | `true`                                      |\n| sleep_duration_secs            | If not *run_once*, sleep duration until integration runs again                                                                                                               | `10`                                        |\n\n> :point_right: **Bold keys** are mandatory or should be customized.\n\n### PR/MR support\n\nIt\'s a pretty handy feature to create a profile from a pull request (merge request). E.g.:\n\n```shell\n$ qd profile create --app-interface PATH_TO_YOUR_LOCAL/app-interface-dev-data --app-interface-pr NUMBER --qontract-schemas-pr NUMBER --qontract-reconcile-pr NUMBER --integration-name glitchtip --integration-extra-args \'\' glitchtip-pr-check\n```\n\nWhich results into this profile:\n\n```shell\n$ qd profile show glitchtip-pr-check\n---\napp_interface_path: PATH_TO_YOUR_LOCAL/app-interface-dev-data\napp_interface_pr: NUMBER\nintegration_name: glitchtip\nqontract_reconcile_pr: NUMBER\nqontract_schemas_pr: NUMBER\n```\n\nRunning this profile will:\n* Create new git worktrees (see `config.worktrees_dir`) for app-interface-dev-data, qontract-schema, and qontract-reconcile PRs\n* Start the containers with the adapted path to these worktrees\n* Restarting the profile will fetch PR updates\n\n> :point_right: A git worktree cleanup isn\'t implemented yet\n\n## Development\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n\n### Commits\n\nUse [Conventional Commit messages](https://www.conventionalcommits.org).\nThe most important prefixes you should have in mind are:\n\n* `fix:` which represents bug fixes and correlates to a [SemVer](https://semver.org/) patch.\n* `feat` represents a new feature and correlates to a SemVer minor.\n* `feat!:`,  or `fix!:`, `refactor!:`, etc., which represent a breaking change\n  (indicated by the `!`) and will result in a SemVer major.\n\n### Release\n\nTo release a new version, run:\n\n```shell\n$ make release\n```\n\nThis will:\n* Bump the version in `pyproject.toml`\n* Update the `CHANGELOG.md`\n* Commit the changes\n\n\n[pypi-link]:                https://pypi.org/project/qontract-development-cli/\n[pypi-platforms]:           https://img.shields.io/pypi/pyversions/qontract-development-cli\n[pypi-version]:             https://badge.fury.io/py/qontract-development-cli.svg\n[qontract-reconcile]:       https://github.com/app-sre/qontract-reconcile\n',
     'author': 'Christian Assing',
     'author_email': 'cassing@redhat.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://github.com/chassing/qontract-development-cli',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qontract_development_cli-0.8.1/PKG-INFO` & `qontract_development_cli-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qontract-development-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: Helper tool for qontract-reconcile development
 Home-page: http://github.com/chassing/qontract-development-cli
 License: MIT
 Author: Christian Assing
 Author-email: cassing@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -148,39 +148,41 @@
 * **rm**: Remove profile.
 * **run**: Run a profile.
 * **show**: Display profile.
 
 
 #### Settings
 
-| **Key**                        | **Description**                                                                            | **Default**                               |
-| ------------------------------ | ------------------------------------------------------------------------------------------ | ----------------------------------------- |
-| additional_environment         | Dictionary of additional environment variables to pass to the qontract-reconcile container | `{}`                                      |
-| container_uid                  | Change ownership of /recconcile files in container to this user id                         | current UID                               |
-| debugger                       | Python debugger                                                                            | debugpy                                   |
-| dry_run                        | Run --dry-run mode                                                                         | true                                      |
-| **integration_name**           | Intergration name                                                                          |                                           |
-| **integration_extra_args**     | Intergration extra arguments                                                               |                                           |
-| log_level                      | Log level                                                                                  | info                                      |
-| app_interface_path             | App-interface instance path. (Overrides *env.app_interface_path*)                          |                                           |
-| app_interface_pr               | App-interface PR/MR number                                                                 |                                           |
-| app_interface_upstream         | Upstream remote name                                                                       | upstream                                  |
-| qontract_reconcile_build_image | Build qontract-reconcile image                                                             | true                                      |
-| qontract_reconcile_image       | Qontract-reconcile image                                                                   | quay.io/app-sre/qontract-reconcile:latest |
-| qontract_reconcile_path        | Qontract-reconcile path                                                                    | ~/workspace/qontract-reconcile            |
-| qontract_reconcile_pr          | Qontract-reconcile PR/MR number                                                            |                                           |
-| qontract_reconcile_upstream    | Upstream remote name                                                                       | upstream                                  |
-| qontract_server_build_image    | Build qontract-server image                                                                | true                                      |
-| qontract_server_image          | Qontract-server image                                                                      | quay.io/app-sre/qontract-server:latest    |
-| qontract_server_path           | Qontract-server path                                                                       | ~/workspace/qontract-server               |
-| qontract_schemas_path          | Qontract-schemas path                                                                      | ~/workspace/qontract-schemas              |
-| qontract_schemas_pr            | Qontract-schemas PR/MR number                                                              |                                           |
-| qontract_schemas_upstream      | Upstream remote name                                                                       | upstream                                  |
-| run_once                       | If 'true', execute the integration once and exit                                           | true                                      |
-| sleep_duration_secs            | If not *run_once*, sleep duration until integration runs again                             | 10                                        |
+| **Key**                        | **Description**                                                                                                                                                              | **Default**                                 |
+| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
+| additional_environment         | Dictionary of additional environment variables to pass to the qontract-reconcile container                                                                                   | `{}`                                        |
+| container_uid                  | Change ownership of /recconcile files in container to this user id                                                                                                           | current UID                                 |
+| debugger                       | Python debugger                                                                                                                                                              | `debugpy`                                   |
+| dry_run                        | Run --dry-run mode                                                                                                                                                           | `true`                                      |
+| extra_hosts                    | List of 'HOSTNAME:IP' mapping entries for qontract-reconcile `/etc/hosts`. See [extra_hosts](https://docs.docker.com/compose/compose-file/#extra_hosts) docker compose file. | `[]`                                        |
+| **integration_name**           | Intergration name                                                                                                                                                            |                                             |
+| **integration_extra_args**     | Intergration extra arguments                                                                                                                                                 |                                             |
+| **internal_redhat_ca**         | Inject Red Hat internal CAs and `REQUESTS_CA_BUNDLE` environment variable                                                                                                    | `false`                                     |
+| log_level                      | Log level                                                                                                                                                                    | `info`                                      |
+| app_interface_path             | App-interface instance path. (Overrides *env.app_interface_path*)                                                                                                            |                                             |
+| app_interface_pr               | App-interface PR/MR number                                                                                                                                                   |                                             |
+| app_interface_upstream         | Upstream remote name                                                                                                                                                         | `upstream`                                  |
+| qontract_reconcile_build_image | Build qontract-reconcile image                                                                                                                                               | `true`                                      |
+| qontract_reconcile_image       | Qontract-reconcile image                                                                                                                                                     | `quay.io/app-sre/qontract-reconcile:latest` |
+| qontract_reconcile_path        | Qontract-reconcile path                                                                                                                                                      | `~/workspace/qontract-reconcile`            |
+| qontract_reconcile_pr          | Qontract-reconcile PR/MR number                                                                                                                                              |                                             |
+| qontract_reconcile_upstream    | Upstream remote name                                                                                                                                                         | `upstream`                                  |
+| qontract_server_build_image    | Build qontract-server image                                                                                                                                                  | `true`                                      |
+| qontract_server_image          | Qontract-server image                                                                                                                                                        | `quay.io/app-sre/qontract-server:lates`t    |
+| qontract_server_path           | Qontract-server path                                                                                                                                                         | `~/workspace/qontract-server`               |
+| qontract_schemas_path          | Qontract-schemas path                                                                                                                                                        | `~/workspace/qontract-schemas`              |
+| qontract_schemas_pr            | Qontract-schemas PR/MR number                                                                                                                                                |                                             |
+| qontract_schemas_upstream      | Upstream remote name                                                                                                                                                         | `upstream`                                  |
+| run_once                       | If 'true', execute the integration once and exit                                                                                                                             | `true`                                      |
+| sleep_duration_secs            | If not *run_once*, sleep duration until integration runs again                                                                                                               | `10`                                        |
 
 > :point_right: **Bold keys** are mandatory or should be customized.
 
 ### PR/MR support
 
 It's a pretty handy feature to create a profile from a pull request (merge request). E.g.:
```

