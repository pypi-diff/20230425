# Comparing `tmp/satdigitalinvoice-4.0.4.tar.gz` & `tmp/satdigitalinvoice-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.4.tar", last modified: Tue Apr 25 07:27:41 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.5.tar", last modified: Tue Apr 25 07:31:38 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.4.tar` & `satdigitalinvoice-4.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.854117 satdigitalinvoice-4.0.4/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    38194 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 07:27:41.000000 satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 07:27:41.000000 satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:27:41.000000 satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:27:41.000000 satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 07:27:41.000000 satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:27:41.858117 satdigitalinvoice-4.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-25 07:27:29.000000 satdigitalinvoice-4.0.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.558736 satdigitalinvoice-4.0.5/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38196 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.558736 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.4/PKG-INFO` & `satdigitalinvoice-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.4
+Version: 4.0.5
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/facturacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         complement_invoices(self.all_invoices, invoice)
 
     def generate_invoice(self, invoice):
         ref_id = random_string()
 
         # Add Serie and Folio and signature
         folio = None
-        if invoice['TipoComprobante'] in self.facturas_con_serie_folio:
+        if invoice['TipoDeComprobante'] in self.facturas_con_serie_folio:
             invoice['Serie'] = self.local_db.serie()
             folio = self.local_db.folio()
             invoice['Folio'] = str(folio)
 
         cfdi40.Comprobante.sign(invoice, self.csd_signer)
 
         attempts = 3
```

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.5/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.5/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.5/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.4
+Version: 4.0.5
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.4/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/setup.py` & `satdigitalinvoice-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.5/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/tests/test_localdb.py` & `satdigitalinvoice-4.0.5/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.4/tests/test_main.py` & `satdigitalinvoice-4.0.5/tests/test_main.py`

 * *Files identical despite different names*

