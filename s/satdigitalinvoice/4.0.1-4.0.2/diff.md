# Comparing `tmp/satdigitalinvoice-4.0.1.tar.gz` & `tmp/satdigitalinvoice-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.1.tar", last modified: Tue Apr 25 04:36:51 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.2.tar", last modified: Tue Apr 25 04:43:20 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.1.tar` & `satdigitalinvoice-4.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37901 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 04:36:51.000000 satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:36:51.891083 satdigitalinvoice-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 04:36:40.000000 satdigitalinvoice-4.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37878 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.094254 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 04:43:20.000000 satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:43:20.098254 satdigitalinvoice-4.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 04:42:58.000000 satdigitalinvoice-4.0.2/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.1/PKG-INFO` & `satdigitalinvoice-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.1
+Version: 4.0.2
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/facturacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,27 +17,26 @@
 from satcfdi.exceptions import ResponseError
 from satcfdi.pacs import Accept
 from satcfdi.pacs.sat import SAT, EstadoSolicitud
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from xlsxwriter.exceptions import XlsxFileError
 
-from tests.utils import open_file
 from . import __version__, PPD, PUE, TEMP_DIRECTORY, ARCHIVOS_DIRECTORY, DATA_DIRECTORY, METADATA_FILE
 from .client_validation import validar_client, clientes_generar_txt
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_folder, period_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis, center_location, \
     CALENDAR_FECHA_FMT, ConsoleErrors, \
     generate_ajustes
 from .layout import make_layout, ActionButtonManager, TipoRecuperar, SearchOptions
 from .localdb import LocalDBSatCFDI, StatusState
 from .log_tools import cfdi_header, header_line, print_yaml
 from .mycfdi import MyCFDI
-from .utils import random_string, to_date_period, load_certificate, to_int, cert_info, add_month, to_uuid
+from .utils import random_string, to_date_period, load_certificate, to_int, cert_info, add_month, to_uuid, open_file
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
```

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/gui_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
 from satcfdi.pacs import sat
 from satcfdi.printer import Representable
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from weasyprint import HTML, CSS
 
-from tests.utils import open_file
 from . import SOURCE_DIRECTORY, ARCHIVOS_DIRECTORY, TEMP_DIRECTORY
 from .environments import facturacion_environment
 from .exceptions import ConsoleErrors
 from .formatting_functions.common import fecha_mes
-from .utils import add_month, find_best_match, months_between, clear_directory
+from .utils import add_month, find_best_match, months_between, clear_directory, open_file
 
 logger = logging.getLogger(__name__)
 logger.level = logging.INFO
 
 sat_manager = sat.SAT()
 
 PERIODICIDAD = {
```

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.2/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.2/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.2/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.2/satdigitalinvoice/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import random
 import shutil
+import subprocess
+import sys
 from datetime import datetime
 from uuid import UUID
 
 from satcfdi import Signer, DatePeriod
 from satcfdi.accounting.models import EstadoComprobante
 
 
@@ -119,7 +121,15 @@
 
 
 def to_datetime(s):
     try:
         return datetime.fromisoformat(s, )
     except ValueError:
         return None
+
+
+def open_file(filename):
+    if sys.platform == "win32":
+        os.startfile(filename)
+    else:
+        opener = "open" if sys.platform == "darwin" else "xdg-open"
+        subprocess.call([opener, filename])
```

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.1
+Version: 4.0.2
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.1/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.2/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/setup.py` & `satdigitalinvoice-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.2/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/tests/test_localdb.py` & `satdigitalinvoice-4.0.2/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.1/tests/test_main.py` & `satdigitalinvoice-4.0.2/tests/test_main.py`

 * *Files identical despite different names*

