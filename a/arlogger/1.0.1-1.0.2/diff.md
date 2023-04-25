# Comparing `tmp/arlogger-1.0.1-py3-none-any.whl.zip` & `tmp/arlogger-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3466 bytes, number of entries: 6
+Zip file size: 3474 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       99 b- defN 23-Jan-13 10:27 arlogger/__init__.py
--rw-rw-rw-  2.0 fat     4611 b- defN 23-Apr-25 06:20 arlogger/main.py
--rw-rw-rw-  2.0 fat     1397 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      449 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/RECORD
-6 files, 6657 bytes uncompressed, 2652 bytes compressed:  60.2%
+-rw-rw-rw-  2.0 fat     4681 b- defN 23-Apr-25 12:24 arlogger/main.py
+-rw-rw-rw-  2.0 fat     1397 b- defN 23-Apr-25 12:25 arlogger-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 12:25 arlogger-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-25 12:25 arlogger-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      449 b- defN 23-Apr-25 12:25 arlogger-1.0.2.dist-info/RECORD
+6 files, 6727 bytes uncompressed, 2660 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: arlogger/__init__.py
 Comment: 
 
 Filename: arlogger/main.py
 Comment: 
 
-Filename: arlogger-1.0.1.dist-info/METADATA
+Filename: arlogger-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: arlogger-1.0.1.dist-info/WHEEL
+Filename: arlogger-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: arlogger-1.0.1.dist-info/top_level.txt
+Filename: arlogger-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: arlogger-1.0.1.dist-info/RECORD
+Filename: arlogger-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arlogger/main.py

```diff
@@ -15,23 +15,24 @@
 INFO = logging.INFO
 WARNING = logging.WARNING
 ERROR = logging.ERROR
 CRITICAL = logging.CRITICAL
 
 
 class ArLogger():
-    def __init__(self):
+    def __init__(self, logAtExit=True):
         self.url = None
         self.projectName = None
         self.logger = None
         self.HTTPHandler = None
         self.localLogHandler = None
         self.localLogLevel = INFO
         self.HTTPLogLevel = ERROR
-        atexit.register(self.on_exit)
+        if logAtExit:
+            atexit.register(self.on_exit)
 
     # same as __del__
     def on_exit(self):
         self.logger.critical(self.projectName + " is crashed or exited.")
 
     def setLevel(self, httpLevel=None, localLevel=None):
 
@@ -122,19 +123,21 @@
             pool_connections=self.MAX_POOLSIZE,
             pool_maxsize=self.MAX_POOLSIZE
         ))
         super().__init__()
 
     def emit(self, record):
 
-        logEntry = json.loads(self.format(record).replace(
-            "\n", " ").replace("\\", "\\\\"))
+        logEntry = record.__dict__
+
         now = datetime.now()
         dt_string = now.strftime("%d/%m/%Y %H:%M:%S.%f")
 
+        logEntry["func"] = logEntry["funcName"]
+        logEntry["line"] = logEntry["lineno"]
         logEntry["fields.time"] = dt_string
         logEntry["fields.levelname"] = logEntry["levelname"]
 
         urgent_log_url = self.url + "/log"
         self.session.headers = {'Content-Type': 'application/json'}
         resp = self.session.post(urgent_log_url, json=logEntry)
```

## Comparing `arlogger-1.0.1.dist-info/METADATA` & `arlogger-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlogger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Send urgent and daily log files to a remote server
 Home-page: https://bitbucket.org/asrturk/ar-ai-logger/src/master/
 Author: Mirza ATLI
 Author-email: mirza.atli@ardictech.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

