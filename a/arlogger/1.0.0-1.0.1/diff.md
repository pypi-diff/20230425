# Comparing `tmp/arlogger-1.0.0-py3-none-any.whl.zip` & `tmp/arlogger-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3482 bytes, number of entries: 6
+Zip file size: 3466 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       99 b- defN 23-Jan-13 10:27 arlogger/__init__.py
--rw-rw-rw-  2.0 fat     4660 b- defN 23-Feb-27 12:20 arlogger/main.py
--rw-rw-rw-  2.0 fat     1397 b- defN 23-Apr-24 17:04 arlogger-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 17:04 arlogger-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-24 17:04 arlogger-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      449 b- defN 23-Apr-24 17:04 arlogger-1.0.0.dist-info/RECORD
-6 files, 6706 bytes uncompressed, 2668 bytes compressed:  60.2%
+-rw-rw-rw-  2.0 fat     4611 b- defN 23-Apr-25 06:20 arlogger/main.py
+-rw-rw-rw-  2.0 fat     1397 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      449 b- defN 23-Apr-25 06:32 arlogger-1.0.1.dist-info/RECORD
+6 files, 6657 bytes uncompressed, 2652 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: arlogger/__init__.py
 Comment: 
 
 Filename: arlogger/main.py
 Comment: 
 
-Filename: arlogger-1.0.0.dist-info/METADATA
+Filename: arlogger-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: arlogger-1.0.0.dist-info/WHEEL
+Filename: arlogger-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: arlogger-1.0.0.dist-info/top_level.txt
+Filename: arlogger-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: arlogger-1.0.0.dist-info/RECORD
+Filename: arlogger-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arlogger/main.py

```diff
@@ -23,24 +23,22 @@
         self.url = None
         self.projectName = None
         self.logger = None
         self.HTTPHandler = None
         self.localLogHandler = None
         self.localLogLevel = INFO
         self.HTTPLogLevel = ERROR
+        atexit.register(self.on_exit)
 
-    # same as __del__ 
+    # same as __del__
     def on_exit(self):
         self.logger.critical(self.projectName + " is crashed or exited.")
-    
-    def activateOnExit(self):
-        atexit.register(self.on_exit)
 
     def setLevel(self, httpLevel=None, localLevel=None):
-        
+
         if httpLevel is not None:
             self.HTTPLogLevel = httpLevel
             self.HTTPHandler.setLevel(self.HTTPLogLevel)
 
         if localLevel is not None:
             self.localLogLevel = localLevel
             self.localLogHandler.setLevel(self.localLogLevel)
@@ -49,39 +47,39 @@
 
     def setUrl(self, url, projectName):
         self.url = url
         self.projectName = projectName
 
         local_format = "%(levelname)s:%(asctime)s:%(name)s:%(message)s"
         http_format = logging.Formatter(json.dumps({
-                'projectname': projectName,
-                'pathname': '%(pathname)s',
-                'line': '%(lineno)d',
-                'levelname': '%(levelname)s',
-                'message': '%(message)s',
-                'func': '%(funcName)s',
+            'projectname': projectName,
+            'pathname': '%(pathname)s',
+            'line': '%(lineno)d',
+            'levelname': '%(levelname)s',
+            'message': '%(message)s',
+            'func': '%(funcName)s',
         }))
 
         os.mkdir("./logs") if not os.path.exists("./logs") else None
 
         self.localLogHandler = TimedRotatingFileHandler(filename="./logs/"+projectName+".log",
-                                                when="midnight",
-                                                backupCount=14
-                                                )
+                                                        when="midnight",
+                                                        backupCount=14
+                                                        )
 
         self.localLogHandler.rotator = self.__bzip_rotator__
         self.localLogHandler.namer = self.__bz2namer__
         self.localLogHandler.setFormatter(logging.Formatter(local_format))
 
         self.HTTPHandler = CustomHttpHandler(
             url=url
         )
         self.HTTPHandler.setLevel(self.HTTPLogLevel)
         self.HTTPHandler.setFormatter(http_format)
-        
+
         self.logger = logging.getLogger()
 
         self.logger.addHandler(self.localLogHandler)
         self.logger.addHandler(self.HTTPHandler)
 
         self.logger.setLevel(self.localLogLevel)
 
@@ -106,15 +104,14 @@
             if resp.status_code == 200:
                 os.remove(source)
 
     def __bz2namer__(self, name):
         return name + ".bz2"
 
 
-
 class CustomHttpHandler(logging.Handler):
     def __init__(self, url: str):
         self.url = url
         self.MAX_POOLSIZE = 100
         self.session = requests.Session()
         self.session.mount('', HTTPAdapter(
             max_retries=Retry(
@@ -125,24 +122,21 @@
             pool_connections=self.MAX_POOLSIZE,
             pool_maxsize=self.MAX_POOLSIZE
         ))
         super().__init__()
 
     def emit(self, record):
 
-        logEntry = json.loads(self.format(record).replace("\n", " ").replace("\\", "\\\\"))
+        logEntry = json.loads(self.format(record).replace(
+            "\n", " ").replace("\\", "\\\\"))
         now = datetime.now()
         dt_string = now.strftime("%d/%m/%Y %H:%M:%S.%f")
 
         logEntry["fields.time"] = dt_string
         logEntry["fields.levelname"] = logEntry["levelname"]
 
         urgent_log_url = self.url + "/log"
         self.session.headers = {'Content-Type': 'application/json'}
-        resp = self.session.post(urgent_log_url,json=logEntry)
+        resp = self.session.post(urgent_log_url, json=logEntry)
 
         if resp.status_code != 200:
             print("Error in sending log to server")
-
-
-
-
```

## Comparing `arlogger-1.0.0.dist-info/METADATA` & `arlogger-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlogger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Send urgent and daily log files to a remote server
 Home-page: https://bitbucket.org/asrturk/ar-ai-logger/src/master/
 Author: Mirza ATLI
 Author-email: mirza.atli@ardictech.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

