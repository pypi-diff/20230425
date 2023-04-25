# Comparing `tmp/bytecli-0.1.1.tar.gz` & `tmp/bytecli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecli-0.1.1.tar", max compression
+gzip compressed data, was "bytecli-0.2.0.tar", max compression
```

## Comparing `bytecli-0.1.1.tar` & `bytecli-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-04-24 19:19:24.275419 bytecli-0.1.1/LICENSE
--rw-r--r--   0        0        0      597 2023-04-24 19:19:24.275419 bytecli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 19:19:24.275419 bytecli-0.1.1/bytecli/__init__.py
--rw-r--r--   0        0        0     2193 2023-04-24 19:19:24.275419 bytecli-0.1.1/bytecli/main.py
--rw-r--r--   0        0        0      456 2023-04-24 19:19:24.275419 bytecli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 bytecli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 09:12:39.624516 bytecli-0.2.0/LICENSE
+-rw-r--r--   0        0        0      597 2023-04-25 09:12:39.624516 bytecli-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 09:12:39.624516 bytecli-0.2.0/bytecli/__init__.py
+-rw-r--r--   0        0        0     3507 2023-04-25 09:12:39.624516 bytecli-0.2.0/bytecli/main.py
+-rw-r--r--   0        0        0      456 2023-04-25 09:12:39.624516 bytecli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 bytecli-0.2.0/PKG-INFO
```

### Comparing `bytecli-0.1.1/LICENSE` & `bytecli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecli-0.1.1/README.md` & `bytecli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bytecli-0.1.1/bytecli/main.py` & `bytecli-0.2.0/bytecli/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 def get_account_info(attribute: str):
     return requests.get(BASE_URL).json()[0][attribute]
 
 
 @app.command()
 def servername() -> None:
-    """Name of serverd"""
+    """Name of server"""
     console.print(
         f'[magenta]Server name:[/magenta] [green]{get_account_info("server_name")}[/green]'
     )
 
 
 @app.command()
 def diskquota() -> None:
@@ -63,25 +63,66 @@
     )
 
 
 @app.command()
 def summary() -> None:
     """Summary of server"""
     response = requests.get(BASE_URL).json()[0]
-    table = Table(
+    server_table = Table(
         show_header=False,
         show_lines=False,
         title=f"Server Summary - [purple]{response['server_name']}[/purple]",
     )
-    table.add_row(
+    server_table.add_row(
         f"[magenta]Disk Quota[/magenta]",
         f"[green]{response['pretty_disk_quota']}[/green]",
     )
-    table.add_row(
+    server_table.add_row(
         f"[magenta]Bandwidth Quota[/magenta]",
         f"[green]{response['pretty_bw_quota']}[/green]",
     )
-    table.add_row(
+    server_table.add_row(
         f"[magenta]Memory Usage[/magenta]",
         f"[green]{round(response['memory_usage'] / 1024, 2)} MB[/green]",
     )
-    console.print(table)
+
+    account_table = Table(
+        show_header=False,
+        show_lines=False,
+        title=f"Account Summary - [purple]{response['server_name']}[/purple]",
+    )
+    account_table.add_row(
+        f"[magenta]Type[/magenta]",
+        f"[green]{response['type']}[/green]",
+    )
+    account_table.add_row(
+        f"[magenta]Plan name[/magenta]",
+        f"[green]{response['plan_name']}[/green]",
+    )
+    account_table.add_row(
+        f"[magenta]Account IP[/magenta]",
+        f"[green]{response['account_ip']}[/green]",
+    )
+
+    console.print(account_table)
+    console.print(server_table)
+
+
+@app.command()
+def apps() -> None:
+    """Installed Applications"""
+    response = requests.get(BASE_URL).json()[0]
+    user_apps = response["user_apps"]
+    app_table = Table(
+        show_header=True,
+        show_lines=False,
+        title=f"Installed Applications - [purple]{response['server_name']}[/purple]",
+    )
+    app_table.add_column("Name", style="dim", width=10, justify="left")
+    app_table.add_column("URL", min_width=20, justify="left")
+    for user_app in user_apps:
+        if user_app["installed"]:
+            app_table.add_row(
+                f'[green]{user_app["app_name"]}[/green]',
+                f'[green]{user_app["webui_url"]}[/green]',
+            )
+    console.print(app_table)
```

### Comparing `bytecli-0.1.1/PKG-INFO` & `bytecli-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecli
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Allan
 Author-email: allanklp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

