# Comparing `tmp/satdigitalinvoice-4.0.2.tar.gz` & `tmp/satdigitalinvoice-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.2.tar", last modified: Tue Apr 25 04:43:20 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.3.tar", last modified: Tue Apr 25 06:22:39 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.2.tar` & `satdigitalinvoice-4.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37878 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.496488 satdigitalinvoice-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.488489 satdigitalinvoice-4.0.3/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37880 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 06:22:39.000000 satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 06:22:39.000000 satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:22:39.000000 satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 06:22:39.000000 satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 06:22:39.000000 satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:22:39.496488 satdigitalinvoice-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:22:39.492488 satdigitalinvoice-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-25 06:22:16.000000 satdigitalinvoice-4.0.3/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.2/PKG-INFO` & `satdigitalinvoice-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.2
+Version: 4.0.3
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/facturacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             f"Facturación Mensual CFDI 4.0 {self.csd_signer.rfc}",
             make_layout(bool(self.fiel_signer), self.local_db),
             size=(1280, 720),
             resizable=True,
             font=("Courier New", 10, "bold"),
             ttk_theme="default",
             margins=(0, 0),
-            use_custom_titlebar=True,
+            # use_custom_titlebar=True,
             titlebar_font=("Courier New", 11, "bold"),
             finalize=True,
         )
 
         self.action_button_manager = ActionButtonManager(
             button=self.window["crear_facturas"],
             preview=self.window["ver_preview"],
```

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.3/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.3/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.3/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.3/satdigitalinvoice/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,13 @@
     if estatus == 'Vigente':
         return EstadoComprobante.Vigente.value
     elif estatus == 'Cancelado':
         return EstadoComprobante.Cancelado.value
     raise ValueError(f"Unknown status: {estatus}")
 
 
-def to_datetime(s):
-    try:
-        return datetime.fromisoformat(s, )
-    except ValueError:
-        return None
-
-
 def open_file(filename):
     if sys.platform == "win32":
         os.startfile(filename)
     else:
         opener = "open" if sys.platform == "darwin" else "xdg-open"
         subprocess.call([opener, filename])
```

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.2
+Version: 4.0.3
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.3/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/setup.py` & `satdigitalinvoice-4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.3/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/tests/test_localdb.py` & `satdigitalinvoice-4.0.3/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.2/tests/test_main.py` & `satdigitalinvoice-4.0.3/tests/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 
 def test_increase_month():
     d = DatePeriod(2021, 1)
     d = add_month(d, 1)
     assert d.year == 2021 and d.month == 2
 
 
-def test_app_setup():
-    config = ConfigManager()
-    a = FacturacionGUI(
-        config
-    )
+# def test_app_setup():
+#     config = ConfigManager()
+#     a = FacturacionGUI(
+#         config
+#     )
```

