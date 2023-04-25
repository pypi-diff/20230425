# Comparing `tmp/gwbackupy-0.8.0.tar.gz` & `tmp/gwbackupy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwbackupy-0.8.0.tar", last modified: Thu Jan 19 22:38:04 2023, max compression
+gzip compressed data, was "gwbackupy-0.9.0.tar", last modified: Mon Jan 23 22:41:57 2023, max compression
```

## Comparing `gwbackupy-0.8.0.tar` & `gwbackupy-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.366146 gwbackupy-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-01-19 22:38:04.366146 gwbackupy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.362146 gwbackupy-0.8.0/gwbackupy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.362146 gwbackupy-0.8.0/gwbackupy/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/filters/filter_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/filters/gmail_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/global_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/gwbackupy_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/process_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.362146 gwbackupy-0.8.0/gwbackupy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/providers/gapi_gmail_service_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/providers/gapi_service_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/providers/gmail_service_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/providers/gmail_service_wrapper_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/providers/service_provider_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.366146 gwbackupy-0.8.0/gwbackupy/storage/
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/gwbackupy/storage/storage_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.362146 gwbackupy-0.8.0/gwbackupy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-01-19 22:38:04.000000 gwbackupy-0.8.0/gwbackupy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-01-19 22:38:04.000000 gwbackupy-0.8.0/gwbackupy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:38:04.000000 gwbackupy-0.8.0/gwbackupy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-19 22:38:04.000000 gwbackupy-0.8.0/gwbackupy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-19 22:38:04.000000 gwbackupy-0.8.0/gwbackupy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:38:04.366146 gwbackupy-0.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/scripts/gwbackupy
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-19 22:38:04.366146 gwbackupy-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-19 22:37:53.000000 gwbackupy-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.583283 gwbackupy-0.9.0/gwbackupy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/gwbackupy/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/filters/filter_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/filters/gmail_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/global_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24377 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/gwbackupy_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/process_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/gwbackupy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/providers/gapi_gmail_service_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/providers/gapi_service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/providers/gmail_service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/providers/gmail_service_wrapper_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/providers/service_provider_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/gwbackupy/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/gwbackupy/storage/storage_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.583283 gwbackupy-0.9.0/gwbackupy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-01-23 22:41:57.000000 gwbackupy-0.9.0/gwbackupy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-01-23 22:41:57.000000 gwbackupy-0.9.0/gwbackupy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 22:41:57.000000 gwbackupy-0.9.0/gwbackupy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-23 22:41:57.000000 gwbackupy-0.9.0/gwbackupy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-23 22:41:57.000000 gwbackupy-0.9.0/gwbackupy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/scripts/gwbackupy
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-23 22:41:57.587283 gwbackupy-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-01-23 22:41:48.000000 gwbackupy-0.9.0/setup.py
```

### Comparing `gwbackupy-0.8.0/LICENSE` & `gwbackupy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/PKG-INFO` & `gwbackupy-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gwbackupy
-Version: 0.8.0
-Summary: Open source Google Workspace backup solution.
-Home-page: https://github.com/smartondev/gwbackupy
-Author: Márton Somogyi
-Author-email: info@smarton.dev
-License: BSD 3-Clause "New" or "Revised" License
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gwbackupy: Google Workspace™ backup and restore solution.
 
 [![0.2.0](https://img.shields.io/github/v/release/smartondev/gwbackupy)](https://github.com/smartondev/gwbackupy/releases)
 [![0.2.0](https://img.shields.io/pypi/v/gwbackupy)](https://pypi.org/project/gwbackupy/)
 [![BSD-3-Clause](https://img.shields.io/github/license/smartondev/gwbackupy)](LICENSE)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/smartondev/gwbackupy)](https://coveralls.io/github/smartondev/gwbackupy?branch=main)
```

### Comparing `gwbackupy-0.8.0/README.md` & `gwbackupy-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: gwbackupy
+Version: 0.9.0
+Summary: Open source Google Workspace backup solution.
+Home-page: https://github.com/smartondev/gwbackupy
+Author: Márton Somogyi
+Author-email: info@smarton.dev
+License: BSD 3-Clause "New" or "Revised" License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gwbackupy: Google Workspace™ backup and restore solution.
 
 [![0.2.0](https://img.shields.io/github/v/release/smartondev/gwbackupy)](https://github.com/smartondev/gwbackupy/releases)
 [![0.2.0](https://img.shields.io/pypi/v/gwbackupy)](https://pypi.org/project/gwbackupy/)
 [![BSD-3-Clause](https://img.shields.io/github/license/smartondev/gwbackupy)](LICENSE)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Coverage Status](https://img.shields.io/coverallsCoverage/github/smartondev/gwbackupy)](https://coveralls.io/github/smartondev/gwbackupy?branch=main)
```

### Comparing `gwbackupy-0.8.0/gwbackupy/filters/gmail_filter.py` & `gwbackupy-0.9.0/gwbackupy/filters/gmail_filter.py`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/gwbackupy/gmail.py` & `gwbackupy-0.9.0/gwbackupy/gmail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import collections
 import concurrent.futures
+import copy
 import gzip
 import json
 import logging
 import threading
 from datetime import datetime, timedelta
 
 from gwbackupy import global_properties
@@ -72,23 +73,47 @@
 
     def __store_message_file(
         self, message_id: str, raw_message: bytes, create_timestamp: float
     ):
         logging.debug("Store message {id}".format(id=message_id))
         link = self.storage.new_link(
             object_id=message_id, extension="eml.gz", created_timestamp=create_timestamp
-        ).set_properties({LinkInterface.property_object: True})
+        ).set_properties(
+            {
+                LinkInterface.property_object: True,
+                LinkInterface.property_content_hash: self.storage.content_hash_generate(
+                    raw_message
+                ),
+            }
+        )
         result = self.__storage_put(
             link, data=gzip.compress(raw_message, compresslevel=9)
         )
         if result:
             logging.info(f"{message_id} message is saved")
         else:
             raise Exception("Mail message save failed")
 
+    def __fix_content_hash_to_message_object(
+        self, message_id: str, link: LinkInterface
+    ) -> LinkInterface:
+        if link.get_property(LinkInterface.property_content_hash) is not None:
+            return link
+        logging.debug(f"{message_id} message object not has content hash, add it")
+        with self.storage.get(link) as mf:
+            message_content = gzip.decompress(mf.read())
+            content_hash = self.storage.content_hash_generate(message_content)
+        new_object_link = copy.deepcopy(link)
+        new_object_link.set_properties(
+            {LinkInterface.property_content_hash: content_hash}
+        )
+        self.storage.modify(link, new_object_link)
+        logging.debug(f"{message_id} message object is signed by content hash")
+        return new_object_link
+
     def __backup_messages(
         self, message, stored_messages: dict[str, dict[int, LinkInterface]]
     ):
         message_id = message.get("id", "UNKNOWN")  # for logging
         try:
             # if message_id != '1853ee437c8ff302':
             #     raise Exception('SKIP')
@@ -98,14 +123,19 @@
                 latest_meta_link = stored_messages[message_id][0]
             is_new = latest_meta_link is None
             if is_new:
                 logging.debug(f"{message_id} is new")
             # TODO: option for force raw mode
             message_format = "raw"
             if not is_new and stored_messages[message_id][1] is not None:
+                stored_messages[message_id][
+                    1
+                ] = self.__fix_content_hash_to_message_object(
+                    message_id, stored_messages[message_id][1]
+                )
                 message_format = "minimal"
             data = self.__get_message_from_server(message_id, message_format)
             if data is None:
                 # (deleted)
                 logging.info(f"{message_id} is not found on server")
                 return
 
@@ -219,15 +249,14 @@
     def backup(self, quick_sync_days: int | None = None) -> bool:
         logging.info(f"Starting backup for {self.email}")
         self.__error_count = 0
 
         logging.info("Scanning backup storage...")
         stored_data_all = self.storage.find()
         logging.info(f"Stored items: {len(stored_data_all)}")
-        self.__service_wrapper.get_service_provider().storage_links(stored_data_all)
 
         labels_link = stored_data_all.find(
             f=lambda l: l.id() == Gmail.object_id_labels and l.is_metadata
         )
         if not self.__backup_labels(labels_link):
             logging.error("Backup finished with storing labels failed")
             return False
@@ -494,15 +523,14 @@
         if not restore_deleted and not restore_missing:
             logging.warning("Tasks not found, see more e.g. --restore-deleted")
             return True
 
         logging.info("Scanning backup storage...")
         stored_data_all = self.storage.find()
         logging.info(f"Stored items: {len(stored_data_all)}")
-        self.__service_wrapper.get_service_provider().storage_links(stored_data_all)
 
         latest_labels_from_storage = self.__load_labels_from_storage(stored_data_all)
         if latest_labels_from_storage is None:
             logging.error("Stored labels loading failed")
             return False
         _labels_from_server = self.__get_labels_from_server()
         if _labels_from_server is None:
```

### Comparing `gwbackupy-0.8.0/gwbackupy/gwbackupy_cli.py` & `gwbackupy-0.9.0/gwbackupy/gwbackupy_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from tzlocal import get_localzone
 
 import gwbackupy.global_properties as global_properties
 from gwbackupy.filters.gmail_filter import GmailFilter
 from gwbackupy.gmail import Gmail
 from gwbackupy.helpers import parse_date
 from gwbackupy.providers.gapi_gmail_service_wrapper import GapiGmailServiceWrapper
+from gwbackupy.providers.gapi_service_provider import AccessNotInitializedError
 from gwbackupy.providers.gmail_service_provider import GmailServiceProvider
 from gwbackupy.storage.file_storage import FileStorage
 
 lock = threading.Lock()
 
 
 def parse_arguments() -> argparse.Namespace:
@@ -81,14 +82,27 @@
         required=False,
         default="./data",
     )
     service_parser = parser.add_subparsers(dest="service")
     gmail_parser = service_parser.add_parser("gmail", help="GMail service commands")
     gmail_command_parser = gmail_parser.add_subparsers(dest="command")
 
+    gmail_oauth_init_parser = gmail_command_parser.add_parser(
+        "access-init", help="Access initialization e.g. OAuth authentication"
+    )
+    gmail_oauth_init_parser.add_argument(
+        "--email", type=str, help="Email account", required=True
+    )
+    gmail_oauth_check_parser = gmail_command_parser.add_parser(
+        "access-check", help="Check access e.g. OAuth tokens"
+    )
+    gmail_oauth_check_parser.add_argument(
+        "--email", type=str, help="Email account", required=True
+    )
+
     gmail_backup_parser = gmail_command_parser.add_parser("backup", help="Backup gmail")
     gmail_backup_parser.add_argument(
         "--email", type=str, help="Email of the account", required=True
     )
     gmail_backup_parser.add_argument(
         "--quick-sync-days",
         type=int,
@@ -166,37 +180,46 @@
 
 
 def cli_startup():
     try:
         args = parse_arguments()
         if args.service == "gmail":
             storage = FileStorage(args.workdir + "/" + args.email + "/gmail")
+            storage_oauth_tokens = FileStorage(args.workdir + "/oauth-tokens")
             service_provider = GmailServiceProvider(
                 credentials_file_path=args.credentials_filepath,
                 service_account_email=args.service_account_email,
                 service_account_file_path=args.service_account_key_filepath,
-                storage=storage,
+                storage=storage_oauth_tokens,
             )
             service_wrapper = GapiGmailServiceWrapper(
                 service_provider=service_provider,
                 dry_mode=args.dry,
             )
             gmail = Gmail(
                 email=args.email,
                 service_wrapper=service_wrapper,
                 batch_size=args.batch_size,
                 storage=storage,
                 dry_mode=args.dry,
             )
-            if args.command == "backup":
+            if args.command == "access-init":
+                service_wrapper.get_labels(args.email)
+            elif args.command == "access-check":
+                try:
+                    with service_provider.get_service(args.email, False) as s:
+                        service_wrapper.get_labels(args.email)
+                except AccessNotInitializedError:
+                    exit(1)
+            elif args.command == "backup":
                 if gmail.backup(quick_sync_days=args.quick_sync_days):
                     exit(0)
                 else:
                     exit(1)
-            if args.command == "restore":
+            elif args.command == "restore":
                 if args.add_labels is None:
                     args.add_labels = ["gwbackupy"]
                 item_filter = GmailFilter()
                 if args.restore_deleted:
                     item_filter.is_deleted()
                     logging.info("Filter options: deleted")
                 if args.restore_missing:
```

### Comparing `gwbackupy-0.8.0/gwbackupy/helpers.py` & `gwbackupy-0.9.0/gwbackupy/helpers.py`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/gwbackupy/process_helpers.py` & `gwbackupy-0.9.0/gwbackupy/process_helpers.py`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/gwbackupy/providers/gapi_gmail_service_wrapper.py` & `gwbackupy-0.9.0/gwbackupy/providers/gapi_gmail_service_wrapper.py`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/gwbackupy/providers/gapi_service_provider.py` & `gwbackupy-0.9.0/gwbackupy/providers/gapi_service_provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,80 +19,84 @@
 from gwbackupy.storage.storage_interface import (
     LinkInterface,
     StorageInterface,
     LinkList,
 )
 
 
+class AccessNotInitializedError(Exception):
+    pass
+
+
 class GapiServiceProvider(ServiceProviderInterface):
     object_id_token = LinkInterface.id_special_prefix + "token--"
     """object ID for access token save and load"""
 
     def __init__(
         self,
         service_name: str,
         version: str,
         scopes: [str],
+        storage: StorageInterface,
         credentials_file_path: str | None = None,
         service_account_file_path: str | None = None,
         service_account_email: str | None = None,
-        storage: StorageInterface | None = None,
     ):
         self.service_name = service_name
         self.version = version
         self.scopes = scopes
         self.credentials_file_path = credentials_file_path
         self.service_account_file_path = service_account_file_path
         self.service_account_email = service_account_email
         self.storage = storage
         self.tlock = threading.RLock()
         self.services: dict[str, list[any]] = dict()
-        self.credentials_token_links: dict[str, LinkInterface] = dict()
+        self.credentials_token_links: dict[
+            str, LinkInterface
+        ] = self.storage.find().find(
+            f=lambda l: l.id() == GapiServiceProvider.object_id_token,
+            g=lambda l: [l.get_properties().get("email", "")],
+        )
 
     def release_service(self, email: str, service):
         logging.debug(f"Release service ({email})")
         if service is None:
             return
         with self.tlock:
             if email not in self.services:
                 return
             self.services[email].append(service)
 
-    def get_service(self, email: str):
+    def get_service(self, email: str, access_init: bool = True):
         service = None
         with self.tlock:
             if email not in self.services.keys():
                 self.services[email] = []
             if len(self.services[email]) > 0:
                 logging.debug(f"Reuse service ({email})")
                 service = self.services[email].pop()
             if service is None:
                 logging.debug("Create new service")
                 if self.credentials_file_path is not None:
-                    credentials = self.__get_credentials_by_oauth(email)
+                    credentials = self.__get_credentials_by_oauth(
+                        email, access_init=access_init
+                    )
                 elif self.service_account_file_path is not None:
                     credentials = self.__get_credentials_by_service_account(email)
                 else:
                     raise Exception(f"Not supported credentials")
                 if not credentials:
                     raise Exception(f"Credentials cannot be None")
                 service = build(
                     self.service_name,
                     self.version,
                     credentials=credentials,
                 )
         return ServiceItem(self, email, service)
 
-    def storage_links(self, links: LinkList):
-        """Filter stored tokens for OAuth authentication"""
-        self.credentials_token_links = links.find(
-            f=lambda l: l.id() == GapiServiceProvider.object_id_token,
-            g=lambda l: [l.get_properties().get("email", "")],
-        )
-
     def __get_credentials_by_service_account(self, email: str):
         """get credentials by service account access"""
         extension = self.service_account_file_path.split(".")[-1].lower()
         if extension == "p12":
             if (
                 self.service_account_email is None
                 or self.service_account_email.strip() == ""
@@ -112,15 +116,15 @@
             pass
         else:
             raise Exception(f"Not supported service account file extension")
 
         credentials = credentials.create_delegated(email)
         return credentials
 
-    def __get_credentials_by_oauth(self, email: str):
+    def __get_credentials_by_oauth(self, email: str, access_init: bool = True):
         """Get credentials object from OAuth access. This method store token and reuse/refresh if required"""
         credentials = None
         fd, temp = tempfile.mkstemp()
         email_md5 = hashlib.md5(email.encode("utf-8")).hexdigest().lower()
         if email_md5 in self.credentials_token_links:
             logging.debug("Try to load previously saved token")
             token_link = self.credentials_token_links.get(email_md5)
@@ -135,19 +139,23 @@
                 try:
                     credentials.refresh(Request())
                 except RefreshError as e:
                     logging.exception(f"Failed to refresh token: {e}")
                     credentials = None
             if not credentials:
                 logging.debug("Credentials not found")
+                if not access_init:
+                    raise AccessNotInitializedError()
                 flow = InstalledAppFlow.from_client_secrets_file(
                     self.credentials_file_path,
                     self.scopes,
                 )
-                credentials = flow.run_local_server(port=0, access_type="offline")
+                credentials = flow.run_local_server(
+                    port=0, access_type="offline", include_granted_scopes="true"
+                )
 
             token_link_new = self.storage.new_link(
                 GapiServiceProvider.object_id_token, "json"
             )
             token_link_new.set_properties({"email": email_md5})
             logging.debug(f"Put token to storage ({token_link_new})")
             result = self.storage.put(token_link_new, credentials.to_json())
```

### Comparing `gwbackupy-0.8.0/gwbackupy/providers/gmail_service_provider.py` & `gwbackupy-0.9.0/gwbackupy/providers/gmail_service_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 
 class GmailServiceProvider(GapiServiceProvider):
     """Gmail service provider from gmail/v1 API with full access scope"""
 
     def __init__(
         self,
+        storage: StorageInterface,
         credentials_file_path: str | None = None,
         service_account_file_path: str | None = None,
         service_account_email: str | None = None,
-        storage: StorageInterface | None = None,
     ):
         super().__init__(
             "gmail",
             "v1",
             ["https://mail.google.com/"],
             credentials_file_path=credentials_file_path,
             storage=storage,
```

### Comparing `gwbackupy-0.8.0/gwbackupy/providers/gmail_service_wrapper_interface.py` & `gwbackupy-0.9.0/gwbackupy/providers/gmail_service_wrapper_interface.py`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/gwbackupy/providers/service_provider_interface.py` & `gwbackupy-0.9.0/gwbackupy/providers/service_provider_interface.py`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/gwbackupy/storage/file_storage.py` & `gwbackupy-0.9.0/gwbackupy/storage/file_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import copy
+import hashlib
 import io
 import logging
 import os
 import re
 import shutil
 from builtins import float
 from datetime import datetime, timezone
@@ -76,15 +77,15 @@
                 if isinstance(value, str):
                     if value == "":
                         value = True
                     self.__properties[key] = value
         return self
 
     def get_file_path(self) -> str:
-        path = self.__path + "/" + self.__id
+        path = os.path.join(self.__path, self.__id)
         keys = list(self.__properties.keys())
         keys.sort()
         for k in keys:
             if self.__properties[k] is None:
                 continue
             path += f".{k}="
             if self.__properties[k] is not True:
@@ -227,59 +228,110 @@
             {
                 "deleted": True,
                 "mutation": self.__gen_mutation(),
             }
         )
         try:
             with self.get(link) as f:
-                if not f:
-                    logging.error(f"{link.get_file_path()} not found or not readable")
-                    return False
-                self.put(dst, f)
+                return self.put(dst, f)
         except BaseException as e:
             logging.exception(
                 f"Copy as new mutation is failed {link.get_file_path()} -> {dst.get_file_path()}: {e}"
             )
             return False
-        return True
 
-    def find(self, f: LinkFilter | None = None) -> LinkList[LinkInterface]:
+    def find(self, f: LinkFilter | None = None) -> LinkList[FileLink]:
         abspath = self.root
         skip_path = len(abspath)
-        result: LinkList[LinkInterface] = LinkList([])
+        result: LinkList[FileLink] = LinkList([])
         for _path, _, filenames in os.walk(abspath):
             for file in filenames:
                 file_path = os.path.join(_path, file)
                 relpath = _path[skip_path:]
                 link = FileLink()
                 if len(relpath) > 0:
                     link.path = relpath
                 m = FileLink.parse_file_name(file)
                 if m is None:
                     continue
                 m["path"] = _path
                 link.fill(m)
 
-                if "extension" not in m:
-                    logging.debug(f"Unknown file without extension: {file_path}")
-                    continue
                 if m["extension"] == "tmp":
                     logging.debug(f"Temporary file {file_path}, remove it")
                     try:
                         os.remove(file_path)
                     except BaseException as e:
                         logging.exception(
                             f"Temporary file remove fail {file_path}: {e}"
                         )
                     continue
 
                 if f is None or f(link):
                     result.append(link)
         return result
 
+    def modify(self, link: FileLink, to_link: FileLink) -> bool:
+        if os.path.exists(to_link.get_file_path()):
+            logging.error(
+                f"Modify fail ({link.get_file_path()}): destination link already exists ({to_link.get_file_path()})"
+            )
+            return False
+        try:
+            shutil.move(link.get_file_path(), to_link.get_file_path())
+        except BaseException as e:
+            logging.exception(
+                f"File move fail: {e} ({link.get_file_path()} -> {to_link.get_file_path()})"
+            )
+            return False
+        return True
+
+    def content_hash_add(self, link: FileLink) -> FileLink:
+        try:
+            with self.get(link) as f:
+                content_hash = self.content_hash_generate(f)
+
+            to_link = copy.deepcopy(link)
+            to_link.set_properties({LinkInterface.property_content_hash: content_hash})
+            if self.modify(link, to_link):
+                return to_link
+            raise RuntimeError(f"Link hashing failed ({link.get_file_path()})")
+        except FileNotFoundError:
+            logging.exception(f"File not found: {link.get_file_path()}")
+            raise
+
+    def content_hash_check(self, link: FileLink) -> bool | None:
+        if not link.has_property(LinkInterface.property_content_hash):
+            return None
+        try:
+            with self.get(link) as f:
+                return self.content_hash_eq(link, f)
+        except FileNotFoundError:
+            logging.exception(f"File not found: {link.get_file_path()}")
+            raise
+
+    def content_hash_eq(self, link: FileLink, data: IO[bytes] | bytes | str) -> bool:
+        if not link.has_property(LinkInterface.property_content_hash):
+            return False
+        return self.content_hash_generate(data) == link.get_property(
+            LinkInterface.property_content_hash
+        )
+
+    def content_hash_generate(self, b: IO[bytes] | bytes | str) -> str:
+        if isinstance(b, bytes):
+            data = b
+        elif isinstance(b, str):
+            data = bytes(b, "utf-8")
+        elif isinstance(b, io.BufferedReader):
+            data = b.read()
+        else:
+            raise NotImplementedError(f"Invalid type: {type(b)}")
+
+        return "m" + hashlib.md5(data).hexdigest().lower()
+
     @staticmethod
     def __remove(file_path: str) -> bool:
         try:
             exists = os.path.exists(file_path)
             if not exists:
                 return True
         except BaseException as e:
@@ -318,15 +370,17 @@
                         f.write(bytes(data, "utf-8"))
                     elif isinstance(data, io.BufferedReader):
                         f.write(data.read())
                         data.close()
                     elif callable(data):
                         data(f)
                     else:
-                        raise RuntimeError(f"Not supported data type: {type(data)}")
+                        raise NotImplementedError(
+                            f"Not supported data type: {type(data)}"
+                        )
             except BaseException as e:
                 logging.exception(f"Temporary file writing fail {file_path_tmp}: {e}")
                 return False
             try:
                 shutil.move(file_path_tmp, file_path)
             except BaseException as e:
                 logging.exception(
```

### Comparing `gwbackupy-0.8.0/gwbackupy/storage/storage_interface.py` & `gwbackupy-0.9.0/gwbackupy/storage/storage_interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     This interface represents a link to an storage item.
     """
 
     property_deleted = "deleted"
     property_metadata = "metadata"
     property_object = "object"
     property_mutation = "mutation"
+    property_content_hash = "ch"
     id_special_prefix = "--gwbackupy-"
 
     def id(self) -> str:
         raise NotImplementedError("LinkInterface#id")
 
     def is_special_id(self) -> bool:
         return self.id().startswith(LinkInterface.id_special_prefix)
@@ -149,7 +150,39 @@
         raise NotImplementedError("StorageInterface#put")
 
     def remove(self, link: LinkInterface, as_new_mutation: bool = True) -> bool:
         raise NotImplementedError("StorageInterface#remove")
 
     def find(self, f: LinkFilter | None = None) -> LinkList[LinkInterface]:
         raise NotImplementedError("StorageInterface#find")
+
+    def modify(self, link: LinkInterface, to_link: LinkInterface) -> bool:
+        """
+        modify link to a new link
+        """
+        raise NotImplementedError("StorageInterface#modify")
+
+    def content_hash_add(self, link: LinkInterface) -> LinkInterface:
+        """
+        Add content hash to link, and return with the new link
+        """
+        raise NotImplementedError("StorageInterface#content_hash_add")
+
+    def content_hash_check(self, link: LinkInterface) -> bool | None:
+        """
+        Check content hash on link. If link not contain content hash then return None else return equality
+        """
+        raise NotImplementedError("StorageInterface#content_hash_check")
+
+    def content_hash_eq(
+        self, link: LinkInterface, data: IO[bytes] | bytes | str
+    ) -> bool:
+        """
+        Check content hash equality. If the link is not contain content hash then return False.
+        """
+        raise NotImplementedError("StorageInterface#content_hash_eq")
+
+    def content_hash_generate(self, data: IO[bytes] | bytes | str) -> str:
+        """
+        Generate content hash from input data
+        """
+        raise NotImplementedError("StorageInterface#content_hash_generate")
```

### Comparing `gwbackupy-0.8.0/gwbackupy.egg-info/PKG-INFO` & `gwbackupy-0.9.0/gwbackupy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 Metadata-Version: 2.1
 Name: gwbackupy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open source Google Workspace backup solution.
 Home-page: https://github.com/smartondev/gwbackupy
 Author: Márton Somogyi
 Author-email: info@smarton.dev
 License: BSD 3-Clause "New" or "Revised" License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gwbackupy: Google Workspace™ backup and restore solution.
 
 [![0.2.0](https://img.shields.io/github/v/release/smartondev/gwbackupy)](https://github.com/smartondev/gwbackupy/releases)
```

### Comparing `gwbackupy-0.8.0/gwbackupy.egg-info/SOURCES.txt` & `gwbackupy-0.9.0/gwbackupy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwbackupy-0.8.0/setup.py` & `gwbackupy-0.9.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,11 +26,24 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requires,
     scripts=["scripts/gwbackupy"],
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: Unix",
+        "Environment :: Console",
+        "Programming Language :: Python",
+        "Topic :: System :: Archiving :: Backup",
+        "Topic :: Utilities",
+        "Typing :: Typed",
     ],
 )
```

