# Comparing `tmp/satdigitalinvoice-4.0.0.tar.gz` & `tmp/satdigitalinvoice-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.0.tar", last modified: Tue Apr 25 01:55:33 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.1.tar", last modified: Tue Apr 25 04:36:51 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.0.tar` & `satdigitalinvoice-4.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.018338 satdigitalinvoice-4.0.0/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37891 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.018338 satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.018338 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 01:55:33.000000 satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:55:33.022338 satdigitalinvoice-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 01:55:15.000000 satdigitalinvoice-4.0.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37901 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.0/PKG-INFO` & `satdigitalinvoice-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.0
+Version: 4.0.1
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/facturacion.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from satcfdi import DatePeriod, csf
 from satcfdi.accounting import EmailManager
 from satcfdi.accounting.models import EstadoComprobante
 from satcfdi.accounting.process import complement_invoices
 from satcfdi.create.cfd import cfdi40
 from satcfdi.exceptions import ResponseError
 from satcfdi.pacs import Accept
-from satcfdi.pacs.sat import SAT, EstadoSolicitud, TipoDescargaMasivaTerceros
+from satcfdi.pacs.sat import SAT, EstadoSolicitud
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from xlsxwriter.exceptions import XlsxFileError
 
+from tests.utils import open_file
 from . import __version__, PPD, PUE, TEMP_DIRECTORY, ARCHIVOS_DIRECTORY, DATA_DIRECTORY, METADATA_FILE
 from .client_validation import validar_client, clientes_generar_txt
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_folder, period_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis, center_location, \
     CALENDAR_FECHA_FMT, ConsoleErrors, \
     generate_ajustes
@@ -678,25 +679,25 @@
                         if s_items := self.window["facturas_table"].selected_items():
                             preview_cfdis(s_items)
 
                     case 'clientes_table_enter':
                         # noinspection PyUnresolvedReferences
                         for client in self.window["clientes_table"].selected_items():
                             url = csf.url(rfc=client["Rfc"], id_cif=client["IdCIF"])
-                            os.startfile(url)
+                            open_file(url)
 
                     case 'emitidas_table_enter':
                         # noinspection PyUnresolvedReferences
                         if s_items := self.window["emitidas_table"].selected_items():
                             preview_cfdis(s_items)
 
                     case 'ajustes_table_enter':
                         # noinspection PyUnresolvedReferences
                         for ajuste in self.window["ajustes_table"].selected_items():
-                            os.startfile(
+                            open_file(
                                 os.path.abspath(ajuste['file_name'])
                             )
 
                     case 'correos_table_enter' | 'solicitudes_table_enter':
                         pass
 
                     case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "emitidas_table" | "solicitudes_table":
@@ -711,15 +712,16 @@
                          "ajustes_table+select_all" | "emitidas_table+select_all" | 'solicitudes_table+select_all':
                         # noinspection PyUnresolvedReferences
                         self.window[event.split("+")[0]].select_all()
 
                     case "facturas_table+delete" | "clientes_table+delete" | "correos_table+delete" | \
                          "ajustes_table+delete" | "emitidas_table+delete":
                         # noinspection PyUnresolvedReferences
-                        self.window[event.split("+")[0]].delete_selected()
+                        # self.window[event.split("+")[0]].delete_selected()
+                        pass
 
                     case "solicitudes_table+delete":
                         solitudes = self.local_db.get_solicitudes()
                         # noinspection PyUnresolvedReferences
                         sel = self.window["solicitudes_table"].selected_items()
                         for s in sel:
                             if s["response"].get("EstadoSolicitud").code < EstadoSolicitud.Terminada:
@@ -778,61 +780,61 @@
                                 self.action_button_manager.clear()
                                 self.action_button(
                                     action_name=action_name,
                                     action_items=action_items
                                 )
 
                     case "editar_clientes":
-                        os.startfile(
+                        open_file(
                             os.path.abspath("clientes.yaml")
                         )
 
                     case "exportar_clientes":
                         filename = 'clientes.txt'
                         clients = ClientsManager()
                         clientes_generar_txt(filename, clients)
-                        os.startfile(
+                        open_file(
                             os.path.dirname(
                                 os.path.abspath(filename)
                             )
                         )
 
                     case "editar_facturas" | "editar_ajustes":
-                        os.startfile(
+                        open_file(
                             os.path.abspath("facturas.yaml")
                         )
 
                     case "editar_configurar":
-                        os.startfile(
+                        open_file(
                             os.path.abspath("config.yaml")
                         )
 
                     case "ver_config":
-                        os.startfile(
+                        open_file(
                             os.path.abspath(".")
                         )
 
                     case "ver_excel":
                         dp = to_date_period(values["periodo"])
                         clients = ClientsManager()
                         emisor_cif = clients[self.csd_signer.rfc]
                         archivo_excel = exportar_facturas(
                             self.get_all_invoices(),
                             dp,
                             emisor_cif,
                             self.rfc_prediales
                         )
-                        os.startfile(
+                        open_file(
                             os.path.abspath(archivo_excel)
                         )
 
                     case "ver_carpeta":
                         dp = to_date_period(values["periodo"])
                         directory = archivos_folder(dp)
-                        os.startfile(
+                        open_file(
                             os.path.abspath(directory)
                         )
 
                     case "organizar_facturas":
                         MyCFDI.rename_invoices(search_path="**/*.xml")
 
                     case "cargar_zip":
```

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/gui_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
 from satcfdi.pacs import sat
 from satcfdi.printer import Representable
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from weasyprint import HTML, CSS
 
+from tests.utils import open_file
 from . import SOURCE_DIRECTORY, ARCHIVOS_DIRECTORY, TEMP_DIRECTORY
 from .environments import facturacion_environment
 from .exceptions import ConsoleErrors
 from .formatting_functions.common import fecha_mes
 from .utils import add_month, find_best_match, months_between, clear_directory
 
 logger = logging.getLogger(__name__)
@@ -360,14 +361,14 @@
 
 def preview_cfdis(cfdis):
     outfile = os.path.join(TEMP_DIRECTORY, "factura.html")
     Representable.html_write_all(
         objs=cfdis,
         target=outfile,
     )
-    os.startfile(
+    open_file(
         os.path.abspath(outfile)
     )
 
 
 def center_location(element) -> tuple[int, int]:
     return tuple((c + s // 3) for c, s in zip(element.current_location(), element.size))
```

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.1/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.1/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.1/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.0
+Version: 4.0.1
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.0/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/setup.py` & `satdigitalinvoice-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.1/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/tests/test_localdb.py` & `satdigitalinvoice-4.0.1/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.0/tests/test_main.py` & `satdigitalinvoice-4.0.1/tests/test_main.py`

 * *Files identical despite different names*

