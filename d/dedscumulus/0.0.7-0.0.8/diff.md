# Comparing `tmp/dedscumulus-0.0.7-py3-none-any.whl.zip` & `tmp/dedscumulus-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 24256 bytes, number of entries: 21
+Zip file size: 24325 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      465 b- defN 23-Apr-21 13:58 dedscumulus/RequestHandler.py
 -rw-rw-rw-  2.0 fat    14421 b- defN 23-Apr-21 13:58 dedscumulus/SharePointHandler.py
 -rw-rw-rw-  2.0 fat     2250 b- defN 23-Feb-20 20:06 dedscumulus/TableLogHandler.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-May-17 10:12 dedscumulus/__init__.py
 -rw-rw-rw-  2.0 fat     8815 b- defN 23-Feb-21 02:51 dedscumulus/brzGlobal.py
--rw-rw-rw-  2.0 fat     4990 b- defN 23-Apr-18 16:46 dedscumulus/gbtGlobal.py
+-rw-rw-rw-  2.0 fat     5689 b- defN 23-Apr-25 11:57 dedscumulus/gbtGlobal.py
 -rw-rw-rw-  2.0 fat    13475 b- defN 23-Apr-21 13:57 dedscumulus/mstAst.py
 -rw-rw-rw-  2.0 fat      824 b- defN 23-Apr-21 13:55 dedscumulus/mstLog.py
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Feb-13 21:12 src/RequestHandler.py
 -rw-rw-rw-  2.0 fat    14421 b- defN 23-Feb-13 13:17 src/SharePointHandler.py
 -rw-rw-rw-  2.0 fat     2250 b- defN 23-Feb-20 20:06 src/TableLogHandler.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-May-17 10:12 src/__init__.py
 -rw-rw-rw-  2.0 fat     8815 b- defN 23-Feb-21 02:51 src/brzGlobal.py
 -rw-rw-rw-  2.0 fat     4990 b- defN 23-Apr-18 16:46 src/gbtGlobal.py
 -rw-rw-rw-  2.0 fat    13474 b- defN 23-Apr-16 12:34 src/mstAst.py
 -rw-rw-rw-  2.0 fat      823 b- defN 23-Apr-20 21:56 src/mstLog.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-21 13:59 dedscumulus-0.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      566 b- defN 23-Apr-21 13:59 dedscumulus-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 13:59 dedscumulus-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-21 13:59 dedscumulus-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1655 b- defN 23-Apr-21 13:59 dedscumulus-0.0.7.dist-info/RECORD
-21 files, 93951 bytes uncompressed, 21592 bytes compressed:  77.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-25 12:13 dedscumulus-0.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      566 b- defN 23-Apr-25 12:13 dedscumulus-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 12:13 dedscumulus-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-25 12:13 dedscumulus-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1655 b- defN 23-Apr-25 12:13 dedscumulus-0.0.8.dist-info/RECORD
+21 files, 94650 bytes uncompressed, 21661 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: src/mstAst.py
 Comment: 
 
 Filename: src/mstLog.py
 Comment: 
 
-Filename: dedscumulus-0.0.7.dist-info/LICENSE
+Filename: dedscumulus-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: dedscumulus-0.0.7.dist-info/METADATA
+Filename: dedscumulus-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: dedscumulus-0.0.7.dist-info/WHEEL
+Filename: dedscumulus-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: dedscumulus-0.0.7.dist-info/top_level.txt
+Filename: dedscumulus-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: dedscumulus-0.0.7.dist-info/RECORD
+Filename: dedscumulus-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dedscumulus/gbtGlobal.py

```diff
@@ -84,8 +84,23 @@
             tries+=1
             LOGGER.debug(f"WARNING: list_tasks from Breeze not received, try {tries}, error: "+str(ge))
             if tries==3:
                 if  "Read timed out" in str(ge):
                     LOGGER.warning(f"WARNING: list_tasks from Breeze timed out. Full error: "+str(ge))
                 else:
                     LOGGER.warning(f"WARNING: list_tasks from Breeze not received, error: "+str(ge))
+                return None
+            
+def getTaskCategories(greenbyte_client,LOGGER):
+    tries=0
+    while tries<3:
+        try:
+            return greenbyte_client.plan.list_task_categories()
+        except Exception as ge:
+            tries+=1
+            LOGGER.debug(f"WARNING: list_task_categories from Breeze not received, try {tries}, error: "+str(ge))
+            if tries==3:
+                if  "Read timed out" in str(ge):
+                    LOGGER.warning(f"WARNING: list_task_categories from Breeze timed out. Full error: "+str(ge))
+                else:
+                    LOGGER.warning(f"WARNING: list_task_categories from Breeze not received, error: "+str(ge))
                 return None
```

## Comparing `dedscumulus-0.0.7.dist-info/LICENSE` & `dedscumulus-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dedscumulus-0.0.7.dist-info/METADATA` & `dedscumulus-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.0.7
+Version: 0.0.8
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 License: UNKNOWN
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Platform: UNKNOWN
```

## Comparing `dedscumulus-0.0.7.dist-info/RECORD` & `dedscumulus-0.0.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 dedscumulus/RequestHandler.py,sha256=1pC4NGey-fk3ICRk3IjDr5jod8mbf2DuVhG43C-cQCg,465
 dedscumulus/SharePointHandler.py,sha256=7-cmaaSqBB5-Y_huofCYVPMA9vcn8nQAtTCDzha---E,14421
 dedscumulus/TableLogHandler.py,sha256=i1jioOVCfK6PxDXPRLmJn20SkhVtGmpBvsTRw9rMDHg,2250
 dedscumulus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dedscumulus/brzGlobal.py,sha256=VB5Wb448lTocPGEoJGaqnTK96W95mmryaJoW0jGcSkA,8815
-dedscumulus/gbtGlobal.py,sha256=XmaY0rhRj2dzwh7LBKcILtb5i3UglmVG2o_aRWqSn5Y,4990
+dedscumulus/gbtGlobal.py,sha256=t9YJu0Qy9xwYEM66hAZ0s8rkWcxKFL5mVH1xrA8XDl8,5689
 dedscumulus/mstAst.py,sha256=S27M_2PZ002b1Fs4_UYOq3beZl1eHTjZp0UwBO-YLBw,13475
 dedscumulus/mstLog.py,sha256=WenDig2YVRQD3iwJo1yk1AoG0mfma0RbYi_nJm0N0g4,824
 src/RequestHandler.py,sha256=QHYYUg2veBvUlS4G-jVmImfc6hzsFuKMV5UrbmNFRCc,522
 src/SharePointHandler.py,sha256=7-cmaaSqBB5-Y_huofCYVPMA9vcn8nQAtTCDzha---E,14421
 src/TableLogHandler.py,sha256=i1jioOVCfK6PxDXPRLmJn20SkhVtGmpBvsTRw9rMDHg,2250
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/brzGlobal.py,sha256=VB5Wb448lTocPGEoJGaqnTK96W95mmryaJoW0jGcSkA,8815
 src/gbtGlobal.py,sha256=XmaY0rhRj2dzwh7LBKcILtb5i3UglmVG2o_aRWqSn5Y,4990
 src/mstAst.py,sha256=U0hF7TJSRf01GXDE1tuI5f27LD_o01Z1XRfwJBOS3Xc,13474
 src/mstLog.py,sha256=0YOK8lkHIt7ma-xMZ7FCv23ERCFD0N5pLhLXy_FNuoA,823
-dedscumulus-0.0.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-dedscumulus-0.0.7.dist-info/METADATA,sha256=Qvbxry9QLytv2uw83XM0XgNX_1aAUzFCToW3j8Uk30E,566
-dedscumulus-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dedscumulus-0.0.7.dist-info/top_level.txt,sha256=dI9ZW3QNfFmeVCcUCLWTMkOMpHPqI6TTn4luigE8TrM,12
-dedscumulus-0.0.7.dist-info/RECORD,,
+dedscumulus-0.0.8.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+dedscumulus-0.0.8.dist-info/METADATA,sha256=vQ6echtnl71e_yPYiR-MS6CuqImjptLRjZKT5QP2hc0,566
+dedscumulus-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dedscumulus-0.0.8.dist-info/top_level.txt,sha256=dI9ZW3QNfFmeVCcUCLWTMkOMpHPqI6TTn4luigE8TrM,12
+dedscumulus-0.0.8.dist-info/RECORD,,
```

