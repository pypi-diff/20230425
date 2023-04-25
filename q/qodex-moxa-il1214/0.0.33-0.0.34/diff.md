# Comparing `tmp/qodex_moxa_il1214-0.0.33-py3-none-any.whl.zip` & `tmp/qodex_moxa_il1214-0.0.34-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2301 bytes, number of entries: 6
+Zip file size: 2239 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 12:26 moxa_contr/__init__.py
--rw-rw-rw-  2.0 fat     3042 b- defN 23-Apr-20 10:45 moxa_contr/main.py
--rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-20 10:46 qodex_moxa_il1214-0.0.33.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:46 qodex_moxa_il1214-0.0.33.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 10:46 qodex_moxa_il1214-0.0.33.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      492 b- defN 23-Apr-20 10:46 qodex_moxa_il1214-0.0.33.dist-info/RECORD
-6 files, 3824 bytes uncompressed, 1399 bytes compressed:  63.4%
+-rw-rw-rw-  2.0 fat     2675 b- defN 23-Apr-25 06:29 moxa_contr/main.py
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-25 06:30 qodex_moxa_il1214-0.0.34.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 06:30 qodex_moxa_il1214-0.0.34.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-25 06:30 qodex_moxa_il1214-0.0.34.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      492 b- defN 23-Apr-25 06:30 qodex_moxa_il1214-0.0.34.dist-info/RECORD
+6 files, 3457 bytes uncompressed, 1337 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: moxa_contr/__init__.py
 Comment: 
 
 Filename: moxa_contr/main.py
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.33.dist-info/METADATA
+Filename: qodex_moxa_il1214-0.0.34.dist-info/METADATA
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.33.dist-info/WHEEL
+Filename: qodex_moxa_il1214-0.0.34.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.33.dist-info/top_level.txt
+Filename: qodex_moxa_il1214-0.0.34.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_moxa_il1214-0.0.33.dist-info/RECORD
+Filename: qodex_moxa_il1214-0.0.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moxa_contr/main.py

```diff
@@ -7,17 +7,15 @@
     schema = "http://"
     api_io = f"/api/slot/0/io"
     api_io_di = f"/api/slot/0/io/di"
     headers = {
         "Content-Type": "application/json",
         "Accept": "vdn.dac.v1"
     }
-
-    def __init__(self, ip):
-        self.ip = ip
+    ip = None
 
     def get_info(self, route):
         return requests.get(url=f"{self.schema}{self.ip}{route}",
                             headers=self.headers)
 
     def put_info(self, route, data=None):
         data = json.dumps(data)
@@ -41,22 +39,14 @@
 
 class MoxaDevice(MoxaServer):
     index = None
     ip = None
     status_on = 1
     status_off = 0
 
-    def __init__(self, ip, index, status_on=1, status_off=0):
-        super().__init__(ip=ip)
-        self.index = index
-        self.status_on = status_on
-        self.status_off = status_off
-        self.api_relay = f"{MoxaServer.api_io}/relay/{index}"
-        self.relay_status_link = f"{self.api_relay}/relayStatus"
-
     def set_relay_link(self, index):
         self.api_relay = f"{MoxaServer.api_io}/relay/{index}"
         self.relay_status_link = f"{self.api_relay}/relayStatus"
 
     def get_relay_info(self):
         return self.get_info(self.relay_status_link)
```

