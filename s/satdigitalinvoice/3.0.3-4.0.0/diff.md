# Comparing `tmp/satdigitalinvoice-3.0.3.tar.gz` & `tmp/satdigitalinvoice-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-3.0.3.tar", last modified: Mon Apr 17 06:15:52 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.0.tar", last modified: Tue Apr 25 01:55:33 2023, max compression
```

## Comparing `satdigitalinvoice-3.0.3.tar` & `satdigitalinvoice-4.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    34675 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.018338 satdigitalinvoice-4.0.0/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37891 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.018338 satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.018338 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_main.py
```

### Comparing `satdigitalinvoice-3.0.3/PKG-INFO` & `satdigitalinvoice-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.3
+Version: 4.0.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 import os
-import sys
 from zipfile import ZipFile
-import PySimpleGUI as sg
-
 
+import PySimpleGUI as sg
 
 SOURCE_DIRECTORY = os.path.dirname(__file__)
 
 DATA_DIRECTORY = ".data"
 ARCHIVOS_DIRECTORY = "archivos"
+METADATA_FILE = os.path.join(ARCHIVOS_DIRECTORY, "metadata.csv")
 TEMPLATES_DIRECTORY = "templates"
 TEMP_DIRECTORY = ".data/temp"
 
 PPD = "PPD"
 PUE = "PUE"
 
 
@@ -28,14 +27,15 @@
     formatter = logging.Formatter('%(asctime)s - %(message)s')
     fh.setFormatter(formatter)
     logging.root.addHandler(fh)
 
 
 class FacturacionLauncher:
     def __init__(self, cwd=None):
+        # sg.theme('Reddit')
         self.app_dir = os.getcwd()
         if cwd:
             os.chdir(cwd)
         add_file_handler()
 
         # layout
         layout = [
@@ -71,15 +71,15 @@
         )
 
     @staticmethod
     def read_config():
         from satdigitalinvoice.file_data_managers import ConfigManager
         return ConfigManager()
 
-    def load_sample_files(self):
+    def add_sample_files(self):
         # loading the sample.zip
         try:
             with ZipFile(os.path.join(self.app_dir, 'sample.zip'), 'r') as zf:
                 for member in zf.infolist():
                     if not os.path.exists(member.filename):
                         zf.extract(member)
         except FileNotFoundError:
@@ -90,25 +90,24 @@
         self.window.read(timeout=0)
 
         try:
             # check if another directory is configured
             from satdigitalinvoice.file_data_managers import InitManager
             if cwd := InitManager().get('cwd'):
                 os.chdir(cwd)
-            self.load_sample_files()
+            self.add_sample_files()
 
             from satdigitalinvoice.facturacion import FacturacionGUI
             app = FacturacionGUI(
                 config=self.read_config()
             )
         except Exception as ex:
             logging.exception(ex)
             self.window['console'].update(
                 f"Error al cargar la aplicación. {ex.__class__.__name__}: {ex}",
                 text_color='red4',
             )
-            self.window.read()
-            self.window.close()
+            self.window.read(close=True)
             return
 
         self.window.close()
         app.run()
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/client_validation.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,56 +12,50 @@
 warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
 
 EMAIL_REGEX = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
 
 
 def validar_client(client):
     rfc = client['Rfc']
+
+    def error(msg):
+        print(f"{rfc}: {msg}")
+
     try:
         rfc = RFC(rfc)
-        if not rfc.is_valid():
-            raise ValueError("RFC Not Valid Regex")
-    except ValueError as ex:
-        print(f"{rfc}: {ex}")
-        return
 
-    for email in client["Email"]:
-        match = re.fullmatch(EMAIL_REGEX, email)
-        if not match:
-            print(f"{rfc}: Correo '{email}' is invalid")
-
-    if id_cif := client["IdCIF"]:
-        try:
-            res = csf.retrieve(rfc, id_cif=id_cif)
-        except ValueError as ex:
-            print(f"{rfc}: idCIF '{id_cif}' is invalid")
-            return
-
-        if rfc.type == RFCType.MORAL:
-            if client['RazonSocial'] != res['Denominación o Razón Social']:
-                print(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Denominación o Razón Social']}'")
-        elif rfc.type == RFCType.FISICA:
-            if client['RazonSocial'] != f"{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}":
-                print(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}'")
+        for email in client["Email"]:
+            if not re.fullmatch(EMAIL_REGEX, email):
+                error(f"Correo '{email}' is invalid")
+
+        res = csf.retrieve(rfc, id_cif=client["IdCIF"])
+
+        if rfc.type == RFCType.FISICA:
+            razon_social = f"{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}"
+        else:
+            razon_social = res['Denominación o Razón Social']
+        if client['RazonSocial'] != razon_social:
+            error(f"RazonSocial '{client['RazonSocial']}' is invalid, expected '{razon_social}'")
 
         if client['CodigoPostal'] != res['CP']:
-            print(f"{rfc}: CodigoPostal '{client['CodigoPostal']}' is invalid, expected '{res['CP']}'")
+            error(f"CodigoPostal '{client['CodigoPostal']}' is invalid, expected '{res['CP']}'")
 
         if client['RegimenFiscal'] not in (r['RegimenFiscal'] for r in res['Regimenes']):
-            print(
-                f"{rfc}: RegimenFiscal '{client['RegimenFiscal']}' is invalid, "
+            error(
+                f"RegimenFiscal '{client['RegimenFiscal']}' is invalid, "
                 f"expected '{(r['RegimenFiscal'].code for r in res['Regimenes'])}'"
             )
 
-        if res['Situación del contribuyente'] not in ['ACTIVO', 'REACTIVADO']:
-            print(f"{rfc}: Is not ACTIVO '{res['Situación del contribuyente']}'")
+        if res['Situación del contribuyente'] not in ('ACTIVO', 'REACTIVADO'):
+            error(f"Is not ACTIVO '{res['Situación del contribuyente']}'")
 
         taxpayer_status = sat_service.list_69b(rfc)
         if taxpayer_status:
-            print(f"{rfc}: has status '{taxpayer_status}'")
+            error(f"has status '{taxpayer_status}'")
+    except ValueError as ex:
+        error(ex)
 
 
-def clientes_generar_txt(clients):
-    with open("clientes.txt", 'w') as f:
+def clientes_generar_txt(filename, clients):
+    with open(filename, 'w', encoding='utf-8') as f:
         for i, (cliente_rfc, cliente_data) in enumerate(clients.items(), start=1):
-            f.write(f"{i}|{cliente_rfc}|{cliente_data['RazonSocial']}|{cliente_data['CodigoPostal']}")
-            f.write("\n")
+            f.write(f"{i}|{cliente_rfc}|{cliente_data['RazonSocial']}|{cliente_data['CodigoPostal']}\n")
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/environments.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from datetime import date
 from html import escape as html_escape
 
 import jinja2
 from jinja2 import Environment, Undefined
 from jinja2.filters import do_mark_safe
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import iterate as h_iterate
-from satdigitalinvoice.formatting_functions.common import pesos, num_letras
+from satdigitalinvoice.formatting_functions.common import pesos, num_letras, fecha as c_fecha
 
 from . import TEMPLATES_DIRECTORY
 
 
 class FacturacionEnvironment(Environment):
     @property
     def filter(self):
@@ -39,14 +40,18 @@
 
         @self.glob
         def iterate(v):
             if isinstance(v, Undefined):
                 return v
             return h_iterate(v)
 
+        @self.glob
+        def today():
+            return date.today()
+
         @self.filter
         def bold(k):
             return do_mark_safe(
                 tag(html_escape(str(k)), "b")
             )
 
         @self.filter
@@ -57,13 +62,17 @@
         def numero(k):
             return str(k) + ' (' + num_letras(k) + ')'
 
         @self.filter
         def porcentaje(k):
             return str(k) + '% (' + num_letras(k) + ' POR CIENTO)'
 
+        @self.filter
+        def fecha(k):
+            return c_fecha(k)
+
 
 def tag(text, tag):
     return '<' + tag + '>' + text + '</' + tag + '>'
 
 
 facturacion_environment = FacturacionEnvironment()
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/facturacion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 import base64
+import csv
 import io
 import itertools
 import logging
 import os
-from datetime import timedelta, date
+from datetime import date, datetime
+from uuid import UUID
 from zipfile import ZipFile
 
-from PySimpleGUI import POPUP_BUTTONS_OK_CANCEL, PySimpleGUI
+from PySimpleGUI import POPUP_BUTTONS_OK_CANCEL, PySimpleGUI as sg, POPUP_BUTTONS_NO_BUTTONS
 from satcfdi import DatePeriod, csf
 from satcfdi.accounting import EmailManager
+from satcfdi.accounting.models import EstadoComprobante
+from satcfdi.accounting.process import complement_invoices
 from satcfdi.create.cfd import cfdi40
 from satcfdi.exceptions import ResponseError
 from satcfdi.pacs import Accept
-from satcfdi.pacs.sat import SAT, TipoDescargaMasivaTerceros, EstadoSolicitud
-from satcfdi.printer import Representable
+from satcfdi.pacs.sat import SAT, EstadoSolicitud, TipoDescargaMasivaTerceros
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
+from xlsxwriter.exceptions import XlsxFileError
 
-from . import __version__, PPD, PUE, TEMP_DIRECTORY
-from .client_validation import validar_client
+from . import __version__, PPD, PUE, TEMP_DIRECTORY, ARCHIVOS_DIRECTORY, DATA_DIRECTORY, METADATA_FILE
+from .client_validation import validar_client, clientes_generar_txt
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
-from .formatting_functions.common import fecha
-from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_filename, mf_pago_fmt, archivos_folder, period_desc, ajustes_directory, find_ajustes, \
-    format_concepto_desc, generate_pdf_template, periodicidad_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis
-from .layout import make_layout, ActionButtonManager
-from .localdb import LocalDBSatCFDI, LiquidatedState
+from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_folder, period_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis, center_location, \
+    CALENDAR_FECHA_FMT, ConsoleErrors, \
+    generate_ajustes
+from .layout import make_layout, ActionButtonManager, TipoRecuperar, SearchOptions
+from .localdb import LocalDBSatCFDI, StatusState
 from .log_tools import cfdi_header, header_line, print_yaml
-from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder
-from .utils import random_string, parse_date_period, load_certificate, to_int, cert_info, add_month, clear_directory, find_best_match, months_between
+from .mycfdi import MyCFDI
+from .utils import random_string, to_date_period, load_certificate, to_int, cert_info, add_month, to_uuid
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
 
 
 def open_launch_window():
-    layout = [[PySimpleGUI.Text("New Window", key="new")]]
-    window = PySimpleGUI.Window("Launch Window", layout, modal=True, size=(300, 300))
+    layout = [[sg.Text("New Window", key="new")]]
+    window = sg.Window("Launch Window", layout, modal=True, size=(300, 300))
     window.read(timeout=1000)
 
     return window
 
 
 class FacturacionGUI:
     def __init__(self, config):
@@ -52,70 +56,66 @@
         )
         pac = config['pac']
         pac_module, pac_class = pac['type'].split(".")
         mod = __import__(f"satcfdi.pacs.{pac_module}", fromlist=[pac_class])
         self.pac_service = getattr(mod, pac_class)(
             **pac['args']
         )
-        self.serie = config['serie']
         self.csd_signer = load_certificate(config.get('csd')) if 'csd' in config else None
         self.fiel_signer = load_certificate(config.get('fiel')) if 'fiel' in config else None
 
         self.sat_service = SAT(signer=self.fiel_signer)
         self.rfc_prediales = config['rfc_prediales']
 
         self.all_invoices = None
         self.local_db = LocalDBSatCFDI(
+            base_path=DATA_DIRECTORY,
             enviar_a_partir=config['enviar_a_partir'],
             pagar_a_partir=config['pagar_a_partir']
         )
-        # noinspection PyTypeChecker
-        self.selected_satcfdi = None  # type: MyCFDI
 
-        self.window = PySimpleGUI.Window(
+        MyCFDI.local_db = self.local_db
+        MyCFDI.base_dir = ARCHIVOS_DIRECTORY
+
+        self.window = sg.Window(
             f"Facturación Mensual CFDI 4.0 {self.csd_signer.rfc}",
             make_layout(bool(self.fiel_signer), self.local_db),
-            size=(1280, 800),
+            size=(1280, 720),
             resizable=True,
             font=("Courier New", 10, "bold"),
+            ttk_theme="default",
+            margins=(0, 0),
+            use_custom_titlebar=True,
+            titlebar_font=("Courier New", 11, "bold"),
+            finalize=True,
         )
 
-        self.action_button_manager = ActionButtonManager(self.window["crear_facturas"])
+        self.action_button_manager = ActionButtonManager(
+            button=self.window["crear_facturas"],
+            preview=self.window["ver_preview"],
+        )
         self.console = self.window["console"]
 
-        MyCFDI.local_db = self.local_db
-
-    def run(self):
-        self.window.finalize()
-
+        self.set_serie()
         self.set_folio()
-        self.window['serie'].update(self.serie)
 
-        self.window['periodo'].bind("<Return>", "_enter")
-        self.window['importe_pago'].bind("<Return>", "_enter")
-        self.window['fecha_pago'].bind("<Return>", "_enter")
-        self.window['forma_pago'].bind("<Return>", "_enter")
-        self.window['emitidas_search'].bind("<Return>", "_enter")
-
-        self.window['facturas_table'].bind('<Double-Button-1>', '_double_click')
-        self.window['clientes_table'].bind('<Double-Button-1>', '_double_click')
-        self.window['emitidas_table'].bind('<Double-Button-1>', '_double_click')
-        self.window['ajustes_table'].bind('<Double-Button-1>', '_double_click')
-
-        self.window['facturas_table'].bind('<Control-KeyPress-a>', '+select_all')
-        self.window['clientes_table'].bind('<Control-KeyPress-a>', '+select_all')
-        self.window['emitidas_table'].bind('<Control-KeyPress-a>', '+select_all')
-        self.window['correos_table'].bind('<Control-KeyPress-a>', '+select_all')
-        self.window['ajustes_table'].bind('<Control-KeyPress-a>', '+select_all')
-
-        # Add logging to the window
-        h = logging.StreamHandler(self.window['console'])
-        h.setLevel(logging.ERROR)
-        logging.root.addHandler(h)
+        self.window.bind("<FocusIn>", "_focus_in")
+        self.window.bind("<FocusOut>", "_focus_out")
+
+        for t in ('facturas_periodo', 'emitidas_search', 'ajustes_periodo', 'serie', 'folio'):
+            self.window[t].bind("<Return>", "_enter")
+            self.window[t].bind("<FocusOut>", "_enter", propagate=False)
+
+        for t in ('facturas_table', 'clientes_table', 'emitidas_table', 'correos_table', 'ajustes_table', 'solicitudes_table'):
+            self.window[t].bind('<Control-KeyPress-a>', '+select_all')
+            self.window[t].bind('<BackSpace>', '+delete')  # BackSpace
+            # self.window[t].bind('<Double-Button-1>', '_enter')
+            self.window[t].bind('<Return>', '_enter')
 
+    def run(self):
         self.main_loop()
         self.window.close()
 
     def initial_screen(self, emisor_cif):
         self.header("ACERCA DE")
         print_yaml({
             "version": __version__.__version__,
@@ -127,24 +127,27 @@
                 "Environment": str(self.pac_service.environment)
             },
             "fiel": cert_info(self.fiel_signer),
             "csd": cert_info(self.csd_signer),
         })
 
     def get_all_invoices(self):
-        if self.all_invoices:
-            return self.all_invoices
-        self.all_invoices = get_all_cfdi()
+        if not self.all_invoices:
+            self.all_invoices = MyCFDI.get_all_cfdi()
         return self.all_invoices
 
+    def add_created_invoice(self, invoice: MyCFDI):
+        self.all_invoices[invoice.uuid] = invoice
+        complement_invoices(self.all_invoices, invoice)
+
     def generate_invoice(self, invoice):
         ref_id = random_string()
 
         # Add Serie and Folio and signature
-        invoice['Serie'] = self.serie
+        invoice['Serie'] = self.local_db.serie()
         folio = self.local_db.folio()
         invoice['Folio'] = str(folio)
         cfdi40.Comprobante.sign(invoice, self.csd_signer)
 
         attempts = 3
         for i in range(attempts):
             if i:
@@ -154,116 +157,181 @@
             try:
                 res = self.pac_service.stamp(
                     cfdi=invoice,
                     accept=Accept.XML_PDF,
                     ref_id=ref_id
                 )
             except Exception as ex:
-                logger.error(f"Error Generando: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}")
+                message = f"Error al generar factura: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}"
+                logger.exception(message)
+                print(message)
                 if isinstance(ex, ResponseError):
                     logger.error(f"Status Code: {ex.response.status_code}")
+                    print(f"Status Code: {ex.response.status_code}")
                     logger.error(f"Response: {ex.response.text}")
+                    print(f"Response: {ex.response.text}")
                 continue
 
             self.set_folio(folio + 1)
-            return move_to_folder(res.xml, pdf_data=res.pdf)
+            cfdi = MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
+            self.add_created_invoice(cfdi)
+            return cfdi
+
+    def set_serie(self, serie: str = None):
+        if serie:
+            self.local_db.serie_set(serie)
+
+        serie = serie or self.local_db.serie()
+        self.window['serie'].update(serie)
+        self.window['serie_folio'].update(f"{serie}{self.local_db.folio()}")
 
     def set_folio(self, folio: int = None):
         if folio:
             self.local_db.folio_set(folio)
-        self.window['folio'].update(folio or self.local_db.folio())
 
-    def recupera_comprobantes(self, id_solicitud):
-        response = self.sat_service.recover_comprobante_status(
-            id_solicitud=id_solicitud
+        folio = folio or self.local_db.folio()
+        self.window['folio'].update(folio)
+        self.window['serie_folio'].update(f"{self.local_db.serie()}{folio}")
+
+    def nueva_solicitud(self, values):
+        tipo_recuperar = values["tipo_recuperar"]
+
+        args = {
+            'fecha_inicial': datetime.strptime(values["fecha_inicial"], CALENDAR_FECHA_FMT),
+            'fecha_final': datetime.strptime(values["fecha_final"], CALENDAR_FECHA_FMT),
+            'rfc_receptor': self.sat_service.signer.rfc if tipo_recuperar == TipoRecuperar.Recibidas else None,
+            'rfc_emisor': self.sat_service.signer.rfc if tipo_recuperar == TipoRecuperar.Emitidas else None,
+            'tipo_solicitud': values["tipo_solicitud"],
+        }
+
+        response = self.sat_service.recover_comprobante_request(
+            **args
         )
-        print_yaml(response)
-        self._read()
+
+        self.local_db.solicitud_merge(response["IdSolicitud"], request=args, response=response)
+
+    def recupera_comprobantes(self, response):
         if response["EstadoSolicitud"] == EstadoSolicitud.Terminada:
             for id_paquete in response['IdsPaquetes']:
-                response, paquete = self.sat_service.recover_comprobante_download(
+                r, paquete = self.sat_service.recover_comprobante_download(
                     id_paquete=id_paquete
                 )
-                print_yaml(response)
-                self._read()
-                yield id_paquete, base64.b64decode(paquete) if paquete else None
+                print(f"paquete: {id_paquete}")
+                print_yaml(r)
+                if paquete:
+                    data = base64.b64decode(paquete)
+                    with io.BytesIO(data) as b:
+                        self.unzip_cfdi(b)
 
     def unzip_cfdi(self, file):
         with ZipFile(file, "r") as zf:
             for fileinfo in zf.infolist():
-                xml_data = zf.read(fileinfo)
-                move_to_folder(xml_data, pdf_data=None)
+                data = zf.read(fileinfo)
+                match os.path.splitext(fileinfo.filename)[1]:
+                    case ".xml":
+                        self.all_invoices = None
+                        MyCFDI.move_to_folder(data, pdf_data=None)
+                    case ".pdf":
+                        pass
+                    case ".txt":
+                        cfdi_metadata_reader = csv.reader(
+                            (c.decode('utf-8') for c in data.splitlines() if c),
+                            delimiter='~',
+                            quotechar='|'
+                        )
+                        header = next(cfdi_metadata_reader)
+                        for row in cfdi_metadata_reader:
+                            row = dict(zip(header, row))
+                            print_yaml(row)
+                            self.local_db.status_merge(
+                                uuid=row['Uuid'],
+                                estatus=row['Estatus'],
+                                fecha_cancelacion=row['FechaCancelacion']
+                            )
                 self._read()
 
     def _read(self, timeout=0):
         event, values = self.window.read(timeout=timeout)
-        if event in ("Exit", PySimpleGUI.WIN_CLOSED):
+        if event in ("Exit", sg.WIN_CLOSED):
             exit(0)
 
     def action_button(self, action_name, action_items):
         match action_name:
-            case 'facturas':
-                self.all_invoices = None
+            case 'solicitudes':
+                for solicitud in action_items:
+                    id_solicitud = solicitud["response"]["IdSolicitud"]
+                    response = self.sat_service.recover_comprobante_status(
+                        id_solicitud=id_solicitud
+                    )
+                    print_yaml(response)
+                    self.local_db.solicitud_merge(id_solicitud, response=response)
+                    self.recupera_comprobantes(response)
+                    self._read()
+
+            case 'facturas' | 'pago':
                 for invoice in action_items:
                     cfdi = self.generate_invoice(invoice=invoice)
                     if cfdi is None:
                         break
                     print_yaml({
                         "FacturaGenerada": cfdi_header(cfdi),
                     })
                     self._read()
 
             case 'correos':
                 clients = ClientsManager()
-                emisor_cif = clients[self.csd_signer.rfc]
+                emisor = clients[self.csd_signer.rfc]
                 with self.email_manager.sender as s:
-                    for receptor, notify_invoices, pendientes_meses_anteriores in action_items:
+                    for receptor, facturas, facturas_facturas_pendientes_meses_anteriores in action_items:
+
                         def attachments():
-                            for ni in notify_invoices:
+                            for ni in facturas:
                                 yield ni.filename + ".xml"
                                 yield ni.filename + ".pdf"
 
                         subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
 
                         s.send_email(
                             subject=subject,
                             to_addrs=receptor["Email"],
                             html=facturacion_environment.get_template('mail_facturas_template.html').render(
-                                facturas=notify_invoices,
-                                pendientes_meses_anteriores=pendientes_meses_anteriores,
-                                emisor=emisor_cif,
+                                facturas=facturas,
+                                facturas_pendientes_meses_anteriores=facturas_facturas_pendientes_meses_anteriores,
+                                emisor=emisor,
+                                receptor=receptor,
                             ),
                             file_attachments=attachments()
                         )
-                        for r in notify_invoices:
+                        for r in facturas:
                             self.local_db.notified_set(r.uuid, True)
                         print_yaml({
                             "correo": subject,
                             "para": receptor["Email"]
                         })
                         self._read()
 
             case 'ajustes':
                 clients = ClientsManager()
-                emisor_cif = clients[self.csd_signer.rfc]
+                emisor = clients[self.csd_signer.rfc]
                 with self.email_manager.sender as s:
                     for data in action_items:
                         receptor = data['receptor']
                         file_name = data['file_name']
                         subject = f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
 
                         if not data['ajuste_porcentaje']:
                             print(f"NO HAY {subject}")
                             continue
 
                         s.send_email(
                             subject=subject,
                             to_addrs=receptor["Email"],
                             html=facturacion_environment.get_template('mail_ajustes_template.html').render(
-                                emisor=emisor_cif,
+                                emisor=emisor,
+                                receptor=receptor,
                             ),
                             file_attachments=[file_name]
                         )
                         print_yaml({
                             "correo": subject,
                             "para": receptor["Email"]
                         })
@@ -279,490 +347,545 @@
                 raise ValueError(f"Invalid action: {action_name}")
 
         print("FIN")
 
     def set_selected_satcfdis(self, cfdis: list):
         i = cfdis[0] if len(cfdis) == 1 else None
 
-        self.selected_satcfdi = i
         if i:
-            estado = self.local_db.status_sat(i).get('Estado', 'Vigente')
+            estatus = EstadoComprobante(i.estatus)
             self.window["status_sat"].update(
-                estado.center(10),
+                estatus.name.center(10),
                 disabled=False,
-                button_color="red4" if estado != "Vigente" else "green",
+                button_color="red4" if estatus != EstadoComprobante.Vigente else "dark green",
             )
         else:
             self.window["status_sat"].update(
-                "".ljust(10), disabled=True, button_color=PySimpleGUI.theme_background_color()
+                "".ljust(10), disabled=True, button_color=sg.theme_background_color()
             )
 
         # Email
-        is_enviable = i \
-                      and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                      and i.estatus == "1"
-        if is_enviable:
+        is_active = \
+            bool(i) \
+            and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+            and i.estatus == EstadoComprobante.Vigente
+        if is_active:
             self.window["email_notificada"].update(
                 "Enviada".center(10) if self.local_db.notified(i) else "Por Enviar",
                 disabled=False,
-                button_color="green" if self.local_db.notified(i) else "red4",
+                button_color="dark green" if self.local_db.notified(i) else "red4",
             )
         else:
             self.window["email_notificada"].update(
-                "".ljust(10), disabled=True, button_color=PySimpleGUI.theme_background_color()
+                "".ljust(10), disabled=True, button_color=sg.theme_background_color()
             )
 
         # Pendiente de Pago
-        is_pendientable = i \
-                          and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                          and i["TipoDeComprobante"] == "I" \
-                          and i.estatus == "1" \
-                          and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
-                          and i["Total"]
+        is_pendientable = \
+            is_active \
+            and i["TipoDeComprobante"] == "I" \
+            and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
+            and i["Total"]
         if is_pendientable:
             self.window["pendiente_pago"].update(
-                ("Pagada".center(10) if i["MetodoPago"] == PUE else "Ignorada".center(10)) if self.local_db.liquidated(i) else "Por Pagar".center(10),
+                (("Pagada" if i["MetodoPago"] == PUE else "Ignorada")
+                 if self.local_db.liquidated(i) else "Por Pagar").center(10),
                 disabled=False,
-                button_color="green" if self.local_db.liquidated(i) else "red4",
+                button_color=("dark green" if i["MetodoPago"] == PUE else "yellow4")
+                if self.local_db.liquidated(i) else "red4",
             )
         else:
-            self.window["pendiente_pago"].update(
-                "".ljust(10), disabled=True, button_color=PySimpleGUI.theme_background_color()
-            )
+            is_ppd_pagada = is_active \
+                            and i["TipoDeComprobante"] == "I" \
+                            and i["MetodoPago"] == PPD \
+                            and i.saldo_pendiente == 0
+            if is_ppd_pagada:
+                self.window["pendiente_pago"].update(
+                    "Pagada".center(10),
+                    disabled=True,
+                    button_color="dark green",
+                )
+            else:
+                self.window["pendiente_pago"].update(
+                    "".ljust(10),
+                    disabled=True,
+                    button_color=sg.theme_background_color()
+                )
 
         # PPD
-        is_ppd_active = i \
-                        and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                        and i.get("MetodoPago") == PPD \
-                        and i.estatus == "1" \
-                        and i.saldo_pendiente
-        is_ppd_active = bool(is_ppd_active)
+        is_ppd_active = \
+            is_active \
+            and i["TipoDeComprobante"] == "I" \
+            and i["MetodoPago"] == PPD \
+            and i.saldo_pendiente > 0
+
         self.window["ppd_action_items"].update(visible=is_ppd_active)
-        self.window["importe_pago"].update("")
+        self.window["importe_pago"].update(i.saldo_pendiente if is_ppd_active else '')
+        if is_ppd_active:
+            self.action_button_manager.set_items("pago", [None])
+        else:
+            self.action_button_manager.clear()
 
     def header(self, name):
-        self.console.update("")
-        print(header_line(name))
+        self.window['console_tab'].select()
+        self.console.update(header_line(name))
+        self._read()
 
-    def facturas_search(self, search_text):
-        search_text = search_text.strip().upper()
-        if len(search_text) < 3:
-            self.window["emitidas_text"].update("El texto de búsqueda debe tener al menos 3 caracteres")
-            return
+    def download_invoice(self, uuid: UUID):
+        res = self.pac_service.recover(uuid, accept=Accept.XML_PDF)
+        self.all_invoices = None
+        return MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
 
-        self.window["emitidas_text"].update(search_text)
+    def facturas_search(self):
+        search_text = self.window["emitidas_search"].get()
+        search_text = search_text.strip()
+
+        if len(search_text) < 3:
+            raise ValueError("Búsqueda debe de tener al menos 3 caracteres")
 
         def fact_iter():
-            for i in self.get_all_invoices().values():
-                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                        and (
-                        i.name == search_text
-                        or i["Receptor"]["Rfc"] == search_text
-                        or search_text in i["Receptor"].get("Nombre", "")
-                ):
-                    yield i
+            if search_text == SearchOptions.PorPagar:
+                for i in self.get_all_invoices().values():
+                    if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                            and self.local_db.liquidated_state(i) == StatusState.PENDING:
+                        yield i
+            elif search_text == SearchOptions.PorEnviar:
+                for i in self.get_all_invoices().values():
+                    if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                            and not self.local_db.notified(i) \
+                            and i.estatus == EstadoComprobante.Vigente:
+                        yield i
+            elif date_search_text := to_date_period(search_text):
+                for i in self.get_all_invoices().values():
+                    if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                            and i["Fecha"] == date_search_text:
+                        yield i
+            elif uuid_search_text := to_uuid(search_text):
+                if uuid_search_text not in self.get_all_invoices():
+                    try:
+                        self.download_invoice(uuid_search_text)
+                    except ResponseError as e:
+                        if e.response.status_code == 404:
+                            self.error_message(f"Factura no encontrada en el PAC")
+                        else:
+                            raise e
+                if c := self.get_all_invoices().get(uuid_search_text):
+                    yield c
+            else:
+                up_search_text = search_text.upper()
+                for i in self.get_all_invoices().values():
+                    if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                            and (
+                            i.name == up_search_text
+                            or i["Receptor"]["Rfc"] == up_search_text
+                            or up_search_text in i["Receptor"].get("Nombre", "")
+                    ):
+                        yield i
 
         self.window['emitidas_table'].update(
             values=list(fact_iter()),
         )
 
-    def facturas_pendientes(self):
-        self.window["emitidas_text"].update("Facturas Pendientes de Pago")
-
-        def fact_iter():
-            for i in self.get_all_invoices().values():
-                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                        and self.local_db.liquidated_state(i) == LiquidatedState.NO:
-                    yield i
-
-        self.window['emitidas_table'].update(
-            values=list(fact_iter()),
+    def crear_pago(self, values):
+        fecha_pago = parse_fecha_pago(values["fecha_pago"])
+        importe_pago = parse_importe_pago(values["importe_pago"])
+        self.window["importe_pago"].update(importe_pago)
+
+        # noinspection PyUnresolvedReferences
+        cfdi = pago_factura(
+            factura_pagar=self.window["emitidas_table"].selected_items()[0],
+            fecha_pago=fecha_pago,
+            forma_pago=values["forma_pago"],
+            importe_pago=importe_pago,
         )
+        return [cfdi]
 
-    def facturas_emitidas(self, dp):
-        self.window["emitidas_text"].update("Facturas Emitidas en " + str(dp))
+    def error_message(self, ex):
+        sg.Popup(
+            ex,
+            no_titlebar=True,
+            background_color="red4",
+            location=center_location(self.window),
+            button_type=POPUP_BUTTONS_NO_BUTTONS,
+            auto_close=True,
+            non_blocking=True,
+        )
 
-        def fact_iter():
-            for i in self.get_all_invoices().values():
-                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                        and i["Fecha"] == dp:
-                    yield i
+    def nuevas_facturas(self, values, force=False):
+        facturas_table = self.window['facturas_table']
+        has_value = bool(facturas_table.metadata)
+        facturas_table.update(values=[])
+        self.window['preparar_facturas_text'].update("")
+
+        if has_value or force:
+            dp = to_date_period(values["facturas_periodo"])
+            if dp is None or dp.month is None:
+                raise ValueError("Periodo no válido")
+
+            self.window['preparar_facturas_text'].update(f"{period_desc(dp)}")
+
+            cfdis = generate_ingresos(
+                clients=ClientsManager(),
+                facturas=FacturasManager(dp)["Facturas"],
+                dp=dp,
+                emisor_rfc=self.csd_signer.rfc
+            )
+            facturas_table.update(
+                values=cfdis,
+            )
 
-        self.window['emitidas_table'].update(
-            values=list(fact_iter()),
-        )
+    def nuevos_ajustes(self, values, force=False):
+        ajustes_table = self.window['ajustes_table']
+        has_value = bool(ajustes_table.metadata)
+        ajustes_table.update(values=[])
+        self.window['preparar_ajustes_text'].update("")
+
+        if has_value or force:
+            dp = to_date_period(values["ajustes_periodo"])
+            if dp is None or dp.month is None:
+                raise ValueError("Periodo no válido")
+
+            dp_effective = add_month(dp, 1)
+            self.window['preparar_ajustes_text'].update(f"{period_desc(dp)}, Ajustes Efectivos Al: {period_desc(dp_effective)}")
+
+            ajustes = generate_ajustes(
+                clients=ClientsManager(),
+                facturas=FacturasManager(None)["Facturas"],
+                dp=dp,
+                dp_effective=dp_effective,
+                emisor_rfc=self.csd_signer.rfc
+            )
+            ajustes_table.update(
+                values=ajustes,
+            )
 
-    def main_loop(self):
-        while True:
-            event, values = self.window.read()
-            try:
-                if event in ("Exit", PySimpleGUI.WIN_CLOSED):
-                    return
+    def main_tab_group(self, values):
+        self.action_button_manager.clear()
 
-                try:
-                    dp = parse_date_period(values["periodo"])
-                except ValueError:
-                    dp = None
+        match values['main_tab_group']:
+            case 'facturas_tab':
+                self.nuevas_facturas(values)
+
+            case 'clientes_tab':
+                self.window['clientes_table'].update(
+                    values=list(ClientsManager().values()),
+                )
 
-                if event in ("periodo_enter", "refresh_facturas", "refresh_ajustes", "refresh_clientes", "refresh_correos"):
-                    event = 'main_tab_group'
+            case 'emitidas_tab':
+                self.facturas_search()
 
-                match event:
-                    case "folio":
-                        self.set_folio(to_int(values["folio"]))
+            case 'correos_tab':
+                now = date.today()
+                dp_now = DatePeriod(now.year, now.month)
+                clients = ClientsManager()
 
-                    case "about":
-                        clients = ClientsManager()
-                        self.initial_screen(clients[self.csd_signer.rfc])
+                def correos():
+                    for receptor_rfc, notify_invoices in itertools.groupby(
+                            sorted(
+                                (i for i in self.get_all_invoices().values()
+                                 if i["Emisor"]["Rfc"] == self.csd_signer.rfc
+                                    and i.estatus == EstadoComprobante.Vigente
+                                    and not self.local_db.notified(i)
+                                 ),
+                                key=lambda r: r["Receptor"]["Rfc"]
+                            ),
+                            lambda r: r["Receptor"]["Rfc"]
+                    ):
+                        notify_invoices = list(notify_invoices)
 
-                    case "recuperar_emitidas" | "recuperar_recibidas":
-                        fecha_final = date.today()
-                        fecha_inicial = fecha_final - timedelta(days=int(values["recuperar_dias"]))
-                        id_solicitud = self.local_db.get(event)
-
-                        if not id_solicitud:
-                            self._read()
-                            response = self.sat_service.recover_comprobante_request(
-                                fecha_inicial=fecha_inicial,
-                                fecha_final=fecha_final,
-                                rfc_receptor=self.sat_service.signer.rfc if "recuperar_recibidas" == event else None,
-                                rfc_emisor=self.sat_service.signer.rfc if "recuperar_emitidas" == event else None,
-                                tipo_solicitud=TipoDescargaMasivaTerceros.CFDI,
-                            )
-                            print_yaml(response)
-                            self.local_db[event] = response['IdSolicitud']
-                            print("Nueva Solicitud Creada")
-                        else:
-                            print_yaml({
-                                'IdSolicitud': id_solicitud
-                            })
-                            self._read()
-                            for paquete_id, data in self.recupera_comprobantes(id_solicitud):
-                                if data:
-                                    self.all_invoices = None
-                                    with io.BytesIO(data) as b:
-                                        self.unzip_cfdi(b)
-                                del self.local_db[event]
-                            print("FIN")
+                        def fac_pen_iter():
+                            for i in self.get_all_invoices().values():
+                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                                        and self.local_db.liquidated_state(i) == StatusState.PENDING \
+                                        and i["Fecha"] < dp_now \
+                                        and i["Receptor"]["Rfc"] == receptor_rfc \
+                                        and i not in notify_invoices:
+                                    yield i
 
-                    case "emitidas_search_enter":
-                        self.action_button_manager.clear()
-                        self.facturas_search(values["emitidas_search"])
+                        fac_pen = sorted(
+                            fac_pen_iter(),
+                            key=lambda r: r["Fecha"]
+                        )
+                        yield clients[receptor_rfc], notify_invoices, fac_pen
 
-                    case 'main_tab_group':
-                        if values['main_tab_group'] == 'console_tab':
-                            self.action_button_manager.clear()
+                self.window['correos_table'].update(
+                    values=list(correos()),
+                )
 
-                        if values['main_tab_group'] == 'recuperar_tab':
-                            self.action_button_manager.clear()
+            case 'ajustes_tab':
+                self.nuevos_ajustes(values)
 
-                        if values['main_tab_group'] == 'facturas_tab':
-                            self.window['facturas_table'].update(values=[])
+            case 'solicitudes_tab':
+                solitudes = self.local_db.get_solicitudes()
+                self.window['solicitudes_table'].update(
+                    values=list(solitudes.values()),
+                )
 
-                            if dp is None or dp.month is None:
-                                self.window['preparar_facturas_text'].update("Periodo no válido")
-                                continue
+    def main_loop(self):
+        has_focus = True
+        _, values = self.window.read(timeout=0)
+        event = "main_tab_group"
 
-                            self.window['preparar_facturas_text'].update(f"{period_desc(dp)}")
-                            self.console.update("")
-                            cfdis = generate_ingresos(
-                                clients=ClientsManager(),
-                                facturas=FacturasManager(dp)["Facturas"],
-                                dp=dp,
-                                emisor_rfc=self.csd_signer.rfc
-                            )
-                            if cfdis:
-                                self.window['facturas_table'].update(
-                                    values=cfdis,
-                                )
-                            else:
-                                self.window['console_tab'].select()
-                                continue
+        while True:
+            try:
+                if event in ("Exit", sg.WIN_CLOSED):
+                    return
 
-                        if values['main_tab_group'] == 'clients_tab':
-                            self.window['clientes_table'].update(
-                                values=list(ClientsManager().values()),
-                            )
+                match event:
+                    case '_focus_in':
+                        if not has_focus:
+                            has_focus = True
+                            if values["main_tab_group"] in ("clientes_tab", "facturas_tab", "ajustes_tab", "correos_tab"):
+                                self.main_tab_group(values)
+
+                    case '_focus_out':
+                        try:
+                            has_focus = bool(self.window.TKroot.focus_get())
+                        except KeyError:
+                            has_focus = True
 
-                        if values['main_tab_group'] == 'emitidas_tab':
-                            self.action_button_manager.clear()
-                            self.facturas_pendientes()
-
-                        if values['main_tab_group'] == 'correos_tab':
-                            now = date.today()
-                            dp_now = DatePeriod(now.year, now.month)
-                            clients = ClientsManager()
-                            a_invoices = self.get_all_invoices()
-
-                            cfdi_correos = []
-                            for receptor_rfc, notify_invoices in itertools.groupby(
-                                    sorted(
-                                        (i for i in a_invoices.values() if i.estatus == "1" and not self.local_db.notified(i)),
-                                        key=lambda r: r["Receptor"]["Rfc"]
-                                    ),
-                                    lambda r: r["Receptor"]["Rfc"]
-                            ):
-                                notify_invoices = list(notify_invoices)
-
-                                def fac_pen_iter():
-                                    for i in self.get_all_invoices().values():
-                                        if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                                and self.local_db.liquidated_state(i) == LiquidatedState.NO \
-                                                and i["Fecha"] < dp_now \
-                                                and i["Receptor"]["Rfc"] == receptor_rfc \
-                                                and i not in notify_invoices:
-                                            yield i
-
-                                fac_pen = sorted(
-                                    fac_pen_iter(),
-                                    key=lambda r: r["Fecha"]
-                                )
-                                receptor = clients[receptor_rfc]
-                                cfdi_correos.append((receptor, notify_invoices, fac_pen))
+                    case "folio_enter":
+                        self.set_folio(to_int(values["folio"]))
 
-                            self.window['correos_table'].update(
-                                values=cfdi_correos,
-                            )
+                    case "serie_enter":
+                        self.set_serie(values["serie"])
 
-                        if values['main_tab_group'] == 'ajustes_tab':
-                            self.window['ajustes_table'].update(values=[])
-                            if dp is None or dp.month is None:
-                                self.window['preparar_ajustes_text'].update("Periodo no válido")
-                                continue
+                    case "about":
+                        clients = ClientsManager()
+                        self.initial_screen(clients[self.csd_signer.rfc])
 
-                            dp_effective = add_month(dp, 1)
-                            self.window['preparar_ajustes_text'].update(f"Ajustes Efectivos Al: {period_desc(dp_effective)}")
+                    case "nueva_solicitud":
+                        self.nueva_solicitud(values)
+                        self.main_tab_group(values)
+
+                    case "buscar_facturas":
+                        self.window["emitidas_search"].update(values["buscar_facturas"])
+                        self.facturas_search()
 
-                            # clear directory
-                            ajustes_dir = ajustes_directory(DatePeriod(dp.year, dp.month))
-                            clear_directory(ajustes_dir)
-                            emisor_rfc = self.csd_signer.rfc
-
-                            clients = ClientsManager()
-                            facturas = FacturasManager(None)["Facturas"]
-
-                            def ajustes_iter():
-                                for i, (receptor_rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month)):
-                                    valor_unitario_raw = concepto["ValorUnitario"]
-
-                                    if isinstance(valor_unitario_raw, dict):
-                                        vu_eff, vu = find_best_match(valor_unitario_raw, dp)
-                                        vun_eff, vun = find_best_match(valor_unitario_raw, dp_effective)
-                                        if vu_eff == vun_eff:
-                                            vun = None
-                                            num_meses = None
-                                        else:
-                                            num_meses = months_between(vun_eff, vu_eff)
-
-                                        if vun and vu:
-                                            ajuste_porcentaje = round((vun / vu - 1) * 100, 2)
-                                        else:
-                                            ajuste_porcentaje = None
-                                    else:
-                                        vu = valor_unitario_raw
-                                        vun = None
-                                        num_meses = None
-                                        ajuste_porcentaje = None
-
-                                    concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
-                                    file_name = os.path.join(ajustes_dir, f'AjusteRenta_{receptor_rfc}_{i}.pdf')
-
-                                    client_receptor = clients[receptor_rfc]  # type: dict
-                                    data = {
-                                        "receptor": client_receptor,
-                                        "emisor": clients[emisor_rfc],
-                                        "concepto": concepto,
-                                        "valor_unitario": vu,
-                                        "valor_unitario_nuevo": vun or '',
-                                        "ajuste_porcentaje": ajuste_porcentaje or "",
-                                        "meses": num_meses or '',
-                                        "efectivo_periodo_desc": periodicidad_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),
-                                        "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
-                                        "fecha_hoy": fecha(date.today()),
-                                        'file_name': file_name
-                                    }
-
-                                    if ajuste_porcentaje:
-                                        res = generate_pdf_template(
-                                            template_name='incremento_template.md',
-                                            fields=data
-                                        )
-                                        with open(file_name, 'wb') as f:
-                                            f.write(res)
-                                    yield data
+                    case "emitidas_search_enter":
+                        self.facturas_search()
 
-                            self.window['ajustes_table'].update(
-                                values=list(ajustes_iter()),
-                            )
+                    case "facturas_periodo_enter":
+                        self.nuevas_facturas(values, force=True)
 
-                    case "facturas_pendientes":
-                        self.facturas_pendientes()
+                    case "ajustes_periodo_enter":
+                        self.nuevos_ajustes(values, force=True)
 
-                    case "facturas_emitidas":
-                        self.facturas_emitidas(dp)
+                    case 'main_tab_group':
+                        self.main_tab_group(values)
 
-                    case 'facturas_table_double_click':
+                    case 'facturas_table_enter':
                         # noinspection PyUnresolvedReferences
-                        s_items = self.window["facturas_table"].selected_items()
-                        preview_cfdis(s_items)
+                        if s_items := self.window["facturas_table"].selected_items():
+                            preview_cfdis(s_items)
 
-                    case 'clientes_table_double_click':
+                    case 'clientes_table_enter':
                         # noinspection PyUnresolvedReferences
                         for client in self.window["clientes_table"].selected_items():
                             url = csf.url(rfc=client["Rfc"], id_cif=client["IdCIF"])
                             os.startfile(url)
 
-                    case 'emitidas_table_double_click':
+                    case 'emitidas_table_enter':
                         # noinspection PyUnresolvedReferences
-                        s_items = self.window["emitidas_table"].selected_items()
-                        preview_cfdis(s_items)
+                        if s_items := self.window["emitidas_table"].selected_items():
+                            preview_cfdis(s_items)
 
-                    case 'ajustes_table_double_click':
+                    case 'ajustes_table_enter':
                         # noinspection PyUnresolvedReferences
                         for ajuste in self.window["ajustes_table"].selected_items():
                             os.startfile(
                                 os.path.abspath(ajuste['file_name'])
                             )
 
-                    case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "emitidas_table":
+                    case 'correos_table_enter' | 'solicitudes_table_enter':
+                        pass
+
+                    case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "emitidas_table" | "solicitudes_table":
                         # noinspection PyUnresolvedReferences
                         s_items = self.window[event].selected_items()
                         if event == "emitidas_table":
                             self.set_selected_satcfdis(s_items)
                         else:
                             self.action_button_manager.set_items(event.split("_")[0], s_items)
 
-                    case "facturas_table+select_all" | "clientes_table+select_all" | "correos_table+select_all" | "ajustes_table+select_all" | "emitidas_table+select_all":
+                    case "facturas_table+select_all" | "clientes_table+select_all" | "correos_table+select_all" | \
+                         "ajustes_table+select_all" | "emitidas_table+select_all" | 'solicitudes_table+select_all':
                         # noinspection PyUnresolvedReferences
                         self.window[event.split("+")[0]].select_all()
 
-                    case "prepare_pago" | "importe_pago_enter" | "fecha_pago_enter" | "forma_pago_enter" | "ver_html_pago":
-                        if i := self.selected_satcfdi:
-                            fecha_pago = parse_fecha_pago(values["fecha_pago"])
-                            importe_pago = parse_importe_pago(values["importe_pago"]) or i.saldo_pendiente
-                            self.window["importe_pago"].update(importe_pago)
-
-                            cfdi = pago_factura(
-                                factura_pagar=i,
-                                fecha_pago=fecha_pago,
-                                forma_pago=values["forma_pago"],
-                                importe_pago=importe_pago,
-                            )
-                            self.action_button_manager.set_items('facturas', [cfdi])
-                            if event == "ver_html_pago":
-                                preview_cfdis([cfdi])
+                    case "facturas_table+delete" | "clientes_table+delete" | "correos_table+delete" | \
+                         "ajustes_table+delete" | "emitidas_table+delete":
+                        # noinspection PyUnresolvedReferences
+                        self.window[event.split("+")[0]].delete_selected()
+
+                    case "solicitudes_table+delete":
+                        solitudes = self.local_db.get_solicitudes()
+                        # noinspection PyUnresolvedReferences
+                        sel = self.window["solicitudes_table"].selected_items()
+                        for s in sel:
+                            if s["response"].get("EstadoSolicitud").code < EstadoSolicitud.Terminada:
+                                self.error_message("No se puede eliminar una solicitud en proceso")
+                                continue
+                            del solitudes[s["response"]["IdSolicitud"]]
+                        self.local_db.set_solicitudes(solitudes)
+                        self.main_tab_group(values)
 
                     case "status_sat":
-                        if i := self.selected_satcfdi:
+                        # noinspection PyUnresolvedReferences
+                        if i := self.window["emitidas_table"].selected_items()[0]:
                             self.local_db.status_sat(i, update=True)
                             self.set_selected_satcfdis([i])
+                            # noinspection PyUnresolvedReferences
+                            self.window['emitidas_table'].refresh()
 
                     case "pendiente_pago":
-                        if i := self.selected_satcfdi:
+                        # noinspection PyUnresolvedReferences
+                        if i := self.window["emitidas_table"].selected_items()[0]:
                             self.local_db.liquidated_flip(i)
                             self.set_selected_satcfdis([i])
+                            # noinspection PyUnresolvedReferences
+                            self.window['emitidas_table'].refresh()
 
                     case "email_notificada":
-                        if i := self.selected_satcfdi:
+                        # noinspection PyUnresolvedReferences
+                        if i := self.window["emitidas_table"].selected_items()[0]:
                             self.local_db.notified_flip(i)
                             self.set_selected_satcfdis([i])
+                            # noinspection PyUnresolvedReferences
+                            self.window['emitidas_table'].refresh()
 
-                    case "crear_facturas":
+                    case "crear_facturas" | "ver_preview":
                         action_text = self.action_button_manager.text()
-                        res = PySimpleGUI.popup(
-                            f"Estas seguro que quieres '{action_text}'?",
-                            title="Confirmar",
-                            button_type=POPUP_BUTTONS_OK_CANCEL,
-                        )
-                        if res == "OK":
-                            self.header(action_text.upper())
-                            self.window['console_tab'].select()
-                            self._read()
-                            self.action_button(
-                                action_name=self.action_button_manager.name,
-                                action_items=self.action_button_manager.items
-                            )
-                            self.action_button_manager.clear()
+                        action_name = self.action_button_manager.name
+                        action_items = self.action_button_manager.items
 
-                    case "ver_excel":
-                        clients = ClientsManager()
-                        emisor_cif = clients[self.csd_signer.rfc]
-                        if archivo_excel := exportar_facturas(
-                                self.get_all_invoices(),
-                                dp,
-                                emisor_cif,
-                                self.rfc_prediales
-                        ):
-                            os.startfile(
-                                os.path.abspath(archivo_excel)
-                            )
-                        else:
-                            raise Exception("No se pudo crear el archivo, cierra el archivo si se tiene abierto")
+                        if action_name == "pago":
+                            action_items = self.crear_pago(values)
 
-                    case "ver_html":
-                        def fact_iter():
-                            for i in self.get_all_invoices().values():
-                                if i["Fecha"] == dp:
-                                    yield i
+                        if event == "ver_preview":
+                            if action_name in ("facturas", "pago"):
+                                preview_cfdis(action_items)
+
+                        elif event == "crear_facturas":
+                            res = sg.popup(
+                                f"Estas seguro que quieres '{action_text}'?",
+                                title="Confirmar",
+                                button_type=POPUP_BUTTONS_OK_CANCEL,
+                                location=center_location(self.window),
+                                keep_on_top=True,
+                            )
+                            if res == "OK":
+                                self.header(action_text.upper())
+                                self.action_button_manager.clear()
+                                self.action_button(
+                                    action_name=action_name,
+                                    action_items=action_items
+                                )
 
-                        if cfdis := list(fact_iter()):
-                            outfile = archivos_filename(dp, ext="html")
-                            Representable.html_write_all(
-                                objs=cfdis,
-                                target=outfile,
-                            )
-                            os.startfile(
-                                os.path.abspath(outfile)
+                    case "editar_clientes":
+                        os.startfile(
+                            os.path.abspath("clientes.yaml")
+                        )
+
+                    case "exportar_clientes":
+                        filename = 'clientes.txt'
+                        clients = ClientsManager()
+                        clientes_generar_txt(filename, clients)
+                        os.startfile(
+                            os.path.dirname(
+                                os.path.abspath(filename)
                             )
-                        else:
-                            raise Exception("No hay facturas para el periodo seleccionado")
+                        )
 
-                    case "ver_carpeta":
-                        directory = archivos_folder(dp)
+                    case "editar_facturas" | "editar_ajustes":
                         os.startfile(
-                            os.path.abspath(directory)
+                            os.path.abspath("facturas.yaml")
+                        )
+
+                    case "editar_configurar":
+                        os.startfile(
+                            os.path.abspath("config.yaml")
                         )
 
                     case "ver_config":
                         os.startfile(
                             os.path.abspath(".")
                         )
 
-                    case "editar_clientes":
+                    case "ver_excel":
+                        dp = to_date_period(values["periodo"])
+                        clients = ClientsManager()
+                        emisor_cif = clients[self.csd_signer.rfc]
+                        archivo_excel = exportar_facturas(
+                            self.get_all_invoices(),
+                            dp,
+                            emisor_cif,
+                            self.rfc_prediales
+                        )
                         os.startfile(
-                            os.path.abspath("clientes.yaml")
+                            os.path.abspath(archivo_excel)
                         )
 
-                    case "editar_facturas":
+                    case "ver_carpeta":
+                        dp = to_date_period(values["periodo"])
+                        directory = archivos_folder(dp)
                         os.startfile(
-                            os.path.abspath("facturas.yaml")
+                            os.path.abspath(directory)
                         )
 
-                    case "sat_status_todas":
-                        def fact_iter():
-                            for i in self.get_all_invoices().values():
-                                if i["Fecha"] == dp:
-                                    yield i
+                    case "organizar_facturas":
+                        MyCFDI.rename_invoices(search_path="**/*.xml")
 
-                        for cfdi in fact_iter():
-                            print(f"Estado SAT: {cfdi_header(cfdi)}")
-                            self._read()
-                            estado = self.local_db.status_sat(cfdi, update=True)
-                            print_yaml(estado)
-                        print("FIN")
-
-                    case "periodo" | "inicio" | "final" | "fecha_pago" | "forma_pago" | "importe_pago" | ' ':
-                        pass
+                    case "cargar_zip":
+                        zip_file = sg.popup_get_file('', multiple_files=False, no_window=True, file_types=(("ZIP Files", "*.zip"),))
+                        if zip_file:
+                            self.header("Cargar ZIP")
+                            self.unzip_cfdi(zip_file)
+
+                    case 'importar_emitidas':
+                        csv_file = sg.popup_get_file('', multiple_files=False, no_window=True, file_types=(("CSV Files", "*.csv"),))
+                        if csv_file:
+                            self.header("Importar emitidas")
+                            all_invoices = self.get_all_invoices()
+                            with open(csv_file, newline='', encoding='utf-8') as f:
+                                reader = csv.reader(f)
+                                header = next(reader)
+                                for row in reader:
+                                    row = dict(zip(header, row))
+                                    uuid = UUID(row["Folio Fiscal (UUID)"])
+                                    if uuid not in all_invoices:
+                                        cfdi = self.download_invoice(uuid)
+
+                                        if row.get("Estatus", "Entregado SAT") != "Entregado SAT":
+                                            estado = self.local_db.status_sat(cfdi, update=True)
+                                            print_yaml(estado)
+                                    self._read()
+                                print("FIN")
+
+                    case "exportar_metadata":
+                        with open(METADATA_FILE, 'w', newline='', encoding='utf-8') as f:
+                            writer = csv.writer(f)
+                            for i in self.get_all_invoices():
+                                if status := self.local_db.status_export(i):
+                                    writer.writerow(status)
+
+                    case "importar_metadata":
+                        with open(METADATA_FILE, newline='', encoding='utf-8') as f:
+                            reader = csv.reader(f)
+                            for row in reader:
+                                self.local_db.status_merge(*row)
 
                     case _:
                         logger.error(f"Unknown event '{event}'")
 
+            except (ValueError, XlsxFileError) as ex:
+                self.error_message(ex)
+            except ConsoleErrors as ex:
+                self.header(str(ex))
+                for error in ex.errors:
+                    self.console.update(f"{error}\n", append=True)
             except Exception as ex:
-                logger.exception(header_line("ERROR"))
-                if values['main_tab_group'] != 'console_tab':
-                    PySimpleGUI.Popup(
-                        ex,
-                        no_titlebar=True,
-                        grab_anywhere=True,
-                        any_key_closes=True,
-                        background_color="red4",
-                    )
+                self.header("Exception")
+                self.console.update(append=True, value=str(ex))
+                logger.exception("Main Loop Exception")
+
+            event, values = self.window.read()
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/file_data_managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import collections.abc
+import decimal
 import json
 import logging
 import os
 import re
 from decimal import Decimal
 
 import jsonschema as jsonschema
@@ -64,15 +65,14 @@
         validator = jsonschema.validators.validator_for(schema)
         validator.check_schema(schema)
         return validator(schema)
 
 
 client_validator = load_validator("cliente.yaml")
 factura_validator = load_validator("factura.yaml")
-config_validator = load_validator("config.yaml")
 
 
 class LocalData(dict):
     file_source = None
 
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
@@ -96,16 +96,14 @@
 
 
 class ConfigManager(LocalData):
     file_source = "config.yaml"
 
     def __init__(self):
         super().__init__()
-        if error := jsonschema.exceptions.best_match(config_validator.iter_errors(self)):
-            raise error
 
 
 class ClientsManager(LocalData):
     file_source = "clientes.yaml"
 
     def __init__(self):
         super().__init__()
@@ -128,23 +126,33 @@
                 cases,
                 dp
             )[1]
 
         DuplicateKeySafeLoader.add_constructor("!case", loading_function)
         super().__init__()
         if dup := first_duplicate(json.dumps(x, sort_keys=True, default=str) for x in self["Facturas"]):
-            raise ValueError("Factura Duplicada: {}".format(dup))
+            raise Exception("Factura Duplicada: {}".format(dup))
 
         if dp:
             for v in self["Facturas"]:
                 if error := jsonschema.exceptions.best_match(factura_validator.iter_errors(v)):
                     raise error
 
 
-DuplicateKeySafeLoader.add_constructor("!decimal", lambda loader, node: Decimal(loader.construct_scalar(node)))
+def decimal_constructor(loader, node):
+    value = loader.construct_scalar(node)
+    try:
+        return Decimal(value)
+    except decimal.InvalidOperation:
+        raise ConstructorError(None, None,
+                               "expected a decimal value, but found %s" % value,
+                               node.start_mark)
+
+
+DuplicateKeySafeLoader.add_constructor("!decimal", decimal_constructor)
 DuplicateKeySafeLoader.add_constructor("!read", lambda loader, node: open(loader.construct_scalar(node), 'rb').read())
 
 
 def represent_decimal(dumper, data):
     return dumper.represent_scalar('tag:yaml.org,2002:str', str(data))
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/gui_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import logging
 import os
 from datetime import datetime, date
 from decimal import Decimal
 from decimal import InvalidOperation
 
 import xlsxwriter
-from babel.dates import format_date
 from markdown2 import markdown
 from satcfdi import DatePeriod
 from satcfdi.accounting import filter_invoices_iter, filter_payments_iter, invoices_export, payments_export
 from satcfdi.accounting.process import payments_groupby_receptor, payments_retentions_export
 from satcfdi.create.cfd import cfdi40
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
 from satcfdi.pacs import sat
 from satcfdi.printer import Representable
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from weasyprint import HTML, CSS
-from xlsxwriter.exceptions import FileCreateError
 
 from . import SOURCE_DIRECTORY, ARCHIVOS_DIRECTORY, TEMP_DIRECTORY
 from .environments import facturacion_environment
+from .exceptions import ConsoleErrors
 from .formatting_functions.common import fecha_mes
-from .utils import add_month
+from .utils import add_month, find_best_match, months_between, clear_directory
 
 logger = logging.getLogger(__name__)
 logger.level = logging.INFO
 
 sat_manager = sat.SAT()
 
 PERIODICIDAD = {
     "Mensual": 1,
     "Bimestral": 2,
     "Trimestral": 3,
     "Cuatrimestral": 4,
     "Semestral": 6,
     "Anual": 12
 }
+CALENDAR_FECHA_FMT = '%Y-%m-%d'
 
 
 def create_cfdi(receptor_cif, factura_details, emisor_cif):
     emisor = cfdi40.Emisor(
         rfc=emisor_cif['Rfc'],
         nombre=emisor_cif['RazonSocial'],
         regimen_fiscal=emisor_cif['RegimenFiscal']
@@ -59,21 +59,14 @@
         metodo_pago=factura_details['MetodoPago'],
         forma_pago=factura_details['FormaPago'],
         # serie=serie,
         # folio=folio,
         conceptos=factura_details["Conceptos"]
     )
     invoice = invoice.process()
-
-    expected_total = factura_details.get('Total')
-    if expected_total is not None:
-        if expected_total != invoice['Total']:
-            print(f"{factura_details['Receptor']}: Total '{expected_total}' is invalid, expected '{invoice['Total']}'")
-            return None
-
     return invoice
 
 
 def parse_periodo_mes_ajuste(periodo_mes_ajuste: str):
     parts = periodo_mes_ajuste.split(".")
     if len(parts) != 2:
         raise ValueError("Periodo Invalido")
@@ -97,37 +90,14 @@
     template = facturacion_environment.from_string(concepto["Descripcion"])
     concepto["Descripcion"] = template.render(
         periodo=periodo
     )
     return concepto
 
 
-def validad_facturas(clients, facturas):
-    is_valid = True
-    for factura_details in facturas:
-        cliente = clients.get(factura_details['Receptor'])
-        if not cliente:
-            print(f"{factura_details['Receptor']}: client not found")
-            is_valid = False
-
-        for c in factura_details["Conceptos"]:
-            periodo_mes_ajuste = c.get("_periodo_mes_ajuste", "")
-            try:
-                parse_periodo_mes_ajuste(periodo_mes_ajuste)
-            except ValueError:
-                print(f"{factura_details['Receptor']}: _periodo_mes_ajuste '{periodo_mes_ajuste}' is invalid")
-                is_valid = False
-
-        if factura_details["MetodoPago"] == "PPD" and factura_details["FormaPago"] != "99":
-            print(f"{factura_details['Receptor']}: FormaPago '{factura_details['FormaPago']}' is invalid, expected '99' for PPD")
-            is_valid = False
-
-    return is_valid
-
-
 def period_desc(dp: DatePeriod):
     return fecha_mes(date(year=dp.year, month=dp.month, day=1))
 
 
 def periodicidad_desc(dp: DatePeriod, periodo_mes_ajuste, offset):
     periodo_meses, mes_ajuste = parse_periodo_mes_ajuste(periodo_mes_ajuste)
 
@@ -142,70 +112,75 @@
             )
 
         return periodo
     return None
 
 
 def generate_ingresos(clients, facturas, dp, emisor_rfc):
-    if not validad_facturas(clients, facturas):
-        return
-
     emisor_cif = clients[emisor_rfc]
-
-    def prepare_concepto(concepto):
-        periodo = periodicidad_desc(
-            dp,
-            concepto['_periodo_mes_ajuste'],
-            concepto.get('_desfase_mes')
-        )
-        if periodo and concepto['ValorUnitario'] is not None:
-            return format_concepto_desc(concepto, periodo=periodo)
+    errors = []
 
     def facturas_iter():
-        i = 0
-        for f in facturas:
-            receptor_cif = clients[f['Receptor']]
-            conceptos = [x for x in (prepare_concepto(c) for c in f["Conceptos"]) if x]
-            if conceptos:
-                f["Conceptos"] = conceptos
-                yield create_cfdi(receptor_cif, f, emisor_cif)
-                i += 1
-
-    cfdis = [i for i in facturas_iter()]
-
-    if None in cfdis:
-        return
-
+        for i, f in enumerate(facturas, start=1):
+            try:
+                def prepare_concepto(c):
+                    periodo = periodicidad_desc(
+                        dp,
+                        c['_periodo_mes_ajuste'],
+                        c.get('_desfase_mes')
+                    )
+                    if periodo and c['ValorUnitario'] is not None:
+                        return format_concepto_desc(c, periodo=periodo)
+
+                receptor_cif = clients.get(f['Receptor'])
+                if not receptor_cif:
+                    raise ValueError("client not found")
+
+                if f["MetodoPago"] == "PPD" and f["FormaPago"] != "99":
+                    raise ValueError(f"FormaPago '{f['FormaPago']}' is invalid, expected '99' for PPD")
+
+                if conceptos := [x for x in (prepare_concepto(c) for c in f["Conceptos"]) if x]:
+                    f["Conceptos"] = conceptos
+                    cfdi = create_cfdi(receptor_cif, f, emisor_cif)
+
+                    expected_total = f.get('Total')
+                    if expected_total is not None and expected_total != cfdi['Total']:
+                        raise ValueError(f"Total '{expected_total}' is invalid, expected '{cfdi['Total']}'")
+
+                    yield cfdi
+            except Exception as e:
+                errors.append(f"{i} {f['Receptor']}: {str(e)}")
+
+    cfdis = list(facturas_iter())
+    if errors:
+        raise ConsoleErrors("Generar Facturas Errores", errors=errors)
     return cfdis
 
 
 def parse_fecha_pago(fecha_pago):
     if not fecha_pago:
         raise ValueError("Fecha de Pago es requerida")
 
-    fecha_pago = datetime.fromisoformat(fecha_pago)
+    fecha_pago = datetime.strptime(fecha_pago, CALENDAR_FECHA_FMT)
     if fecha_pago > datetime.now():
         raise ValueError("Fecha de Pago es mayor a la fecha actual")
 
     if fecha_pago.replace(hour=12) > datetime.now():
         fecha_pago = datetime.now()
     else:
         fecha_pago = fecha_pago.replace(hour=12)
 
     dif = datetime.now() - fecha_pago
-    if dif.days > 30:
-        raise ValueError("Fecha de Pago es de hace mas de 30 dias")
+    if dif.days > 35:
+        raise ValueError("Fecha de Pago es de hace mas de 35 dias")
 
     return fecha_pago
 
 
 def parse_importe_pago(importe_pago: str):
-    if not importe_pago:
-        return None
-
     try:
         return round(Decimal(importe_pago), 2)
     except InvalidOperation:
         raise ValueError("Importe de Pago es invalido")
 
 
 def pago_factura(factura_pagar, fecha_pago: datetime, forma_pago: str, importe_pago: Decimal = None):
@@ -230,14 +205,77 @@
         rfc = f["Receptor"]
         for concepto in f["Conceptos"]:
             _, mes_aj = parse_periodo_mes_ajuste(concepto['_periodo_mes_ajuste'])
             if mes_aj == mes_ajuste:
                 yield rfc, concepto
 
 
+def generate_ajustes(clients, facturas, dp, dp_effective, emisor_rfc):
+    errors = []
+    ajustes_dir = ajustes_directory(DatePeriod(dp.year, dp.month))
+    clear_directory(ajustes_dir)
+
+    def ajustes_iter():
+        for i, (receptor_rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month), start=1):
+            try:
+                valor_unitario_raw = concepto["ValorUnitario"]
+
+                if isinstance(valor_unitario_raw, dict):
+                    vu_eff, vu = find_best_match(valor_unitario_raw, dp)
+                    vun_eff, vun = find_best_match(valor_unitario_raw, dp_effective)
+                    if vu_eff == vun_eff:
+                        vun = None
+                        num_meses = None
+                    else:
+                        num_meses = months_between(vun_eff, vu_eff)
+
+                    if vun and vu:
+                        ajuste_porcentaje = round((vun / vu - 1) * 100, 2)
+                    else:
+                        ajuste_porcentaje = None
+                else:
+                    vu = valor_unitario_raw
+                    vun = None
+                    num_meses = None
+                    ajuste_porcentaje = None
+
+                concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
+                file_name = os.path.join(ajustes_dir, f'AjusteRenta_{receptor_rfc}_{i}.pdf')
+
+                client_receptor = clients[receptor_rfc]  # type: dict
+                data = {
+                    "receptor": client_receptor,
+                    "emisor": clients[emisor_rfc],
+                    "concepto": concepto,
+                    "valor_unitario": vu,
+                    "valor_unitario_nuevo": vun or '',
+                    "ajuste_porcentaje": ajuste_porcentaje or "",
+                    "meses": num_meses or '',
+                    "efectivo_periodo_desc": periodicidad_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),
+                    "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
+                    'file_name': file_name
+                }
+
+                if ajuste_porcentaje:
+                    res = generate_pdf_template(
+                        template_name='incremento_template.md',
+                        fields=data
+                    )
+                    with open(file_name, 'wb') as f:
+                        f.write(res)
+                yield data
+            except Exception as e:
+                errors.append(f"{i} {receptor_rfc}: {str(e)}")
+
+    cfdis = list(ajustes_iter())
+    if errors:
+        raise ConsoleErrors("Generar Ajustes Errores", errors=errors)
+    return cfdis
+
+
 def archivos_folder(dp: DatePeriod):
     if dp.month:
         return os.path.join(ARCHIVOS_DIRECTORY, str(dp.year), str(dp.year) + "-{:02d}".format(dp.month))
     return os.path.join(ARCHIVOS_DIRECTORY, str(dp.year))
 
 
 def archivos_filename(dp: DatePeriod, ext="xlsx"):
@@ -283,19 +321,16 @@
 
     # RETENCIONES
     if dp.month is None:
         archivo_retenciones = archivos_filename(dp, ext="retenciones.txt")
         pagos_agrupados = payments_groupby_receptor(emitidas_pagos)
         payments_retentions_export(archivo_retenciones, pagos_agrupados)
 
-    try:
-        workbook.close()
-        return archivo_excel
-    except FileCreateError:
-        return None
+    workbook.close()
+    return archivo_excel
 
 
 def generate_pdf_template(template_name, fields):
     increment_template = facturacion_environment.get_template(template_name)
     md5_document = increment_template.render(
         fields
     )
@@ -311,16 +346,16 @@
     )
     return pdf
 
 
 def mf_pago_fmt(cfdi):
     i = cfdi
     if i['TipoDeComprobante'] == "I":
-        return i['TipoDeComprobante'].code + ' ' + i['MetodoPago'].code + ' ' + (i['FormaPago'].code if i['FormaPago'].code != '99' else '')
-    return i['TipoDeComprobante'].code
+        return i['TipoDeComprobante'].code + ' ' + i['MetodoPago'].code + ' ' + (i['FormaPago'].code if i['FormaPago'].code != '99' else '  ')
+    return i['TipoDeComprobante'].code + '       '
 
 
 def ajustes_directory(dp: DatePeriod):
     return os.path.join(archivos_folder(dp), 'ajustes')
 
 
 def preview_cfdis(cfdis):
@@ -328,7 +363,11 @@
     Representable.html_write_all(
         objs=cfdis,
         target=outfile,
     )
     os.startfile(
         os.path.abspath(outfile)
     )
+
+
+def center_location(element) -> tuple[int, int]:
+    return tuple((c + s // 3) for c, s in zip(element.current_location(), element.size))
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.0/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/layout.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from datetime import date, datetime
+from datetime import date, datetime, timedelta
+from enum import StrEnum
 
 import PySimpleGUI as sg
+from satcfdi.pacs.sat import TipoDescargaMasivaTerceros
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
-from satdigitalinvoice.gui_functions import mf_pago_fmt
+from satdigitalinvoice.gui_functions import mf_pago_fmt, CALENDAR_FECHA_FMT
 
 from .log_tools import *
 
 FORMA_PAGO = CATALOGS['{http://www.sat.gob.mx/sitio_internet/cfd/catalogos}c_FormaPago']
 TEXT_PADDING = ((5, 0), 3)
 
 # 24 x 24
@@ -54,15 +56,39 @@
               "+tLU1GOzfXiEVirBDvgE9gA70A9oauL20izU85aHgcxAlZACxgAH0DDo29IM1DOSh6paAI/QJQyVwJCIFaE4lxE8rBe//AALIA90HbMY5VgqTDikou0lbuQVyrugIkMnsSFGttN/ENHnJ1DWqNc6+FFV" \
               "+J7jWO9tYul5pDWKJc8FxhnXSBriQKNa8eUqPBNbh5xTMeK4JRjWviP5msVkdMqnsVts7aKtGbX8zS7XtZmdwhDff5tol2/ckkXTrXoK/N88Qvnr38CSEQRlwAAAABJRU5ErkJggg=="
 
 EDIT_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAA10lEQVR4nO3UPUpDQRSG4cfCQgn" \
             "+LSPLSCcEC1u3EXdgEXdg3EC2IXYS0N4itZWWGkGvDHyBkE45Npq3usyB95tz5s6w4ZfZwwQveMIFtqvkB5jhDZe4xmdCyuQdxivrk3RSIl/gAe84Ta118oytCvkQPdwmZJxxXVXJl/TSSZd6O/hvs4+7yE" \
             "/Wasd4xT2ONvIl/3gsuys3dLRWGyZ0ll/2RwwiX2SnZ5XyxnkerD5uEjKqkjemmOe7H3FXJW885rGaR9xVyg/xkZBpxjXIwZewU7VTf4ovf6VSMafchm4AAAAASUVORK5CYII="
 
+ZIP_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAAt0lEQVR4nOXVPQrCQBCG4Qd7wTPYWtulsPAa5hq2KS0svYRnSKuNvZ3aWXgDESQibBECgWQl4s8HA8vAzMs3u" \
+           "+zwi0qRR0baBJChiGhehNrGgLYq/gcwxSICsAi1n6NJsF1U7FfPz9hj1BYwDLa3ocmsBrDBBesYF32csUOvBnDCFasYwBJ3jEu5KuAYmg9iRnTDAXMkNYBGT/OVS858mpIwkraal8b4439R9i5A3tXC6Xxl" \
+           "+io9AMiJawPDOx2QAAAAAElFTkSuQmCC"
+
+IMPORT_CSV = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAABVElEQVR4nN3Vv0scYRDG8U+EQApjl4AIAYMIFqIEhGAnpLBJIRZ2goV" \
+             "/gZIiIqY8rkklIb2VlWjAYq1yXGVvlzSSIlqKkZjIhoM5OJaL9+6qCTgwsDs7z3zfeff9wX20RWQJvoX+KoB3yHsU/xI5n6tA2oCUnF9VIGUA87hEE4/vAvAKH+K5kdpJGUBe8LXbAjyP0Xd6HtrkZVrWstD+f+vDW" \
+             "+xiLmLj2MZHPCl0WbrjhZjPb7EEh3CEU/zAOpYiZxKf8LUMYCPEI6jFDz3DYfhYdPEb7/ET9TKAbqtoGt9xheWINWInt3KnygDehKjWIR7GaxzjIPJW43treh5EbBY7eHQdoFXsJMRNPMRmvJ" \
+             "/jZeSNRqzeUfwiYvu9IAN4EcXFCCcwWMibwdNC8bwXpL1LU+0Z9grHePtYX6l6VPzNkrQpF07WxZMBqVdmVhVwE/v3gD+of4e/h7E8SwAAAABJRU5ErkJggg=="
+
 BUTTON_COLOR = (sg.theme_background_color(), sg.theme_background_color())
+LARGE_FONT = ("Courier New", 11, "bold")
+PERIODO_FMT = "%Y-%m"
+
+
+class TipoRecuperar(StrEnum):
+    Emitidas = 'Emitidas'
+    Recibidas = 'Recibidas'
+
+
+class SearchOptions(StrEnum):
+    PorPagar = 'Por Pagar'
+    PorEnviar = 'Por Enviar'
+    Hoy = datetime.now().strftime(CALENDAR_FECHA_FMT)
+    Mes = datetime.now().strftime(PERIODO_FMT)
+    Anio = datetime.now().strftime("%Y")
 
 
 class MyTable(sg.Table):
     def __init__(self, key, headings, row_fn):
         super().__init__(
             values=[],
             key=key,
@@ -75,123 +101,151 @@
             background_color="white",
             # headings=HEADINGS,
             # values=[],
             # auto_size_columns=False,
             # col_widths=COL_WIDTHS,
             # justification="center",
             # num_rows=20,
-            alternating_row_color="grey95", #"aliceblue",
+            alternating_row_color="grey95",  # "aliceblue",
             # row_height=ROW_HEIGHT,
             # header_text_color="white",
             # header_background_color="darkblue",
             # font=FONT,
             # bind_return_key=True,
-            tooltip="Doble click para ver factura",
+            # tooltip="Doble click para ver factura",
             # right_click_menu=RIGHT_CLICK_MENU
-            metadata=[]
+            metadata=True
         )
         self.row_fn = row_fn
 
     def selected_items(self):
         return [self.metadata[i] for i in self.SelectedRows]
 
     def select_all(self):
         self.update(
             select_rows=list(range(len(self.metadata)))
         )
 
+    def delete_selected(self):
+
+        def iter_metadata():
+            s = 0
+            for i in self.SelectedRows + [len(self.metadata)]:
+                for j in range(s, i):
+                    yield self.metadata[j]
+                s = i + 1
+
+        self.update(
+            values=list(iter_metadata())
+        )
+
     def update(self, values=None, **kwargs):
-        super().update(
-            values=[
-                self.row_fn(i, item)
-                for i, item in enumerate(values, start=1)
-            ],
-            **kwargs
+        if values is not None:
+            super().update(
+                values=[
+                    self.row_fn(i, item)
+                    for i, item in enumerate(values, start=1)
+                ],
+                **kwargs
+            )
+            self.metadata = values
+        else:
+            super().update(**kwargs)
+
+    def refresh(self):
+        self.update(
+            self.metadata,
+            select_rows=self.SelectedRows
         )
-        self.metadata = values
 
 
 def make_layout(has_fiel, local_db):
-    # LAYOUT
-    button_column = [
-        sg.Button(image_data=CONFIG_ICON, key="ver_config", border_width=0, button_color=BUTTON_COLOR),
-        sg.Text("Periodo:", pad=TEXT_PADDING),
-        sg.Input(date.today().strftime('%Y-%m'), size=(11, 1), key="periodo"),
-        sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
-        sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
-        sg.Button(image_data=HTML_ICON, key="ver_html", border_width=0, button_color=BUTTON_COLOR),
-
-        sg.Push(),
-        sg.Text("Factura:", pad=TEXT_PADDING),
-        sg.Text("", key="serie", pad=TEXT_PADDING, text_color="black"),
-        sg.Input("", key="folio", size=(8, 1), enable_events=True),
-        sg.Button("".center(22), disabled=True, key="crear_facturas", border_width=0, button_color=sg.theme_background_color()),
-    ]
-
     # ----- Full layout -----
     return [
-        button_column,
         [
             sg.TabGroup(
                 [[
                     sg.Tab(
-                        'Consola'.center(13),
+                        'Emitidas '.center(13),
                         [
                             [
-                                sg.Push(),
-                                sg.Button(image_data=ABOUT_ICON, key="about", border_width=0, button_color=BUTTON_COLOR),
+                                sg.Column([[
+                                    sg.Button(image_data=IMPORT_CSV, key="importar_emitidas", border_width=0, button_color=BUTTON_COLOR),
+                                    sg.ButtonMenu(
+                                        image_data=SEARCH_ICON, button_text="", key="buscar_facturas", border_width=0, button_color=BUTTON_COLOR,
+                                        menu_def=[
+                                            [],
+                                            [str(o) for o in SearchOptions],
+                                        ],
+                                    ),
+                                    sg.Input(datetime.now().strftime(PERIODO_FMT), size=(40, 1), key="emitidas_search"),
+                                ]],
+                                    expand_x=True
+                                )
                             ],
-                            [sg.Multiline(
-                                expand_x=True,
-                                expand_y=True,
-                                key="console",
-                                write_only=True,
-                                autoscroll=True,
-                                reroute_stdout=True
-                            )]
-                        ],
-                        key='console_tab',
-                    ),
-                    sg.Tab(
-                        'Clientes'.center(13),
-                        [
                             [
-                                sg.Button("Refrescar", key="refresh_clientes", border_width=0),
-                                sg.Push(),
-                                sg.Button(image_data=EDIT_ICON, key="editar_clientes", border_width=0, button_color=BUTTON_COLOR),
+                                sg.HorizontalSeparator(color="black"),
+                            ],
+                            [
+                                sg.Column([[
+                                    sg.Button("".ljust(10), key="status_sat", border_width=0, button_color=sg.theme_background_color()),
+                                    sg.Button("".ljust(10), key="email_notificada", border_width=0, button_color=sg.theme_background_color()),
+                                    sg.Button("".ljust(10), key="pendiente_pago", border_width=0, button_color=sg.theme_background_color()),
+                                ]]),
+                                sg.VSeparator(color="black"),
+                                sg.Column([[
+                                    sg.CalendarButton("FechaPago:", format=CALENDAR_FECHA_FMT, title="FechaPago", no_titlebar=False, target="fecha_pago", pad=TEXT_PADDING,
+                                                      border_width=0),
+                                    sg.Input(datetime.now().strftime(CALENDAR_FECHA_FMT), size=(12, 1), key="fecha_pago"),
+                                    sg.Text("FormaPago:", pad=TEXT_PADDING, border_width=0),
+                                    sg.Combo([Code(k, v) for k, v in FORMA_PAGO.items()],
+                                             default_value=Code("03", FORMA_PAGO["03"]), key="forma_pago", size=(35, 1)),
+                                    sg.Text("ImpPagado:", pad=TEXT_PADDING, border_width=0),
+                                    sg.Input("", size=(12, 1), key="importe_pago"),
+                                ]], visible=False, key="ppd_action_items"),
                             ],
                             [
                                 MyTable(
-                                    key="clientes_table",
+                                    key="emitidas_table",
                                     headings=[
-                                        "#",
-                                        "Razon Social",
-                                        "Rfc",
-                                        "Reg",
-                                        "CP"
+                                        '#',
+                                        'Receptor Razon Social',
+                                        'Recep. Rfc',
+                                        'Factura',
+                                        "Fecha",
+                                        "Total",
+                                        "Pendiente",
+                                        "Status",
+                                        "Tipo",
+                                        "Folio"
                                     ],
                                     row_fn=lambda i, r: [
                                         i,
-                                        r["RazonSocial"],
-                                        r["Rfc"],
-                                        r["RegimenFiscal"].code,
-                                        r["CodigoPostal"]
+                                        r['Receptor'].get('Nombre', ''),
+                                        r['Receptor']['Rfc'],
+                                        r.name,
+                                        r["Fecha"].strftime(CALENDAR_FECHA_FMT),
+                                        r["Total"],
+                                        r.saldo_pendiente if r.saldo_pendiente else "",
+                                        str(local_db.liquidated_state(r)) + str(" 📧" if local_db.notified(r) else "   "),
+                                        mf_pago_fmt(r),
+                                        r.uuid
                                     ]
                                 )
                             ]],
-                        key='clients_tab',
+                        key='emitidas_tab',
                     ),
                     sg.Tab(
-                        'Facturas'.center(13),
+                        'Facturas '.center(13),
                         [
                             [
-                                sg.Button("Refrescar", key="refresh_facturas", border_width=0, ),
-                                sg.Text("", pad=TEXT_PADDING, key="preparar_facturas_text"),
-                                sg.Push(),
                                 sg.Button(image_data=EDIT_ICON, key="editar_facturas", border_width=0, button_color=BUTTON_COLOR),
+                                sg.Text("Periodo:", pad=TEXT_PADDING),
+                                sg.Input(date.today().strftime(PERIODO_FMT), size=(11, 1), key="facturas_periodo"),
+                                sg.Text("", pad=TEXT_PADDING, key="preparar_facturas_text", font=LARGE_FONT),
                             ],
                             [
                                 MyTable(
                                     key="facturas_table",
                                     headings=[
                                         '#',
                                         'EReg',
@@ -211,102 +265,48 @@
                                         r['Total']
                                     ]
                                 )
                             ]],
                         key='facturas_tab',
                     ),
                     sg.Tab(
-                        'Emitidas'.center(13),
-                        [
-                            [
-                                sg.Button("Pendientes", key="facturas_pendientes", border_width=0),
-                                sg.Button("Todas", key="facturas_emitidas", border_width=0),
-                                sg.Button(image_data=SEARCH_ICON, key="emitidas_search_enter", border_width=0, button_color=BUTTON_COLOR),
-                                sg.Input("", size=(20, 1), key="emitidas_search", border_width=0),
-                                sg.Text("", pad=TEXT_PADDING, key="emitidas_text"),
-                            ],
-                            [
-                                sg.Column([[
-                                    sg.Button("".ljust(10), key="status_sat", border_width=0, button_color=sg.theme_background_color()),
-                                    sg.Button("".ljust(10), key="email_notificada", border_width=0, button_color=sg.theme_background_color()),
-                                    sg.Button("".ljust(10), key="pendiente_pago", border_width=0, button_color=sg.theme_background_color()),
-                                ]]),
-                                sg.VSeparator(),
-                                sg.Column([[
-                                    sg.CalendarButton("FechaPago:", format='%Y-%m-%d', title="FechaPago", no_titlebar=False, target="fecha_pago", pad=TEXT_PADDING,
-                                                      border_width=0,
-                                                      key="fecha_pago_select"),
-                                    sg.Input(datetime.now().strftime('%Y-%m-%d'), size=(12, 1), key="fecha_pago", border_width=0),
-                                    sg.Combo([Code(k, v) for k, v in FORMA_PAGO.items()], default_value=Code("03", FORMA_PAGO["03"]), key="forma_pago", size=(28, 1)),
-                                    sg.Text("ImpPagado:", pad=TEXT_PADDING, key="imp_pagado_text", border_width=0),
-                                    sg.Input("", size=(12, 1), key="importe_pago", border_width=0),
-                                    sg.Button("Comprobante Pago", key="prepare_pago", border_width=0),
-                                    sg.Button(image_data=PREVIEW_ICON, key="ver_html_pago", border_width=0, button_color=BUTTON_COLOR),
-                                ]], visible=False, key="ppd_action_items"),
-                            ],
-                            [
-                                MyTable(
-                                    key="emitidas_table",
-                                    headings=[
-                                        '#',
-                                        'Receptor Razon Social',
-                                        'Recep. Rfc',
-                                        'Factura',
-                                        "Fecha",
-                                        "Total",
-                                        "Pagada",
-                                        "Tipo",
-                                    ],
-                                    row_fn=lambda i, r: [
-                                        i,
-                                        r['Receptor'].get('Nombre', ''),
-                                        r['Receptor']['Rfc'],
-                                        r.name,
-                                        r["Fecha"].strftime("%Y-%m-%d"),
-                                        r["Total"],
-                                        local_db.liquidated_state(r),
-                                        mf_pago_fmt(r)
-                                    ]
-                                )
-                            ]],
-                        key='emitidas_tab',
-                    ),
-                    sg.Tab(
                         'Correos'.center(13),
                         [
                             [
-                                sg.Button("Refrescar", key="refresh_correos", border_width=0, ),
+                                sg.Text("", pad=TEXT_PADDING),
                             ],
                             [
                                 MyTable(
                                     key="correos_table",
                                     headings=[
                                         '#',
                                         'Receptor Razon Social',
                                         'Recep. Rfc',
                                         'Facturas',
                                         'Pendientes Emitidas Meses Anteriores'
                                     ],
                                     row_fn=lambda i, r: [
                                         i,
-                                        r[0]["RazonSocial"][0:36],
+                                        r[0]["RazonSocial"],
                                         r[0]["Rfc"],
                                         ",".join(n.name for n in r[1]),
                                         ",".join(n.name for n in r[2])
                                     ]
                                 )
                             ]],
                         key='correos_tab',
                     ),
                     sg.Tab(
                         'Ajustes'.center(13),
                         [
                             [
-                                sg.Button("Refrescar", key="refresh_ajustes", border_width=0, ),
-                                sg.Text("", pad=TEXT_PADDING, key="preparar_ajustes_text"),
+                                sg.Button(image_data=EDIT_ICON, key="editar_ajustes", border_width=0, button_color=BUTTON_COLOR),
+                                sg.Text("Periodo:", pad=TEXT_PADDING),
+                                sg.Input(date.today().strftime(PERIODO_FMT), size=(11, 1), key="ajustes_periodo"),
+                                sg.Text("", pad=TEXT_PADDING, key="preparar_ajustes_text", font=LARGE_FONT),
                             ],
                             [
                                 MyTable(
                                     key="ajustes_table",
                                     headings=[
                                         "#",
                                         "Receptor Razon Social",
@@ -330,59 +330,222 @@
                                         r["efectivo_periodo_desc"]
                                     ]
                                 )
                             ]],
                         key='ajustes_tab'
                     ),
                     sg.Tab(
-                        'Recuperar'.center(13),
+                        'Clientes '.center(13),
+                        [
+                            [
+                                sg.Button(image_data=EDIT_ICON, key="editar_clientes", border_width=0, button_color=BUTTON_COLOR),
+                                sg.Push(),
+                                sg.Button("Exportar", key="exportar_clientes", border_width=0),
+                            ],
+                            [
+                                MyTable(
+                                    key="clientes_table",
+                                    headings=[
+                                        "#",
+                                        "Razon Social",
+                                        "Rfc",
+                                        "Reg",
+                                        "CP",
+                                        "IdCIF"
+                                    ],
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r["RazonSocial"],
+                                        r["Rfc"],
+                                        r["RegimenFiscal"].code,
+                                        r["CodigoPostal"],
+                                        r["IdCIF"]
+                                    ]
+                                )
+                            ]],
+                        key='clientes_tab',
+                    ),
+                    sg.Tab(
+                        'Solicitudes'.center(13),
+                        [
+                            [
+                                sg.Column([[
+                                    sg.Button(image_data=ZIP_ICON, key="cargar_zip", border_width=0, button_color=BUTTON_COLOR),
+                                    sg.Text("Recuperar:", pad=TEXT_PADDING),
+                                    sg.Combo([TipoRecuperar.Recibidas, TipoRecuperar.Emitidas], default_value=TipoRecuperar.Recibidas, key="tipo_recuperar", size=(10, 1)),
+
+                                    sg.CalendarButton("Inicio:", format=CALENDAR_FECHA_FMT, title="Inicio", no_titlebar=False, target="fecha_inicial", pad=TEXT_PADDING,
+                                                      border_width=0),
+                                    sg.Input((datetime.now() - timedelta(days=40)).strftime(CALENDAR_FECHA_FMT), size=(12, 1), key="fecha_inicial"),
+
+                                    sg.CalendarButton("Final:", format=CALENDAR_FECHA_FMT, title="Final", no_titlebar=False, target="fecha_final", pad=TEXT_PADDING,
+                                                      border_width=0),
+                                    sg.Input(datetime.now().strftime(CALENDAR_FECHA_FMT), size=(12, 1), key="fecha_final"),
+
+                                    sg.Text("Tipo:", pad=TEXT_PADDING),
+                                    sg.Combo([TipoDescargaMasivaTerceros.CFDI, TipoDescargaMasivaTerceros.Metadata], default_value=TipoDescargaMasivaTerceros.CFDI,
+                                             key="tipo_solicitud", size=(10, 1)),
+
+                                    sg.Button("Nueva Solicitud", key="nueva_solicitud", border_width=0),
+                                ]],
+                                    expand_x=True
+                                )
+                            ],
+                            [
+                                MyTable(
+                                    key="solicitudes_table",
+                                    headings=[
+                                        "#",
+                                        "IdSolicitud",
+                                        "Mensaje",
+                                        "EstadoSolicitud",
+                                        "FechaInicial",
+                                        "FechaFinal",
+                                        "TipoSolicitud",
+                                        "RfcReceptor",
+                                        "RfcEmisor",
+                                    ],
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r["response"]["IdSolicitud"],
+                                        r["response"]["Mensaje"],
+                                        r["response"].get("EstadoSolicitud", ""),
+                                        r["request"]["fecha_inicial"].strftime(CALENDAR_FECHA_FMT),
+                                        r["request"]["fecha_final"].strftime(CALENDAR_FECHA_FMT),
+                                        r["request"]["tipo_solicitud"],
+                                        r["request"]["rfc_receptor"] or "",
+                                        r["request"]["rfc_emisor"] or "",
+                                    ]
+                                )
+                            ]
+                        ],
+                        key='solicitudes_tab',
+                        # visible=has_fiel
+                    ),
+                    sg.Tab(
+                        'Contabilidad '.center(13),
+                        [[
+                            sg.Column([[
+                                sg.Text("Periodo:", pad=TEXT_PADDING),
+                                sg.Input(date.today().strftime(PERIODO_FMT), size=(11, 1), key="periodo"),
+                                sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
+                                sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
+                            ]])
+                        ]],
+                        key='contabilidad_tab',
+                    ),
+                    sg.Tab(
+                        'Consola'.center(13),
                         [
                             [
-                                sg.Button("SAT Status", key="sat_status_todas", border_width=0),
-                                sg.Text("Recuperar:", pad=TEXT_PADDING),
-                                sg.Button("Emitidas ", key="recuperar_emitidas", border_width=0),
-                                sg.Button("Recibidas", key="recuperar_recibidas", border_width=0),
-                                sg.Text("Dias:", pad=TEXT_PADDING),
-                                sg.Input("40", size=(4, 1), key="recuperar_dias"),
+                                sg.Push(),
+                                sg.Button(image_data=ABOUT_ICON, key="about", border_width=0, button_color=BUTTON_COLOR),
+                            ],
+                            [sg.Multiline(
+                                expand_x=True,
+                                expand_y=True,
+                                key="console",
+                                write_only=True,
+                                autoscroll=True,
+                                reroute_stdout=True
+                            )]
+                        ],
+                        key='console_tab',
+                    ),
+                    sg.Tab(
+                        'Configuracion'.center(13),
+                        [
+                            [
+                                sg.Column([[
+                                    sg.Button(image_data=EDIT_ICON, key="editar_configurar", border_width=0, button_color=BUTTON_COLOR),
+                                    sg.Button(image_data=CONFIG_ICON, key="ver_config", border_width=0, button_color=BUTTON_COLOR),
+                                    sg.Text("Proxima Factura:", pad=TEXT_PADDING),
+                                    sg.Text("Serie:", pad=TEXT_PADDING),
+                                    sg.Input("", key="serie", size=(8, 1)),
+                                    sg.Text("Folio:", pad=TEXT_PADDING),
+                                    sg.Input("", key="folio", size=(8, 1)),
+                                ]],
+                                    expand_x=True
+                                )
+                            ],
+                            [
+                                sg.Column([[
+                                    sg.Button("Organizar Facturas", key="organizar_facturas", border_width=0),
+                                ]],
+                                    expand_x=True
+                                )
+                            ],
+                            [
+                                sg.Column([[
+                                    sg.Button("Exportar Metadata", key="exportar_metadata", border_width=0),
+                                    sg.Button("Importar Metadata", key="importar_metadata", border_width=0),
+                                ]],
+                                    expand_x=True
+                                )
                             ]
                         ],
-                        key='recuperar_tab',
-                        visible=has_fiel
+                        key='configuracion_tab',
                     ),
                 ]],
                 expand_x=True,
                 expand_y=True,
                 enable_events=True,
                 key="main_tab_group",
             )
+        ],
+        [
+            sg.Column([[
+                sg.Push(),
+                sg.Text("Factura:", pad=TEXT_PADDING),
+                sg.Text("", key="serie_folio", pad=TEXT_PADDING),
+                sg.Button(image_data=PREVIEW_ICON, key="ver_preview", border_width=0, button_color=BUTTON_COLOR, disabled=True),
+                sg.Button("".center(22), disabled=True, key="crear_facturas", border_width=0, button_color=sg.theme_background_color()),
+                sg.Sizegrip(),
+            ]],
+                expand_x=True,
+            ),
         ]
     ]
 
 
 class ActionButtonManager:
-    def __init__(self, button):
+    def __init__(self, button, preview):
         self.name = ""
         self.items = []
         self.button = button
+        self.preview = preview
 
     def set_items(self, name, items):
         self.name = name
         self.items = items
         self.style_button()
 
     def clear(self):
         self.name = ""
         self.items = []
         self.style_button()
 
     def text(self):
+        header = "Procesar"
+        if self.name == "clientes":
+            header = "Validar"
+        elif self.name in ("facturas", "pago"):
+            header = "Crear"
+        elif self.name == "correos":
+            header = "Enviar"
+        elif self.name == "ajustes":
+            header = "Enviar"
+
         if self.items:
-            return f"Procesar {len(self.items)} {self.name.capitalize()}"
+            return f"{header} {len(self.items)} {self.name.capitalize()}"
         else:
             return ""
 
     def style_button(self):
+        self.preview.update(
+            disabled=not (bool(self.items) and self.name in ("facturas", "pago")),
+        )
         self.button.update(
             self.text().center(22),
             disabled=not self.items,
             button_color=sg.theme_button_color() if self.items else sg.theme_background_color()
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/log_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     print(
         yaml.dump(data, Dumper=NoAliasDumper, allow_unicode=True, width=1280, sort_keys=False)
     )
 
 
 def header_line(text):
     ln = (150 - len(text)) // 2
-    return ("=" * ln) + " " + text + " " + ("=" * ln)
+    return ("=" * ln) + " " + text + " " + ("=" * ln) + "\n"
 
 
 def cfdi_header(cfdi):
     receptor = Code(cfdi['Receptor']['Rfc'], cfdi['Receptor']['Nombre'])
     return f"{cfdi.name} - {cfdi.uuid} {receptor}"
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.0/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.0/satdigitalinvoice/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 import os
 import random
 import shutil
 from datetime import datetime
 from uuid import UUID
 
 from satcfdi import Signer, DatePeriod
+from satcfdi.accounting.models import EstadoComprobante
 
 
-def parse_date_period(periodo):
+def to_date_period(periodo):
     if not periodo:
         return DatePeriod(year=None)
 
-    fmt, period = try_parsing_date(periodo)
-    if fmt == '%Y':
-        return DatePeriod(period.year)
-    if fmt == '%Y-%m':
-        return DatePeriod(period.year, period.month)
-    if fmt == '%Y-%m-%d':
-        return DatePeriod(period.year, period.month, period.day)
-
-
-def try_parsing_date(text):
-    for fmt in ('%Y', '%Y-%m', '%Y-%m-%d'):
+    for f in ('%Y', '%Y-%m', '%Y-%m-%d'):
         try:
-            return fmt, datetime.strptime(text, fmt)
+            d = datetime.strptime(periodo, f)
+            return DatePeriod(
+                d.year,
+                d.month if '%Y-%m' in f else None,
+                d.day if f == '%Y-%m-%d' else None
+            )
         except ValueError:
             pass
-    raise ValueError('no valid date format found')
 
 
 def to_uuid(s):
     try:
         return UUID(s)
     except ValueError:
         return None
@@ -111,15 +106,20 @@
     for x in seq:
         if x in seen:
             return x
         seen.add(x)
     return None
 
 
-def parse_rango(rango):
-    if rango == "":
-        return 1, None
-    if rango.isdigit():
-        return int(rango), int(rango)
-    if "-" in rango:
-        start, end = rango.split("-")
-        return int(start), int(end)
+def estado_to_estatus(estatus):
+    if estatus == 'Vigente':
+        return EstadoComprobante.Vigente.value
+    elif estatus == 'Cancelado':
+        return EstadoComprobante.Cancelado.value
+    raise ValueError(f"Unknown status: {estatus}")
+
+
+def to_datetime(s):
+    try:
+        return datetime.fromisoformat(s, )
+    except ValueError:
+        return None
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.3
+Version: 4.0.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 setup.py
 satdigitalinvoice/__init__.py
 satdigitalinvoice/__version__.py
 satdigitalinvoice/client_validation.py
 satdigitalinvoice/environments.py
+satdigitalinvoice/exceptions.py
 satdigitalinvoice/facturacion.py
 satdigitalinvoice/file_data_managers.py
 satdigitalinvoice/gui_functions.py
 satdigitalinvoice/layout.py
 satdigitalinvoice/localdb.py
 satdigitalinvoice/log_tools.py
 satdigitalinvoice/mycfdi.py
@@ -17,14 +18,13 @@
 satdigitalinvoice.egg-info/requires.txt
 satdigitalinvoice.egg-info/top_level.txt
 satdigitalinvoice/formatting_functions/__init__.py
 satdigitalinvoice/formatting_functions/common.py
 satdigitalinvoice/images/logo.png
 satdigitalinvoice/markdown_styles/markdown6.css
 satdigitalinvoice/schemas/cliente.yaml
-satdigitalinvoice/schemas/config.yaml
 satdigitalinvoice/schemas/factura.yaml
 tests/test_clients.py
 tests/test_common.py
 tests/test_crear_facturas.py
 tests/test_localdb.py
 tests/test_main.py
```

### Comparing `satdigitalinvoice-3.0.3/setup.py` & `satdigitalinvoice-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.11',
+        'satcfdi==4.0.18',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-3.0.3/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.0/tests/test_crear_facturas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,89 +1,79 @@
-import logging
 from datetime import date, datetime
 from decimal import Decimal
 from unittest import mock
 
+import pytest
 from satcfdi import Signer, DatePeriod
 
 from satdigitalinvoice.__version__ import __package__
-from satdigitalinvoice.file_data_managers import ClientsManager, FacturasManager, ConfigManager
+from satdigitalinvoice.exceptions import ConsoleErrors
+from satdigitalinvoice.file_data_managers import ClientsManager, FacturasManager
 from satdigitalinvoice.gui_functions import generate_ingresos, periodicidad_desc
 from satdigitalinvoice.utils import find_best_match
 from tests.utils import verify_result, XElementPrettyPrinter
 
 csd_signer = Signer.load(
     certificate=open('csd/cacx7605101p8.cer', 'rb').read(),
     key=open('csd/cacx7605101p8.key', 'rb').read(),
     password=open('csd/cacx7605101p8.txt', 'rb').read(),
 )
 ym_date = DatePeriod(year=2023, month=4)
 clients = ClientsManager()
 module = __package__
 
 
-def test_generar_ingresos(caplog):
-    caplog.set_level(logging.INFO)
+def test_generar_ingresos():
     facturas = FacturasManager(ym_date)["Facturas"]
 
     with mock.patch(f'satcfdi.create.cfd.cfdi40.datetime') as m:
         m.now = mock.Mock(return_value=datetime(2022, 1, 1))
 
         facturas = generate_ingresos(
             clients=clients,
             facturas=facturas,
             dp=date(year=2023, month=4, day=1),
             emisor_rfc=csd_signer.rfc
         )
 
-        assert caplog.records == []
         assert len(facturas) == 3
 
         pp = XElementPrettyPrinter()
         verify = verify_result(data=pp.pformat(facturas), filename=f"facturas.pretty.py")
         assert verify
 
-    # assert facturas[0]["Total"] == Decimal('18065.66')
-    # assert facturas[0]["Conceptos"][0]["Descripcion"] == 1000
 
-
-def test_generar_ingresos_error(caplog, capsys):
-    caplog.set_level(logging.INFO)
+def test_generar_ingresos_error():
     facturas = FacturasManager(ym_date)["FacturasIncorrectas"]
-    print(len(facturas))
+    assert len(facturas) == 1
+
+    with pytest.raises(ConsoleErrors) as e:
+        generate_ingresos(
+            clients=clients,
+            facturas=facturas,
+            dp=date(year=2023, month=4, day=1),
+            emisor_rfc=csd_signer.rfc
+        )
 
-    ingresos = generate_ingresos(
-        clients=clients,
-        facturas=facturas,
-        dp=date(year=2023, month=4, day=1),
-        emisor_rfc=csd_signer.rfc
-    )
-
-    captured = capsys.readouterr()
-    assert captured.out == "1\nABMG891115PD7: Total '41000.16' is invalid, expected '37019.16'\n"
-    assert captured.err == ""
-    assert ingresos is None
+    assert e.value.errors == ["1 ABMG891115PD7: Total '41000.16' is invalid, expected '37019.16'"]
 
 
-def test_generar_ingresos_error2(caplog, capsys):
-    caplog.set_level(logging.INFO)
+def test_generar_ingresos_error2():
     facturas = FacturasManager(ym_date)["FacturasIncorrectas2"]
-    print(len(facturas))
+    assert len(facturas) == 1
+
+    with pytest.raises(ConsoleErrors) as e:
+        generate_ingresos(
+            clients=ClientsManager(),
+            facturas=facturas,
+            dp=date(year=2023, month=4, day=1),
+            emisor_rfc=csd_signer.rfc
+        )
 
-    ingresos = generate_ingresos(
-        clients=ClientsManager(),
-        facturas=facturas,
-        dp=date(year=2023, month=4, day=1),
-        emisor_rfc=csd_signer.rfc
-    )
-
-    captured = capsys.readouterr()
-    assert captured.out == "1\nXXXNOEXISTO: client not found\n"
-    assert captured.err == ""
-    assert ingresos is None
+    assert e.value.errors == ['1 XXXNOEXISTO: client not found']
 
 
 def test_periodo_desc():
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=0) == 'MES DE ENERO DEL 2021'
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=0) is None
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=0) is None
     assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=0) is None
```

### Comparing `satdigitalinvoice-3.0.3/tests/test_localdb.py` & `satdigitalinvoice-4.0.0/tests/test_localdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from datetime import datetime
 
-from satdigitalinvoice.localdb import LocalDB, LocalDBSatCFDI, save_data, load_data
+from satdigitalinvoice.localdb import LocalDB, LocalDBSatCFDI
 from satdigitalinvoice.utils import random_string
 
 
 def test_localdb():
     db = LocalDBSatCFDI(
+        base_path=".data",
         enviar_a_partir=datetime(2020, 1, 1),
         pagar_a_partir={
             "PUE": datetime(2020, 1, 1),
             "PPD": datetime(2020, 1, 1),
         }
     )
 
     db.folio_set(10)
     assert db.folio() == 10
 
-
-def test_save_data():
     a = random_string()
 
-    save_data('test_save_data', a)
-    assert load_data('test_save_data') == a
+    db.save_data('test_save_data', a)
+    assert db.load_data('test_save_data') == a
```

### Comparing `satdigitalinvoice-3.0.3/tests/test_main.py` & `satdigitalinvoice-4.0.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 
 
 def test_duplicated_facturas():
     class MyFacturasManager(FacturasManager):
         file_source = "facturas_duplicated.yaml"
 
     # expect exception thrown
-
-    with pytest.raises(ValueError) as e:
+    with pytest.raises(Exception) as e:
         MyFacturasManager(DatePeriod(2021, 1, 1))
     assert str(e.value)[0:20] == 'Factura Duplicada: {'
 
 
 def test_increase_month():
     d = DatePeriod(2021, 1)
     d = add_month(d, 1)
```

