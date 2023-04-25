# Comparing `tmp/auterion-cli-1.0.5.tar.gz` & `tmp/auterion-cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.0.5.tar", last modified: Thu Apr 13 14:30:59 2023, max compression
+gzip compressed data, was "auterion-cli-1.0.6.tar", last modified: Tue Apr 25 12:58:48 2023, max compression
```

## Comparing `auterion-cli-1.0.5.tar` & `auterion-cli-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.743423 auterion-cli-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 14:30:59.000000 auterion-cli-1.0.5/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:59.739423 auterion-cli-1.0.5/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:30:59.743423 auterion-cli-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-13 14:30:51.000000 auterion-cli-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 12:58:47.000000 auterion-cli-1.0.6/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 12:58:48.000000 auterion-cli-1.0.6/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 12:58:48.532378 auterion-cli-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-25 12:58:38.000000 auterion-cli-1.0.6/setup.py
```

### Comparing `auterion-cli-1.0.5/README.md` & `auterion-cli-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.0.6/auterion_cli.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 auterioncli/commands/utils.py
 auterioncli/commands/app_sdk/__init__.py
 auterioncli/commands/app_sdk/app_build_command.py
 auterioncli/commands/app_sdk/app_init_command.py
 auterioncli/commands/app_sdk/app_install_command.py
 auterioncli/commands/app_sdk/environment.py
 auterioncli/commands/app_sdk/slimify.py
-auterioncli/commands/app_sdk/update.py
+auterioncli/commands/app_sdk/update.py
+auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
```

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_command.py` & `auterion-cli-1.0.6/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 import shutil
 import pathlib
 import yaml
+import json
 import tempfile
+import jsonschema
 from auterioncli.commands.command_base import CliCommand
-from auterioncli.commands.app_sdk.environment import ensure_docker, ensure_mender_artifact, MENDER_CI_TOOLS_TAG
+from auterioncli.commands.app_sdk.environment import \
+    ensure_docker, ensure_mender_artifact, check_not_running_in_docker, MENDER_CI_TOOLS_TAG
 from auterioncli.commands.app_sdk.slimify import slimify
 import subprocess
 import collections.abc
 import re
 import copy
 import sys
 
@@ -53,24 +56,29 @@
 
     def __init__(self, config):
         self._temp_dir = None
         self._config = config
 
     def setup_parser(self, parser):
         parser.add_argument('project_dir', help='Location of the project', nargs='?', default='.')
-        parser.add_argument('--skip-docker-build', '-s', help='Do not execute docker build step. Just package.')
+        parser.add_argument('--skip-docker-build', help='Do not execute docker build step. Just package.', action='store_true')
+        parser.add_argument('--skip-packaging', help='Do not create an AuterionOS app, just build the docker images and leave them in local docker.', action='store_true')
 
     def run(self, args):
         compose_cmd = ensure_docker()
         ensure_mender_artifact()
+        check_not_running_in_docker()
 
         self._temp_dir = tempfile.mkdtemp()
         meta = self._load_metadata(args)
+        self._verify_metadata(meta)
 
         image_path = self._generate_image(compose_cmd, args, meta)
+        if args.skip_packaging:
+            return
 
         if re.match('^v\d+$', meta['auterion-app-base']):
             v = meta['auterion-app-base']
             base_image_name = 'auterion/app-base:' + meta['auterion-app-base']
             slimify(image_path, base_image_name, self._config['persistent_dir'])
             print('┌──────────────────────────────────────────────────────────────────────────────────────┐')
             print('│                                                                                      │')
@@ -88,27 +96,33 @@
             print(f'.. {meta["auterion-app-base"]} does not match a valid app-base version. Skipping slimify step.')
         compressed_image = self._compress_image(image_path)
 
         self._mender_package_app(args, meta, compressed_image)
         shutil.rmtree(self._temp_dir)
 
     @staticmethod
+    def _verify_metadata(meta):
+        schema_path = pathlib.Path(os.path.join(os.path.dirname(__file__), 'app-yml-spec'))
+        resolver = jsonschema.validators.RefResolver(base_uri=f'{schema_path.as_uri()}/', referrer=True)
+        try:
+            jsonschema.validate(instance=meta, schema={'$ref': 'app-yml-spec.json'}, resolver=resolver)
+        except jsonschema.ValidationError as e:
+            error(f'Error: auterion-app.yml contains error. {e.message}')
+
+    @staticmethod
     def _load_metadata(args):
         project_dir = args.project_dir
         meta_file = os.path.join(project_dir, 'auterion-app.yml')
 
         if not os.path.exists(meta_file):
             error(f'File \'{meta_file}\' does not exist. App structure invalid. Aborting...')
 
         with open(meta_file, 'r') as f:
             meta = yaml.safe_load(f)
 
-        if 'app-name' not in meta or 'app-version' not in meta:
-            error(f'{meta_file} does not contain app-name or app-version')
-
         if 'app-author' not in meta:
             error(f'{meta_file} does not contain `app-author` key. This field should contain a reverse-domain of the'
                   f'entity that authored the app, e.g. `com.auterion`')
         return meta
 
     def _extract_target_devices(self, meta):
         target_devices = [meta['target-platform']] \
@@ -196,14 +210,20 @@
         for image in images:
             # Make sure that we correctly tag all images with the docker.io prefix. This is not
             # guaranteed on alternative runtimes such as podman
             run_command(['docker', 'tag', image, 'docker.io/' + image], cwd=project_dir)
             print('retagging...')
         images = ['docker.io/' + image for image in images]
 
+        if (args.skip_packaging):
+            print('Skipping packaging of images. Leaving images in docker:')
+            for image in images:
+                print(f'- {image}')
+            return None
+
         print('Packaging those images...')
         if os.path.isfile(target_file):
             os.remove(target_file)
         run_command(['docker', 'save'] + images + ['-o', target_file], cwd=project_dir)
 
         return target_file
```

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.0.6/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.0.6/auterioncli/commands/app_sdk/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,7 +74,14 @@
         print('> Pulling mender ci-tools ...')
         code, result = try_command(['docker', 'pull', MENDER_CI_TOOLS_TAG])
         if code != 0:
             error(f'Could not pull {MENDER_CI_TOOLS_TAG} image from docker hub. Exiting.')
 
     if not _test_mender_artifact():
         error(f'Error: Failed to execute mender artifact in image {MENDER_CI_TOOLS_TAG}. Aborting.')
+
+
+def check_not_running_in_docker():
+    if os.path.exists('/.dockerenv'):
+        print('Detected to be running inside docker. The app build command needs to to execute docker commands'
+              'that are only possible from the host system.', file=sys.stderr)
+        error('Error: auterion-cli app build should not be run inside a docker container. Exiting.')
```

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.0.6/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.0.6/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/container_command.py` & `auterion-cli-1.0.6/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/device_command.py` & `auterion-cli-1.0.6/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/info_command.py` & `auterion-cli-1.0.6/auterioncli/commands/info_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,32 +81,32 @@
         print("\n===== Software Information =====")
         software = self._get_information("software")
         if software:
             for name, data in software.items():
                 print("{}:".format(name))
                 if data['status'] == "running":
                     status_str = "[\033[32mRUNNING\033[39m]"
-                elif data['status'] == "succeed":
-                    status_str = "[\033[32mSUCCEED\033[39m]"
+                elif data['status'] == "succeeded":
+                    status_str = "[\033[32mSUCCEEDED\033[39m]"
                 else:
                     status_str = "[\033[31mERROR\033[39m]"
                 print("\thash: {}".format(data['hash']))
                 print("\tstatus: {}".format(status_str))
         else:
             print("No software information available")
 
         print("\n===== System services Information =====")
         services = self._get_information("services")
         if services:
             for software, data in services.items():
                 print("{}:".format(software))
                 if data['status'] == "running":
                     status_str = "[\033[32mRUNNING\033[39m]"
-                elif data['status'] == "succeed":
-                    status_str = "[\033[32mSUCCEED\033[39m]"
+                elif data['status'] == "succeeded":
+                    status_str = "[\033[32mSUCCEEDED\033[39m]"
                 else:
                     status_str = "[\033[31mERROR\033[39m]"
                 print("\tstatus: {}".format(status_str))
         else:
             print("No services information available")
 
         print("\n===== USB devices Information =====")
```

### Comparing `auterion-cli-1.0.5/auterioncli/commands/report_command.py` & `auterion-cli-1.0.6/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/commands/utils.py` & `auterion-cli-1.0.6/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/main.py` & `auterion-cli-1.0.6/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/auterioncli/meta_util.py` & `auterion-cli-1.0.6/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.5/setup.py` & `auterion-cli-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
           'tabulate',
           'requests',
           'requests_toolbelt',
           'zeroconf',
           'websockets',
           'packaging',
           'tqdm',
-          'pyyaml'
+          'pyyaml',
+          'jsonschema'
       ],
       python_requires='>=3.6',
       zip_safe=False,
+      include_package_data=True,
       entry_points={
           'console_scripts': ['auterion-cli=auterioncli.main:main']
       })
```

