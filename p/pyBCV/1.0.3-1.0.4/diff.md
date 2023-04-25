# Comparing `tmp/pyBCV-1.0.3-py3-none-any.whl.zip` & `tmp/pyBCV-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4579 bytes, number of entries: 7
+Zip file size: 4894 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-02 04:16 pyBCV/__init__.py
--rw-rw-rw-  2.0 fat     3527 b- defN 23-Apr-19 18:41 pyBCV/pyBCV.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4473 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      518 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/RECORD
-7 files, 9735 bytes uncompressed, 3665 bytes compressed:  62.4%
+-rw-rw-rw-  2.0 fat     4453 b- defN 23-Apr-25 00:04 pyBCV/pyBCV.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-25 00:34 pyBCV-1.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4493 b- defN 23-Apr-25 00:34 pyBCV-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 00:34 pyBCV-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-25 00:34 pyBCV-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      518 b- defN 23-Apr-25 00:34 pyBCV-1.0.4.dist-info/RECORD
+7 files, 10681 bytes uncompressed, 3980 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyBCV/__init__.py
 Comment: 
 
 Filename: pyBCV/pyBCV.py
 Comment: 
 
-Filename: pyBCV-1.0.3.dist-info/LICENSE
+Filename: pyBCV-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: pyBCV-1.0.3.dist-info/METADATA
+Filename: pyBCV-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pyBCV-1.0.3.dist-info/WHEEL
+Filename: pyBCV-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyBCV-1.0.3.dist-info/top_level.txt
+Filename: pyBCV-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBCV-1.0.3.dist-info/RECORD
+Filename: pyBCV-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBCV/pyBCV.py

```diff
@@ -2,15 +2,29 @@
 
 import requests
 from bs4 import BeautifulSoup
 
 requests.packages.urllib3.disable_warnings()
 
 class Currency:
+    """
+    `pyBCV.Currency()`. Es la instancia principal para obtener los datos de tipo de cambio del BCV.\n
+    https://github.com/fcoagz/pyBCV#uso
+
+    ```py
+    import pyBCV
+
+    bcv = pyBCV.Currency()
+    bcv.get_rate(currency_code='USD')
+    ```
+    """
     def get_rate(self, currency_code=None) -> dict[str, str] | str:
+        """
+        El módulo `get_rate()` acepta un código de moneda como argumento y devuelve la tasa de cambio actual de esa moneda.
+        """
         response = requests.get('https://www.bcv.org.ve/', verify=False)
 
         if response.status_code == requests.codes.ok:
             soup = BeautifulSoup(response.content, 'html.parser')
 
             rates_of_cambie = []
             date_valid = []
@@ -32,15 +46,29 @@
             if not currency_code:
                 return rates
             
             elif currency_code in rates:
                 return rates[currency_code]
     
 class Bank:
+    """
+    `pyBCV.Bank()`. Es la segunda instancia para obtener los datos del sistema bancario del BCV.\n
+    https://github.com/fcoagz/pyBCV#uso
+
+    ```py
+    import pyBCV
+
+    bcv = pyBCV.Bank()
+    bcv.get_by_bank(bank_code='Banesco', rate_or_sale='Compra')
+    ```
+    """
     def get_by_bank(self, bank_code=None, rate_or_sale=None) -> dict[Any, dict[str, str]] | str | dict[str, str]:
+        """
+        El módulo `get_by_bank()` acepta el nombre de un banco como argumento y devuelve la fecha vigente y el sistema cambiario de compra y venta de moneda extranjera para ese banco.
+        """
         response = requests.get('https://www.bcv.org.ve/tasas-informativas-sistema-bancario', verify=False)
 
         if response.status_code == requests.codes.ok:
             soup = BeautifulSoup(response.content, 'html.parser')
 
             date_indicator = []
             title_bank = []
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pyBCV-1.0.3.dist-info/LICENSE` & `pyBCV-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBCV-1.0.3.dist-info/METADATA` & `pyBCV-1.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBCV
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).
 Home-page: https://github.com/fcoagz/pyBCV
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pyBCV
 Project-URL: Bug Tracker, https://github.com/fcoagz/pyBCV/issues
@@ -25,19 +25,19 @@
 
 # pyBCV
 PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y la tasas informativas del sistema bancario proporcionados por el Banco Central de Venezuela (BCV). Esta librería se centra específicamente en la obtención de los datos de tipos de cambio y las tasas informativas del BCV y los convierte en un formato fácilmente utilizable en Python.
 
 ## Instalación
 Para instalar esta librería, puedes utilizar el siguiente comando de pip:
 ```py
-pip install pyBCV
+pip install --upgrade pyBCV
 ```
 Si usas un Sistema Operativo como Linux o Mac:
 ```py
-pip3 install pyBCV
+pip3 install --upgrade pyBCV
 ```
 
 ## Uso
 Para obtener información del BCV, creamos una instancia de la clase `Currency` o `Bank` y elegimos el módulo que deseamos utilizar para obtener la información. En pyBCV, los módulos disponibles son:
 
 - Currency().get_rate(): Obtiene la tasa de cambio actual de una moneda específica.
 - Bank().get_by_bank(): Obtiene la fecha vigente y el sistema cambiario de compra y venta de moneda extranjera para un banco específico.
```

## Comparing `pyBCV-1.0.3.dist-info/RECORD` & `pyBCV-1.0.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pyBCV/__init__.py,sha256=SZ6EoGVEUueFJA0MDTWGqgeobENhu1fFFDiZwIY8Mns,25
-pyBCV/pyBCV.py,sha256=w02nubZVcI8MT9iPjlkhdrpxdhgzLJCjHORW6cXk4sw,3527
-pyBCV-1.0.3.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
-pyBCV-1.0.3.dist-info/METADATA,sha256=oQql2IuRJtNg9Mn5CnZ5TCZTIZd-8kJnBYJF85yThrc,4473
-pyBCV-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyBCV-1.0.3.dist-info/top_level.txt,sha256=lmSpnf39p5nhU1AD7bYr8VERsutkAjoN25gojXaQh90,6
-pyBCV-1.0.3.dist-info/RECORD,,
+pyBCV/pyBCV.py,sha256=KSK_q-we-DYvba6D9hUZAJj3KsRFdIjUIpeoIVKpMRU,4453
+pyBCV-1.0.4.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
+pyBCV-1.0.4.dist-info/METADATA,sha256=ihJ3UDWh7Bu8L0_WbJsmJdese0V6hxwImAt6-pxMDmQ,4493
+pyBCV-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyBCV-1.0.4.dist-info/top_level.txt,sha256=lmSpnf39p5nhU1AD7bYr8VERsutkAjoN25gojXaQh90,6
+pyBCV-1.0.4.dist-info/RECORD,,
```

