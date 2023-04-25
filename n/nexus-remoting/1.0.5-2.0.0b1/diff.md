# Comparing `tmp/nexus_remoting-1.0.5-py3-none-any.whl.zip` & `tmp/nexus_remoting-2.0.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6611 bytes, number of entries: 7
--rw-r--r--  2.0 unx       24 b- defN 22-Dec-08 10:16 nexus_remoting/__init__.py
--rw-r--r--  2.0 unx     7346 b- defN 22-Dec-08 10:16 nexus_remoting/_encoder.py
--rw-r--r--  2.0 unx     9630 b- defN 22-Dec-08 10:16 nexus_remoting/_remoting.py
--rw-r--r--  2.0 unx      938 b- defN 22-Dec-08 10:17 nexus_remoting-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-08 10:17 nexus_remoting-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 22-Dec-08 10:17 nexus_remoting-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      573 b- defN 22-Dec-08 10:17 nexus_remoting-1.0.5.dist-info/RECORD
-7 files, 18618 bytes uncompressed, 5587 bytes compressed:  70.0%
+Zip file size: 6630 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       24 b- defN 23-Apr-25 11:02 nexus_remoting/__init__.py
+-rw-r--r--  2.0 unx     7346 b- defN 23-Apr-25 11:02 nexus_remoting/_encoder.py
+-rw-r--r--  2.0 unx     9630 b- defN 23-Apr-25 11:02 nexus_remoting/_remoting.py
+-rw-r--r--  2.0 unx      942 b- defN 23-Apr-25 11:03 nexus_remoting-2.0.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 11:03 nexus_remoting-2.0.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-25 11:03 nexus_remoting-2.0.0b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      581 b- defN 23-Apr-25 11:03 nexus_remoting-2.0.0b1.dist-info/RECORD
+7 files, 18630 bytes uncompressed, 5590 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: nexus_remoting/_encoder.py
 Comment: 
 
 Filename: nexus_remoting/_remoting.py
 Comment: 
 
-Filename: nexus_remoting-1.0.5.dist-info/METADATA
+Filename: nexus_remoting-2.0.0b1.dist-info/METADATA
 Comment: 
 
-Filename: nexus_remoting-1.0.5.dist-info/WHEEL
+Filename: nexus_remoting-2.0.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: nexus_remoting-1.0.5.dist-info/top_level.txt
+Filename: nexus_remoting-2.0.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: nexus_remoting-1.0.5.dist-info/RECORD
+Filename: nexus_remoting-2.0.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nexus_remoting-1.0.5.dist-info/METADATA` & `nexus_remoting-2.0.0b1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nexus-remoting
-Version: 1.0.5
+Version: 2.0.0b1
 Summary: This package contains types to easily implement a Nexus.Sources.Remote client for the Nexus software (a GUI for time-series data lakes).
 Home-page: https://github.com/malstroem-labs/nexus-sources-remote
 Author: https://github.com/malstroem-labs
 License: MIT
 Project-URL: Project, https://malstroem-labs.github.io/Nexus
 Project-URL: Repository, https://github.com/malstroem-labs/nexus-sources-remote
 Keywords: Nexus time-series data lake remoting
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: nexus-extensibility (>=1.0.0)
+Requires-Dist: nexus-extensibility (>=2.0.0b8)
 
 # nexus-remoting
 
 This package contains types to easily implement a Nexus.Sources.Remote client for the Nexus software (a GUI for time-series data lakes).
```

