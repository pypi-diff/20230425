# Comparing `tmp/boman-cli-1.4.tar.gz` & `tmp/boman-cli-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boman-cli-1.4.tar", last modified: Fri Mar 31 07:29:55 2023, max compression
+gzip compressed data, was "boman-cli-1.5.tar", last modified: Tue Apr 25 09:57:24 2023, max compression
```

## Comparing `boman-cli-1.4.tar` & `boman-cli-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-03-31 07:29:55.229461 boman-cli-1.4/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1882 2023-03-31 07:29:55.229461 boman-cli-1.4/PKG-INFO
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1049 2023-03-31 07:08:15.000000 boman-cli-1.4/README.md
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-03-31 07:29:55.205461 boman-cli-1.4/boman_cli.egg-info/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1882 2023-03-31 07:29:54.000000 boman-cli-1.4/boman_cli.egg-info/PKG-INFO
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      388 2023-03-31 07:29:54.000000 boman-cli-1.4/boman_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        1 2023-03-31 07:29:54.000000 boman-cli-1.4/boman_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       53 2023-03-31 07:29:54.000000 boman-cli-1.4/boman_cli.egg-info/entry_points.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       45 2023-03-31 07:29:54.000000 boman-cli-1.4/boman_cli.egg-info/requires.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        9 2023-03-31 07:29:54.000000 boman-cli-1.4/boman_cli.egg-info/top_level.txt
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-03-31 07:29:55.229461 boman-cli-1.4/bomancli/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1692 2023-03-31 06:56:04.000000 boman-cli-1.4/bomancli/Config.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        0 2023-03-31 06:44:46.000000 boman-cli-1.4/bomancli/_init_.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2176 2023-02-12 15:08:47.000000 boman-cli-1.4/bomancli/auth.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      968 2022-11-21 13:35:27.000000 boman-cli-1.4/bomancli/base_logger.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1340 2022-11-21 13:35:27.000000 boman-cli-1.4/bomancli/loc_finder.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    30766 2023-03-31 07:29:04.000000 boman-cli-1.4/bomancli/main.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     8744 2023-02-12 15:08:47.000000 boman-cli-1.4/bomancli/utils.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     7848 2023-03-31 06:44:46.000000 boman-cli-1.4/bomancli/validation.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       38 2023-03-31 07:29:55.233461 boman-cli-1.4/setup.cfg
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1069 2023-03-31 06:46:30.000000 boman-cli-1.4/setup.py
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:57:24.104062 boman-cli-1.5/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2064 2023-04-25 09:57:24.104062 boman-cli-1.5/PKG-INFO
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1189 2023-04-25 09:54:14.000000 boman-cli-1.5/README.md
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:57:24.100062 boman-cli-1.5/boman_cli.egg-info/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2064 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      388 2023-04-25 09:57:24.000000 boman-cli-1.5/boman_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        1 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       53 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       45 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/requires.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        9 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/top_level.txt
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:57:24.104062 boman-cli-1.5/bomancli/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1774 2023-04-25 09:51:00.000000 boman-cli-1.5/bomancli/Config.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:42:53.000000 boman-cli-1.5/bomancli/_init_.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2176 2023-04-25 09:45:35.000000 boman-cli-1.5/bomancli/auth.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      968 2022-11-21 13:35:27.000000 boman-cli-1.5/bomancli/base_logger.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1340 2022-11-21 13:35:27.000000 boman-cli-1.5/bomancli/loc_finder.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    32981 2023-04-25 09:55:05.000000 boman-cli-1.5/bomancli/main.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     9230 2023-04-25 09:52:22.000000 boman-cli-1.5/bomancli/utils.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     7848 2023-04-25 09:42:53.000000 boman-cli-1.5/bomancli/validation.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      101 2023-04-25 09:57:24.104062 boman-cli-1.5/setup.cfg
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1575 2023-04-25 09:42:53.000000 boman-cli-1.5/setup.py
```

### Comparing `boman-cli-1.4/PKG-INFO` & `boman-cli-1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boman-cli
-Version: 1.4
+Version: 1.5
 Summary: CLI tool of boman.ai
 Home-page: https://boman.ai
 Author: Sumeru Software Solutions Pvt. Ltd.
 Author-email: support@boman.ai
 License: BSD 2-clause
 Description: # Introduction 
         Boman CLI is a Orchestration script written in python to run security scans on the customer's local or CI/CD environment and upload the results to Boman.ai SaaS server.
@@ -54,13 +54,19 @@
         
         
         
         ### V1.4
         
         Added scanning on jenkins env with limited permission for SAST/DAST scans.
         check-user argument added in --action, to check the permssion of the running user.
+        
+        
+        
+        ### V1.5
+        
+        Failing Build Filter implemented, you can now pass values sucha as 'only-high,only-medium,only-low' to the -fb argument.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `boman-cli-1.4/README.md` & `boman-cli-1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,8 +45,14 @@
 SCA scan bug fixed
 
 
 
 ### V1.4
 
 Added scanning on jenkins env with limited permission for SAST/DAST scans.
-check-user argument added in --action, to check the permssion of the running user.
+check-user argument added in --action, to check the permssion of the running user.
+
+
+
+### V1.5
+
+Failing Build Filter implemented, you can now pass values sucha as 'only-high,only-medium,only-low' to the -fb argument.
```

### Comparing `boman-cli-1.4/boman_cli.egg-info/PKG-INFO` & `boman-cli-1.5/boman_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boman-cli
-Version: 1.4
+Version: 1.5
 Summary: CLI tool of boman.ai
 Home-page: https://boman.ai
 Author: Sumeru Software Solutions Pvt. Ltd.
 Author-email: support@boman.ai
 License: BSD 2-clause
 Description: # Introduction 
         Boman CLI is a Orchestration script written in python to run security scans on the customer's local or CI/CD environment and upload the results to Boman.ai SaaS server.
@@ -54,13 +54,19 @@
         
         
         
         ### V1.4
         
         Added scanning on jenkins env with limited permission for SAST/DAST scans.
         check-user argument added in --action, to check the permssion of the running user.
+        
+        
+        
+        ### V1.5
+        
+        Failing Build Filter implemented, you can now pass values sucha as 'only-high,only-medium,only-low' to the -fb argument.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `boman-cli-1.4/bomancli/Config.py` & `boman-cli-1.5/bomancli/Config.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,22 @@
     secret_scan_message = None
     secret_scan_status = None
     secret_scan_upload_status = None
     secret_scan_errors = None
 
 
     jenkins = None
+    low_count = 0
+    medium_count = 0
+    high_count = 0
+    critical_count = 0
+
 
     app_loc = 0
     
     scan_token = None
     scan_name = 'NA'
 
 
     log_level = "INFO"
 
-    version = 'v1.04'
+    version = 'v1.05'
```

### Comparing `boman-cli-1.4/bomancli/auth.py` & `boman-cli-1.5/bomancli/auth.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.4/bomancli/base_logger.py` & `boman-cli-1.5/bomancli/base_logger.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.4/bomancli/loc_finder.py` & `boman-cli-1.5/bomancli/loc_finder.py`

 * *Files identical despite different names*

### Comparing `boman-cli-1.4/bomancli/main.py` & `boman-cli-1.5/bomancli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     scan_details_id= data['scan_details_id']
     conversion_required = data['conversion_required']
    
 
     #print(docker_image,tool_name,command_line,output_file,will_generate_output,tool_id,scan_details_id)
 
     if docker_image is None:
-        print('Problem with running the scanner, image not specified.')
+        logging.info('Problem with running the scanner, image not specified.')
         exit('3') ## docker/system error
 
     try:
 
         uid = os.getuid()
         gid = os.getgid()
 
@@ -548,14 +548,59 @@
     except Exception as error:
          logging.error(' Error Occured while generating report for secert scan')
 
     return True
 
 
 
+## filtering the vuln and exit code
+
+def exitFunction():
+    scan_token = Config.scan_token
+    app_token = Config.app_token
+    customer_token =  Config.customer_token
+
+    logging.info('Analyzing Vulnerabitlites reported by the tools')
+    url = Config.boman_url+"/api/vuln/get"
+    values = {'app_token':app_token, 'scan_token':scan_token, 'customer_token':customer_token}
+    try:
+        vuln = {"LOW":0,"MEDIUM":0,"HIGH":0,"CRITICAL":0}
+        x = requests.post(url,json=values)  
+
+
+        response = x.json()
+
+        if response['status'] == True:
+            logging.info('Counting the vulnerabilities found')
+            for data in response['data'] :
+                vuln[data['_id']] = data['count']
+
+            Config.low_count = vuln['LOW']
+            Config.medium_count = vuln['MEDIUM']
+            Config.high_count = vuln['HIGH']
+            Config.critical_count = vuln['CRITICAL'] 
+           
+            logging.info('Analyzing Vulnerabitlites Done')
+
+        else:
+            logging.info('Error Analyzing Vulnerabitlites.')
+
+
+
+    except requests.ConnectionError as e:
+        
+        logging.error("Can't connect to the Server, Please check your Internet connection.")
+        print(e)
+        exit(1) #server/saas error
+    
+
+
+
+
+
 #main fucntion where all the actions have been initiated
 def main():
 
 
 
     init()
     Validation.yamlValidation()
@@ -678,15 +723,15 @@
             
         #print('running sca')
         ##runImage(imagename= content['data']['sca']['image'], toolname= content['data']['sca']['tool'],type='SCA',output_file=content['data']['sca']['output_file'],tool_id=content['data']['sca']['tool_id'], scan_details_id=content['data']['sca']['scan_details_id'])
     else:
         logging.info('Ignoring SCA scan')
 
 
-
+    exitFunction()
     return 1
 
 def default():
 
     parser.add_argument('-a','--action',default='init',help="Action arugment, you need to pass the value for action (eg: test-saas, test-docker, run , test-yaml, version, check-user)")
     parser.add_argument('-u','--url',default='https://dashboard.boman.ai/v2/',help="Provide the URL of the boman saas (eg: Prod, On-prem)")
     parser.add_argument('-v','--version',default='show',help="Will show the version of boman-cli tool",action='store_true')
@@ -724,17 +769,47 @@
         logging.info("#################################### -  BOMAN Scanner Initiated - ####################################")
         if main():
             logging.info('################################ BOMAN Scanning Done ################################')
             logging.info('#####################################################################################')
             Utils.uploadLogs()
             Utils.showSummary()
 
-            ## checking the failbuild argument
+           ## checking the failbuild argument
             if args.failBuild == 'fail':
-                exit(-1)
+                total_vuln = Config.high_count + Config.medium_count + Config.low_count + Config.critical_count
+                if total_vuln > 0:
+                    exit(-1)
+                else:
+                    exit(0)    
+
+            elif args.failBuild == 'only-high':
+                if Config.high_count > 0:
+                    exit(-1)
+                else:
+                    exit(0)     
+
+            elif args.failBuild == 'only-medium':
+                if Config.medium_count > 0:
+                    exit(-1)
+                else:
+                    exit(0)    
+
+            elif args.failBuild == 'only-low':
+                if Config.low_count > 0:
+                    exit(-1)
+                else:
+                    exit(0)  
+
+            elif args.failBuild == 'only-critical':
+                if Config.critical_count > 0:
+                    exit(-1)
+                else:
+                    exit(0)                     
+
+
             else:
                 exit(0)  
 
             
         else:
             logging.info('All tasks done')
             exit(0)
```

### Comparing `boman-cli-1.4/bomancli/utils.py` & `boman-cli-1.5/bomancli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 
 
 ### fucntion to test SaaS server, whether is up or not:
 def testServer():
     logging.info('Testing Boman.ai Server')
-    url = Config.boman_url+"/v1/api/app/ping"
+    url = Config.boman_url+"/api/app/ping"
     try:
         x = requests.get(url)  #var ="renga"
     except requests.ConnectionError as e:
         print(e)
         logging.error("Can't connect to the Server, Please check your Internet connection.")
         exit(1) #server/saas error
     else:
@@ -235,15 +235,20 @@
 
 ## summary function
 
 def showSummary():
     logging.info('---------------------------------------------------------------------------------------------------------------')
     logging.info('--------------------------  SUMMARY FOR SCAN: %s  -----------------------------------------------',Config.scan_name,)
     logging.info('--------------------------- Scan Token: %s --------------------------------------------------------',Config.scan_token)
-
+    logging.info('---------------------------------------------------------------------------------------------------------------')
+    logging.info('----------------------------------------')
+    logging.info('-------- Vulnerabilities Found ---------')
+    logging.info('HIGH : %s | MEDIUM : %s | LOW : %s ', Config.high_count, Config.medium_count, Config.low_count)
+    logging.info('----------------------------------------')
+    logging.info('----------------------------------------')
     logging.info('-------- SAST STATUS ---------')
     if Config.sast_present == True:
         logging.info('SCAN STATUS: %s',Config.sast_scan_status)
         logging.info('UPLOAD STATUS: %s',Config.sast_upload_status)
         logging.info('SCAN MESSAGE : %s', Config.sast_message)
 
         logging.info('ERRORS: %s',Config.sast_errors)
```

### Comparing `boman-cli-1.4/bomancli/validation.py` & `boman-cli-1.5/bomancli/validation.py`

 * *Files identical despite different names*

