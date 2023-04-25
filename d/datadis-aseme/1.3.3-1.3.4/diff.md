# Comparing `tmp/datadis-aseme-1.3.3.tar.gz` & `tmp/datadis-aseme-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datadis-aseme-1.3.3.tar", last modified: Tue May 24 16:27:52 2022, max compression
+gzip compressed data, was "datadis-aseme-1.3.4.tar", last modified: Tue Apr 25 10:59:53 2023, max compression
```

## Comparing `datadis-aseme-1.3.3.tar` & `datadis-aseme-1.3.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/
--rw-rw-r--   0 david     (1000) david     (1000)      723 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/setup.py
--rw-rw-r--   0 david     (1000) david     (1000)        8 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/requirements.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis/
--rw-rw-r--   0 david     (1000) david     (1000)     9839 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/webservice.py
--rw-rw-r--   0 david     (1000) david     (1000)     5273 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/validators.py
--rw-rw-r--   0 david     (1000) david     (1000)     4373 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/adaptors.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis/templates/
--rw-rw-r--   0 david     (1000) david     (1000)      440 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/templates/codigos_error.error
--rw-rw-r--   0 david     (1000) david     (1000)      532 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/templates/contrato.json
--rw-rw-r--   0 david     (1000) david     (1000)       35 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/templates/maximaspotencia.json
--rw-rw-r--   0 david     (1000) david     (1000)      125 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/templates/autoconsumo.json
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis/data/
--rw-rw-r--   0 david     (1000) david     (1000)   216244 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/datadis/data/20codmun.csv
--rw-rw-r--   0 david     (1000) david     (1000)       75 2022-05-24 16:22:06.000000 datadis-aseme-1.3.3/datadis/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1231 2021-11-17 14:40:03.000000 datadis-aseme-1.3.3/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis_aseme.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)        8 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis_aseme.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)        9 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis_aseme.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis_aseme.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      485 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis_aseme.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)     1926 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/datadis_aseme.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      119 2022-05-24 16:21:51.000000 datadis-aseme-1.3.3/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1926 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)       38 2022-05-24 16:27:52.000000 datadis-aseme-1.3.3/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/
+-rw-rw-r--   0 david     (1000) david     (1000)     1516 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1549 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1231 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis/
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-04-25 10:55:31.000000 datadis-aseme-1.3.4/datadis/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4373 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/adaptors.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis/data/
+-rw-rw-r--   0 david     (1000) david     (1000)   216244 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/data/20codmun.csv
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis/templates/
+-rw-rw-r--   0 david     (1000) david     (1000)      125 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/autoconsumo.json
+-rw-rw-r--   0 david     (1000) david     (1000)      440 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/codigos_error.error
+-rw-rw-r--   0 david     (1000) david     (1000)      532 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/contrato.json
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/maximaspotencia.json
+-rw-rw-r--   0 david     (1000) david     (1000)     5273 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/validators.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9839 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/webservice.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis_aseme.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1549 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      493 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        9 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)      841 2023-04-25 10:55:20.000000 datadis-aseme-1.3.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datadis-aseme-1.3.3/setup.py` & `datadis-aseme-1.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 from datadis import __version__, __author__
 
+PACKAGES_DATA = {'datadis': ['data/*.csv', 'templates/*.json', 'templates/*.error']}
+
 with open('requirements.txt', 'r') as f:
     requirements = f.readlines()
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='datadis-aseme',
     version=__version__,
     description="Herramienta gestión API ASEME DATADIS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     provides=['datadis'],
     packages=find_packages(),
+    package_data=PACKAGES_DATA,
     install_requires=requirements,
     license='BSD 3-Clause License',
     author=__author__,
     author_email='devel@gisce.net',
     url = 'https://github.com/gisce/datadis-aseme',
 )
```

### Comparing `datadis-aseme-1.3.3/datadis/webservice.py` & `datadis-aseme-1.3.4/datadis/webservice.py`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.3/datadis/validators.py` & `datadis-aseme-1.3.4/datadis/validators.py`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.3/datadis/adaptors.py` & `datadis-aseme-1.3.4/datadis/adaptors.py`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.3/datadis/templates/contrato.json` & `datadis-aseme-1.3.4/datadis/templates/contrato.json`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.3/datadis/data/20codmun.csv` & `datadis-aseme-1.3.4/datadis/data/20codmun.csv`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.3/README.md` & `datadis-aseme-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.3/datadis_aseme.egg-info/PKG-INFO` & `datadis-aseme-1.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: datadis-aseme
-Version: 1.3.3
+Version: 1.3.4
 Summary: Herramienta gestión API ASEME DATADIS
 Home-page: https://github.com/gisce/datadis-aseme
 Author: Francesc Puig
 Author-email: devel@gisce.net
 License: BSD 3-Clause License
-Description: ## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
-        - Publicación de datos de distribuidora al sistema DATADIS
-        - Gestión de peticiones
-        
-        
-        ### Informaciones de:
-        
-        - Contrato
-        - Máximas potencia
-        - AUtoconsumo
-        
-        
-        ### Fácil de utilizar
-        
-        ```python
-        from datadis.webservice import DatadisWebServiceController
-        controller = DatadisWebserviceController()
-        controller.autenticar(usuario, password)
-        controller.contrato.__doc__
-        >>>
-        Publicar contrato al sistema DATADIS.
-                Si el contrato ya existe en el sistema, se modificara
-                Enviar un diccionario con las claves requeridas indicadas a continuacion
-                data: {
-                    "nif": "",
-                    "nombre": "",
-                    "comercializadora": "",
-                    "tensionConexion": "",
-                    "tarifaAcceso": "",
-                    "discriminacionHoraria": "",
-                    "tipoPunto": "",
-                    "modoControlPotencia": "",
-                    "fechaInicioContrato": "",
-                    "cups": "",
-                    "distribuidora": "",
-                    "codigoPostal": "",
-                    "provincia": "",
-                    "municipio": ""
-                }
-                method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
-        
-        >>>
-        respuesta = controller.contrato(data)
-        ```
-        
-        
-        
-Platform: UNKNOWN
 Provides: datadis
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
+- Publicación de datos de distribuidora al sistema DATADIS
+- Gestión de peticiones
+
+
+### Informaciones de:
+
+- Contrato
+- Máximas potencia
+- AUtoconsumo
+
+
+### Fácil de utilizar
+
+```python
+from datadis.webservice import DatadisWebServiceController
+controller = DatadisWebserviceController()
+controller.autenticar(usuario, password)
+controller.contrato.__doc__
+>>>
+Publicar contrato al sistema DATADIS.
+        Si el contrato ya existe en el sistema, se modificara
+        Enviar un diccionario con las claves requeridas indicadas a continuacion
+        data: {
+            "nif": "",
+            "nombre": "",
+            "comercializadora": "",
+            "tensionConexion": "",
+            "tarifaAcceso": "",
+            "discriminacionHoraria": "",
+            "tipoPunto": "",
+            "modoControlPotencia": "",
+            "fechaInicioContrato": "",
+            "cups": "",
+            "distribuidora": "",
+            "codigoPostal": "",
+            "provincia": "",
+            "municipio": ""
+        }
+        method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
+
+>>>
+respuesta = controller.contrato(data)
+```
+
+
```

### Comparing `datadis-aseme-1.3.3/PKG-INFO` & `datadis-aseme-1.3.4/datadis_aseme.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: datadis-aseme
-Version: 1.3.3
+Version: 1.3.4
 Summary: Herramienta gestión API ASEME DATADIS
 Home-page: https://github.com/gisce/datadis-aseme
 Author: Francesc Puig
 Author-email: devel@gisce.net
 License: BSD 3-Clause License
-Description: ## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
-        - Publicación de datos de distribuidora al sistema DATADIS
-        - Gestión de peticiones
-        
-        
-        ### Informaciones de:
-        
-        - Contrato
-        - Máximas potencia
-        - AUtoconsumo
-        
-        
-        ### Fácil de utilizar
-        
-        ```python
-        from datadis.webservice import DatadisWebServiceController
-        controller = DatadisWebserviceController()
-        controller.autenticar(usuario, password)
-        controller.contrato.__doc__
-        >>>
-        Publicar contrato al sistema DATADIS.
-                Si el contrato ya existe en el sistema, se modificara
-                Enviar un diccionario con las claves requeridas indicadas a continuacion
-                data: {
-                    "nif": "",
-                    "nombre": "",
-                    "comercializadora": "",
-                    "tensionConexion": "",
-                    "tarifaAcceso": "",
-                    "discriminacionHoraria": "",
-                    "tipoPunto": "",
-                    "modoControlPotencia": "",
-                    "fechaInicioContrato": "",
-                    "cups": "",
-                    "distribuidora": "",
-                    "codigoPostal": "",
-                    "provincia": "",
-                    "municipio": ""
-                }
-                method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
-        
-        >>>
-        respuesta = controller.contrato(data)
-        ```
-        
-        
-        
-Platform: UNKNOWN
 Provides: datadis
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
+- Publicación de datos de distribuidora al sistema DATADIS
+- Gestión de peticiones
+
+
+### Informaciones de:
+
+- Contrato
+- Máximas potencia
+- AUtoconsumo
+
+
+### Fácil de utilizar
+
+```python
+from datadis.webservice import DatadisWebServiceController
+controller = DatadisWebserviceController()
+controller.autenticar(usuario, password)
+controller.contrato.__doc__
+>>>
+Publicar contrato al sistema DATADIS.
+        Si el contrato ya existe en el sistema, se modificara
+        Enviar un diccionario con las claves requeridas indicadas a continuacion
+        data: {
+            "nif": "",
+            "nombre": "",
+            "comercializadora": "",
+            "tensionConexion": "",
+            "tarifaAcceso": "",
+            "discriminacionHoraria": "",
+            "tipoPunto": "",
+            "modoControlPotencia": "",
+            "fechaInicioContrato": "",
+            "cups": "",
+            "distribuidora": "",
+            "codigoPostal": "",
+            "provincia": "",
+            "municipio": ""
+        }
+        method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
+
+>>>
+respuesta = controller.contrato(data)
+```
+
+
```

