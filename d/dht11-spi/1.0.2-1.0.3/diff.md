# Comparing `tmp/dht11_spi-1.0.2.tar.gz` & `tmp/dht11_spi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dht11_spi-1.0.2.tar", last modified: Sat Mar  4 04:46:19 2023, max compression
+gzip compressed data, was "dht11_spi-1.0.3.tar", last modified: Tue Apr 25 06:16:09 2023, max compression
```

## Comparing `dht11_spi-1.0.2.tar` & `dht11_spi-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-04 04:46:18.988828 dht11_spi-1.0.2/
--rw-r--r--   0 pi        (1000) pi        (1000)     1069 2023-02-12 05:05:14.000000 dht11_spi-1.0.2/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     4454 2023-03-04 04:46:18.988828 dht11_spi-1.0.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3660 2023-02-12 05:50:46.000000 dht11_spi-1.0.2/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-04 04:46:18.988828 dht11_spi-1.0.2/dht11_spi/
--rw-r--r--   0 pi        (1000) pi        (1000)    15977 2023-02-12 05:41:46.000000 dht11_spi-1.0.2/dht11_spi/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9725 2023-03-04 03:56:03.000000 dht11_spi-1.0.2/dht11_spi/__main__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-04 04:46:18.988828 dht11_spi-1.0.2/dht11_spi.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     4454 2023-03-04 04:46:18.000000 dht11_spi-1.0.2/dht11_spi.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      240 2023-03-04 04:46:18.000000 dht11_spi-1.0.2/dht11_spi.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-03-04 04:46:18.000000 dht11_spi-1.0.2/dht11_spi.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       35 2023-03-04 04:46:18.000000 dht11_spi-1.0.2/dht11_spi.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       10 2023-03-04 04:46:18.000000 dht11_spi-1.0.2/dht11_spi.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      933 2023-03-04 04:45:28.000000 dht11_spi-1.0.2/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-03-04 04:46:18.988828 dht11_spi-1.0.2/setup.cfg
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-25 06:16:09.109564 dht11_spi-1.0.3/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-04-25 06:12:39.000000 dht11_spi-1.0.3/LICENSE
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4454 2023-04-25 06:16:09.109564 dht11_spi-1.0.3/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3660 2023-04-25 06:12:39.000000 dht11_spi-1.0.3/README.md
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-25 06:16:09.109564 dht11_spi-1.0.3/dht11_spi/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    16104 2023-04-25 06:14:40.000000 dht11_spi-1.0.3/dht11_spi/__init__.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     9725 2023-04-25 06:12:39.000000 dht11_spi-1.0.3/dht11_spi/__main__.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-25 06:16:09.109564 dht11_spi-1.0.3/dht11_spi.egg-info/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4454 2023-04-25 06:16:09.000000 dht11_spi-1.0.3/dht11_spi.egg-info/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      240 2023-04-25 06:16:09.000000 dht11_spi-1.0.3/dht11_spi.egg-info/SOURCES.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-04-25 06:16:09.000000 dht11_spi-1.0.3/dht11_spi.egg-info/dependency_links.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       35 2023-04-25 06:16:09.000000 dht11_spi-1.0.3/dht11_spi.egg-info/requires.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       10 2023-04-25 06:16:09.000000 dht11_spi-1.0.3/dht11_spi.egg-info/top_level.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      933 2023-04-25 06:15:13.000000 dht11_spi-1.0.3/pyproject.toml
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-04-25 06:16:09.109564 dht11_spi-1.0.3/setup.cfg
```

### Comparing `dht11_spi-1.0.2/LICENSE` & `dht11_spi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dht11_spi-1.0.2/PKG-INFO` & `dht11_spi-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dht11_spi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module to use the SPI bus to read DHT11/DHT22 sensors.
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/dht11_spi/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/dht11_spi/issues
 Project-URL: Source Code, https://github.com/LearningToPi/dht11_spi
 Keywords: dht11,dht22,spi
 Classifier: Topic :: System :: Logging
```

### Comparing `dht11_spi-1.0.2/README.md` & `dht11_spi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dht11_spi-1.0.2/dht11_spi/__init__.py` & `dht11_spi-1.0.3/dht11_spi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,17 @@
 DHT_INIT_SIGNAL_MS   = 20
 
 DHT_SIG_0 = (20, 28)
 DHT_SIG_LOW = (46, 56)
 DHT_SIG_1 = (66, 74)
 DHT_SIG_START = (76,90)
 
+DHT11_MIN_INTERVAL = 1
+DHT22_MIN_INTERVAL = 2
+
 BIT_VALS = (128, 64, 32, 16, 8, 4, 2, 1)
 
 class DHT11_Exception(Exception):
     pass
 
 # Attempt import of different gpio libraries
 try:
@@ -150,14 +153,15 @@
         self.spi_clock_us = 1 / self.spi_bus_hz * 1_000_000
         self.init_ms = DHT_INIT_SIGNAL_MS
         self._data = []
         self._bit_counts = []
         self._binary_data = []
         self.discard_count = 0
         self.dht22 = dht22
+        self.min_interval = DHT22_MIN_INTERVAL if dht22 else DHT11_MIN_INTERVAL
         
         self._read_lock = Lock()
         self._log_extra = f"SPI{spiBus}-{self.spi_bus_hz/1000}kHz"
         self._logger = logger if logger is not None else logging_handler.create_logger('DEBUG' if DEBUG else 'INFO', name=__name__)
         self._logger.info(f"{self.info_str}: Opening")
         self._spi = spidev.SpiDev()
         self._spi.open(spiBus, 0)
```

### Comparing `dht11_spi-1.0.2/dht11_spi/__main__.py` & `dht11_spi-1.0.3/dht11_spi/__main__.py`

 * *Files identical despite different names*

### Comparing `dht11_spi-1.0.2/dht11_spi.egg-info/PKG-INFO` & `dht11_spi-1.0.3/dht11_spi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dht11-spi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python module to use the SPI bus to read DHT11/DHT22 sensors.
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/dht11_spi/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/dht11_spi/issues
 Project-URL: Source Code, https://github.com/LearningToPi/dht11_spi
 Keywords: dht11,dht22,spi
 Classifier: Topic :: System :: Logging
```

### Comparing `dht11_spi-1.0.2/pyproject.toml` & `dht11_spi-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dht11_spi"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python module to use the SPI bus to read DHT11/DHT22 sensors."
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
 keywords = ["dht11", "dht22", "spi"]
 readme = "README.md"
 requires-python =">=3.6"
 classifiers = [
     "Topic :: System :: Logging",
```

