# Comparing `tmp/zscaler_api_talkers-4.0.1.tar.gz` & `tmp/zscaler_api_talkers-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_api_talkers-4.0.1.tar", last modified: Thu Apr 20 16:54:51 2023, max compression
+gzip compressed data, was "zscaler_api_talkers-4.0.2.tar", last modified: Tue Apr 25 00:45:25 2023, max compression
```

## Comparing `zscaler_api_talkers-4.0.1.tar` & `zscaler_api_talkers-4.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.044587 zscaler_api_talkers-4.0.1/
--rw-r--r--   0 spereira   (501) staff       (20)     1071 2022-04-21 16:27:44.000000 zscaler_api_talkers-4.0.1/LICENSE.txt
--rw-r--r--   0 spereira   (501) staff       (20)     3031 2023-04-20 16:54:51.044207 zscaler_api_talkers-4.0.1/PKG-INFO
--rw-r--r--   0 spereira   (501) staff       (20)     2683 2023-04-19 16:20:53.000000 zscaler_api_talkers-4.0.1/README.md
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.033077 zscaler_api_talkers-4.0.1/models/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/models/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)    14364 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/models/models.py
--rw-r--r--   0 spereira   (501) staff       (20)       84 2022-04-21 20:33:36.000000 zscaler_api_talkers-4.0.1/pyproject.toml
--rw-r--r--   0 spereira   (501) staff       (20)       38 2023-04-20 16:54:51.044690 zscaler_api_talkers-4.0.1/setup.cfg
--rw-r--r--   0 spereira   (501) staff       (20)      568 2023-04-07 21:48:18.000000 zscaler_api_talkers-4.0.1/setup.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.034284 zscaler_api_talkers-4.0.1/zcc_talker/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/zcc_talker/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)     4747 2023-04-05 17:08:58.000000 zscaler_api_talkers-4.0.1/zcc_talker/zcc_talker.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.037046 zscaler_api_talkers-4.0.1/zia_talker/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 02:12:49.000000 zscaler_api_talkers-4.0.1/zia_talker/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)    15297 2023-04-20 16:51:44.000000 zscaler_api_talkers-4.0.1/zia_talker/zia_portaltalker.py
--rw-r--r--   0 spereira   (501) staff       (20)    66881 2023-04-14 15:49:45.000000 zscaler_api_talkers-4.0.1/zia_talker/zia_talker.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.040067 zscaler_api_talkers-4.0.1/zpa_talker/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/zpa_talker/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)     2369 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.1/zpa_talker/zpa_portaltalker.py
--rw-r--r--   0 spereira   (501) staff       (20)    20237 2023-04-19 16:14:30.000000 zscaler_api_talkers-4.0.1/zpa_talker/zpa_talker.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.042693 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/
--rw-r--r--   0 spereira   (501) staff       (20)     3031 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/PKG-INFO
--rw-r--r--   0 spereira   (501) staff       (20)      559 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/SOURCES.txt
--rw-r--r--   0 spereira   (501) staff       (20)        1 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/dependency_links.txt
--rw-r--r--   0 spereira   (501) staff       (20)       25 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/requires.txt
--rw-r--r--   0 spereira   (501) staff       (20)       56 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/top_level.txt
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.043375 zscaler_api_talkers-4.0.1/zscaler_helpers/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/zscaler_helpers/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)     7203 2023-04-19 03:45:34.000000 zscaler_api_talkers-4.0.1/zscaler_helpers/http_calls.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.062869 zscaler_api_talkers-4.0.2/
+-rw-r--r--   0 spereira   (501) staff       (20)     1071 2022-04-21 16:27:44.000000 zscaler_api_talkers-4.0.2/LICENSE.txt
+-rw-r--r--   0 spereira   (501) staff       (20)     3031 2023-04-25 00:45:25.062569 zscaler_api_talkers-4.0.2/PKG-INFO
+-rw-r--r--   0 spereira   (501) staff       (20)     2683 2023-04-19 16:20:53.000000 zscaler_api_talkers-4.0.2/README.md
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.054010 zscaler_api_talkers-4.0.2/models/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.2/models/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)    14364 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.2/models/models.py
+-rw-r--r--   0 spereira   (501) staff       (20)       84 2022-04-21 20:33:36.000000 zscaler_api_talkers-4.0.2/pyproject.toml
+-rw-r--r--   0 spereira   (501) staff       (20)       38 2023-04-25 00:45:25.062949 zscaler_api_talkers-4.0.2/setup.cfg
+-rw-r--r--   0 spereira   (501) staff       (20)      568 2023-04-20 16:58:56.000000 zscaler_api_talkers-4.0.2/setup.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.054922 zscaler_api_talkers-4.0.2/zcc_talker/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.2/zcc_talker/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)     4747 2023-04-05 17:08:58.000000 zscaler_api_talkers-4.0.2/zcc_talker/zcc_talker.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.056552 zscaler_api_talkers-4.0.2/zia_talker/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 02:12:49.000000 zscaler_api_talkers-4.0.2/zia_talker/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)    15297 2023-04-20 16:51:44.000000 zscaler_api_talkers-4.0.2/zia_talker/zia_portaltalker.py
+-rw-r--r--   0 spereira   (501) staff       (20)    66881 2023-04-14 15:49:45.000000 zscaler_api_talkers-4.0.2/zia_talker/zia_talker.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.059265 zscaler_api_talkers-4.0.2/zpa_talker/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.2/zpa_talker/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)     2369 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.2/zpa_talker/zpa_portaltalker.py
+-rw-r--r--   0 spereira   (501) staff       (20)    22113 2023-04-25 00:44:34.000000 zscaler_api_talkers-4.0.2/zpa_talker/zpa_talker.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.061355 zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/
+-rw-r--r--   0 spereira   (501) staff       (20)     3031 2023-04-25 00:45:24.000000 zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/PKG-INFO
+-rw-r--r--   0 spereira   (501) staff       (20)      559 2023-04-25 00:45:25.000000 zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/SOURCES.txt
+-rw-r--r--   0 spereira   (501) staff       (20)        1 2023-04-25 00:45:24.000000 zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/dependency_links.txt
+-rw-r--r--   0 spereira   (501) staff       (20)       25 2023-04-25 00:45:24.000000 zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/requires.txt
+-rw-r--r--   0 spereira   (501) staff       (20)       56 2023-04-25 00:45:24.000000 zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/top_level.txt
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-25 00:45:25.061847 zscaler_api_talkers-4.0.2/zscaler_helpers/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.2/zscaler_helpers/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)     7203 2023-04-19 03:45:34.000000 zscaler_api_talkers-4.0.2/zscaler_helpers/http_calls.py
```

### Comparing `zscaler_api_talkers-4.0.1/LICENSE.txt` & `zscaler_api_talkers-4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/PKG-INFO` & `zscaler_api_talkers-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler_api_talkers
-Version: 4.0.1
+Version: 4.0.2
 Summary: Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC
 Home-page: https://github.com/sergitopereira/zscaler_api_talkers.git
 Author: Sergio Pereira
 Author-email: sergitopereira@hotmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `zscaler_api_talkers-4.0.1/README.md` & `zscaler_api_talkers-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/models/models.py` & `zscaler_api_talkers-4.0.2/models/models.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/setup.py` & `zscaler_api_talkers-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zscaler_api_talkers',
-    version='4.0.1',
+    version='4.0.2',
     author='Sergio Pereira',
     author_email='sergitopereira@hotmail.com',
     packages=find_packages(),
     url='https://github.com/sergitopereira/zscaler_api_talkers.git',
     license='LICENSE.txt',
     description='Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC',
     long_description_content_type="text/markdown",
```

### Comparing `zscaler_api_talkers-4.0.1/zcc_talker/zcc_talker.py` & `zscaler_api_talkers-4.0.2/zcc_talker/zcc_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/zia_talker/zia_portaltalker.py` & `zscaler_api_talkers-4.0.2/zia_talker/zia_portaltalker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/zia_talker/zia_talker.py` & `zscaler_api_talkers-4.0.2/zia_talker/zia_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/zpa_talker/zpa_portaltalker.py` & `zscaler_api_talkers-4.0.2/zpa_talker/zpa_portaltalker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/zpa_talker/zpa_talker.py` & `zscaler_api_talkers-4.0.2/zpa_talker/zpa_talker.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,51 +93,74 @@
             response = self.hp_http.get_call(url, headers=self.header, error_handling=True)
             return response.json()
         url = f'/mgmtconfig/v1/admin/customers/{self.customerId}/application'
         response = self._obtain_all_results(url)
         return response
 
     def add_application_segment(self, name, healthReporting, domainNames, segmentGroupId, serverGroups,
-                                tcpPortRanges=[], udpPortRanges=[], description='', enabled=True, ipAnchored=False,
-                                doubleEncrypt=False, bypassType='NEVER', isCnameEnabled=True, cnameConfig='NOFLATTEN'):
+                                commonAppsDto={}, segmentGroupName='', healthCheckType='DEFAULT', clientlessApps=[],
+                                inspectionApps=[], sraApps=[], tcpPortRange=[], tcpPortRanges=[], udpPortRanges=[],
+                                udpPortRange=[], description='', enabled=True, icmpAccessType='NONE', ipAnchored=False,
+                                doubleEncrypt=False, bypassType='NEVER', isCnameEnabled=True,
+                                selectConnectorCloseToApp=False, passiveHealthEnabled=True):
         """
         Adds a new Application Segment for a ZPA tenant.
         :param name: type string. App Name
         :param description: type string. Description
         :param enabled: type boolean (True|False)
         :param healthReporting: type string. possible values: NONE, ON_ACCESS, CONTINUOUS
+        :param icmpAccessType: type string. possible values: PING_TRACEROUTING, PING, NONE
         :param ipAnchored: type boolean (True|False)
         :param doubleEncrypt: type boolean (True|False)
         :param bypassType: type string. possible values ALWAYS, NEVER, ON_NET
+        :param clientlessApps: type list. List of application domains in Application Segment with Browser access enabled
+        :param inspectionApps: type list. List of application domains in Application Segment with Inspection enabled
+        :param sraApps: type list. List of application domains in Application Segment with Privileged Remote Access enabled
+        :param commonAppsDto: type list. list of dictionaries, where appsConfig will list the apps with Browser Access or Inspection
         :param isCnameEnabled: type boolean (True|False)
-        :param tcpPortRanges: type list.  ["from", "to"]
-        :param udpPortRanges: type list.  ["from", "to"]
+        :param selectConnectorCloseToApp: type boolean (True|False)
+        :param passiveHealthEnabled: type boolean (True|False)
+        :param tcpPortRange: type dict.  [{"from":int, "to":int}]
+        :param udpPortRange: type dict.  [{"from":int, "to":int}]
+        :param tcpPortRanges: type list.  ["from", "to"]. This will be deprecated in future.
+        :param udpPortRanges: type list.  ["from", "to"]. This will be deprecated in future.
         :param domainNames: type list. List of domains or IP addresses
         :param segmentGroupId: type string. Application Segment Group id
+        :param segmentGroupName: type string. Application Segment Group Name
         :param serverGroups=type list. list of dictionaries, where key is id and value is serverGroupId [{
                 "id": "<serverGroupId>"}]
         :return: type dict. HTTP response
         """
 
         url = f"/mgmtconfig/v1/admin/customers/{self.customerId}/application"
         payload = {
             "name": name,
             "description": description,
             "enabled": enabled,
+            "healthCheckType": healthCheckType,
             "healthReporting": healthReporting,
+            "icmpAccessType": icmpAccessType,
             "ipAnchored": ipAnchored,
             "doubleEncrypt": doubleEncrypt,
             "bypassType": bypassType,
             "isCnameEnabled": isCnameEnabled,
+            "clientlessApps": clientlessApps,
+            "inspectionApps": inspectionApps,
+            "sraApps": sraApps,
+            "commonAppsDto": commonAppsDto,
+            "selectConnectorCloseToApp": selectConnectorCloseToApp,
+            "passiveHealthEnabled": passiveHealthEnabled,
             "tcpPortRanges": tcpPortRanges,
+            "tcpPortRange": tcpPortRange,
+            "udpPortRange": udpPortRange,
             "udpPortRanges": udpPortRanges,
             "domainNames": domainNames,
             "segmentGroupId": segmentGroupId,
+            "segmentGroupName": segmentGroupName,
             "serverGroups": serverGroups,
-            "cnameConfig": cnameConfig
         }
         response = self.hp_http.post_call(url=url, payload=payload, headers=self.header, error_handling=True)
         return response.json()
 
     def update_application_segment(self,applicationId,payload):
         """
         Updates the Application Segment details for the specified ID
@@ -355,29 +378,27 @@
         response = self._obtain_all_results(url)
         return response
 
     # global-policy-controller
 
     def list_policies(self, policyType='ACCESS_POLICY'):
         """list policie(s)  by policy type,
-         :param policyType: Type string. Supportef values Possible values=ACCESS_POLICY,GLOBAL_POLICY, TIMEOUT_POLICY,REAUTH_POLICY,
+         :param policyType: Type string. Supported values Possible values=ACCESS_POLICY,GLOBAL_POLICY, TIMEOUT_POLICY,REAUTH_POLICY,
          SIEM_POLICY, CLIENT_FORWARDING_POLICY,BYPASS_POLICY
          """
         url = f"/mgmtconfig/v1/admin/customers/{self.customerId}/policySet/rules/policyType/{policyType}"
         response = self._obtain_all_results(url)
         return response
 
-    def list_global_policy_id(self, query=False):
+    def list_policySet(self, policyType='ACCESS_POLICY'):
+        """ Gets the policy set for the specified policy type
+        :param policyType: Type string. Supported values are ACCESS_POLICY,GLOBAL_POLICY, TIMEOUT_POLICY,REAUTH_POLICY,
+        SIEM_POLICY, CLIENT_FORWARDING_POLICY,BYPASS_POLICY
         """
-        Method to get the global policy
-        :param query: ?page=1&pagesize=20&search=consequat
-        """
-        if not query:
-            query = '?pagesize=500'
-        url = f'/mgmtconfig/v1/admin/customers/{self.customerId}/policySet/global{query}'
+        url = f'/mgmtconfig/v1/admin/customers/{self.customerId}/policySet/policyType/{policyType}'
         response = self.hp_http.get_call(url, headers=self.header, error_handling=True)
         return response.json()
 
     def add_policySet(self, app_operands, RuleName, Action, policySetId, operands, operator, MsgString=None):
         """
         Method to create a new access Policy
         :param app_operands: list of app_operands: Examples
```

### Comparing `zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/PKG-INFO` & `zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-api-talkers
-Version: 4.0.1
+Version: 4.0.2
 Summary: Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC
 Home-page: https://github.com/sergitopereira/zscaler_api_talkers.git
 Author: Sergio Pereira
 Author-email: sergitopereira@hotmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/SOURCES.txt` & `zscaler_api_talkers-4.0.2/zscaler_api_talkers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.1/zscaler_helpers/http_calls.py` & `zscaler_api_talkers-4.0.2/zscaler_helpers/http_calls.py`

 * *Files identical despite different names*

