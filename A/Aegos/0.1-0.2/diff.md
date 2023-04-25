# Comparing `tmp/Aegos-0.1.tar.gz` & `tmp/Aegos-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aegos-0.1.tar", last modified: Sun Apr 23 18:25:11 2023, max compression
+gzip compressed data, was "Aegos-0.2.tar", last modified: Tue Apr 25 00:42:12 2023, max compression
```

## Comparing `Aegos-0.1.tar` & `Aegos-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:25:11.392438 Aegos-0.1/
-drwxrwxrwx   0        0        0        0 2023-04-23 18:25:11.362996 Aegos-0.1/Aegos/
--rw-rw-rw-   0        0        0     8148 2023-04-23 16:18:48.000000 Aegos-0.1/Aegos/Aegos.py
--rw-rw-rw-   0        0        0      139 2023-04-23 18:13:09.000000 Aegos-0.1/Aegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:25:11.388448 Aegos-0.1/Aegos.egg-info/
--rw-rw-rw-   0        0        0      344 2023-04-23 18:25:11.000000 Aegos-0.1/Aegos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-04-23 18:25:11.000000 Aegos-0.1/Aegos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:25:11.000000 Aegos-0.1/Aegos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 18:17:02.000000 Aegos-0.1/Aegos.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-04-23 18:25:11.000000 Aegos-0.1/Aegos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      344 2023-04-23 18:25:11.390443 Aegos-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 18:25:11.393443 Aegos-0.1/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-04-23 18:12:37.000000 Aegos-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:42:12.267222 Aegos-0.2/
+drwxrwxrwx   0        0        0        0 2023-04-25 00:42:12.207140 Aegos-0.2/Aegos/
+-rw-rw-rw-   0        0        0     8001 2023-04-25 00:40:41.000000 Aegos-0.2/Aegos/Aegos.py
+-rw-rw-rw-   0        0        0      139 2023-04-23 18:13:09.000000 Aegos-0.2/Aegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:42:12.263233 Aegos-0.2/Aegos.egg-info/
+-rw-rw-rw-   0        0        0      344 2023-04-25 00:42:12.000000 Aegos-0.2/Aegos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-04-25 00:42:12.000000 Aegos-0.2/Aegos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:42:12.000000 Aegos-0.2/Aegos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 18:17:02.000000 Aegos-0.2/Aegos.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-25 00:42:12.000000 Aegos-0.2/Aegos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      344 2023-04-25 00:42:12.266224 Aegos-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:42:12.267222 Aegos-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-04-25 00:41:52.000000 Aegos-0.2/setup.py
```

### Comparing `Aegos-0.1/Aegos/Aegos.py` & `Aegos-0.2/Aegos/Aegos.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,18 @@
 	 'userid-domain': 'yahoo',
 	 'userId': f'{email2}',
 	 'password': 'szdxfefdgfh',
 	 'birthYear': '1998',
 	 'signup': '',
     }
     response2 = requests.post(url2,headers=headers2,data=data2).text
-    if '{"errors":[{"name":"userId","error":"IDENTIFIER_EXISTS"}]}' in response2:
-        return {'Status':'UnAvailable','AEGOS':'@G_4_2'}
-    elif '{"errors":[]}' in response2:
+    if '{"errors":[]}' in response2:
         return {'Status':'Available','AEGOS':'@G_4_2'}
+    else:
+        return {'Status':'UnAvailable','AEGOS':'@G_4_2'}
 def A_Hotmail(email):
     url3 = f'https://odc.officeapps.live.com/odc/emailhrd/getidp?hm=0&emailAddress={email}&_=1604288577990'
     headers3 = {
         'content-type': 'application/x-www-form-urlencoded',
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.102 Safari/537.36',
     }
     response3 = requests.post(url3, headers=headers3).text
@@ -116,18 +116,18 @@
         'mm': '11',
         'dd': '1',
         'yyyy': '1998',
         'freeformGender': '',
         'signup': '',
     }
     response4 = requests.post(url4,headers=headers4,data=data4).text
-    if ('{"errors":[{"name":"yid","error":"IDENTIFIER_EXISTS"}]}') in response4:
-        return {'Status':'UnAvailable','AEGOS':'@G_4_2'}
-    elif ('{"errors":[]}') in response4:
+    if ('{"errors":[]}') in response4:
         return {'Status':'Available','AEGOS':'@G_4_2'}
+    else:
+        return {'Status':'UnAvailable','AEGOS':'@G_4_2'}
 def A_MailRu(email):
     url5 = 'https://account.mail.ru/api/v1/user/exists'
     headers5 = {
 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.51 Safari/537.36'
     }
     data5 = {
 'email': str(email)
```

