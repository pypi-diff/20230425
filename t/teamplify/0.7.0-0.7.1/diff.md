# Comparing `tmp/teamplify-0.7.0.tar.gz` & `tmp/teamplify-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamplify-0.7.0.tar", last modified: Sun Apr 16 11:50:21 2023, max compression
+gzip compressed data, was "teamplify-0.7.1.tar", last modified: Tue Apr 25 12:33:05 2023, max compression
```

## Comparing `teamplify-0.7.0.tar` & `teamplify-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.100014 teamplify-0.7.0/
--rw-r--r--   0 ipeterov   (501) staff       (20)     1066 2023-04-12 15:29:52.000000 teamplify-0.7.0/LICENSE
--rw-r--r--   0 ipeterov   (501) staff       (20)      272 2023-04-12 15:29:52.000000 teamplify-0.7.0/MANIFEST.in
--rw-r--r--   0 ipeterov   (501) staff       (20)    23510 2023-04-16 11:50:21.100110 teamplify-0.7.0/PKG-INFO
--rw-r--r--   0 ipeterov   (501) staff       (20)    23187 2023-04-12 15:29:52.000000 teamplify-0.7.0/README.md
--rw-r--r--   0 ipeterov   (501) staff       (20)       48 2023-04-12 15:29:52.000000 teamplify-0.7.0/requirements-tests.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      102 2023-04-12 21:17:51.000000 teamplify-0.7.0/requirements.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      251 2023-04-16 11:50:21.100386 teamplify-0.7.0/setup.cfg
--rw-r--r--   0 ipeterov   (501) staff       (20)     1255 2023-04-12 15:29:52.000000 teamplify-0.7.0/setup.py
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.097565 teamplify-0.7.0/teamplify.egg-info/
--rw-r--r--   0 ipeterov   (501) staff       (20)    23510 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/PKG-INFO
--rw-r--r--   0 ipeterov   (501) staff       (20)      617 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/SOURCES.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)        1 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/dependency_links.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       56 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/entry_points.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      159 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/requires.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       17 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/top_level.txt
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.099724 teamplify-0.7.0/teamplify_runner/
--rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-16 11:49:30.000000 teamplify-0.7.0/teamplify_runner/__init__.py
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.099876 teamplify-0.7.0/teamplify_runner/backup/
--rw-r--r--   0 ipeterov   (501) staff       (20)       51 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/backup/readme.txt
--rwxr-xr-x   0 ipeterov   (501) staff       (20)    13690 2023-04-16 11:43:21.000000 teamplify-0.7.0/teamplify_runner/cli.py
--rw-r--r--   0 ipeterov   (501) staff       (20)    13723 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/configurator.py
--rw-r--r--   0 ipeterov   (501) staff       (20)     5304 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/docker-compose.yml
--rw-r--r--   0 ipeterov   (501) staff       (20)      270 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/mysql.cnf
--rw-r--r--   0 ipeterov   (501) staff       (20)       66 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/postfix.cf
--rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/redis.conf
--rw-r--r--   0 ipeterov   (501) staff       (20)     1748 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/utils.py
--rw-r--r--   0 ipeterov   (501) staff       (20)      766 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/uwsgi_params.conf
--rw-r--r--   0 ipeterov   (501) staff       (20)      512 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/vhost.conf
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 12:33:05.944276 teamplify-0.7.1/
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1066 2023-04-12 15:29:52.000000 teamplify-0.7.1/LICENSE
+-rw-r--r--   0 ipeterov   (501) staff       (20)      272 2023-04-12 15:29:52.000000 teamplify-0.7.1/MANIFEST.in
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23372 2023-04-25 12:33:05.944371 teamplify-0.7.1/PKG-INFO
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23049 2023-04-25 12:30:22.000000 teamplify-0.7.1/README.md
+-rw-r--r--   0 ipeterov   (501) staff       (20)       63 2023-04-18 11:09:50.000000 teamplify-0.7.1/requirements-tests.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      102 2023-04-12 21:17:51.000000 teamplify-0.7.1/requirements.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      253 2023-04-25 12:33:05.944844 teamplify-0.7.1/setup.cfg
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1276 2023-04-18 11:02:31.000000 teamplify-0.7.1/setup.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 12:33:05.941462 teamplify-0.7.1/teamplify.egg-info/
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23372 2023-04-25 12:33:05.000000 teamplify-0.7.1/teamplify.egg-info/PKG-INFO
+-rw-r--r--   0 ipeterov   (501) staff       (20)      617 2023-04-25 12:33:05.000000 teamplify-0.7.1/teamplify.egg-info/SOURCES.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)        1 2023-04-25 12:33:05.000000 teamplify-0.7.1/teamplify.egg-info/dependency_links.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       56 2023-04-25 12:33:05.000000 teamplify-0.7.1/teamplify.egg-info/entry_points.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      175 2023-04-25 12:33:05.000000 teamplify-0.7.1/teamplify.egg-info/requires.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       17 2023-04-25 12:33:05.000000 teamplify-0.7.1/teamplify.egg-info/top_level.txt
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 12:33:05.943993 teamplify-0.7.1/teamplify_runner/
+-rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-25 12:30:22.000000 teamplify-0.7.1/teamplify_runner/__init__.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 12:33:05.944136 teamplify-0.7.1/teamplify_runner/backup/
+-rw-r--r--   0 ipeterov   (501) staff       (20)       51 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/backup/readme.txt
+-rwxr-xr-x   0 ipeterov   (501) staff       (20)    14178 2023-04-25 12:30:22.000000 teamplify-0.7.1/teamplify_runner/cli.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)    13881 2023-04-18 11:02:31.000000 teamplify-0.7.1/teamplify_runner/configurator.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)     5304 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/docker-compose.yml
+-rw-r--r--   0 ipeterov   (501) staff       (20)      270 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/mysql.cnf
+-rw-r--r--   0 ipeterov   (501) staff       (20)       66 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/postfix.cf
+-rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/redis.conf
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1755 2023-04-18 11:02:31.000000 teamplify-0.7.1/teamplify_runner/utils.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)      766 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/uwsgi_params.conf
+-rw-r--r--   0 ipeterov   (501) staff       (20)      512 2023-04-12 15:29:52.000000 teamplify-0.7.1/teamplify_runner/vhost.conf
```

### Comparing `teamplify-0.7.0/LICENSE` & `teamplify-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teamplify-0.7.0/PKG-INFO` & `teamplify-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.7.0
+Version: 0.7.1
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # Teamplify runner
 
-[![image](https://travis-ci.org/teamplify/teamplify-runner.svg?branch=master)](https://travis-ci.org/teamplify/teamplify-runner)
-
 [Teamplify](https://teamplify.com) is a personal assistant for your development
 team. It helps you track work progress and notify your team about situations
 that may require their attention. It is available
 [in the cloud](https://teamplify.com) or as an on-premise installation.
 
 This package is the installer and runner for the on-premise version.
 
@@ -371,15 +369,15 @@
 activity. The `update` command restarts the service only when necessary. If no
 update has been downloaded, there is no restart and therefore no service
 interruption.
 
 ## Backup and restore
 
 Teamplify stores your data in a MySQL database. As with any other database, it
-might be a good idea to make backups from time to time to time.
+might be a good idea to make backups from time to time.
 
 To back up the built-in Teamplify database, run:
 
 ``` shell
 $ teamplify backup [optional-backup-file-or-directory]
 ```
```

### Comparing `teamplify-0.7.0/README.md` & `teamplify-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Teamplify runner
 
-[![image](https://travis-ci.org/teamplify/teamplify-runner.svg?branch=master)](https://travis-ci.org/teamplify/teamplify-runner)
-
 [Teamplify](https://teamplify.com) is a personal assistant for your development
 team. It helps you track work progress and notify your team about situations
 that may require their attention. It is available
 [in the cloud](https://teamplify.com) or as an on-premise installation.
 
 This package is the installer and runner for the on-premise version.
 
@@ -358,15 +356,15 @@
 activity. The `update` command restarts the service only when necessary. If no
 update has been downloaded, there is no restart and therefore no service
 interruption.
 
 ## Backup and restore
 
 Teamplify stores your data in a MySQL database. As with any other database, it
-might be a good idea to make backups from time to time to time.
+might be a good idea to make backups from time to time.
 
 To back up the built-in Teamplify database, run:
 
 ``` shell
 $ teamplify backup [optional-backup-file-or-directory]
 ```
```

### Comparing `teamplify-0.7.0/setup.py` & `teamplify-0.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 MIN_PYTHON_VER = (3, 6)
 MIN_PYTHON_STR = '.'.join(map(str, MIN_PYTHON_VER))
 
 if sys.version_info < MIN_PYTHON_VER:
     sys.exit(
-        'Teamplify runner requires Python %s or later' % MIN_PYTHON_STR,
+        'Teamplify runner requires Python {0} or later'.format(MIN_PYTHON_STR),
     )
 
 
 def get_requirements(extra=None):
-    filename = 'requirements-%s.txt' % extra if extra else 'requirements.txt'
+    filename = 'requirements-{0}.txt'.format(extra) if extra else 'requirements.txt'
     with open(filename) as fp:
         return [
             x.strip() for x in fp.read().split('\n') if not x.startswith('#')
         ]
 
 
 setup(
@@ -34,15 +34,15 @@
     url='https://github.com/teamplify/teamplify-runner/',
     install_requires=get_requirements(),
     extras_require={
         'tests': get_requirements('tests'),
     },
     packages=['teamplify_runner'],
     include_package_data=True,
-    python_requires='>=%s' % MIN_PYTHON_STR,
+    python_requires='>={0}'.format(MIN_PYTHON_STR),
     license='MIT',
     entry_points={
         'console_scripts': [
             'teamplify = teamplify_runner.cli:main',
         ],
     },
 )
```

### Comparing `teamplify-0.7.0/teamplify.egg-info/PKG-INFO` & `teamplify-0.7.1/teamplify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.7.0
+Version: 0.7.1
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # Teamplify runner
 
-[![image](https://travis-ci.org/teamplify/teamplify-runner.svg?branch=master)](https://travis-ci.org/teamplify/teamplify-runner)
-
 [Teamplify](https://teamplify.com) is a personal assistant for your development
 team. It helps you track work progress and notify your team about situations
 that may require their attention. It is available
 [in the cloud](https://teamplify.com) or as an on-premise installation.
 
 This package is the installer and runner for the on-premise version.
 
@@ -371,15 +369,15 @@
 activity. The `update` command restarts the service only when necessary. If no
 update has been downloaded, there is no restart and therefore no service
 interruption.
 
 ## Backup and restore
 
 Teamplify stores your data in a MySQL database. As with any other database, it
-might be a good idea to make backups from time to time to time.
+might be a good idea to make backups from time to time.
 
 To back up the built-in Teamplify database, run:
 
 ``` shell
 $ teamplify backup [optional-backup-file-or-directory]
 ```
```

### Comparing `teamplify-0.7.0/teamplify.egg-info/SOURCES.txt` & `teamplify-0.7.1/teamplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `teamplify-0.7.0/teamplify_runner/cli.py` & `teamplify-0.7.1/teamplify_runner/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import time
 from datetime import datetime
 
 import click
 import requests
 
 from teamplify_runner import __version__
-from teamplify_runner.configurator import BASE_DIR, ConfigurationError, \
-    Configurator
+from teamplify_runner.configurator import BASE_DIR, ConfigurationError, Configurator
 from teamplify_runner.utils import cd, run
 
 
 IMAGES = {
     'db': 'mysql:8.0.29-oracle',
     'redis': 'redis:6.2.6',
     'nginx': 'jwilder/nginx-proxy:latest',
@@ -26,57 +25,62 @@
     port = env['WEB_PORT']
     root_url = 'http://' + env['WEB_HOST']
     if port != '80':
         root_url += ':' + port
     return root_url
 
 
-def _wait_for_teamplify_start(url, max_minutes=5, check_interval_seconds=5):
-    click.echo(
-        '\nWaiting for Teamplify to start at %s,'
-        ' checking every %s seconds...' % (url, check_interval_seconds),
-        nl=False,
-    )
+def _wait_for_teamplify_start(url, max_minutes=10, check_interval_seconds=1):
+    click.echo('\nTeamplify will be available at {0}\n'.format(url))
 
     start_time = time.time()
     while time.time() < start_time + max_minutes * 60:
-        response = requests.get(url).text
+        seconds_since_launch = int(time.time() - start_time)
+        minutes, seconds = divmod(seconds_since_launch, 60)
+        # Add two spaces so we always overwrite the previous string
+        click.echo(
+            'Startup in progress, {0} min {1} sec ...  \r'.format(minutes, seconds),
+            nl=False,
+        )
+
+        try:
+            response = requests.get(url).text
+        except (requests.ConnectionError, requests.Timeout):
+            time.sleep(check_interval_seconds)
+            continue
 
         if 'window.BUILD_NUMBER' in response:
-            click.echo('\nTeamplify successfully started!')
+            click.echo('\n\nTeamplify successfully started!')
             return
         elif any(
             marker in response
             for marker in (
                 'Welcome to nginx!',
                 'Teamplify is starting...',
             )
         ):
             time.sleep(check_interval_seconds)
-            click.echo('.', nl=False)
             continue
         else:
             raise RuntimeError(
-                '\n\nUnexpected response from Teamplify: %s\n\n'
+                '\n\nUnexpected response from Teamplify: {0}\n\n'
                 'Please check the Troubleshooting guide:\n -> '
-                'https://github.com/teamplify/teamplify-runner/#troubleshooting'
-                % response,
+                'https://github.com/teamplify/teamplify-runner/#troubleshooting'.format(response)
             )
-    else:
-        raise RuntimeError(
-            "\n\nTeamplify didn't start in %s minutes. "
-            'Please check the Troubleshooting guide:\n'
-            ' -> https://github.com/teamplify/teamplify-runner/#troubleshooting'
-            % max_minutes,
-        )
+
+    raise RuntimeError(
+        "\n\nTeamplify didn't start in {0} minutes. "
+        'Please check the Troubleshooting guide:\n'
+        ' -> https://github.com/teamplify/teamplify-runner/#troubleshooting'.format(max_minutes)
+    )
 
 
 def _start(env):
     click.echo('Starting services...')
-    run('mkdir -p %s' % env['DB_BACKUP_MOUNT'])
+    run('mkdir -p {0}'.format(env['DB_BACKUP_MOUNT']))
     with cd(BASE_DIR):
         run(
             'docker-compose up '
             '--detach '
             '--remove-orphans '
             '--scale worker_slim={worker_slim_count} '
             '--scale worker_fat={worker_fat_count}'.format(
@@ -105,17 +109,17 @@
         click.echo(click.style(str(e), fg='red'))
         exit(1)
 
 
 def _create_admin(env, email, full_name):
     click.echo('Creating admin...')
     cmd = 'docker exec teamplify_app ' \
-          '/code/manage.py createadmin --email %s' % email
+          '/code/manage.py createadmin --email {0}'.format(email)
     if full_name:
-        cmd += ' --full-name "%s"' % full_name
+        cmd += ' --full-name "{0}"'.format(full_name)
     run(cmd, capture_output=False, env=env)
 
 
 def _stop(env):
     click.echo('Stopping services...')
     with cd(BASE_DIR):
         run(
@@ -139,140 +143,140 @@
     db_host = env['DB_HOST']
     if db_host != Configurator.defaults['db']['host']:
         click.echo(
             '\nWe are sorry, but the "teamplify backup" and '
             '"teamplify restore" commands are designed to work with '
             '"builtin_db" only. The current configuration specifies an '
             'external DB at:\n'
-            ' -> %s\n'
+            ' -> {0}\n'
             'To perform backup or restore operations, please use tools that '
             'connect to this DB server directly.\n\n'
-            'Command aborted.' % db_host,
+            'Command aborted.'.format(db_host),
             err=True,
         )
         exit(1)
 
 
 def _backup(env, filename=None):
     now = datetime.utcnow().replace(microsecond=0)
-    default_filename = '%s_%s.sql.gz' % (
+    default_filename = '{0}_{1}.sql.gz'.format(
         env['DB_NAME'],
         now.isoformat('_').replace(':', '-'),
     )
     if not filename:
         target_file = default_filename
     elif os.path.isdir(filename):
         target_file = os.path.join(filename, default_filename)
     else:
         target_file = filename
     temp_filename = os.path.join('/backup', default_filename)
     cleanup_on_error = not os.path.exists(target_file)
     # check for write access on the host
-    run('touch %s' % target_file)
+    run('touch {0}'.format(temp_filename))
     # check for write access inside docker
-    run('docker exec teamplify_db bash -c "touch %s"' % temp_filename)
+    run('docker exec teamplify_db bash -c "touch {0}"'.format(target_file))
     command = (
         'MYSQL_PWD={password} mysqldump --single-transaction -u{user} '
         '-h {host} {db} | gzip > {filename}'.format(
             user=env['DB_USER'],
             password=env['DB_PASSWORD'],
             host='localhost',
             db=env['DB_NAME'],
             filename=os.path.join('/backup', default_filename),
         )
     )
-    click.echo('Making backup of Teamplify DB to:\n -> %s' % target_file)
+    click.echo('Making backup of Teamplify DB to:\n -> {0}'.format(target_file))
     click.echo('Please wait...')
     try:
         run(
             'docker exec teamplify_db bash -c "{command}"'.format(
                 command=command,
             ),
             exit_on_error=False,
         )
     except RuntimeError:
         if cleanup_on_error:
-            run('rm %s' % target_file)
+            run('rm {0}'.format(target_file))
         exit(1)
     run('mv {source} {target}'.format(
         source=os.path.join(env['DB_BACKUP_MOUNT'], default_filename),
         target=target_file,
     ))
     click.echo('Done.')
 
 
 def _restore(env, filename):
     click.echo('Copying the backup...')
     restore_filename = 'restore.sql.gz'
     restore_mount = os.path.join(env['DB_BACKUP_MOUNT'], restore_filename)
-    run('cp %s %s' % (filename, restore_mount))
+    run('cp {0} {1}'.format(filename, restore_mount))
     try:
         sql = (
             'docker exec -e MYSQL_PWD="{password}" teamplify_db mysql -u{user} '
             '-e "%s"'.format(
                 user=env['DB_USER'],
                 password=env['DB_PASSWORD'],
             )
         )
         click.echo('Dropping and re-creating the DB...')
-        run(sql % ('drop database %s' % env['DB_NAME']))
-        run(sql % ('create database %s' % env['DB_NAME']))
+        run(sql % ('drop database {0}'.format(env['DB_NAME'])))
+        run(sql % ('create database {0}'.format(env['DB_NAME'])))
         click.echo('Restoring DB backup...')
         run(
             'docker exec -e MYSQL_PWD="{password}" teamplify_db bash -c "'
             'gunzip < {filename} | mysql -u{user} {db}"'.format(
                 filename='/'.join(('/backup', restore_filename)),
                 user=env['DB_USER'],
                 password=env['DB_PASSWORD'],
                 db=env['DB_NAME'],
             ),
         )
     finally:
-        run('rm %s' % restore_mount)
+        run('rm {0}'.format(restore_mount))
     click.echo('Done.')
 
 
 def _remove_unused_images():
     unused_images = run(
-        'docker images -f reference=%s -f dangling=true -q' % (IMAGES['app']),
+        'docker images -f reference={0} -f dangling=true -q'.format(IMAGES['app']),
         suppress_output=True,
     ).stdout_lines
-    click.echo('Cleanup: %s stale image(s) found' % len(unused_images))
+    click.echo('Cleanup: {0} stale image(s) found'.format(len(unused_images)))
     if unused_images:
         # Suppress errors because it might be possible
         # that some images are still used
         run(
-            'docker rmi %s' % ' '.join(unused_images),
+            'docker rmi {0}'.format(' '.join(unused_images)),
             suppress_output=True,
             raise_on_error=False,
         )
 
 
 def cli(ctx, config):
     config = Configurator(config).load()
     if config.config_path:
-        click.echo('Using the configuration file at %s' % config.config_path)
+        click.echo('Using the configuration file at {0}'.format(config.config_path))
     if ctx.invoked_subcommand != 'configure':
         try:
             config.validate()
         except ConfigurationError as e:
             title = 'Configuration problem'
             title += ' - ' if len(e.messages) > 1 else ':\n -> '
-            click.echo('%s%s' % (title, str(e)), err=True)
+            click.echo(title + str(e), err=True)
             click.echo('Command aborted.', err=True)
             exit(1)
     ctx.obj['config'] = config
     env = config.env()
     for image_id, reference in IMAGES.items():
-        env['IMAGE_%s' % image_id.upper()] = reference
+        env['IMAGE_{0}'.format(image_id.upper())] = reference
     env['IMAGE_APP'] += ':' + env['MAIN_UPDATE_CHANNEL']
     ctx.obj['env'] = env
 
 
-cli.__doc__ = 'Teamplify runner v%s' % __version__
+cli.__doc__ = 'Teamplify runner v{0}'.format(__version__)
 
 
 cli = click.group()(
     click.option('--config', type=click.Path(exists=True, dir_okay=False),
                  default=None, help='Optional, config file to use')(
         click.pass_context(cli),
     ))
@@ -282,15 +286,15 @@
 @click.pass_context
 def configure(ctx):
     """
     Interactive configuration wizard
     """
     config = ctx.obj['config']
     config.remove_unknown().dump()
-    click.echo('Current configuration saved to:\n -> %s' % config.config_path)
+    click.echo('Current configuration saved to:\n -> {0}'.format(config.config_path))
     click.echo(
         '\nThe file above contains the full list of configurable options. '
         'Please use your favorite text editor to adjust them as necessary. '
         'When ready, run the following command to verify and apply your '
         'changes:\n'
         ' -> teamplify restart',
     )
@@ -366,27 +370,27 @@
     Restore Teamplify DB from a GZipped archive
     """
     env = ctx.obj['env']
     _assert_builtin_db(env)
     if not quiet:
         confirm = input(
             'Current Teamplify DB will be overwritten from:\n'
-            ' -> %s\n'
-            'Continue (y/N)? ' % filename,
+            ' -> {0}\n'
+            'Continue (y/N)? '.format(filename),
         )
         if confirm.lower() != 'y':
             click.echo('DB restore cancelled, exiting')
             return
     _restore(env, filename)
 
 
 def _image_id(name):
     try:
         return run(
-            'docker image ls -q --no-trunc %s' % name,
+            'docker image ls -q --no-trunc {0}'.format(name),
             suppress_output=True,
         ).stdout_lines[0]
     except IndexError:
         return None
 
 
 @cli.command()
@@ -394,22 +398,22 @@
 def update(ctx):
     """
     Update to the latest version
     """
     env = ctx.obj['env']
     if _running(env):
         current_image = _image_id(env['IMAGE_APP'])
-        run('docker pull %s' % env['IMAGE_APP'], capture_output=False)
+        run('docker pull {0}'.format(env['IMAGE_APP']), capture_output=False)
         new_image = _image_id(env['IMAGE_APP'])
         if current_image != new_image:
             _stop(env)
             _start(env)
             click.echo('')
     else:
-        run('docker pull %s' % env['IMAGE_APP'])
+        run('docker pull {0}'.format(env['IMAGE_APP']))
     _remove_unused_images()
     click.echo('Done.')
 
 
 @cli.command()
 @click.option('--quiet', 'quiet', flag_value='quiet', default=None)
 @click.pass_context
@@ -431,32 +435,32 @@
     _stop(env)
     click.echo('')
     networks = run(
         'docker network ls -f name=teamplify_runner* -q',
         suppress_output=True,
     ).stdout_lines
     if networks:
-        click.echo('Removing %s Docker network(s):' % len(networks))
-        run('docker network rm %s' % ' '.join(networks), raise_on_error=False)
+        click.echo('Removing {0} Docker network(s):'.format(len(networks)))
+        run('docker network rm {0}'.format(' '.join(networks)), raise_on_error=False)
     volumes = run(
         'docker volume ls -f name=teamplify_runner* -q',
         suppress_output=True,
     ).stdout_lines
     if volumes:
-        click.echo('Removing %s Docker volume(s):' % len(volumes))
-        run('docker volume rm %s' % ' '.join(volumes), raise_on_error=False)
+        click.echo('Removing {0} Docker volume(s):'.format(len(volumes)))
+        run('docker volume rm {0}'.format(' '.join(volumes)), raise_on_error=False)
     click.echo('Removing Docker images:')
     images = []
     for image_id, reference in IMAGES.items():
         if image_id == 'app':
             for channel in ('stable', 'latest'):
-                images.append('%s:%s' % (reference, channel))
+                images.append('{0}:{1}'.format(reference, channel))
         else:
             images.append(reference)
-    run('docker rmi %s' % ' '.join(images), raise_on_error=False)
+    run('docker rmi {0}'.format(' '.join(images)), raise_on_error=False)
     click.echo('Done.')
 
 
 def main():
     cli(obj={})
```

### Comparing `teamplify-0.7.0/teamplify_runner/configurator.py` & `teamplify-0.7.1/teamplify_runner/configurator.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,118 +16,118 @@
     """
     Supports a single error or a list of errors
     """
     def __init__(self, message, *args, **kwargs):
         if isinstance(message, (list, tuple)):
             self.messages = message
             if len(self.messages) > 1:
-                message = '%s errors found' % len(self.messages)
+                message = '{0} errors found'.format(len(self.messages))
             else:
                 message = self.messages[0]
         else:
             self.messages = [message]
         super().__init__(message, *args, **kwargs)
 
     def __str__(self):
         if len(self.messages) > 1:
-            return '%s errors found:\n' % len(self.messages) + '\n'.join([
-                ' -> %s' % m for m in self.messages
+            return '{0} errors found:\n'.format(len(self.messages)) + '\n'.join([
+                ' -> {0}'.format(m) for m in self.messages
             ])
         return self.messages[0]
 
 
 def validate_hostname(hostname):
     try:
         socket.gethostbyname(hostname)
     except socket.gaierror:
-        raise ConfigurationError("Can't resolve hostname: %s" % hostname)
+        raise ConfigurationError("Can't resolve hostname: {0}".format(hostname))
 
 
 def validate_integer(value, min=None, max=None):    # noqa C901
     try:
         value = int(value)
     except ValueError:
-        raise ConfigurationError('Must be an integer. You provided: %s' % value)
+        raise ConfigurationError('Must be an integer. You provided: {0}'.format(value))
     if min is not None and value < min:
         raise ConfigurationError(
-            'Must be greater or equal to %s. You provided: %s' % (min, value),
+            'Must be greater or equal to {0}. You provided: {1}'.format(min, value),
         )
     if max is not None and value > max:
         raise ConfigurationError(
-            'Must be less or equal to %s. You provided: %s' % (max, value),
+            'Must be less or equal to {0}. You provided: {1}'.format(max, value),
         )
 
 
 def validate_certs(path, hostname):
     if not os.path.isdir(path):
         raise ConfigurationError(
             'The path to certificates directory must be valid. '
-            'You provided: %s' % path,
+            'You provided: {0}'.format(path),
         )
 
-    cert_filename = '%s.crt' % hostname
-    key_filename = '%s.key' % hostname
+    cert_filename = '{0}.crt'.format(hostname)
+    key_filename = '{0}.key'.format(hostname)
     cert_found = os.path.isfile(os.path.join(path, cert_filename))
     key_found = os.path.isfile(os.path.join(path, key_filename))
     cert_files_found = cert_found and key_found
 
     cert_dirname = os.path.join(path, hostname)
     cert_dir_exists = os.path.isdir(cert_dirname)
     cert_dir_found = cert_dir_exists and any(
         [fname.endswith('.pem') for fname in os.listdir(cert_dirname)],
     )
 
     if not (cert_files_found or cert_dir_found):
         raise ConfigurationError(
             'The path to certificates directory must contain both '
             'certificate and key files for the specified host '
-            "('%s', '%s') or '%s' directory with .pem files. "
-            'You provided: %s' % (cert_filename, key_filename, hostname, path),
+            "('{0}', '{1}') or '{2}' directory with .pem files. "
+            'You provided: {3}'.format(cert_filename, key_filename, hostname, path),
         )
 
 
 validate_port = partial(validate_integer, min=0, max=65535)
 
 
 def validate_boolean(value):
     if value.lower() not in ('yes', 'no', 'y', 'n', 'true', 'false', '0', '1'):
         raise ConfigurationError(
             'Must be yes or no, or true / false, or 1 / 0. '
-            'You provided: %s' % value,
+            'You provided: {0}'.format(value),
         )
 
 
 def str_to_bool(s):
     return s.lower() in ('yes', 'y', 'true', '1')
 
 
 def validate_choice(value, choices):
     if value not in choices:
         raise ConfigurationError(
-            'Must be one of the following: %s. You provided: %s' % (
+            'Must be one of the following: {0}. You provided: {1}'.format(
                 ', '.join(choices),
                 value,
             ),
         )
 
 
 def validate_email(value):
     """
     Not going to write insane regex here,
     just make sure that it contains exactly one @ surrounded by letters.
     """
     if not re.match(r'^[^@]*\w+@\w+[^@]*$', value):
-        raise ConfigurationError('Invalid email: %s' % value)
+        raise ConfigurationError('Invalid email: {0}'.format(value))
 
 
 def validate_product_key(value):
     if not value:
         raise ConfigurationError('Product key is missing')
     if not re.match('^svr_[A-Za-z0-9]{16}-[A-Za-z0-9]{20}$', value):
-        raise ConfigurationError('Invalid product key: %s' % value)
+        raise ConfigurationError('Invalid product key: {0}'.format(value))
 
 
 class Configurator:
     defaults = OrderedDict((
         ('main', OrderedDict((
             ('product_key', ''),
             ('update_channel', 'stable'),
@@ -184,15 +184,15 @@
         self.parser.read_dict(self.defaults)
 
     def load(self, config_path=None):
         if config_path:
             self.config_path = config_path
         if self.config_path:
             if not os.path.exists(self.config_path):
-                raise RuntimeError('File not found: %s' % self.config_path)
+                raise RuntimeError('File not found: {0}'.format(self.config_path))
             self.parser.read(self.config_path)
         return self
 
     def loads(self, configuration):
         self.parser.read_string(configuration)
         return self
 
@@ -256,35 +256,35 @@
 
     def validate(self):
         errors = []
         for section in self.parser.sections():
             if section not in self.defaults:
                 # Check unknown sections here, because we don't want lots of
                 # errors for each option in unknown section
-                errors.append('Unknown section: [%s]' % section)
+                errors.append('Unknown section: [{0}]'.format(section))
                 continue
             for option in self.parser.options(section):
                 try:
                     self.validate_option(
                         section=section,
                         option=option,
                         value=self.parser.get(section, option),
                     )
                 except ConfigurationError as e:
-                    errors.append('[%s] %s: %s' % (section, option, str(e)))
+                    errors.append('[{0}] {1}: {2}'.format(section, option, str(e)))
         if errors:
             raise ConfigurationError(errors)
         return self
 
     def is_letsencrypt(self):
         return self.parser.get('web', 'ssl_certs', fallback='') == ''
 
     def validate_option(self, section, option, value):
         if section not in self.defaults:
-            raise ConfigurationError('Unknown section: [%s]' % section)
+            raise ConfigurationError('Unknown section: [{}]'.format(section))
 
         if option not in self.defaults[section]:
             raise ConfigurationError('Unknown option')
 
         value = self.parser.get(section, option)
         if section == 'main':
             if option == 'product_key':
@@ -307,15 +307,15 @@
                 if value != '80'\
                         and self.ssl_mode() == 'builtin' \
                         and self.is_letsencrypt():
                     raise ConfigurationError(
                         'For the built-in support of the SSL-enabled '
                         'configuration if there is no SSL certificates '
                         'provided, the web port must be set to 80. '
-                        'You provided: %s' % value,
+                        'You provided: {0}'.format(value),
                     )
             elif option == 'ssl_port':
                 validate_port(value)
                 if value == '80':
                     raise ConfigurationError(
                         "Can't use port 80 because it's reserved for the "
                         'SSL-enabled configuration. Please choose another port',
@@ -323,33 +323,33 @@
                 if value != '443' \
                         and self.ssl_mode() == 'builtin' \
                         and self.is_letsencrypt():
                     raise ConfigurationError(
                         'For the built-in support of the SSL-enabled '
                         'configuration if there is no SSL certificates '
                         'provided, the ssl port must be set to 443. '
-                        'You provided: %s' % value,
+                        'You provided: {0}'.format(value),
                     )
             elif option == 'use_ssl':
                 validate_choice(value, ['no', 'builtin', 'external'])
             elif option == 'ssl_certs':
                 hostname = self.parser.get('web', 'host', fallback='').lower()
                 if value and hostname and self.ssl_mode() == 'builtin':
                     validate_certs(value, hostname)
         elif section == 'db':
             if option == 'host' and value.lower() != 'builtin_db':
                 validate_hostname(value)
             elif option == 'port':
                 validate_port(value)
             elif option == 'backup_mount':
                 if not os.path.isdir(value):
-                    raise ConfigurationError('Must be a directory: %s' % value)
+                    raise ConfigurationError('Must be a directory: {0}'.format(value))
                 if not os.access(value, os.W_OK):
                     raise ConfigurationError(
-                        'Write permission denied: %s' % value,
+                        'Write permission denied: {0}'.format(value),
                     )
         elif section == 'email':
             if option == 'smtp_host' and value.lower() != 'builtin_smtp':
                 validate_hostname(value)
             elif option == 'smtp_protocol':
                 validate_choice(value, ['plain', 'ssl', 'tls'])
             elif option == 'smtp_port':
```

### Comparing `teamplify-0.7.0/teamplify_runner/docker-compose.yml` & `teamplify-0.7.1/teamplify_runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `teamplify-0.7.0/teamplify_runner/utils.py` & `teamplify-0.7.1/teamplify_runner/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     result = sarge.run(cmd, **kwargs)
     code = result.returncode
     if code and raise_on_error:
         if capture_output:
             echo_output(result.stdout.read(), result.stderr.read())
         # print two last traceback records: current line and run caller
         traceback.print_stack(limit=2)
-        msg = 'Command failed, exit code %s' % code
+        msg = 'Command failed, exit code {0}'.format(code)
         if exit_on_error:
             click.echo(msg)
             exit(1)
         else:
             raise RuntimeError(msg)
     if capture_output:
         stdout = result.stdout.read()
```

### Comparing `teamplify-0.7.0/teamplify_runner/uwsgi_params.conf` & `teamplify-0.7.1/teamplify_runner/uwsgi_params.conf`

 * *Files identical despite different names*

### Comparing `teamplify-0.7.0/teamplify_runner/vhost.conf` & `teamplify-0.7.1/teamplify_runner/vhost.conf`

 * *Files identical despite different names*

