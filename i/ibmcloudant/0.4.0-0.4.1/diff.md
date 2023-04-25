# Comparing `tmp/ibmcloudant-0.4.0.tar.gz` & `tmp/ibmcloudant-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmcloudant-0.4.0.tar", last modified: Mon Mar 27 14:30:47 2023, max compression
+gzip compressed data, was "ibmcloudant-0.4.1.tar", last modified: Tue Apr 25 09:05:09 2023, max compression
```

## Comparing `ibmcloudant-0.4.0.tar` & `ibmcloudant-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-27 14:30:47.916496 ibmcloudant-0.4.0/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11357 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       70 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27202 2023-03-27 14:30:47.916496 ibmcloudant-0.4.0/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26200 2023-03-27 14:17:50.000000 ibmcloudant-0.4.0/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-27 14:30:47.912496 ibmcloudant-0.4.0/ibmcloudant/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1596 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6630 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/cloudant_base_service.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   750934 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/cloudant_v1.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1811 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/common.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3396 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/couchdb_session_authenticator.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1543 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/couchdb_session_get_authenticator_patch.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/ibmcloudant/couchdb_session_token_manager.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      655 2023-03-27 14:17:50.000000 ibmcloudant-0.4.0/ibmcloudant/version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-27 14:30:47.916496 ibmcloudant-0.4.0/ibmcloudant.egg-info/
--rw-rw-rw-   0 jenkins   (1000) jenkins   (1000)    27202 2023-03-27 14:30:47.000000 ibmcloudant-0.4.0/ibmcloudant.egg-info/PKG-INFO
--rw-rw-rw-   0 jenkins   (1000) jenkins   (1000)      558 2023-03-27 14:30:47.000000 ibmcloudant-0.4.0/ibmcloudant.egg-info/SOURCES.txt
--rw-rw-rw-   0 jenkins   (1000) jenkins   (1000)        1 2023-03-27 14:30:47.000000 ibmcloudant-0.4.0/ibmcloudant.egg-info/dependency_links.txt
--rw-rw-rw-   0 jenkins   (1000) jenkins   (1000)       97 2023-03-27 14:30:47.000000 ibmcloudant-0.4.0/ibmcloudant.egg-info/requires.txt
--rw-rw-rw-   0 jenkins   (1000) jenkins   (1000)       12 2023-03-27 14:30:47.000000 ibmcloudant-0.4.0/ibmcloudant.egg-info/top_level.txt
--rw-rw-rw-   0 jenkins   (1000) jenkins   (1000)        1 2023-03-27 14:16:23.000000 ibmcloudant-0.4.0/ibmcloudant.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      231 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      135 2023-03-27 14:15:48.000000 ibmcloudant-0.4.0/requirements.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-03-27 14:30:47.916496 ibmcloudant-0.4.0/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3435 2023-03-27 14:17:50.000000 ibmcloudant-0.4.0/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11357 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       70 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27202 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26200 2023-04-25 08:51:15.000000 ibmcloudant-0.4.1/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/ibmcloudant/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1596 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6630 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/cloudant_base_service.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   745079 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/cloudant_v1.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1811 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/common.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3396 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/couchdb_session_authenticator.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1543 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/couchdb_session_get_authenticator_patch.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/ibmcloudant/couchdb_session_token_manager.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      655 2023-04-25 08:51:15.000000 ibmcloudant-0.4.1/ibmcloudant/version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/ibmcloudant.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27202 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      558 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       97 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       12 2023-04-25 09:05:09.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-25 08:48:29.000000 ibmcloudant-0.4.1/ibmcloudant.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      232 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      135 2023-04-25 08:48:06.000000 ibmcloudant-0.4.1/requirements.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-04-25 09:05:09.503718 ibmcloudant-0.4.1/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3435 2023-04-25 08:51:15.000000 ibmcloudant-0.4.1/setup.py
```

### Comparing `ibmcloudant-0.4.0/LICENSE` & `ibmcloudant-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/PKG-INFO` & `ibmcloudant-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloudant
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python client library for IBM Cloudant
 Home-page: https://github.com/IBM/cloudant-python-sdk
 Author: IBM
 Author-email: cldtsdks@us.ibm.com
 License: Apache 2.0
 Keywords: ibmcloudant
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.0
+# IBM Cloudant Python SDK Version 0.4.1
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -123,21 +123,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.0"
+pip install --upgrade "ibmcloudant>=0.4.1"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.0"
+easy_install --upgrade "ibmcloudant>=0.4.1"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
```

### Comparing `ibmcloudant-0.4.0/README.md` & `ibmcloudant-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.0
+# IBM Cloudant Python SDK Version 0.4.1
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -98,21 +98,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.0"
+pip install --upgrade "ibmcloudant>=0.4.1"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.0"
+easy_install --upgrade "ibmcloudant>=0.4.1"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
```

### Comparing `ibmcloudant-0.4.0/ibmcloudant/__init__.py` & `ibmcloudant-0.4.1/ibmcloudant/__init__.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/ibmcloudant/cloudant_base_service.py` & `ibmcloudant-0.4.1/ibmcloudant/cloudant_base_service.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/ibmcloudant/cloudant_v1.py` & `ibmcloudant-0.4.1/ibmcloudant/cloudant_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,59 +33,59 @@
 
 from .common import get_sdk_headers
 
 ##############################################################################
 # Service
 ##############################################################################
 
+
 class CloudantV1(BaseService):
     """The Cloudant V1 service."""
 
     DEFAULT_SERVICE_URL = 'http://localhost:5984'
     DEFAULT_SERVICE_NAME = 'cloudant'
 
     @classmethod
-    def new_instance(cls,
-                     service_name: str = DEFAULT_SERVICE_NAME,
-                    ) -> 'CloudantV1':
+    def new_instance(
+        cls,
+        service_name: str = DEFAULT_SERVICE_NAME,
+    ) -> 'CloudantV1':
         """
         Return a new client for the Cloudant service using the specified parameters
                and external configuration.
         """
         authenticator = get_authenticator_from_environment(service_name)
         service = cls(
             authenticator
             )
         service.configure_service(service_name)
         return service
 
-    def __init__(self,
-                 authenticator: Authenticator = None,
-                ) -> None:
+    def __init__(
+        self,
+        authenticator: Authenticator = None,
+    ) -> None:
         """
         Construct a new client for the Cloudant service.
 
         :param Authenticator authenticator: The authenticator specifies the authentication mechanism.
                Get up to date information from https://github.com/IBM/python-sdk-core/blob/main/README.md
                about initializing the authenticator of your choice.
         """
-        BaseService.__init__(self,
-                             service_url=self.DEFAULT_SERVICE_URL,
-                             authenticator=authenticator)
+        BaseService.__init__(self, service_url=self.DEFAULT_SERVICE_URL, authenticator=authenticator)
         # enable gzip compression of request bodies
         self.set_enable_gzip_compression(True)
 
-
     #########################
     # Server
     #########################
 
-
-    def get_server_information(self,
-        **kwargs
+    def get_server_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve server instance information.
 
         When you access the root of an instance, IBM Cloudant returns meta-information
         about the instance. The response includes a JSON structure that contains
         information about the server, including a welcome message and the server's
@@ -94,72 +94,80 @@
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ServerInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_server_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_server_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_membership_information(self,
-        **kwargs
+    def get_membership_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve cluster membership information.
 
         Displays the nodes that are part of the cluster as `cluster_nodes`. The field,
         `all_nodes`, displays all nodes this node knows about, including the ones that are
         part of the cluster. This endpoint is useful when you set up a cluster.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `MembershipInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_membership_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_membership_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_membership'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_uuids(self,
+    def get_uuids(
+        self,
         *,
         count: int = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve one or more UUIDs.
 
         Requests one or more Universally Unique Identifiers (UUIDs) from the instance. The
         response is a JSON object that provides a list of UUIDs.
         **Tip:**  The authentication for this endpoint is only enforced when using IAM.
@@ -168,75 +176,83 @@
                to return.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `UuidsResult` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_uuids')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_uuids',
+        )
         headers.update(sdk_headers)
 
         params = {
             'count': count,
         }
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_uuids'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_capacity_throughput_information(self,
-        **kwargs
+    def get_capacity_throughput_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve provisioned throughput capacity information.
 
         View the amount of provisioned throughput capacity that is allocated to an IBM
         Cloudant instance and what is the target provisioned throughput capacity.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CapacityThroughputInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_capacity_throughput_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_capacity_throughput_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/capacity/throughput'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_capacity_throughput_configuration(self,
+    def put_capacity_throughput_configuration(
+        self,
         blocks: int,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Update the target provisioned throughput capacity.
 
         Sets the target provisioned throughput capacity for an IBM Cloudant instance. When
         target capacity is changed, the current capacity asynchronously changes to meet
         the target capacity.
@@ -248,17 +264,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CapacityThroughputInformation` object
         """
 
         if blocks is None:
             raise ValueError('blocks must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_capacity_throughput_configuration')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_capacity_throughput_configuration',
+        )
         headers.update(sdk_headers)
 
         data = {
             'blocks': blocks,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -266,34 +284,36 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/capacity/throughput'
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Databases
     #########################
 
-
-    def get_db_updates(self,
+    def get_db_updates(
+        self,
         *,
         feed: str = None,
         heartbeat: int = None,
         timeout: int = None,
         since: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve change events for all databases.
 
         Lists changes to databases, like a global changes feed. Types of changes include
         updating the database and creating or deleting a database. Like the changes feed,
         the feed is not guaranteed to return changes in the correct order and might repeat
@@ -320,17 +340,19 @@
                a valid update sequence or `now` value. Default is `0` i.e. all changes.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DbUpdates` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_db_updates')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_db_updates',
+        )
         headers.update(sdk_headers)
 
         params = {
             'feed': feed,
             'heartbeat': heartbeat,
             'timeout': timeout,
             'since': since,
@@ -338,24 +360,26 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_db_updates'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_changes(self,
+    def post_changes(
+        self,
         db: str,
         *,
         doc_ids: List[str] = None,
         fields: List[str] = None,
         selector: dict = None,
         last_event_id: str = None,
         att_encoding_info: bool = None,
@@ -368,15 +392,15 @@
         include_docs: bool = None,
         limit: int = None,
         seq_interval: int = None,
         since: str = None,
         style: str = None,
         timeout: int = None,
         view: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query the database document changes feed.
 
         Requests the database changes feed in the same way as `GET /{db}/_changes` does.
         It is widely used with the `filter` query parameter because it allows one to pass
         more information to the filter.
@@ -487,17 +511,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {
             'Last-Event-ID': last_event_id,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_changes')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_changes',
+        )
         headers.update(sdk_headers)
 
         params = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -527,25 +553,27 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_changes'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_changes_as_stream(self,
+    def post_changes_as_stream(
+        self,
         db: str,
         *,
         doc_ids: List[str] = None,
         fields: List[str] = None,
         selector: dict = None,
         last_event_id: str = None,
         att_encoding_info: bool = None,
@@ -558,15 +586,15 @@
         include_docs: bool = None,
         limit: int = None,
         seq_interval: int = None,
         since: str = None,
         style: str = None,
         timeout: int = None,
         view: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query the database document changes feed as stream.
 
         Requests the database changes feed in the same way as `GET /{db}/_changes` does.
         It is widely used with the `filter` query parameter because it allows one to pass
         more information to the filter.
@@ -677,17 +705,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {
             'Last-Event-ID': last_event_id,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_changes_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_changes_as_stream',
+        )
         headers.update(sdk_headers)
 
         params = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -717,31 +747,33 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_changes'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
     #########################
     # Databases
     #########################
 
-
-    def head_database(self,
+    def head_database(
+        self,
         db: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the HTTP headers for a database.
 
         Returns the HTTP headers that contain a minimal amount of information about the
         specified database. Since the response body is empty, using the HEAD method is a
         lightweight way to check if the database exists or not.
@@ -751,43 +783,47 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_database')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_database',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_all_dbs(self,
+    def get_all_dbs(
+        self,
         *,
         descending: bool = None,
         end_key: str = None,
         limit: int = None,
         skip: int = None,
         start_key: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a list of all database names in the instance.
 
         :param bool descending: (optional) Query parameter to specify whether to
                return the documents in descending by key order.
         :param str end_key: (optional) Query parameter to specify to stop returning
@@ -802,17 +838,19 @@
                type that matches the key type emitted by the view function.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `List[str]` result
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_all_dbs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_all_dbs',
+        )
         headers.update(sdk_headers)
 
         params = {
             'descending': descending,
             'end_key': end_key,
             'limit': limit,
             'skip': skip,
@@ -821,26 +859,28 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_all_dbs'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_dbs_info(self,
+    def post_dbs_info(
+        self,
         keys: List[str],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query information about multiple databases.
 
         This operation enables you to request information about multiple databases in a
         single request, instead of issuing multiple `GET /{db}` requests. It returns a
         list that contains an information object for each database specified in the
@@ -851,17 +891,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `List[DbsInfoResult]` result
         """
 
         if keys is None:
             raise ValueError('keys must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_dbs_info')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_dbs_info',
+        )
         headers.update(sdk_headers)
 
         data = {
             'keys': keys,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -869,26 +911,28 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_dbs_info'
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def delete_database(self,
+    def delete_database(
+        self,
         db: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Delete a database.
 
         Deletes the specified database and all documents and attachments contained within
         it. To avoid deleting a database, the server responds with a 400 HTTP status code
         when the request URL includes a `?rev=` parameter. This response suggests that a
@@ -899,80 +943,88 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Ok` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_database')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_database',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_database_information(self,
+    def get_database_information(
+        self,
         db: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about a database.
 
         :param str db: Path parameter to specify the database name.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DatabaseInformation` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_database_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_database_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_database(self,
+    def put_database(
+        self,
         db: str,
         *,
         partitioned: bool = None,
         q: int = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create a database.
 
         :param str db: Path parameter to specify the database name.
         :param bool partitioned: (optional) Query parameter to specify whether to
                enable database partitions when creating a database.
@@ -984,17 +1036,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Ok` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_database')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_database',
+        )
         headers.update(sdk_headers)
 
         params = {
             'partitioned': partitioned,
             'q': q,
         }
 
@@ -1003,35 +1057,37 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Documents
     #########################
 
-
-    def head_document(self,
+    def head_document(
+        self,
         db: str,
         doc_id: str,
         *,
         if_none_match: str = None,
         latest: bool = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the HTTP headers for the document.
 
         This method supports the same query arguments as the `GET /{db}/{docid}` method,
         but only the header information (including document size and the revision as an
         ETag) is returned. The ETag header shows the current revision for the requested
@@ -1054,17 +1110,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'latest': latest,
             'rev': rev,
         }
 
@@ -1072,30 +1130,32 @@
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_document(self,
+    def post_document(
+        self,
         db: str,
         document: Union['Document', BinaryIO],
         *,
         content_type: str = None,
         batch: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create or modify a document in a database.
 
         Creates or modifies a document in the specified database by using the supplied
         JSON document.
         For creation, you may specify the document ID but you should not specify the
@@ -1123,17 +1183,19 @@
             raise ValueError('document must be provided')
         if isinstance(document, Document):
             document = convert_model(document)
             content_type = content_type or 'application/json'
         headers = {
             'Content-Type': content_type,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
         }
 
         if isinstance(document, dict):
@@ -1148,25 +1210,27 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_all_docs(self,
+    def post_all_docs(
+        self,
         db: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
         descending: bool = None,
         include_docs: bool = None,
@@ -1174,15 +1238,15 @@
         limit: int = None,
         skip: int = None,
         update_seq: bool = None,
         end_key: str = None,
         key: str = None,
         keys: List[str] = None,
         start_key: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a list of all documents in a database.
 
         Queries the primary index (all document IDs). The results that match the request
         body parameters are returned in a JSON object, including a list of matching
         documents with basic contents, such as the ID and revision. When no request body
@@ -1220,17 +1284,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `AllDocsResult` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_all_docs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_all_docs',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -1253,24 +1319,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_all_docs'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_all_docs_as_stream(self,
+    def post_all_docs_as_stream(
+        self,
         db: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
         descending: bool = None,
         include_docs: bool = None,
@@ -1278,15 +1346,15 @@
         limit: int = None,
         skip: int = None,
         update_seq: bool = None,
         end_key: str = None,
         key: str = None,
         keys: List[str] = None,
         start_key: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a list of all documents in a database as stream.
 
         Queries the primary index (all document IDs). The results that match the request
         body parameters are returned in a JSON object, including a list of matching
         documents with basic contents, such as the ID and revision. When no request body
@@ -1324,17 +1392,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `BinaryIO` result
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_all_docs_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_all_docs_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -1357,27 +1427,29 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_all_docs'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def post_all_docs_queries(self,
+    def post_all_docs_queries(
+        self,
         db: str,
         queries: List['AllDocsQuery'],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Multi-query the list of all documents in a database.
 
         Runs multiple queries using the primary index (all document IDs). Returns a JSON
         object that contains a list of result objects, one for each query, with a
         structure equivalent to that of a single `_all_docs` request. This enables you to
@@ -1396,17 +1468,19 @@
 
         if not db:
             raise ValueError('db must be provided')
         if queries is None:
             raise ValueError('queries must be provided')
         queries = [convert_model(x) for x in queries]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_all_docs_queries')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_all_docs_queries',
+        )
         headers.update(sdk_headers)
 
         data = {
             'queries': queries,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -1417,27 +1491,29 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_all_docs/queries'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_all_docs_queries_as_stream(self,
+    def post_all_docs_queries_as_stream(
+        self,
         db: str,
         queries: List['AllDocsQuery'],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Multi-query the list of all documents in a database as stream.
 
         Runs multiple queries using the primary index (all document IDs). Returns a JSON
         object that contains a list of result objects, one for each query, with a
         structure equivalent to that of a single `_all_docs` request. This enables you to
@@ -1456,17 +1532,19 @@
 
         if not db:
             raise ValueError('db must be provided')
         if queries is None:
             raise ValueError('queries must be provided')
         queries = [convert_model(x) for x in queries]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_all_docs_queries_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_all_docs_queries_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'queries': queries,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -1477,27 +1555,29 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_all_docs/queries'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def post_bulk_docs(self,
+    def post_bulk_docs(
+        self,
         db: str,
         bulk_docs: Union['BulkDocs', BinaryIO],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Bulk modify multiple documents in a database.
 
         The bulk document API allows you to create, update, and delete multiple documents
         at the same time within a single request. The basic operation is similar to
         creating, updating, or deleting a single document, except that you batch the
@@ -1513,17 +1593,19 @@
         if not db:
             raise ValueError('db must be provided')
         if bulk_docs is None:
             raise ValueError('bulk_docs must be provided')
         if isinstance(bulk_docs, BulkDocs):
             bulk_docs = convert_model(bulk_docs)
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_bulk_docs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_bulk_docs',
+        )
         headers.update(sdk_headers)
 
         if isinstance(bulk_docs, dict):
             data = json.dumps(bulk_docs)
         else:
             data = bulk_docs
         headers['content-type'] = 'application/json'
@@ -1533,32 +1615,34 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_bulk_docs'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_bulk_get(self,
+    def post_bulk_get(
+        self,
         db: str,
         docs: List['BulkGetQueryDocument'],
         *,
         attachments: bool = None,
         att_encoding_info: bool = None,
         latest: bool = None,
         revs: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Bulk query revision information for multiple documents.
 
         Fetch specific revisions or revision histories for multiple documents in bulk as
         replicators do.
 
@@ -1581,17 +1665,19 @@
 
         if not db:
             raise ValueError('db must be provided')
         if docs is None:
             raise ValueError('docs must be provided')
         docs = [convert_model(x) for x in docs]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_bulk_get')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_bulk_get',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'latest': latest,
             'revs': revs,
@@ -1609,33 +1695,35 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_bulk_get'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_bulk_get_as_mixed(self,
+    def post_bulk_get_as_mixed(
+        self,
         db: str,
         docs: List['BulkGetQueryDocument'],
         *,
         attachments: bool = None,
         att_encoding_info: bool = None,
         latest: bool = None,
         revs: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Bulk query revision information for multiple documents as mixed.
 
         Fetch specific revisions or revision histories for multiple documents in bulk as
         replicators do.
 
@@ -1658,17 +1746,19 @@
 
         if not db:
             raise ValueError('db must be provided')
         if docs is None:
             raise ValueError('docs must be provided')
         docs = [convert_model(x) for x in docs]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_bulk_get_as_mixed')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_bulk_get_as_mixed',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'latest': latest,
             'revs': revs,
@@ -1686,33 +1776,35 @@
             del kwargs['headers']
         headers['Accept'] = 'multipart/mixed'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_bulk_get'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_bulk_get_as_related(self,
+    def post_bulk_get_as_related(
+        self,
         db: str,
         docs: List['BulkGetQueryDocument'],
         *,
         attachments: bool = None,
         att_encoding_info: bool = None,
         latest: bool = None,
         revs: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Bulk query revision information for multiple documents as related.
 
         Fetch specific revisions or revision histories for multiple documents in bulk as
         replicators do.
 
@@ -1735,17 +1827,19 @@
 
         if not db:
             raise ValueError('db must be provided')
         if docs is None:
             raise ValueError('docs must be provided')
         docs = [convert_model(x) for x in docs]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_bulk_get_as_related')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_bulk_get_as_related',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'latest': latest,
             'revs': revs,
@@ -1763,33 +1857,35 @@
             del kwargs['headers']
         headers['Accept'] = 'multipart/related'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_bulk_get'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_bulk_get_as_stream(self,
+    def post_bulk_get_as_stream(
+        self,
         db: str,
         docs: List['BulkGetQueryDocument'],
         *,
         attachments: bool = None,
         att_encoding_info: bool = None,
         latest: bool = None,
         revs: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Bulk query revision information for multiple documents as stream.
 
         Fetch specific revisions or revision histories for multiple documents in bulk as
         replicators do.
 
@@ -1812,17 +1908,19 @@
 
         if not db:
             raise ValueError('db must be provided')
         if docs is None:
             raise ValueError('docs must be provided')
         docs = [convert_model(x) for x in docs]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_bulk_get_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_bulk_get_as_stream',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'latest': latest,
             'revs': revs,
@@ -1840,32 +1938,34 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_bulk_get'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def delete_document(self,
+    def delete_document(
+        self,
         db: str,
         doc_id: str,
         *,
         if_match: str = None,
         batch: str = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Delete a document.
 
         Marks the specified document as deleted by adding a `_deleted` field with the
         value `true`. Documents with this field are not returned within requests anymore
         but stay in the database. You must supply the current (latest) revision, either by
@@ -1888,17 +1988,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
             'rev': rev,
         }
 
@@ -1907,39 +2009,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_document(self,
+    def get_document(
+        self,
         db: str,
         doc_id: str,
         *,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         conflicts: bool = None,
         deleted_conflicts: bool = None,
         latest: bool = None,
         local_seq: bool = None,
         meta: bool = None,
         rev: str = None,
         revs: bool = None,
         revs_info: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a document.
 
         Returns document with the specified `doc_id` from the specified database. Unless
         you request a specific revision, the latest revision of the document is always
         returned.
@@ -1979,17 +2083,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'conflicts': conflicts,
             'deleted_conflicts': deleted_conflicts,
@@ -2006,39 +2112,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_document_as_mixed(self,
+    def get_document_as_mixed(
+        self,
         db: str,
         doc_id: str,
         *,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         conflicts: bool = None,
         deleted_conflicts: bool = None,
         latest: bool = None,
         local_seq: bool = None,
         meta: bool = None,
         rev: str = None,
         revs: bool = None,
         revs_info: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a document as mixed.
 
         Returns document with the specified `doc_id` from the specified database. Unless
         you request a specific revision, the latest revision of the document is always
         returned.
@@ -2078,17 +2186,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_document_as_mixed')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_document_as_mixed',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'conflicts': conflicts,
             'deleted_conflicts': deleted_conflicts,
@@ -2105,39 +2215,41 @@
             del kwargs['headers']
         headers['Accept'] = 'multipart/mixed'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_document_as_related(self,
+    def get_document_as_related(
+        self,
         db: str,
         doc_id: str,
         *,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         conflicts: bool = None,
         deleted_conflicts: bool = None,
         latest: bool = None,
         local_seq: bool = None,
         meta: bool = None,
         rev: str = None,
         revs: bool = None,
         revs_info: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a document as related.
 
         Returns document with the specified `doc_id` from the specified database. Unless
         you request a specific revision, the latest revision of the document is always
         returned.
@@ -2177,17 +2289,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_document_as_related')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_document_as_related',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'conflicts': conflicts,
             'deleted_conflicts': deleted_conflicts,
@@ -2204,39 +2318,41 @@
             del kwargs['headers']
         headers['Accept'] = 'multipart/related'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_document_as_stream(self,
+    def get_document_as_stream(
+        self,
         db: str,
         doc_id: str,
         *,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         conflicts: bool = None,
         deleted_conflicts: bool = None,
         latest: bool = None,
         local_seq: bool = None,
         meta: bool = None,
         rev: str = None,
         revs: bool = None,
         revs_info: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a document as stream.
 
         Returns document with the specified `doc_id` from the specified database. Unless
         you request a specific revision, the latest revision of the document is always
         returned.
@@ -2276,17 +2392,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_document_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_document_as_stream',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'conflicts': conflicts,
             'deleted_conflicts': deleted_conflicts,
@@ -2303,34 +2421,36 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def put_document(self,
+    def put_document(
+        self,
         db: str,
         doc_id: str,
         document: Union['Document', BinaryIO],
         *,
         content_type: str = None,
         if_match: str = None,
         batch: str = None,
         new_edits: bool = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create or modify a document.
 
         Creates or modifies a document in the specified database.
         For creation, you must specify the document ID but you should not specify the
         revision.
@@ -2365,17 +2485,19 @@
         if isinstance(document, Document):
             document = convert_model(document)
             content_type = content_type or 'application/json'
         headers = {
             'Content-Type': content_type,
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
             'new_edits': new_edits,
             'rev': rev,
         }
@@ -2392,34 +2514,36 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Design Documents
     #########################
 
-
-    def head_design_document(self,
+    def head_design_document(
+        self,
         db: str,
         ddoc: str,
         *,
         if_none_match: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the HTTP headers for a design document.
 
         This method supports the same query arguments as the `GET /{db}/_design/{ddoc}`
         method, but the results include only the header information (including design
         document size, and the revision as an ETag). The ETag header shows the current
@@ -2442,43 +2566,47 @@
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_design_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_design_document',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db', 'ddoc']
         path_param_values = self.encode_path_vars(db, ddoc)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def delete_design_document(self,
+    def delete_design_document(
+        self,
         db: str,
         ddoc: str,
         *,
         if_match: str = None,
         batch: str = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Delete a design document.
 
         Marks the specified design document as deleted by adding a `_deleted` field with
         the value `true`. Documents with this field are not returned with requests but
         stay in the database. You must supply the current (latest) revision, either by
@@ -2503,17 +2631,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         headers = {
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_design_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_design_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
             'rev': rev,
         }
 
@@ -2522,39 +2652,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc']
         path_param_values = self.encode_path_vars(db, ddoc)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_design_document(self,
+    def get_design_document(
+        self,
         db: str,
         ddoc: str,
         *,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         conflicts: bool = None,
         deleted_conflicts: bool = None,
         latest: bool = None,
         local_seq: bool = None,
         meta: bool = None,
         rev: str = None,
         revs: bool = None,
         revs_info: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a design document.
 
         Returns design document with the specified `doc_id` from the specified database.
         Unless you request a specific revision, the current revision of the design
         document is always returned.
@@ -2596,17 +2728,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_design_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_design_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'conflicts': conflicts,
             'deleted_conflicts': deleted_conflicts,
@@ -2623,33 +2757,35 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc']
         path_param_values = self.encode_path_vars(db, ddoc)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_design_document(self,
+    def put_design_document(
+        self,
         db: str,
         ddoc: str,
         design_document: 'DesignDocument',
         *,
         if_match: str = None,
         batch: str = None,
         new_edits: bool = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create or modify a design document.
 
         The PUT method creates a new named design document, or creates a new revision of
         the existing design document.
 
@@ -2682,17 +2818,19 @@
         if design_document is None:
             raise ValueError('design_document must be provided')
         if isinstance(design_document, DesignDocument):
             design_document = convert_model(design_document)
         headers = {
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_design_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_design_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
             'new_edits': new_edits,
             'rev': rev,
         }
@@ -2705,28 +2843,30 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc']
         path_param_values = self.encode_path_vars(db, ddoc)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_design_document_information(self,
+    def get_design_document_information(
+        self,
         db: str,
         ddoc: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about a design document.
 
         Retrieves information about the specified design document, including the index,
         index size, and current status of the design document and associated index
         information.
@@ -2741,37 +2881,41 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_design_document_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_design_document_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc']
         path_param_values = self.encode_path_vars(db, ddoc)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_info'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_design_docs(self,
+    def post_design_docs(
+        self,
         db: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
         descending: bool = None,
         include_docs: bool = None,
@@ -2780,15 +2924,15 @@
         skip: int = None,
         update_seq: bool = None,
         end_key: str = None,
         key: str = None,
         keys: List[str] = None,
         start_key: str = None,
         accept: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a list of all design documents in a database.
 
         Queries the index of all design document IDs. The results matching the request
         body parameters are returned in a JSON object, including a list of matching design
         documents with basic contents, such as the ID and revision. When no request body
@@ -2830,17 +2974,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {
             'Accept': accept,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_design_docs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_design_docs',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -2862,29 +3008,31 @@
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design_docs'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_design_docs_queries(self,
+    def post_design_docs_queries(
+        self,
         db: str,
         queries: List['AllDocsQuery'],
         *,
         accept: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Multi-query the list of all design documents.
 
         This operation runs multiple view queries of all design documents in the database.
         This operation enables you to request numerous queries in a single request, in
         place of multiple POST `/{db}/_design_docs` requests.
@@ -2905,17 +3053,19 @@
             raise ValueError('db must be provided')
         if queries is None:
             raise ValueError('queries must be provided')
         queries = [convert_model(x) for x in queries]
         headers = {
             'Accept': accept,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_design_docs_queries')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_design_docs_queries',
+        )
         headers.update(sdk_headers)
 
         data = {
             'queries': queries,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -2925,28 +3075,30 @@
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design_docs/queries'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Views
     #########################
 
-
-    def post_view(self,
+    def post_view(
+        self,
         db: str,
         ddoc: str,
         view: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
@@ -2963,15 +3115,15 @@
         key: object = None,
         keys: List[object] = None,
         reduce: bool = None,
         stable: bool = None,
         start_key: object = None,
         start_key_doc_id: str = None,
         update: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a MapReduce view.
 
         This operation queries the specified MapReduce view of the specified design
         document. By default, the map and reduce functions of the view are run to update
         the view before returning the response. The advantage of using the HTTP `POST`
@@ -3050,17 +3202,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not view:
             raise ValueError('view must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_view')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_view',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -3090,24 +3244,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'view']
         path_param_values = self.encode_path_vars(db, ddoc, view)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_view/{view}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_view_as_stream(self,
+    def post_view_as_stream(
+        self,
         db: str,
         ddoc: str,
         view: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
@@ -3124,15 +3280,15 @@
         key: object = None,
         keys: List[object] = None,
         reduce: bool = None,
         stable: bool = None,
         start_key: object = None,
         start_key_doc_id: str = None,
         update: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a MapReduce view as stream.
 
         This operation queries the specified MapReduce view of the specified design
         document. By default, the map and reduce functions of the view are run to update
         the view before returning the response. The advantage of using the HTTP `POST`
@@ -3211,17 +3367,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not view:
             raise ValueError('view must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_view_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_view_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -3251,29 +3409,31 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'view']
         path_param_values = self.encode_path_vars(db, ddoc, view)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_view/{view}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def post_view_queries(self,
+    def post_view_queries(
+        self,
         db: str,
         ddoc: str,
         view: str,
         queries: List['ViewQuery'],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Multi-query a MapReduce view.
 
         This operation runs multiple specified view queries against the view function from
         the specified design document.
 
@@ -3298,17 +3458,19 @@
             raise ValueError('ddoc must be provided')
         if not view:
             raise ValueError('view must be provided')
         if queries is None:
             raise ValueError('queries must be provided')
         queries = [convert_model(x) for x in queries]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_view_queries')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_view_queries',
+        )
         headers.update(sdk_headers)
 
         data = {
             'queries': queries,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -3319,29 +3481,31 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'view']
         path_param_values = self.encode_path_vars(db, ddoc, view)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_view/{view}/queries'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_view_queries_as_stream(self,
+    def post_view_queries_as_stream(
+        self,
         db: str,
         ddoc: str,
         view: str,
         queries: List['ViewQuery'],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Multi-query a MapReduce view as stream.
 
         This operation runs multiple specified view queries against the view function from
         the specified design document.
 
@@ -3366,17 +3530,19 @@
             raise ValueError('ddoc must be provided')
         if not view:
             raise ValueError('view must be provided')
         if queries is None:
             raise ValueError('queries must be provided')
         queries = [convert_model(x) for x in queries]
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_view_queries_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_view_queries_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'queries': queries,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -3387,31 +3553,33 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'view']
         path_param_values = self.encode_path_vars(db, ddoc, view)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_view/{view}/queries'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
     #########################
     # Queries
     #########################
 
-
-    def get_partition_information(self,
+    def get_partition_information(
+        self,
         db: str,
         partition_key: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about a database partition.
 
         Given a partition key, return the database name, sizes, partition, doc count, and
         doc delete count.
 
@@ -3424,37 +3592,41 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if not partition_key:
             raise ValueError('partition_key must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_partition_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_partition_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key']
         path_param_values = self.encode_path_vars(db, partition_key)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_partition_all_docs(self,
+    def post_partition_all_docs(
+        self,
         db: str,
         partition_key: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
         descending: bool = None,
@@ -3463,15 +3635,15 @@
         limit: int = None,
         skip: int = None,
         update_seq: bool = None,
         end_key: str = None,
         key: str = None,
         keys: List[str] = None,
         start_key: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a list of all documents in a database partition.
 
         Queries the primary index (all document IDs). The results that match the query
         parameters are returned in a JSON object, including a list of matching documents
         with basic contents, such as the ID and revision. When no query parameters are
@@ -3513,17 +3685,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if not partition_key:
             raise ValueError('partition_key must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_all_docs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_all_docs',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -3546,24 +3720,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key']
         path_param_values = self.encode_path_vars(db, partition_key)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_all_docs'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_partition_all_docs_as_stream(self,
+    def post_partition_all_docs_as_stream(
+        self,
         db: str,
         partition_key: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
         conflicts: bool = None,
         descending: bool = None,
@@ -3572,15 +3748,15 @@
         limit: int = None,
         skip: int = None,
         update_seq: bool = None,
         end_key: str = None,
         key: str = None,
         keys: List[str] = None,
         start_key: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a list of all documents in a database partition as stream.
 
         Queries the primary index (all document IDs). The results that match the query
         parameters are returned in a JSON object, including a list of matching documents
         with basic contents, such as the ID and revision. When no query parameters are
@@ -3622,17 +3798,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if not partition_key:
             raise ValueError('partition_key must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_all_docs_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_all_docs_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -3655,24 +3833,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key']
         path_param_values = self.encode_path_vars(db, partition_key)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_all_docs'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def post_partition_search(self,
+    def post_partition_search(
+        self,
         db: str,
         partition_key: str,
         ddoc: str,
         index: str,
         query: str,
         *,
         bookmark: str = None,
@@ -3682,15 +3862,15 @@
         highlight_pre_tag: str = None,
         highlight_size: int = None,
         include_docs: bool = None,
         include_fields: List[str] = None,
         limit: int = None,
         sort: List[str] = None,
         stale: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a database partition search index.
 
         Partitioned Search indexes, which are defined in design documents, allow partition
         databases to be queried by using Lucene Query Parser Syntax. Search indexes are
         defined by an index function, similar to a map function in MapReduce views. The
@@ -3750,17 +3930,19 @@
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not index:
             raise ValueError('index must be provided')
         if query is None:
             raise ValueError('query must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_search')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_search',
+        )
         headers.update(sdk_headers)
 
         data = {
             'query': query,
             'bookmark': bookmark,
             'highlight_fields': highlight_fields,
             'highlight_number': highlight_number,
@@ -3782,24 +3964,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key', 'ddoc', 'index']
         path_param_values = self.encode_path_vars(db, partition_key, ddoc, index)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_design/{ddoc}/_search/{index}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_partition_search_as_stream(self,
+    def post_partition_search_as_stream(
+        self,
         db: str,
         partition_key: str,
         ddoc: str,
         index: str,
         query: str,
         *,
         bookmark: str = None,
@@ -3809,15 +3993,15 @@
         highlight_pre_tag: str = None,
         highlight_size: int = None,
         include_docs: bool = None,
         include_fields: List[str] = None,
         limit: int = None,
         sort: List[str] = None,
         stale: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a database partition search index as stream.
 
         Partitioned Search indexes, which are defined in design documents, allow partition
         databases to be queried by using Lucene Query Parser Syntax. Search indexes are
         defined by an index function, similar to a map function in MapReduce views. The
@@ -3877,17 +4061,19 @@
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not index:
             raise ValueError('index must be provided')
         if query is None:
             raise ValueError('query must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_search_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_search_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'query': query,
             'bookmark': bookmark,
             'highlight_fields': highlight_fields,
             'highlight_number': highlight_number,
@@ -3909,24 +4095,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key', 'ddoc', 'index']
         path_param_values = self.encode_path_vars(db, partition_key, ddoc, index)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_design/{ddoc}/_search/{index}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def post_partition_view(self,
+    def post_partition_view(
+        self,
         db: str,
         partition_key: str,
         ddoc: str,
         view: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
@@ -3943,15 +4131,15 @@
         group_level: int = None,
         key: object = None,
         keys: List[object] = None,
         reduce: bool = None,
         start_key: object = None,
         start_key_doc_id: str = None,
         update: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a database partition MapReduce view function.
 
         Runs the specified view function from the specified design document. Unlike `GET
         /{db}/_design/{ddoc}/_view/{view}` for accessing views, the POST method supports
         the specification of explicit keys to be retrieved from the view results. The
@@ -4024,17 +4212,19 @@
         if not partition_key:
             raise ValueError('partition_key must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not view:
             raise ValueError('view must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_view')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_view',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -4063,24 +4253,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key', 'ddoc', 'view']
         path_param_values = self.encode_path_vars(db, partition_key, ddoc, view)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_design/{ddoc}/_view/{view}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_partition_view_as_stream(self,
+    def post_partition_view_as_stream(
+        self,
         db: str,
         partition_key: str,
         ddoc: str,
         view: str,
         *,
         att_encoding_info: bool = None,
         attachments: bool = None,
@@ -4097,15 +4289,15 @@
         group_level: int = None,
         key: object = None,
         keys: List[object] = None,
         reduce: bool = None,
         start_key: object = None,
         start_key_doc_id: str = None,
         update: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a database partition MapReduce view function as stream.
 
         Runs the specified view function from the specified design document. Unlike `GET
         /{db}/_design/{ddoc}/_view/{view}` for accessing views, the POST method supports
         the specification of explicit keys to be retrieved from the view results. The
@@ -4178,17 +4370,19 @@
         if not partition_key:
             raise ValueError('partition_key must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not view:
             raise ValueError('view must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_view_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_view_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'att_encoding_info': att_encoding_info,
             'attachments': attachments,
             'conflicts': conflicts,
             'descending': descending,
@@ -4217,39 +4411,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key', 'ddoc', 'view']
         path_param_values = self.encode_path_vars(db, partition_key, ddoc, view)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_design/{ddoc}/_view/{view}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def post_partition_find(self,
+    def post_partition_find(
+        self,
         db: str,
         partition_key: str,
         selector: dict,
         *,
         bookmark: str = None,
         conflicts: bool = None,
         execution_stats: bool = None,
         fields: List[str] = None,
         limit: int = None,
         skip: int = None,
         sort: List[dict] = None,
         stable: bool = None,
         update: str = None,
         use_index: List[str] = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a database partition index by using selector syntax.
 
         Query documents by using a declarative JSON querying syntax. It's best practice to
         create an appropriate index for all fields in selector by using the `_index`
         endpoint.
@@ -4334,17 +4530,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not partition_key:
             raise ValueError('partition_key must be provided')
         if selector is None:
             raise ValueError('selector must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_find')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_find',
+        )
         headers.update(sdk_headers)
 
         data = {
             'selector': selector,
             'bookmark': bookmark,
             'conflicts': conflicts,
             'execution_stats': execution_stats,
@@ -4365,39 +4563,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key']
         path_param_values = self.encode_path_vars(db, partition_key)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_find'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_partition_find_as_stream(self,
+    def post_partition_find_as_stream(
+        self,
         db: str,
         partition_key: str,
         selector: dict,
         *,
         bookmark: str = None,
         conflicts: bool = None,
         execution_stats: bool = None,
         fields: List[str] = None,
         limit: int = None,
         skip: int = None,
         sort: List[dict] = None,
         stable: bool = None,
         update: str = None,
         use_index: List[str] = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a database partition index by using selector syntax as stream.
 
         Query documents by using a declarative JSON querying syntax. It's best practice to
         create an appropriate index for all fields in selector by using the `_index`
         endpoint.
@@ -4482,17 +4682,19 @@
         if not db:
             raise ValueError('db must be provided')
         if not partition_key:
             raise ValueError('partition_key must be provided')
         if selector is None:
             raise ValueError('selector must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_partition_find_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_partition_find_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'selector': selector,
             'bookmark': bookmark,
             'conflicts': conflicts,
             'execution_stats': execution_stats,
@@ -4513,43 +4715,45 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'partition_key']
         path_param_values = self.encode_path_vars(db, partition_key)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_partition/{partition_key}/_find'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
     #########################
     # Queries
     #########################
 
-
-    def post_explain(self,
+    def post_explain(
+        self,
         db: str,
         selector: dict,
         *,
         bookmark: str = None,
         conflicts: bool = None,
         execution_stats: bool = None,
         fields: List[str] = None,
         limit: int = None,
         skip: int = None,
         sort: List[dict] = None,
         stable: bool = None,
         update: str = None,
         use_index: List[str] = None,
         r: int = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about which index is used for a query.
 
         Shows which index is being used by the query. Parameters are the same as the
         [`_find` endpoint](#query-an-index-by-using-selector-syntax).
 
@@ -4631,17 +4835,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if selector is None:
             raise ValueError('selector must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_explain')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_explain',
+        )
         headers.update(sdk_headers)
 
         data = {
             'selector': selector,
             'bookmark': bookmark,
             'conflicts': conflicts,
             'execution_stats': execution_stats,
@@ -4663,39 +4869,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_explain'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_find(self,
+    def post_find(
+        self,
         db: str,
         selector: dict,
         *,
         bookmark: str = None,
         conflicts: bool = None,
         execution_stats: bool = None,
         fields: List[str] = None,
         limit: int = None,
         skip: int = None,
         sort: List[dict] = None,
         stable: bool = None,
         update: str = None,
         use_index: List[str] = None,
         r: int = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query an index by using selector syntax.
 
         Query documents by using a declarative JSON querying syntax. It's best practice to
         create an appropriate index for all fields in selector by using the `_index`
         endpoint.
@@ -4783,17 +4991,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if selector is None:
             raise ValueError('selector must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_find')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_find',
+        )
         headers.update(sdk_headers)
 
         data = {
             'selector': selector,
             'bookmark': bookmark,
             'conflicts': conflicts,
             'execution_stats': execution_stats,
@@ -4815,39 +5025,41 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_find'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_find_as_stream(self,
+    def post_find_as_stream(
+        self,
         db: str,
         selector: dict,
         *,
         bookmark: str = None,
         conflicts: bool = None,
         execution_stats: bool = None,
         fields: List[str] = None,
         limit: int = None,
         skip: int = None,
         sort: List[dict] = None,
         stable: bool = None,
         update: str = None,
         use_index: List[str] = None,
         r: int = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query an index by using selector syntax as stream.
 
         Query documents by using a declarative JSON querying syntax. It's best practice to
         create an appropriate index for all fields in selector by using the `_index`
         endpoint.
@@ -4935,17 +5147,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if selector is None:
             raise ValueError('selector must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_find_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_find_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'selector': selector,
             'bookmark': bookmark,
             'conflicts': conflicts,
             'execution_stats': execution_stats,
@@ -4967,26 +5181,28 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_find'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def get_indexes_information(self,
+    def get_indexes_information(
+        self,
         db: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about all indexes.
 
         When you make a GET request to `/db/_index`, you get a list of all indexes used by
         Cloudant Query in the database, including the primary index. In addition to the
         information available through this API, indexes are also stored in the `indexes`
@@ -4997,46 +5213,50 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `IndexesInformation` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_indexes_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_indexes_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_index'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_index(self,
+    def post_index(
+        self,
         db: str,
         index: 'IndexDefinition',
         *,
         ddoc: str = None,
         def_: 'IndexDefinition' = None,
         name: str = None,
         partitioned: bool = None,
         type: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create a new index on a database.
 
         Create a new index on a database.
 
         :param str db: Path parameter to specify the database name.
@@ -5069,17 +5289,19 @@
             raise ValueError('db must be provided')
         if index is None:
             raise ValueError('index must be provided')
         index = convert_model(index)
         if def_ is not None:
             def_ = convert_model(def_)
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_index')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_index',
+        )
         headers.update(sdk_headers)
 
         data = {
             'index': index,
             'ddoc': ddoc,
             'def': def_,
             'name': name,
@@ -5095,29 +5317,31 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_index'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def delete_index(self,
+    def delete_index(
+        self,
         db: str,
         ddoc: str,
         type: str,
         index: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Delete an index.
 
         :param str db: Path parameter to specify the database name.
         :param str ddoc: Path parameter to specify the design document name. The
                design document name is the design document ID excluding the `_design/`
@@ -5134,44 +5358,48 @@
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not type:
             raise ValueError('type must be provided')
         if not index:
             raise ValueError('index must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_index')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_index',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'type', 'index']
         path_param_values = self.encode_path_vars(db, ddoc, type, index)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_index/_design/{ddoc}/{type}/{index}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Searches
     #########################
 
-
-    def post_search_analyze(self,
+    def post_search_analyze(
+        self,
         analyzer: str,
         text: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query tokenization of sample text.
 
         Returns the results of analyzer tokenization of the provided sample text. This
         endpoint can be used for testing analyzer tokenization.
 
@@ -5184,17 +5412,19 @@
         """
 
         if analyzer is None:
             raise ValueError('analyzer must be provided')
         if text is None:
             raise ValueError('text must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_search_analyze')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_search_analyze',
+        )
         headers.update(sdk_headers)
 
         data = {
             'analyzer': analyzer,
             'text': text,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
@@ -5203,24 +5433,26 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_search_analyze'
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_search(self,
+    def post_search(
+        self,
         db: str,
         ddoc: str,
         index: str,
         query: str,
         *,
         bookmark: str = None,
         highlight_fields: List[str] = None,
@@ -5235,15 +5467,15 @@
         stale: str = None,
         counts: List[str] = None,
         drilldown: List[List[str]] = None,
         group_field: str = None,
         group_limit: int = None,
         group_sort: List[str] = None,
         ranges: dict = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a search index.
 
         Search indexes, which are defined in design documents, allow databases to be
         queried by using Lucene Query Parser Syntax. An index function defines a search
         index, similar to a map function in MapReduce views. The index function decides
@@ -5331,17 +5563,19 @@
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not index:
             raise ValueError('index must be provided')
         if query is None:
             raise ValueError('query must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_search')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_search',
+        )
         headers.update(sdk_headers)
 
         data = {
             'query': query,
             'bookmark': bookmark,
             'highlight_fields': highlight_fields,
             'highlight_number': highlight_number,
@@ -5369,24 +5603,26 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'index']
         path_param_values = self.encode_path_vars(db, ddoc, index)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_search/{index}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_search_as_stream(self,
+    def post_search_as_stream(
+        self,
         db: str,
         ddoc: str,
         index: str,
         query: str,
         *,
         bookmark: str = None,
         highlight_fields: List[str] = None,
@@ -5401,15 +5637,15 @@
         stale: str = None,
         counts: List[str] = None,
         drilldown: List[List[str]] = None,
         group_field: str = None,
         group_limit: int = None,
         group_sort: List[str] = None,
         ranges: dict = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query a search index as stream.
 
         Search indexes, which are defined in design documents, allow databases to be
         queried by using Lucene Query Parser Syntax. An index function defines a search
         index, similar to a map function in MapReduce views. The index function decides
@@ -5497,17 +5733,19 @@
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not index:
             raise ValueError('index must be provided')
         if query is None:
             raise ValueError('query must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_search_as_stream')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_search_as_stream',
+        )
         headers.update(sdk_headers)
 
         data = {
             'query': query,
             'bookmark': bookmark,
             'highlight_fields': highlight_fields,
             'highlight_number': highlight_number,
@@ -5535,28 +5773,30 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'index']
         path_param_values = self.encode_path_vars(db, ddoc, index)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_search/{index}'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, stream=True, **kwargs)
         return response
 
-
-    def get_search_info(self,
+    def get_search_info(
+        self,
         db: str,
         ddoc: str,
         index: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about a search index.
 
         Retrieve search index metadata information, such as the size of the index on disk.
 
         :param str db: Path parameter to specify the database name.
@@ -5572,45 +5812,49 @@
         if not db:
             raise ValueError('db must be provided')
         if not ddoc:
             raise ValueError('ddoc must be provided')
         if not index:
             raise ValueError('index must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_search_info')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_search_info',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'ddoc', 'index']
         path_param_values = self.encode_path_vars(db, ddoc, index)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_design/{ddoc}/_search_info/{index}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Replication
     #########################
 
-
-    def head_replication_document(self,
+    def head_replication_document(
+        self,
         doc_id: str,
         *,
         if_none_match: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the HTTP headers for a replication document.
 
         Retrieves the HTTP headers containing minimal amount of information about the
         specified replication document from the `_replicator` database.  The method
         supports the same query arguments as the `GET /_replicator/{doc_id}` method, but
@@ -5625,38 +5869,42 @@
         """
 
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_replication_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_replication_document',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['doc_id']
         path_param_values = self.encode_path_vars(doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_replicator/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def head_scheduler_document(self,
+    def head_scheduler_document(
+        self,
         doc_id: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve HTTP headers for a replication scheduler document.
 
         Retrieves the HTTP headers containing minimal amount of information about the
         specified replication scheduler document.  Since the response body is empty, using
         the HEAD method is a lightweight way to check if the replication scheduler
@@ -5667,38 +5915,42 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_scheduler_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_scheduler_document',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['doc_id']
         path_param_values = self.encode_path_vars(doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_scheduler/docs/_replicator/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def head_scheduler_job(self,
+    def head_scheduler_job(
+        self,
         job_id: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the HTTP headers for a replication scheduler job.
 
         Returns the HTTP headers that contain a minimal amount of information about the
         specified replication task. Only the header information is returned.
 
@@ -5707,42 +5959,46 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not job_id:
             raise ValueError('job_id must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_scheduler_job')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_scheduler_job',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['job_id']
         path_param_values = self.encode_path_vars(job_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_scheduler/jobs/{job_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def delete_replication_document(self,
+    def delete_replication_document(
+        self,
         doc_id: str,
         *,
         if_match: str = None,
         batch: str = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Cancel a replication.
 
         Cancels a replication by deleting the document that describes it from the
         `_replicator` database.
 
@@ -5759,17 +6015,19 @@
         """
 
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_replication_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_replication_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
             'rev': rev,
         }
 
@@ -5778,38 +6036,40 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['doc_id']
         path_param_values = self.encode_path_vars(doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_replicator/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_replication_document(self,
+    def get_replication_document(
+        self,
         doc_id: str,
         *,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         conflicts: bool = None,
         deleted_conflicts: bool = None,
         latest: bool = None,
         local_seq: bool = None,
         meta: bool = None,
         rev: str = None,
         revs: bool = None,
         revs_info: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a replication document.
 
         Retrieves a replication document from the `_replicator` database to view the
         configuration of the replication. The status of the replication is no longer
         recorded in the document but can be checked via the replication scheduler.
@@ -5846,17 +6106,19 @@
         """
 
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_replication_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_replication_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'conflicts': conflicts,
             'deleted_conflicts': deleted_conflicts,
@@ -5873,32 +6135,34 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['doc_id']
         path_param_values = self.encode_path_vars(doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_replicator/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_replication_document(self,
+    def put_replication_document(
+        self,
         doc_id: str,
         replication_document: 'ReplicationDocument',
         *,
         if_match: str = None,
         batch: str = None,
         new_edits: bool = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create or modify a replication using a replication document.
 
         Creates or modifies a document in the `_replicator` database to start a new
         replication or to edit an existing replication.
 
@@ -5926,17 +6190,19 @@
         if replication_document is None:
             raise ValueError('replication_document must be provided')
         if isinstance(replication_document, ReplicationDocument):
             replication_document = convert_model(replication_document)
         headers = {
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_replication_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_replication_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
             'new_edits': new_edits,
             'rev': rev,
         }
@@ -5949,30 +6215,32 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['doc_id']
         path_param_values = self.encode_path_vars(doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_replicator/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_scheduler_docs(self,
+    def get_scheduler_docs(
+        self,
         *,
         limit: int = None,
         skip: int = None,
         states: List[str] = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve replication scheduler documents.
 
         Lists replication documents, including information about all documents, even the
         ones in a completed or failed state. For each document, the endpoint returns the
         document ID, database, replication ID, source and target, and other information.
@@ -5986,43 +6254,47 @@
                comma-delimited string.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SchedulerDocsResult` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_scheduler_docs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_scheduler_docs',
+        )
         headers.update(sdk_headers)
 
         params = {
             'limit': limit,
             'skip': skip,
             'states': convert_list(states),
         }
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_scheduler/docs'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_scheduler_document(self,
+    def get_scheduler_document(
+        self,
         doc_id: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a replication scheduler document.
 
         Retrieves information about a replication document from the replicator database.
         The endpoint returns the document ID, database, replication ID, source and target,
         and other information.
@@ -6032,41 +6304,45 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SchedulerDocument` object
         """
 
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_scheduler_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_scheduler_document',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['doc_id']
         path_param_values = self.encode_path_vars(doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_scheduler/docs/_replicator/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_scheduler_jobs(self,
+    def get_scheduler_jobs(
+        self,
         *,
         limit: int = None,
         skip: int = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve replication scheduler jobs.
 
         Retrieves information about replications that were created via `/_replicate`
         endpoint, as well as those created from replication documents. It doesn't include
         replications that completed or failed to start because replication documents were
@@ -6079,42 +6355,46 @@
                records before starting to return the results.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SchedulerJobsResult` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_scheduler_jobs')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_scheduler_jobs',
+        )
         headers.update(sdk_headers)
 
         params = {
             'limit': limit,
             'skip': skip,
         }
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_scheduler/jobs'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_scheduler_job(self,
+    def get_scheduler_job(
+        self,
         job_id: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a replication scheduler job.
 
         Retrieves the state of a single replication task based on its replication ID.
 
         :param str job_id: Path parameter to specify the replication job id.
@@ -6122,80 +6402,88 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SchedulerJob` object
         """
 
         if not job_id:
             raise ValueError('job_id must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_scheduler_job')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_scheduler_job',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['job_id']
         path_param_values = self.encode_path_vars(job_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_scheduler/jobs/{job_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Authentication
     #########################
 
-
-    def get_session_information(self,
-        **kwargs
+    def get_session_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve current session cookie information.
 
         Retrieves information about the authenticated user's session.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `SessionInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_session_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_session_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_session'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Authorization
     #########################
 
-
-    def get_security(self,
+    def get_security(
+        self,
         db: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve database permissions information.
 
         See who has permission to read, write, and manage the database. The credentials
         you use to log in to the dashboard automatically include `_admin` permissions to
         all databases you create. Everyone and everything else, including users you share
@@ -6207,44 +6495,48 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Security` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_security')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_security',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_security'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_security(self,
+    def put_security(
+        self,
         db: str,
         *,
         admins: 'SecurityObject' = None,
         members: 'SecurityObject' = None,
         cloudant: dict = None,
         couchdb_auth_only: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Modify database permissions.
 
         Modify who has permission to read, write, or manage a database. This endpoint can
         be used to modify both Cloudant and CouchDB related permissions. Be careful: by
         removing a Cloudant API key, a member or an admin from the list of users that have
@@ -6273,17 +6565,19 @@
         if not db:
             raise ValueError('db must be provided')
         if admins is not None:
             admins = convert_model(admins)
         if members is not None:
             members = convert_model(members)
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_security')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_security',
+        )
         headers.update(sdk_headers)
 
         data = {
             'admins': admins,
             'members': members,
             'cloudant': cloudant,
             'couchdb_auth_only': couchdb_auth_only,
@@ -6297,25 +6591,27 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_security'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_api_keys(self,
-        **kwargs
+    def post_api_keys(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Generates API keys for apps or persons to enable database access.
 
         Generates API keys to enable database access for a person or application, but
         without creating a new IBM Cloudant account for that person or application. An API
         key is a randomly generated username and password. The key is given the wanted
@@ -6323,41 +6619,45 @@
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ApiKeysResult` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_api_keys')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_api_keys',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/api_keys'
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_cloudant_security_configuration(self,
+    def put_cloudant_security_configuration(
+        self,
         db: str,
         cloudant: dict,
         *,
         admins: 'SecurityObject' = None,
         members: 'SecurityObject' = None,
         couchdb_auth_only: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Modify only Cloudant related database permissions.
 
         Modify only Cloudant related permissions to database. Be careful: by removing an
         API key from the list, you remove the API key from the list of users that have
         access to the database.
@@ -6386,17 +6686,19 @@
         if cloudant is None:
             raise ValueError('cloudant must be provided')
         if admins is not None:
             admins = convert_model(admins)
         if members is not None:
             members = convert_model(members)
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_cloudant_security_configuration')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_cloudant_security_configuration',
+        )
         headers.update(sdk_headers)
 
         data = {
             'cloudant': cloudant,
             'admins': admins,
             'members': members,
             'couchdb_auth_only': couchdb_auth_only,
@@ -6410,68 +6712,74 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/_api/v2/db/{db}/_security'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # CORS
     #########################
 
-
-    def get_cors_information(self,
-        **kwargs
+    def get_cors_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve CORS configuration information.
 
         Lists all Cross-origin resource sharing (CORS) configuration. CORS defines a way
         in which the browser and the server interact to determine whether or not to allow
         the request.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CorsInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_cors_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_cors_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/config/cors'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_cors_configuration(self,
+    def put_cors_configuration(
+        self,
         origins: List[str],
         *,
         allow_credentials: bool = None,
         enable_cors: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Modify CORS configuration.
 
         Sets the CORS configuration. The configuration applies to all databases and all
         account level endpoints in your account.
 
@@ -6487,17 +6795,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Ok` object
         """
 
         if origins is None:
             raise ValueError('origins must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_cors_configuration')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_cors_configuration',
+        )
         headers.update(sdk_headers)
 
         data = {
             'origins': origins,
             'allow_credentials': allow_credentials,
             'enable_cors': enable_cors,
         }
@@ -6507,36 +6817,38 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/config/cors'
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Attachments
     #########################
 
-
-    def head_attachment(self,
+    def head_attachment(
+        self,
         db: str,
         doc_id: str,
         attachment_name: str,
         *,
         if_match: str = None,
         if_none_match: str = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the HTTP headers for an attachment.
 
         Returns the HTTP headers that contain a minimal amount of information about the
         specified attachment. This method supports the same query arguments as the `GET
         /{db}/{doc_id}/{attachment_name}` method, but only the header information
@@ -6561,49 +6873,53 @@
             raise ValueError('doc_id must be provided')
         if not attachment_name:
             raise ValueError('attachment_name must be provided')
         headers = {
             'If-Match': if_match,
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_attachment')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_attachment',
+        )
         headers.update(sdk_headers)
 
         params = {
             'rev': rev,
         }
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db', 'doc_id', 'attachment_name']
         path_param_values = self.encode_path_vars(db, doc_id, attachment_name)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}/{attachment_name}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def delete_attachment(self,
+    def delete_attachment(
+        self,
         db: str,
         doc_id: str,
         attachment_name: str,
         *,
         if_match: str = None,
         rev: str = None,
         batch: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Delete an attachment.
 
         Deletes the attachment with the filename, `{attachment_name}`, from the specified
         doc. You must supply the `rev` query parameter or `If-Match` header with the
         current revision to delete the attachment.
@@ -6627,17 +6943,19 @@
         if not doc_id:
             raise ValueError('doc_id must be provided')
         if not attachment_name:
             raise ValueError('attachment_name must be provided')
         headers = {
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_attachment')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_attachment',
+        )
         headers.update(sdk_headers)
 
         params = {
             'rev': rev,
             'batch': batch,
         }
 
@@ -6646,33 +6964,35 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id', 'attachment_name']
         path_param_values = self.encode_path_vars(db, doc_id, attachment_name)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}/{attachment_name}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_attachment(self,
+    def get_attachment(
+        self,
         db: str,
         doc_id: str,
         attachment_name: str,
         *,
         if_match: str = None,
         if_none_match: str = None,
         range: str = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve an attachment.
 
         Returns the file attachment that is associated with the document. The raw data of
         the associated attachment is returned, just as if you were accessing a static
         file. The returned Content-Type header is the same as the content type set when
@@ -6701,17 +7021,19 @@
         if not attachment_name:
             raise ValueError('attachment_name must be provided')
         headers = {
             'If-Match': if_match,
             'If-None-Match': if_none_match,
             'Range': range,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_attachment')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_attachment',
+        )
         headers.update(sdk_headers)
 
         params = {
             'rev': rev,
         }
 
         if 'headers' in kwargs:
@@ -6719,33 +7041,35 @@
             del kwargs['headers']
         headers['Accept'] = '*/*'
 
         path_param_keys = ['db', 'doc_id', 'attachment_name']
         path_param_values = self.encode_path_vars(db, doc_id, attachment_name)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}/{attachment_name}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_attachment(self,
+    def put_attachment(
+        self,
         db: str,
         doc_id: str,
         attachment_name: str,
         attachment: BinaryIO,
         content_type: str,
         *,
         if_match: str = None,
         rev: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create or modify an attachment.
 
         Uploads the supplied content as an attachment to the specified document. The
         attachment name that you provide must be a URL encoded string. You must supply the
         Content-Type header, and for an existing document, you must also supply either the
@@ -6779,17 +7103,19 @@
             raise ValueError('attachment must be provided')
         if not content_type:
             raise ValueError('content_type must be provided')
         headers = {
             'Content-Type': content_type,
             'If-Match': if_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_attachment')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_attachment',
+        )
         headers.update(sdk_headers)
 
         params = {
             'rev': rev,
         }
 
         data = attachment
@@ -6799,34 +7125,36 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id', 'attachment_name']
         path_param_values = self.encode_path_vars(db, doc_id, attachment_name)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/{doc_id}/{attachment_name}'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Local Documents
     #########################
 
-
-    def head_local_document(self,
+    def head_local_document(
+        self,
         db: str,
         doc_id: str,
         *,
         if_none_match: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve HTTP headers for a local document.
 
         Retrieves the HTTP headers containing minimal amount of information about the
         specified local document. Since the response body is empty, using the HEAD method
         is a lightweight way to check if the local document exists or not.
@@ -6843,41 +7171,45 @@
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_local_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_local_document',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_local/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def delete_local_document(self,
+    def delete_local_document(
+        self,
         db: str,
         doc_id: str,
         *,
         batch: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Delete a local document.
 
         Deletes the specified local document. The semantics are identical to deleting a
         standard document in the specified database, except that the document is not
         replicated.
@@ -6893,17 +7225,19 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='delete_local_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_local_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
         }
 
         if 'headers' in kwargs:
@@ -6911,33 +7245,35 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_local/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='DELETE',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_local_document(self,
+    def get_local_document(
+        self,
         db: str,
         doc_id: str,
         *,
         accept: str = None,
         if_none_match: str = None,
         attachments: bool = None,
         att_encoding_info: bool = None,
         local_seq: bool = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve a local document.
 
         Retrieves the specified local document. The semantics are identical to accessing a
         standard document in the specified database, except that the document is not
         replicated.
@@ -6964,17 +7300,19 @@
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {
             'Accept': accept,
             'If-None-Match': if_none_match,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_local_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_local_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'attachments': attachments,
             'att_encoding_info': att_encoding_info,
             'local_seq': local_seq,
         }
@@ -6983,31 +7321,33 @@
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_local/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers,
-                                       params=params)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def put_local_document(self,
+    def put_local_document(
+        self,
         db: str,
         doc_id: str,
         document: Union['Document', BinaryIO],
         *,
         content_type: str = None,
         batch: str = None,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Create or modify a local document.
 
         Stores the specified local document. The semantics are identical to storing a
         standard document in the specified database, except that the document is not
         replicated.
@@ -7032,17 +7372,19 @@
             raise ValueError('document must be provided')
         if isinstance(document, Document):
             document = convert_model(document)
             content_type = content_type or 'application/json'
         headers = {
             'Content-Type': content_type,
         }
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='put_local_document')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='put_local_document',
+        )
         headers.update(sdk_headers)
 
         params = {
             'batch': batch,
         }
 
         if isinstance(document, dict):
@@ -7057,32 +7399,34 @@
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_local/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='PUT',
-                                       url=url,
-                                       headers=headers,
-                                       params=params,
-                                       data=data)
+        request = self.prepare_request(
+            method='PUT',
+            url=url,
+            headers=headers,
+            params=params,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Database Details
     #########################
 
-
-    def post_revs_diff(self,
+    def post_revs_diff(
+        self,
         db: str,
         document_revisions: dict,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Query the document revisions and possible ancestors missing from the database.
 
         The replicator is the primary user of this operation. After receiving a set of new
         revision IDs from the source database, the replicator sends this set to the
         destination database's `_revs_diff` to find out which of them already exists
@@ -7097,43 +7441,47 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if document_revisions is None:
             raise ValueError('document_revisions must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_revs_diff')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_revs_diff',
+        )
         headers.update(sdk_headers)
 
         data = json.dumps(document_revisions)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_revs_diff'.format(**path_param_dict)
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_shards_information(self,
+    def get_shards_information(
+        self,
         db: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve shard information.
 
         List each shard range and the corresponding replicas for a specified database.
 
         :param str db: Path parameter to specify the database name.
@@ -7141,40 +7489,44 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ShardsInformation` object
         """
 
         if not db:
             raise ValueError('db must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_shards_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_shards_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db']
         path_param_values = self.encode_path_vars(db)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_shards'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_document_shards_info(self,
+    def get_document_shards_info(
+        self,
         db: str,
         doc_id: str,
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve shard information for a specific document.
 
         Retrieves information about a specific shard where a particular document is
         stored, along with information about the nodes where that shard has a replica.
 
@@ -7186,74 +7538,82 @@
         """
 
         if not db:
             raise ValueError('db must be provided')
         if not doc_id:
             raise ValueError('doc_id must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_document_shards_info')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_document_shards_info',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         path_param_keys = ['db', 'doc_id']
         path_param_values = self.encode_path_vars(db, doc_id)
         path_param_dict = dict(zip(path_param_keys, path_param_values))
         url = '/{db}/_shards/{doc_id}'.format(**path_param_dict)
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
     #########################
     # Monitoring
     #########################
 
-
-    def head_up_information(self,
-        **kwargs
+    def head_up_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve HTTP headers about whether the server is up.
 
         Retrieves the HTTP headers about whether the server is up.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='head_up_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='head_up_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
 
         url = '/_up'
-        request = self.prepare_request(method='HEAD',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='HEAD',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_active_tasks(self,
-        **kwargs
+    def get_active_tasks(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve list of running tasks.
 
         Lists running tasks, including the task type, name, status, and process ID. The
         result includes a JSON array of the currently running tasks, with each task
         described as a single object. Depending on the operation type, the set of response
@@ -7261,105 +7621,117 @@
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `List[ActiveTask]` result
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_active_tasks')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_active_tasks',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_active_tasks'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_up_information(self,
-        **kwargs
+    def get_up_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve information about whether the server is up.
 
         Confirms that the server is up, running, and ready to respond to requests. If
         `maintenance_mode` is `true` or `nolb`, the endpoint returns a 404 response.
         **Tip:**  The authentication for this endpoint is only enforced when using IAM.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `UpInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_up_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_up_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_up'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_activity_tracker_events(self,
-        **kwargs
+    def get_activity_tracker_events(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve Activity Tracker events information.
 
         Check event types that are being sent to IBM Cloud Activity Tracker for the IBM
         Cloudant instance.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ActivityTrackerEvents` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_activity_tracker_events')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_activity_tracker_events',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/activity_tracker/events'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def post_activity_tracker_events(self,
+    def post_activity_tracker_events(
+        self,
         types: List[str],
-        **kwargs
+        **kwargs,
     ) -> DetailedResponse:
         """
         Modify Activity Tracker events configuration.
 
         Configure event types that are being sent to IBM Cloud Activity Tracker for the
         IBM Cloudant instance.
 
@@ -7370,17 +7742,19 @@
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Ok` object
         """
 
         if types is None:
             raise ValueError('types must be provided')
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='post_activity_tracker_events')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='post_activity_tracker_events',
+        )
         headers.update(sdk_headers)
 
         data = {
             'types': types,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -7388,67 +7762,74 @@
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/activity_tracker/events'
-        request = self.prepare_request(method='POST',
-                                       url=url,
-                                       headers=headers,
-                                       data=data)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
-
-    def get_current_throughput_information(self,
-        **kwargs
+    def get_current_throughput_information(
+        self,
+        **kwargs,
     ) -> DetailedResponse:
         """
         Retrieve the current provisioned throughput capacity consumption.
 
         View the current consumption of provisioned throughput capacity for an IBM
         Cloudant instance. The current consumption shows the quantities of reads, writes,
         and global queries conducted against the instance for a given second.
 
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CurrentThroughputInformation` object
         """
 
         headers = {}
-        sdk_headers = get_sdk_headers(service_name=self.DEFAULT_SERVICE_NAME,
-                                      service_version='V1',
-                                      operation_id='get_current_throughput_information')
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_current_throughput_information',
+        )
         headers.update(sdk_headers)
 
         if 'headers' in kwargs:
             headers.update(kwargs.get('headers'))
             del kwargs['headers']
         headers['Accept'] = 'application/json'
 
         url = '/_api/v2/user/current/throughput'
-        request = self.prepare_request(method='GET',
-                                       url=url,
-                                       headers=headers)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
 
         response = self.send(request, **kwargs)
         return response
 
 
 class GetDbUpdatesEnums:
     """
     Enums for get_db_updates parameters.
     """
 
     class Feed(str, Enum):
         """
         Query parameter to specify the changes feed type.
         """
+
         CONTINUOUS = 'continuous'
         EVENTSOURCE = 'eventsource'
         LONGPOLL = 'longpoll'
         NORMAL = 'normal'
 
 
 class PostChangesEnums:
@@ -7456,14 +7837,15 @@
     Enums for post_changes parameters.
     """
 
     class Feed(str, Enum):
         """
         Query parameter to specify the changes feed type.
         """
+
         CONTINUOUS = 'continuous'
         EVENTSOURCE = 'eventsource'
         LONGPOLL = 'longpoll'
         NORMAL = 'normal'
 
 
 class PostChangesAsStreamEnums:
@@ -7471,14 +7853,15 @@
     Enums for post_changes_as_stream parameters.
     """
 
     class Feed(str, Enum):
         """
         Query parameter to specify the changes feed type.
         """
+
         CONTINUOUS = 'continuous'
         EVENTSOURCE = 'eventsource'
         LONGPOLL = 'longpoll'
         NORMAL = 'normal'
 
 
 class PostDocumentEnums:
@@ -7486,121 +7869,131 @@
     Enums for post_document parameters.
     """
 
     class ContentType(str, Enum):
         """
         The type of the input.
         """
+
         APPLICATION_JSON = 'application/json'
         MULTIPART_MIXED = 'multipart/mixed'
         MULTIPART_RELATED = 'multipart/related'
         APPLICATION_OCTET_STREAM = 'application/octet-stream'
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class DeleteDocumentEnums:
     """
     Enums for delete_document parameters.
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class PutDocumentEnums:
     """
     Enums for put_document parameters.
     """
 
     class ContentType(str, Enum):
         """
         The type of the input.
         """
+
         APPLICATION_JSON = 'application/json'
         MULTIPART_MIXED = 'multipart/mixed'
         MULTIPART_RELATED = 'multipart/related'
         APPLICATION_OCTET_STREAM = 'application/octet-stream'
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class DeleteDesignDocumentEnums:
     """
     Enums for delete_design_document parameters.
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class PutDesignDocumentEnums:
     """
     Enums for put_design_document parameters.
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class PostDesignDocsEnums:
     """
     Enums for post_design_docs parameters.
     """
 
     class Accept(str, Enum):
         """
         The type of the response: application/json or application/octet-stream.
         """
+
         APPLICATION_JSON = 'application/json'
         APPLICATION_OCTET_STREAM = 'application/octet-stream'
 
 
 class PostDesignDocsQueriesEnums:
     """
     Enums for post_design_docs_queries parameters.
     """
 
     class Accept(str, Enum):
         """
         The type of the response: application/json or application/octet-stream.
         """
+
         APPLICATION_JSON = 'application/json'
         APPLICATION_OCTET_STREAM = 'application/octet-stream'
 
 
 class DeleteIndexEnums:
     """
     Enums for delete_index parameters.
     """
 
     class Type(str, Enum):
         """
         Path parameter to specify the index type.
         """
+
         JSON = 'json'
         SPECIAL = 'special'
         TEXT = 'text'
 
 
 class DeleteReplicationDocumentEnums:
     """
@@ -7608,40 +8001,43 @@
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class PutReplicationDocumentEnums:
     """
     Enums for put_replication_document parameters.
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class GetSchedulerDocsEnums:
     """
     Enums for get_scheduler_docs parameters.
     """
 
     class States(str, Enum):
         """
         Query parameter to include only replication documents in the specified states.
         String must be a comma-delimited string.
         """
+
         INITIALIZING = 'initializing'
         ERROR = 'error'
         PENDING = 'pending'
         RUNNING = 'running'
         CRASHING = 'crashing'
         COMPLETED = 'completed'
         FAILED = 'failed'
@@ -7653,40 +8049,43 @@
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class DeleteLocalDocumentEnums:
     """
     Enums for delete_local_document parameters.
     """
 
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 class GetLocalDocumentEnums:
     """
     Enums for get_local_document parameters.
     """
 
     class Accept(str, Enum):
         """
         The type of the response: application/json, multipart/mixed, multipart/related, or
         application/octet-stream.
         """
+
         APPLICATION_JSON = 'application/json'
         MULTIPART_MIXED = 'multipart/mixed'
         MULTIPART_RELATED = 'multipart/related'
         APPLICATION_OCTET_STREAM = 'application/octet-stream'
 
 
 class PutLocalDocumentEnums:
@@ -7694,32 +8093,34 @@
     Enums for put_local_document parameters.
     """
 
     class ContentType(str, Enum):
         """
         The type of the input.
         """
+
         APPLICATION_JSON = 'application/json'
         MULTIPART_MIXED = 'multipart/mixed'
         MULTIPART_RELATED = 'multipart/related'
         APPLICATION_OCTET_STREAM = 'application/octet-stream'
     class Batch(str, Enum):
         """
         Query parameter to specify whether to store in batch mode. The server will respond
         with a HTTP 202 Accepted response code immediately.
         """
+
         OK = 'ok'
 
 
 ##############################################################################
 # Models
 ##############################################################################
 
 
-class ActiveTask():
+class ActiveTask:
     """
     Schema for information about a running task.
 
     :attr int bulk_get_attempts: (optional) The total count of attempted doc
           revisions fetched with `_bulk_get`. Available for `replication` type tasks.
     :attr int bulk_get_docs: (optional) The total count of successful docs fetched
           with `_bulk_get`. Available for `replication` type tasks.
@@ -7782,50 +8183,52 @@
     :attr int updated_on: Schema for a Unix epoch timestamp.
     :attr str user: (optional) Name of user running replication or owning the
           indexer. Available for `indexer`, `replication` type tasks.
     :attr int view: (optional) Number of view indexes. Available for
           `view_compaction` type tasks.
     """
 
-    def __init__(self,
-                 database: str,
-                 node: str,
-                 pid: str,
-                 started_on: int,
-                 type: str,
-                 updated_on: int,
-                 *,
-                 bulk_get_attempts: int = None,
-                 bulk_get_docs: int = None,
-                 changes_done: int = None,
-                 changes_pending: int = None,
-                 checkpoint_interval: int = None,
-                 checkpointed_source_seq: str = None,
-                 continuous: bool = None,
-                 design_document: str = None,
-                 doc_id: str = None,
-                 doc_write_failures: int = None,
-                 docs_read: int = None,
-                 docs_written: int = None,
-                 index: str = None,
-                 indexer_pid: str = None,
-                 missing_revisions_found: int = None,
-                 phase: str = None,
-                 process_status: str = None,
-                 progress: int = None,
-                 replication_id: str = None,
-                 retry: bool = None,
-                 revisions_checked: int = None,
-                 source: str = None,
-                 source_seq: str = None,
-                 target: str = None,
-                 through_seq: str = None,
-                 total_changes: int = None,
-                 user: str = None,
-                 view: int = None) -> None:
+    def __init__(
+        self,
+        database: str,
+        node: str,
+        pid: str,
+        started_on: int,
+        type: str,
+        updated_on: int,
+        *,
+        bulk_get_attempts: int = None,
+        bulk_get_docs: int = None,
+        changes_done: int = None,
+        changes_pending: int = None,
+        checkpoint_interval: int = None,
+        checkpointed_source_seq: str = None,
+        continuous: bool = None,
+        design_document: str = None,
+        doc_id: str = None,
+        doc_write_failures: int = None,
+        docs_read: int = None,
+        docs_written: int = None,
+        index: str = None,
+        indexer_pid: str = None,
+        missing_revisions_found: int = None,
+        phase: str = None,
+        process_status: str = None,
+        progress: int = None,
+        replication_id: str = None,
+        retry: bool = None,
+        revisions_checked: int = None,
+        source: str = None,
+        source_seq: str = None,
+        target: str = None,
+        through_seq: str = None,
+        total_changes: int = None,
+        user: str = None,
+        view: int = None,
+    ) -> None:
         """
         Initialize a ActiveTask object.
 
         :param str database: Source database.
         :param str node: Cluster node where the task is running.
         :param str pid: Process ID.
         :param int started_on: Schema for a Unix epoch timestamp.
@@ -8114,55 +8517,61 @@
 
     class PhaseEnum(str, Enum):
         """
         The phase the active task is in. `docid_sort`, `docid_copy`, `document_copy`
         phases are available for `database_compaction`, while `ids` and `view` phases are
         available for `view_compaction` type tasks.
         """
+
         DOCID_SORT = 'docid_sort'
         DOCID_COPY = 'docid_copy'
         DOCUMENT_COPY = 'document_copy'
         IDS = 'ids'
         VIEW = 'view'
 
 
     class ProcessStatusEnum(str, Enum):
         """
         Process status.
         """
+
         EXITING = 'exiting'
         GARBAGE_COLLECTING = 'garbage_collecting'
         RUNNABLE = 'runnable'
         RUNNING = 'running'
         SUSPENDED = 'suspended'
         WAITING = 'waiting'
 
 
     class TypeEnum(str, Enum):
         """
         Operation type.
         """
+
         DATABASE_COMPACTION = 'database_compaction'
         INDEXER = 'indexer'
         REPLICATION = 'replication'
         SEARCH_INDEXER = 'search_indexer'
         VIEW_COMPACTION = 'view_compaction'
 
 
-class ActivityTrackerEvents():
+
+class ActivityTrackerEvents:
     """
     Schema for Activity Tracker events.
 
     :attr List[str] types: An array of event types that are being sent to IBM Cloud
           Activity Tracker for the IBM Cloudant instance. "management" is a required
           element of this array.
     """
 
-    def __init__(self,
-                 types: List[str]) -> None:
+    def __init__(
+        self,
+        types: List[str],
+    ) -> None:
         """
         Initialize a ActivityTrackerEvents object.
 
         :param List[str] types: An array of event types that are being sent to IBM
                Cloud Activity Tracker for the IBM Cloudant instance. "management" is a
                required element of this array.
         """
@@ -8208,29 +8617,33 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class TypesEnum(str, Enum):
         """
         types.
         """
+
         MANAGEMENT = 'management'
         DATA = 'data'
 
 
-class AllDocsQueriesResult():
+
+class AllDocsQueriesResult:
     """
     Schema for the result of an all documents queries operation.
 
     :attr List[AllDocsResult] results: An array of result objects - one for each
           query. Each result object contains the same fields as the response to a regular
           `/_all_docs` request.
     """
 
-    def __init__(self,
-                 results: List['AllDocsResult']) -> None:
+    def __init__(
+        self,
+        results: List['AllDocsResult'],
+    ) -> None:
         """
         Initialize a AllDocsQueriesResult object.
 
         :param List[AllDocsResult] results: An array of result objects - one for
                each query. Each result object contains the same fields as the response to
                a regular `/_all_docs` request.
         """
@@ -8278,15 +8691,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'AllDocsQueriesResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class AllDocsQuery():
+
+class AllDocsQuery:
     """
     Schema for an all documents query operation.
 
     :attr bool att_encoding_info: (optional) Parameter to specify whether to include
           the encoding information in attachment stubs if the particular attachment is
           compressed.
     :attr bool attachments: (optional) Parameter to specify whether to include
@@ -8309,29 +8723,31 @@
           reflects.
     :attr str end_key: (optional) Schema for a document ID.
     :attr str key: (optional) Schema for a document ID.
     :attr List[str] keys: (optional) Schema for a list of document IDs.
     :attr str start_key: (optional) Schema for a document ID.
     """
 
-    def __init__(self,
-                 *,
-                 att_encoding_info: bool = None,
-                 attachments: bool = None,
-                 conflicts: bool = None,
-                 descending: bool = None,
-                 include_docs: bool = None,
-                 inclusive_end: bool = None,
-                 limit: int = None,
-                 skip: int = None,
-                 update_seq: bool = None,
-                 end_key: str = None,
-                 key: str = None,
-                 keys: List[str] = None,
-                 start_key: str = None) -> None:
+    def __init__(
+        self,
+        *,
+        att_encoding_info: bool = None,
+        attachments: bool = None,
+        conflicts: bool = None,
+        descending: bool = None,
+        include_docs: bool = None,
+        inclusive_end: bool = None,
+        limit: int = None,
+        skip: int = None,
+        update_seq: bool = None,
+        end_key: str = None,
+        key: str = None,
+        keys: List[str] = None,
+        start_key: str = None,
+    ) -> None:
         """
         Initialize a AllDocsQuery object.
 
         :param bool att_encoding_info: (optional) Parameter to specify whether to
                include the encoding information in attachment stubs if the particular
                attachment is compressed.
         :param bool attachments: (optional) Parameter to specify whether to include
@@ -8453,28 +8869,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'AllDocsQuery') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class AllDocsResult():
+
+class AllDocsResult:
     """
     Schema for the result of an all documents operation.
 
     :attr int total_rows: Number of total rows.
     :attr List[DocsResultRow] rows: List of doc results.
     :attr str update_seq: (optional) Current update sequence for the database.
     """
 
-    def __init__(self,
-                 total_rows: int,
-                 rows: List['DocsResultRow'],
-                 *,
-                 update_seq: str = None) -> None:
+    def __init__(
+        self,
+        total_rows: int,
+        rows: List['DocsResultRow'],
+        *,
+        update_seq: str = None,
+    ) -> None:
         """
         Initialize a AllDocsResult object.
 
         :param int total_rows: Number of total rows.
         :param List[DocsResultRow] rows: List of doc results.
         :param str update_seq: (optional) Current update sequence for the database.
         """
@@ -8534,31 +8953,34 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'AllDocsResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Analyzer():
+
+class Analyzer:
     """
     Schema for a full text search analyzer.
 
     :attr str name: (optional) Schema for the name of the Apache Lucene analyzer to
           use for text indexing. The default value varies depending on the analyzer usage:
           * For search indexes the default is `standard` * For query text indexes the
           default is `keyword` * For a query text index default_field the default is
           `standard`.
     :attr List[str] stopwords: (optional) Custom stopwords to use with the named
           analyzer.
     """
 
-    def __init__(self,
-                 *,
-                 name: str = None,
-                 stopwords: List[str] = None) -> None:
+    def __init__(
+        self,
+        *,
+        name: str = None,
+        stopwords: List[str] = None,
+    ) -> None:
         """
         Initialize a Analyzer object.
 
         :param str name: (optional) Schema for the name of the Apache Lucene
                analyzer to use for text indexing. The default value varies depending on
                the analyzer usage:
                * For search indexes the default is `standard` * For query text indexes the
@@ -8616,14 +9038,15 @@
         """
         Schema for the name of the Apache Lucene analyzer to use for text indexing. The
         default value varies depending on the analyzer usage:
         * For search indexes the default is `standard` * For query text indexes the
         default is `keyword` * For a query text index default_field the default is
         `standard`.
         """
+
         CLASSIC = 'classic'
         EMAIL = 'email'
         KEYWORD = 'keyword'
         SIMPLE = 'simple'
         STANDARD = 'standard'
         WHITESPACE = 'whitespace'
         ARABIC = 'arabic'
@@ -8659,34 +9082,37 @@
         SPANISH = 'spanish'
         SWEDISH = 'swedish'
         THAI = 'thai'
         TURKISH = 'turkish'
         PERFIELD = 'perfield'
 
 
-class AnalyzerConfiguration():
+
+class AnalyzerConfiguration:
     """
     Schema for a search analyzer configuration.
 
     :attr str name: (optional) Schema for the name of the Apache Lucene analyzer to
           use for text indexing. The default value varies depending on the analyzer usage:
           * For search indexes the default is `standard` * For query text indexes the
           default is `keyword` * For a query text index default_field the default is
           `standard`.
     :attr List[str] stopwords: (optional) Custom stopwords to use with the named
           analyzer.
     :attr dict fields: (optional) Schema for mapping a field name to a per field
           analyzer.
     """
 
-    def __init__(self,
-                 *,
-                 name: str = None,
-                 stopwords: List[str] = None,
-                 fields: dict = None) -> None:
+    def __init__(
+        self,
+        *,
+        name: str = None,
+        stopwords: List[str] = None,
+        fields: dict = None,
+    ) -> None:
         """
         Initialize a AnalyzerConfiguration object.
 
         :param str name: (optional) Schema for the name of the Apache Lucene
                analyzer to use for text indexing. The default value varies depending on
                the analyzer usage:
                * For search indexes the default is `standard` * For query text indexes the
@@ -8706,15 +9132,15 @@
         """Initialize a AnalyzerConfiguration object from a json dictionary."""
         args = {}
         if 'name' in _dict:
             args['name'] = _dict.get('name')
         if 'stopwords' in _dict:
             args['stopwords'] = _dict.get('stopwords')
         if 'fields' in _dict:
-            args['fields'] = {k : Analyzer.from_dict(v) for k, v in _dict.get('fields').items()}
+            args['fields'] = {k: Analyzer.from_dict(v) for k, v in _dict.get('fields').items()}
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a AnalyzerConfiguration object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8757,14 +9183,15 @@
         """
         Schema for the name of the Apache Lucene analyzer to use for text indexing. The
         default value varies depending on the analyzer usage:
         * For search indexes the default is `standard` * For query text indexes the
         default is `keyword` * For a query text index default_field the default is
         `standard`.
         """
+
         CLASSIC = 'classic'
         EMAIL = 'email'
         KEYWORD = 'keyword'
         SIMPLE = 'simple'
         STANDARD = 'standard'
         WHITESPACE = 'whitespace'
         ARABIC = 'arabic'
@@ -8800,27 +9227,30 @@
         SPANISH = 'spanish'
         SWEDISH = 'swedish'
         THAI = 'thai'
         TURKISH = 'turkish'
         PERFIELD = 'perfield'
 
 
-class ApiKeysResult():
+
+class ApiKeysResult:
     """
     Schema for api keys.
 
     :attr bool ok: ok.
     :attr str key: The generated api key.
     :attr str password: The password associated with the api key.
     """
 
-    def __init__(self,
-                 ok: bool,
-                 key: str,
-                 password: str) -> None:
+    def __init__(
+        self,
+        ok: bool,
+        key: str,
+        password: str,
+    ) -> None:
         """
         Initialize a ApiKeysResult object.
 
         :param bool ok: ok.
         :param str key: The generated api key.
         :param str password: The password associated with the api key.
         """
@@ -8876,15 +9306,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ApiKeysResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Attachment():
+
+class Attachment:
     """
     Schema for an attachment.
 
     :attr str content_type: (optional) Attachment MIME type.
     :attr bytes data: (optional) Base64-encoded content. Available if attachment
           content is requested by using the query parameters `attachments=true` or
           `atts_since`. Note that when used with a view or changes feed `include_docs`
@@ -8904,25 +9335,27 @@
     :attr int length: (optional) Real attachment size in bytes. Not available if
           inline attachment content requested.
     :attr int revpos: (optional) Revision number when attachment was added.
     :attr bool stub: (optional) Has `true` value if object contains stub info and no
           content. Otherwise omitted in response.
     """
 
-    def __init__(self,
-                 *,
-                 content_type: str = None,
-                 data: bytes = None,
-                 digest: str = None,
-                 encoded_length: int = None,
-                 encoding: str = None,
-                 follows: bool = None,
-                 length: int = None,
-                 revpos: int = None,
-                 stub: bool = None) -> None:
+    def __init__(
+        self,
+        *,
+        content_type: str = None,
+        data: bytes = None,
+        digest: str = None,
+        encoded_length: int = None,
+        encoding: str = None,
+        follows: bool = None,
+        length: int = None,
+        revpos: int = None,
+        stub: bool = None,
+    ) -> None:
         """
         Initialize a Attachment object.
 
         :param str content_type: (optional) Attachment MIME type.
         :param bytes data: (optional) Base64-encoded content. Available if
                attachment content is requested by using the query parameters
                `attachments=true` or `atts_since`. Note that when used with a view or
@@ -9024,27 +9457,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Attachment') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class BulkDocs():
+
+class BulkDocs:
     """
     Schema for submitting documents for bulk modifications.
 
     :attr List[Document] docs: Array of documents.
     :attr bool new_edits: (optional) If `false`, prevents the database from
           assigning them new revision IDs. Default is `true`.
     """
 
-    def __init__(self,
-                 docs: List['Document'],
-                 *,
-                 new_edits: bool = None) -> None:
+    def __init__(
+        self,
+        docs: List['Document'],
+        *,
+        new_edits: bool = None,
+    ) -> None:
         """
         Initialize a BulkDocs object.
 
         :param List[Document] docs: Array of documents.
         :param bool new_edits: (optional) If `false`, prevents the database from
                assigning them new revision IDs. Default is `true`.
         """
@@ -9097,29 +9533,32 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'BulkDocs') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class BulkGetQueryDocument():
+
+class BulkGetQueryDocument:
     """
     Schema for a document item in a bulk get query.
 
     :attr List[str] atts_since: (optional) Includes attachments only since specified
           revisions.
     :attr str id: Schema for a document ID.
     :attr str rev: (optional) Schema for a document revision identifier.
     """
 
-    def __init__(self,
-                 id: str,
-                 *,
-                 atts_since: List[str] = None,
-                 rev: str = None) -> None:
+    def __init__(
+        self,
+        id: str,
+        *,
+        atts_since: List[str] = None,
+        rev: str = None,
+    ) -> None:
         """
         Initialize a BulkGetQueryDocument object.
 
         :param str id: Schema for a document ID.
         :param List[str] atts_since: (optional) Includes attachments only since
                specified revisions.
         :param str rev: (optional) Schema for a document revision identifier.
@@ -9172,23 +9611,26 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'BulkGetQueryDocument') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class BulkGetResult():
+
+class BulkGetResult:
     """
     Schema for the results object of a bulk get operation.
 
     :attr List[BulkGetResultItem] results: Results.
     """
 
-    def __init__(self,
-                 results: List['BulkGetResultItem']) -> None:
+    def __init__(
+        self,
+        results: List['BulkGetResultItem'],
+    ) -> None:
         """
         Initialize a BulkGetResult object.
 
         :param List[BulkGetResultItem] results: Results.
         """
         self.results = results
 
@@ -9234,28 +9676,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'BulkGetResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class BulkGetResultDocument():
+
+class BulkGetResultDocument:
     """
     Schema for BulkGetResult object containing a successfully retrieved document or error
     information.
 
     :attr DocumentResult error: (optional) Schema for the result of a document
           modification.
     :attr Document ok: (optional) Schema for a document.
     """
 
-    def __init__(self,
-                 *,
-                 error: 'DocumentResult' = None,
-                 ok: 'Document' = None) -> None:
+    def __init__(
+        self,
+        *,
+        error: 'DocumentResult' = None,
+        ok: 'Document' = None,
+    ) -> None:
         """
         Initialize a BulkGetResultDocument object.
 
         :param DocumentResult error: (optional) Schema for the result of a document
                modification.
         :param Document ok: (optional) Schema for a document.
         """
@@ -9306,26 +9751,29 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'BulkGetResultDocument') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class BulkGetResultItem():
+
+class BulkGetResultItem:
     """
     Schema for the document revisions information from a bulk get operation.
 
     :attr List[BulkGetResultDocument] docs: Array of document revisions or error
           information.
     :attr str id: Schema for a document ID.
     """
 
-    def __init__(self,
-                 docs: List['BulkGetResultDocument'],
-                 id: str) -> None:
+    def __init__(
+        self,
+        docs: List['BulkGetResultDocument'],
+        id: str,
+    ) -> None:
         """
         Initialize a BulkGetResultItem object.
 
         :param List[BulkGetResultDocument] docs: Array of document revisions or
                error information.
         :param str id: Schema for a document ID.
         """
@@ -9380,28 +9828,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'BulkGetResultItem') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class CapacityThroughputInformation():
+
+class CapacityThroughputInformation:
     """
     Schema for information about the currently provisioned and target throughput capacity.
 
     :attr CapacityThroughputInformationCurrent current: Detailed information about
           provisioned throughput capacity.
     :attr CapacityThroughputInformationTarget target: (optional) Detailed
           information about target throughput capacity.
     """
 
-    def __init__(self,
-                 current: 'CapacityThroughputInformationCurrent',
-                 *,
-                 target: 'CapacityThroughputInformationTarget' = None) -> None:
+    def __init__(
+        self,
+        current: 'CapacityThroughputInformationCurrent',
+        *,
+        target: 'CapacityThroughputInformationTarget' = None,
+    ) -> None:
         """
         Initialize a CapacityThroughputInformation object.
 
         :param CapacityThroughputInformationCurrent current: Detailed information
                about provisioned throughput capacity.
         :param CapacityThroughputInformationTarget target: (optional) Detailed
                information about target throughput capacity.
@@ -9455,24 +9906,27 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CapacityThroughputInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class CapacityThroughputInformationCurrent():
+
+class CapacityThroughputInformationCurrent:
     """
     Detailed information about provisioned throughput capacity.
 
     :attr ThroughputInformation throughput: Schema for detailed information about
           throughput capacity with breakdown by specific throughput requests classes.
     """
 
-    def __init__(self,
-                 throughput: 'ThroughputInformation') -> None:
+    def __init__(
+        self,
+        throughput: 'ThroughputInformation',
+    ) -> None:
         """
         Initialize a CapacityThroughputInformationCurrent object.
 
         :param ThroughputInformation throughput: Schema for detailed information
                about throughput capacity with breakdown by specific throughput requests
                classes.
         """
@@ -9517,24 +9971,27 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CapacityThroughputInformationCurrent') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class CapacityThroughputInformationTarget():
+
+class CapacityThroughputInformationTarget:
     """
     Detailed information about target throughput capacity.
 
     :attr ThroughputInformation throughput: Schema for detailed information about
           throughput capacity with breakdown by specific throughput requests classes.
     """
 
-    def __init__(self,
-                 throughput: 'ThroughputInformation') -> None:
+    def __init__(
+        self,
+        throughput: 'ThroughputInformation',
+    ) -> None:
         """
         Initialize a CapacityThroughputInformationTarget object.
 
         :param ThroughputInformation throughput: Schema for detailed information
                about throughput capacity with breakdown by specific throughput requests
                classes.
         """
@@ -9579,23 +10036,26 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CapacityThroughputInformationTarget') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Change():
+
+class Change:
     """
     Schema for a document leaf with single field rev.
 
     :attr str rev: Schema for a document revision identifier.
     """
 
-    def __init__(self,
-                 rev: str) -> None:
+    def __init__(
+        self,
+        rev: str,
+    ) -> None:
         """
         Initialize a Change object.
 
         :param str rev: Schema for a document revision identifier.
         """
         self.rev = rev
 
@@ -9635,27 +10095,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Change') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ChangesResult():
+
+class ChangesResult:
     """
     Schema for normal changes feed result.
 
     :attr str last_seq: last_seq.
     :attr int pending: pending.
     :attr List[ChangesResultItem] results: results.
     """
 
-    def __init__(self,
-                 last_seq: str,
-                 pending: int,
-                 results: List['ChangesResultItem']) -> None:
+    def __init__(
+        self,
+        last_seq: str,
+        pending: int,
+        results: List['ChangesResultItem'],
+    ) -> None:
         """
         Initialize a ChangesResult object.
 
         :param str last_seq: last_seq.
         :param int pending: pending.
         :param List[ChangesResultItem] results: results.
         """
@@ -9717,32 +10180,35 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ChangesResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ChangesResultItem():
+
+class ChangesResultItem:
     """
     Schema for an item in the changes results array.
 
     :attr List[Change] changes: List of document's leaves with single field rev.
     :attr bool deleted: (optional) if `true` then the document is deleted.
     :attr Document doc: (optional) Schema for a document.
     :attr str id: Schema for a document ID.
     :attr str seq: Update sequence.
     """
 
-    def __init__(self,
-                 changes: List['Change'],
-                 id: str,
-                 seq: str,
-                 *,
-                 deleted: bool = None,
-                 doc: 'Document' = None) -> None:
+    def __init__(
+        self,
+        changes: List['Change'],
+        id: str,
+        seq: str,
+        *,
+        deleted: bool = None,
+        doc: 'Document' = None,
+    ) -> None:
         """
         Initialize a ChangesResultItem object.
 
         :param List[Change] changes: List of document's leaves with single field
                rev.
         :param str id: Schema for a document ID.
         :param str seq: Update sequence.
@@ -9820,27 +10286,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ChangesResultItem') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ContentInformationSizes():
+
+class ContentInformationSizes:
     """
     Schema for size information of content.
 
     :attr int active: The active size of the content, in bytes.
     :attr int external: The total uncompressed size of the content, in bytes.
     :attr int file: The total size of the content as stored on disk, in bytes.
     """
 
-    def __init__(self,
-                 active: int,
-                 external: int,
-                 file: int) -> None:
+    def __init__(
+        self,
+        active: int,
+        external: int,
+        file: int,
+    ) -> None:
         """
         Initialize a ContentInformationSizes object.
 
         :param int active: The active size of the content, in bytes.
         :param int external: The total uncompressed size of the content, in bytes.
         :param int file: The total size of the content as stored on disk, in bytes.
         """
@@ -9896,31 +10365,34 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ContentInformationSizes') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class CorsInformation():
+
+class CorsInformation:
     """
     Schema for information about the CORS configuration.
 
     :attr bool allow_credentials: Boolean value to allow authentication credentials.
           If set to true, browser requests must be done by using withCredentials = true.
     :attr bool enable_cors: Boolean value to turn CORS on and off.
     :attr List[str] origins: An array of strings that contain allowed origin
           domains. You have to specify the full URL including the protocol. It is
           recommended that only the HTTPS protocol is used. Subdomains count as separate
           domains, so you have to specify all subdomains used.
     """
 
-    def __init__(self,
-                 allow_credentials: bool,
-                 enable_cors: bool,
-                 origins: List[str]) -> None:
+    def __init__(
+        self,
+        allow_credentials: bool,
+        enable_cors: bool,
+        origins: List[str],
+    ) -> None:
         """
         Initialize a CorsInformation object.
 
         :param bool allow_credentials: Boolean value to allow authentication
                credentials. If set to true, browser requests must be done by using
                withCredentials = true.
         :param bool enable_cors: Boolean value to turn CORS on and off.
@@ -9981,24 +10453,27 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CorsInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class CurrentThroughputInformation():
+
+class CurrentThroughputInformation:
     """
     Schema for information about current consumption of a provisioned throughput capacity.
 
     :attr CurrentThroughputInformationThroughput throughput: Detailed information
           about current consumption.
     """
 
-    def __init__(self,
-                 throughput: 'CurrentThroughputInformationThroughput') -> None:
+    def __init__(
+        self,
+        throughput: 'CurrentThroughputInformationThroughput',
+    ) -> None:
         """
         Initialize a CurrentThroughputInformation object.
 
         :param CurrentThroughputInformationThroughput throughput: Detailed
                information about current consumption.
         """
         self.throughput = throughput
@@ -10042,30 +10517,33 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CurrentThroughputInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class CurrentThroughputInformationThroughput():
+
+class CurrentThroughputInformationThroughput:
     """
     Detailed information about current consumption.
 
     :attr int query: Number of global queries conducted against the instance for a
           given second.
     :attr int read: Number of reads conducted against the instance for a given
           second.
     :attr int write: Number of writes conducted against the instance for a given
           second.
     """
 
-    def __init__(self,
-                 query: int,
-                 read: int,
-                 write: int) -> None:
+    def __init__(
+        self,
+        query: int,
+        read: int,
+        write: int,
+    ) -> None:
         """
         Initialize a CurrentThroughputInformationThroughput object.
 
         :param int query: Number of global queries conducted against the instance
                for a given second.
         :param int read: Number of reads conducted against the instance for a given
                second.
@@ -10124,15 +10602,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CurrentThroughputInformationThroughput') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DatabaseInformation():
+
+class DatabaseInformation:
     """
     Schema for information about a database.
 
     :attr DatabaseInformationCluster cluster: Schema for database cluster
           information.
     :attr str committed_update_seq: (optional) An opaque string that describes the
           committed state of the database.
@@ -10149,29 +10628,31 @@
     :attr DatabaseInformationProps props: Schema for database properties.
     :attr ContentInformationSizes sizes: Schema for size information of content.
     :attr str update_seq: An opaque string that describes the state of the database.
           Do not rely on this string for counting the number of updates.
     :attr str uuid: (optional) The UUID of the database.
     """
 
-    def __init__(self,
-                 cluster: 'DatabaseInformationCluster',
-                 compact_running: bool,
-                 db_name: str,
-                 disk_format_version: int,
-                 doc_count: int,
-                 doc_del_count: int,
-                 props: 'DatabaseInformationProps',
-                 sizes: 'ContentInformationSizes',
-                 update_seq: str,
-                 *,
-                 committed_update_seq: str = None,
-                 compacted_seq: str = None,
-                 engine: str = None,
-                 uuid: str = None) -> None:
+    def __init__(
+        self,
+        cluster: 'DatabaseInformationCluster',
+        compact_running: bool,
+        db_name: str,
+        disk_format_version: int,
+        doc_count: int,
+        doc_del_count: int,
+        props: 'DatabaseInformationProps',
+        sizes: 'ContentInformationSizes',
+        update_seq: str,
+        *,
+        committed_update_seq: str = None,
+        compacted_seq: str = None,
+        engine: str = None,
+        uuid: str = None,
+    ) -> None:
         """
         Initialize a DatabaseInformation object.
 
         :param DatabaseInformationCluster cluster: Schema for database cluster
                information.
         :param bool compact_running: True if the database compaction routine is
                operating on this database.
@@ -10315,32 +10796,35 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DatabaseInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DatabaseInformationCluster():
+
+class DatabaseInformationCluster:
     """
     Schema for database cluster information.
 
     :attr int n: Schema for the number of replicas of a database in a cluster.
     :attr int q: Schema for the number of shards in a database. Each shard is a
           partition of the hash value range.
     :attr int r: Read quorum. The number of consistent copies of a document that
           need to be read before a successful reply.
     :attr int w: Write quorum. The number of copies of a document that need to be
           written before a successful reply.
     """
 
-    def __init__(self,
-                 n: int,
-                 q: int,
-                 r: int,
-                 w: int) -> None:
+    def __init__(
+        self,
+        n: int,
+        q: int,
+        r: int,
+        w: int,
+    ) -> None:
         """
         Initialize a DatabaseInformationCluster object.
 
         :param int n: Schema for the number of replicas of a database in a cluster.
         :param int q: Schema for the number of shards in a database. Each shard is
                a partition of the hash value range.
         :param int r: Read quorum. The number of consistent copies of a document
@@ -10407,25 +10891,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DatabaseInformationCluster') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DatabaseInformationProps():
+
+class DatabaseInformationProps:
     """
     Schema for database properties.
 
     :attr bool partitioned: (optional) The value is `true` for a partitioned
           database.
     """
 
-    def __init__(self,
-                 *,
-                 partitioned: bool = None) -> None:
+    def __init__(
+        self,
+        *,
+        partitioned: bool = None,
+    ) -> None:
         """
         Initialize a DatabaseInformationProps object.
 
         :param bool partitioned: (optional) The value is `true` for a partitioned
                database.
         """
         self.partitioned = partitioned
@@ -10464,27 +10951,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DatabaseInformationProps') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DbEvent():
+
+class DbEvent:
     """
     Schema for a database change event.
 
     :attr str db_name: Database name.
     :attr str seq: Sequence number.
     :attr str type: A database event.
     """
 
-    def __init__(self,
-                 db_name: str,
-                 seq: str,
-                 type: str) -> None:
+    def __init__(
+        self,
+        db_name: str,
+        seq: str,
+        type: str,
+    ) -> None:
         """
         Initialize a DbEvent object.
 
         :param str db_name: Database name.
         :param str seq: Sequence number.
         :param str type: A database event.
         """
@@ -10544,30 +11034,34 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class TypeEnum(str, Enum):
         """
         A database event.
         """
+
         CREATED = 'created'
         DELETED = 'deleted'
         UPDATED = 'updated'
 
 
-class DbUpdates():
+
+class DbUpdates:
     """
     Schema for database updates.
 
     :attr str last_seq: Last sequence number.
     :attr List[DbEvent] results: results.
     """
 
-    def __init__(self,
-                 last_seq: str,
-                 results: List['DbEvent']) -> None:
+    def __init__(
+        self,
+        last_seq: str,
+        results: List['DbEvent'],
+    ) -> None:
         """
         Initialize a DbUpdates object.
 
         :param str last_seq: Last sequence number.
         :param List[DbEvent] results: results.
         """
         self.last_seq = last_seq
@@ -10621,29 +11115,32 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DbUpdates') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DbsInfoResult():
+
+class DbsInfoResult:
     """
     Schema for database information keyed by database name.
 
     :attr str error: (optional) The name of the error.
     :attr DatabaseInformation info: (optional) Schema for information about a
           database.
     :attr str key: Database name.
     """
 
-    def __init__(self,
-                 key: str,
-                 *,
-                 error: str = None,
-                 info: 'DatabaseInformation' = None) -> None:
+    def __init__(
+        self,
+        key: str,
+        *,
+        error: str = None,
+        info: 'DatabaseInformation' = None,
+    ) -> None:
         """
         Initialize a DbsInfoResult object.
 
         :param str key: Database name.
         :param str error: (optional) The name of the error.
         :param DatabaseInformation info: (optional) Schema for information about a
                database.
@@ -10699,15 +11196,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DbsInfoResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DesignDocument():
+
+class DesignDocument:
     """
     Schema for a design document.
 
     :attr dict attachments: (optional) Schema for a map of attachment name to
           attachment metadata.
     :attr List[str] conflicts: (optional) Schema for a list of document revision
           identifiers.
@@ -10792,33 +11290,35 @@
               see the `SecurityObject`.
     :attr dict views: (optional) Schema for design document views.
     """
 
     # The set of defined properties for the class
     _properties = frozenset(['attachments', '_attachments', 'conflicts', '_conflicts', 'deleted', '_deleted', 'deleted_conflicts', '_deleted_conflicts', 'id', '_id', 'local_seq', '_local_seq', 'rev', '_rev', 'revisions', '_revisions', 'revs_info', '_revs_info', 'autoupdate', 'filters', 'indexes', 'language', 'options', 'validate_doc_update', 'views'])
 
-    def __init__(self,
-                 *,
-                 attachments: dict = None,
-                 conflicts: List[str] = None,
-                 deleted: bool = None,
-                 deleted_conflicts: List[str] = None,
-                 id: str = None,
-                 local_seq: str = None,
-                 rev: str = None,
-                 revisions: 'Revisions' = None,
-                 revs_info: List['DocumentRevisionStatus'] = None,
-                 autoupdate: bool = None,
-                 filters: dict = None,
-                 indexes: dict = None,
-                 language: str = None,
-                 options: 'DesignDocumentOptions' = None,
-                 validate_doc_update: str = None,
-                 views: dict = None,
-                 **kwargs) -> None:
+    def __init__(
+        self,
+        *,
+        attachments: dict = None,
+        conflicts: List[str] = None,
+        deleted: bool = None,
+        deleted_conflicts: List[str] = None,
+        id: str = None,
+        local_seq: str = None,
+        rev: str = None,
+        revisions: 'Revisions' = None,
+        revs_info: List['DocumentRevisionStatus'] = None,
+        autoupdate: bool = None,
+        filters: dict = None,
+        indexes: dict = None,
+        language: str = None,
+        options: 'DesignDocumentOptions' = None,
+        validate_doc_update: str = None,
+        views: dict = None,
+        **kwargs,
+    ) -> None:
         """
         Initialize a DesignDocument object.
 
         :param dict attachments: (optional) Schema for a map of attachment name to
                attachment metadata.
         :param List[str] conflicts: (optional) Schema for a list of document
                revision identifiers.
@@ -10927,15 +11427,15 @@
             setattr(self, _key, _value)
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'DesignDocument':
         """Initialize a DesignDocument object from a json dictionary."""
         args = {}
         if '_attachments' in _dict:
-            args['attachments'] = {k : Attachment.from_dict(v) for k, v in _dict.get('_attachments').items()}
+            args['attachments'] = {k: Attachment.from_dict(v) for k, v in _dict.get('_attachments').items()}
         if '_conflicts' in _dict:
             args['conflicts'] = _dict.get('_conflicts')
         if '_deleted' in _dict:
             args['deleted'] = _dict.get('_deleted')
         if '_deleted_conflicts' in _dict:
             args['deleted_conflicts'] = _dict.get('_deleted_conflicts')
         if '_id' in _dict:
@@ -10949,24 +11449,24 @@
         if '_revs_info' in _dict:
             args['revs_info'] = [DocumentRevisionStatus.from_dict(v) for v in _dict.get('_revs_info')]
         if 'autoupdate' in _dict:
             args['autoupdate'] = _dict.get('autoupdate')
         if 'filters' in _dict:
             args['filters'] = _dict.get('filters')
         if 'indexes' in _dict:
-            args['indexes'] = {k : SearchIndexDefinition.from_dict(v) for k, v in _dict.get('indexes').items()}
+            args['indexes'] = {k: SearchIndexDefinition.from_dict(v) for k, v in _dict.get('indexes').items()}
         if 'language' in _dict:
             args['language'] = _dict.get('language')
         if 'options' in _dict:
             args['options'] = DesignDocumentOptions.from_dict(_dict.get('options'))
         if 'validate_doc_update' in _dict:
             args['validate_doc_update'] = _dict.get('validate_doc_update')
         if 'views' in _dict:
-            args['views'] = {k : DesignDocumentViewsMapReduce.from_dict(v) for k, v in _dict.get('views').items()}
-        args.update({k:v for (k, v) in _dict.items() if k not in cls._properties})
+            args['views'] = {k: DesignDocumentViewsMapReduce.from_dict(v) for k, v in _dict.get('views').items()}
+        args.update({k: v for (k, v) in _dict.items() if k not in cls._properties})
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a DesignDocument object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -11070,25 +11570,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DesignDocument') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DesignDocumentInformation():
+
+class DesignDocumentInformation:
     """
     Schema for information about a design document.
 
     :attr str name: name.
     :attr DesignDocumentViewIndex view_index: View index information.
     """
 
-    def __init__(self,
-                 name: str,
-                 view_index: 'DesignDocumentViewIndex') -> None:
+    def __init__(
+        self,
+        name: str,
+        view_index: 'DesignDocumentViewIndex',
+    ) -> None:
         """
         Initialize a DesignDocumentInformation object.
 
         :param str name: name.
         :param DesignDocumentViewIndex view_index: View index information.
         """
         self.name = name
@@ -11139,25 +11642,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DesignDocumentInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DesignDocumentOptions():
+
+class DesignDocumentOptions:
     """
     Schema for design document options.
 
     :attr bool partitioned: (optional) Whether this design document describes
           partitioned or global indexes.
     """
 
-    def __init__(self,
-                 *,
-                 partitioned: bool = None) -> None:
+    def __init__(
+        self,
+        *,
+        partitioned: bool = None,
+    ) -> None:
         """
         Initialize a DesignDocumentOptions object.
 
         :param bool partitioned: (optional) Whether this design document describes
                partitioned or global indexes.
         """
         self.partitioned = partitioned
@@ -11196,67 +11702,76 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DesignDocumentOptions') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DesignDocumentViewIndex():
+
+class DesignDocumentViewIndex:
     """
     View index information.
 
     :attr List[str] collator_versions: List of collator versions. If there are
           multiple entries this implies a libicu upgrade has occurred but compaction has
           not run yet.
     :attr bool compact_running: Indicates whether a compaction routine is currently
           running on the view.
     :attr str language: Language for the defined views.
     :attr str signature: MD5 signature of the views for the design document.
     :attr ContentInformationSizes sizes: Schema for size information of content.
     :attr bool updater_running: Indicates if the view is currently being updated.
+    :attr UpdatesPending updates_pending: Schema for an ability to tell if view is
+          up-to-date without querying it.
     :attr int waiting_clients: Number of clients waiting on views from this design
           document.
     :attr bool waiting_commit: Indicates if there are outstanding commits to the
           underlying database that need to processed.
     """
 
-    def __init__(self,
-                 collator_versions: List[str],
-                 compact_running: bool,
-                 language: str,
-                 signature: str,
-                 sizes: 'ContentInformationSizes',
-                 updater_running: bool,
-                 waiting_clients: int,
-                 waiting_commit: bool) -> None:
+    def __init__(
+        self,
+        collator_versions: List[str],
+        compact_running: bool,
+        language: str,
+        signature: str,
+        sizes: 'ContentInformationSizes',
+        updater_running: bool,
+        updates_pending: 'UpdatesPending',
+        waiting_clients: int,
+        waiting_commit: bool,
+    ) -> None:
         """
         Initialize a DesignDocumentViewIndex object.
 
         :param List[str] collator_versions: List of collator versions. If there are
                multiple entries this implies a libicu upgrade has occurred but compaction
                has not run yet.
         :param bool compact_running: Indicates whether a compaction routine is
                currently running on the view.
         :param str language: Language for the defined views.
         :param str signature: MD5 signature of the views for the design document.
         :param ContentInformationSizes sizes: Schema for size information of
                content.
         :param bool updater_running: Indicates if the view is currently being
                updated.
+        :param UpdatesPending updates_pending: Schema for an ability to tell if
+               view is up-to-date without querying it.
         :param int waiting_clients: Number of clients waiting on views from this
                design document.
         :param bool waiting_commit: Indicates if there are outstanding commits to
                the underlying database that need to processed.
         """
         self.collator_versions = collator_versions
         self.compact_running = compact_running
         self.language = language
         self.signature = signature
         self.sizes = sizes
         self.updater_running = updater_running
+        self.updates_pending = updates_pending
         self.waiting_clients = waiting_clients
         self.waiting_commit = waiting_commit
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'DesignDocumentViewIndex':
         """Initialize a DesignDocumentViewIndex object from a json dictionary."""
         args = {}
@@ -11280,14 +11795,18 @@
             args['sizes'] = ContentInformationSizes.from_dict(_dict.get('sizes'))
         else:
             raise ValueError('Required property \'sizes\' not present in DesignDocumentViewIndex JSON')
         if 'updater_running' in _dict:
             args['updater_running'] = _dict.get('updater_running')
         else:
             raise ValueError('Required property \'updater_running\' not present in DesignDocumentViewIndex JSON')
+        if 'updates_pending' in _dict:
+            args['updates_pending'] = UpdatesPending.from_dict(_dict.get('updates_pending'))
+        else:
+            raise ValueError('Required property \'updates_pending\' not present in DesignDocumentViewIndex JSON')
         if 'waiting_clients' in _dict:
             args['waiting_clients'] = _dict.get('waiting_clients')
         else:
             raise ValueError('Required property \'waiting_clients\' not present in DesignDocumentViewIndex JSON')
         if 'waiting_commit' in _dict:
             args['waiting_commit'] = _dict.get('waiting_commit')
         else:
@@ -11313,14 +11832,19 @@
         if hasattr(self, 'sizes') and self.sizes is not None:
             if isinstance(self.sizes, dict):
                 _dict['sizes'] = self.sizes
             else:
                 _dict['sizes'] = self.sizes.to_dict()
         if hasattr(self, 'updater_running') and self.updater_running is not None:
             _dict['updater_running'] = self.updater_running
+        if hasattr(self, 'updates_pending') and self.updates_pending is not None:
+            if isinstance(self.updates_pending, dict):
+                _dict['updates_pending'] = self.updates_pending
+            else:
+                _dict['updates_pending'] = self.updates_pending.to_dict()
         if hasattr(self, 'waiting_clients') and self.waiting_clients is not None:
             _dict['waiting_clients'] = self.waiting_clients
         if hasattr(self, 'waiting_commit') and self.waiting_commit is not None:
             _dict['waiting_commit'] = self.waiting_commit
         return _dict
 
     def _to_dict(self):
@@ -11337,26 +11861,29 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DesignDocumentViewIndex') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DesignDocumentViewsMapReduce():
+
+class DesignDocumentViewsMapReduce:
     """
     Schema for view functions definition.
 
     :attr str map: JavaScript map function as a string.
     :attr str reduce: (optional) JavaScript reduce function as a string.
     """
 
-    def __init__(self,
-                 map: str,
-                 *,
-                 reduce: str = None) -> None:
+    def __init__(
+        self,
+        map: str,
+        *,
+        reduce: str = None,
+    ) -> None:
         """
         Initialize a DesignDocumentViewsMapReduce object.
 
         :param str map: JavaScript map function as a string.
         :param str reduce: (optional) JavaScript reduce function as a string.
         """
         self.map = map
@@ -11402,37 +11929,40 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DesignDocumentViewsMapReduce') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DocsResultRow():
+
+class DocsResultRow:
     """
     Schema for a row of document information in a DocsResult.
 
     :attr str caused_by: (optional) The cause of the error (if available).
     :attr str error: (optional) The name of the error.
     :attr str reason: (optional) The reason the error occurred (if available).
     :attr Document doc: (optional) Schema for a document.
     :attr str id: (optional) id.
     :attr str key: Document ID.
     :attr DocsResultRowValue value: (optional) Value of built-in `/_all_docs` style
           view.
     """
 
-    def __init__(self,
-                 key: str,
-                 *,
-                 caused_by: str = None,
-                 error: str = None,
-                 reason: str = None,
-                 doc: 'Document' = None,
-                 id: str = None,
-                 value: 'DocsResultRowValue' = None) -> None:
+    def __init__(
+        self,
+        key: str,
+        *,
+        caused_by: str = None,
+        error: str = None,
+        reason: str = None,
+        doc: 'Document' = None,
+        id: str = None,
+        value: 'DocsResultRowValue' = None,
+    ) -> None:
         """
         Initialize a DocsResultRow object.
 
         :param str key: Document ID.
         :param str caused_by: (optional) The cause of the error (if available).
         :param str error: (optional) The name of the error.
         :param str reason: (optional) The reason the error occurred (if available).
@@ -11515,27 +12045,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DocsResultRow') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DocsResultRowValue():
+
+class DocsResultRowValue:
     """
     Value of built-in `/_all_docs` style view.
 
     :attr bool deleted: (optional) If `true` then the document is deleted. Not
           present for undeleted documents.
     :attr str rev: Schema for a document revision identifier.
     """
 
-    def __init__(self,
-                 rev: str,
-                 *,
-                 deleted: bool = None) -> None:
+    def __init__(
+        self,
+        rev: str,
+        *,
+        deleted: bool = None,
+    ) -> None:
         """
         Initialize a DocsResultRowValue object.
 
         :param str rev: Schema for a document revision identifier.
         :param bool deleted: (optional) If `true` then the document is deleted. Not
                present for undeleted documents.
         """
@@ -11582,15 +12115,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DocsResultRowValue') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Document():
+
+class Document:
     """
     Schema for a document.
 
     :attr dict attachments: (optional) Schema for a map of attachment name to
           attachment metadata.
     :attr List[str] conflicts: (optional) Schema for a list of document revision
           identifiers.
@@ -11605,26 +12139,28 @@
     :attr List[DocumentRevisionStatus] revs_info: (optional) Schema for a list of
           objects with information about local revisions and their status.
     """
 
     # The set of defined properties for the class
     _properties = frozenset(['attachments', '_attachments', 'conflicts', '_conflicts', 'deleted', '_deleted', 'deleted_conflicts', '_deleted_conflicts', 'id', '_id', 'local_seq', '_local_seq', 'rev', '_rev', 'revisions', '_revisions', 'revs_info', '_revs_info'])
 
-    def __init__(self,
-                 *,
-                 attachments: dict = None,
-                 conflicts: List[str] = None,
-                 deleted: bool = None,
-                 deleted_conflicts: List[str] = None,
-                 id: str = None,
-                 local_seq: str = None,
-                 rev: str = None,
-                 revisions: 'Revisions' = None,
-                 revs_info: List['DocumentRevisionStatus'] = None,
-                 **kwargs) -> None:
+    def __init__(
+        self,
+        *,
+        attachments: dict = None,
+        conflicts: List[str] = None,
+        deleted: bool = None,
+        deleted_conflicts: List[str] = None,
+        id: str = None,
+        local_seq: str = None,
+        rev: str = None,
+        revisions: 'Revisions' = None,
+        revs_info: List['DocumentRevisionStatus'] = None,
+        **kwargs,
+    ) -> None:
         """
         Initialize a Document object.
 
         :param dict attachments: (optional) Schema for a map of attachment name to
                attachment metadata.
         :param List[str] conflicts: (optional) Schema for a list of document
                revision identifiers.
@@ -11655,15 +12191,15 @@
             setattr(self, _key, _value)
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'Document':
         """Initialize a Document object from a json dictionary."""
         args = {}
         if '_attachments' in _dict:
-            args['attachments'] = {k : Attachment.from_dict(v) for k, v in _dict.get('_attachments').items()}
+            args['attachments'] = {k: Attachment.from_dict(v) for k, v in _dict.get('_attachments').items()}
         if '_conflicts' in _dict:
             args['conflicts'] = _dict.get('_conflicts')
         if '_deleted' in _dict:
             args['deleted'] = _dict.get('_deleted')
         if '_deleted_conflicts' in _dict:
             args['deleted_conflicts'] = _dict.get('_deleted_conflicts')
         if '_id' in _dict:
@@ -11672,15 +12208,15 @@
             args['local_seq'] = _dict.get('_local_seq')
         if '_rev' in _dict:
             args['rev'] = _dict.get('_rev')
         if '_revisions' in _dict:
             args['revisions'] = Revisions.from_dict(_dict.get('_revisions'))
         if '_revs_info' in _dict:
             args['revs_info'] = [DocumentRevisionStatus.from_dict(v) for v in _dict.get('_revs_info')]
-        args.update({k:v for (k, v) in _dict.items() if k not in cls._properties})
+        args.update({k: v for (k, v) in _dict.items() if k not in cls._properties})
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Document object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -11755,34 +12291,37 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Document') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DocumentResult():
+
+class DocumentResult:
     """
     Schema for the result of a document modification.
 
     :attr str id: Schema for a document ID.
     :attr str rev: (optional) Schema for a document revision identifier.
     :attr bool ok: (optional) ok.
     :attr str caused_by: (optional) The cause of the error (if available).
     :attr str error: (optional) The name of the error.
     :attr str reason: (optional) The reason the error occurred (if available).
     """
 
-    def __init__(self,
-                 id: str,
-                 *,
-                 rev: str = None,
-                 ok: bool = None,
-                 caused_by: str = None,
-                 error: str = None,
-                 reason: str = None) -> None:
+    def __init__(
+        self,
+        id: str,
+        *,
+        rev: str = None,
+        ok: bool = None,
+        caused_by: str = None,
+        error: str = None,
+        reason: str = None,
+    ) -> None:
         """
         Initialize a DocumentResult object.
 
         :param str id: Schema for a document ID.
         :param str rev: (optional) Schema for a document revision identifier.
         :param bool ok: (optional) ok.
         :param str caused_by: (optional) The cause of the error (if available).
@@ -11852,27 +12391,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DocumentResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class DocumentRevisionStatus():
+
+class DocumentRevisionStatus:
     """
     Schema for information about revisions and their status.
 
     :attr str rev: Schema for a document revision identifier.
     :attr str status: Status of the revision. May be one of: - `available`: Revision
           is available for retrieving with rev query parameter - `missing`: Revision is
           not available - `deleted`: Revision belongs to deleted document.
     """
 
-    def __init__(self,
-                 rev: str,
-                 status: str) -> None:
+    def __init__(
+        self,
+        rev: str,
+        status: str,
+    ) -> None:
         """
         Initialize a DocumentRevisionStatus object.
 
         :param str rev: Schema for a document revision identifier.
         :param str status: Status of the revision. May be one of: - `available`:
                Revision is available for retrieving with rev query parameter - `missing`:
                Revision is not available - `deleted`: Revision belongs to deleted
@@ -11929,30 +12471,34 @@
 
     class StatusEnum(str, Enum):
         """
         Status of the revision. May be one of: - `available`: Revision is available for
         retrieving with rev query parameter - `missing`: Revision is not available -
         `deleted`: Revision belongs to deleted document.
         """
+
         AVAILABLE = 'available'
         MISSING = 'missing'
         DELETED = 'deleted'
 
 
-class DocumentShardInfo():
+
+class DocumentShardInfo:
     """
     Schema for document shard information.
 
     :attr List[str] nodes: List of nodes serving a replica of the shard.
     :attr str range: The shard range in which the document is stored.
     """
 
-    def __init__(self,
-                 nodes: List[str],
-                 range: str) -> None:
+    def __init__(
+        self,
+        nodes: List[str],
+        range: str,
+    ) -> None:
         """
         Initialize a DocumentShardInfo object.
 
         :param List[str] nodes: List of nodes serving a replica of the shard.
         :param str range: The shard range in which the document is stored.
         """
         self.nodes = nodes
@@ -12000,32 +12546,35 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DocumentShardInfo') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ExecutionStats():
+
+class ExecutionStats:
     """
     Schema for find query execution statistics.
 
     :attr float execution_time_ms: Time to execute the query.
     :attr int results_returned: Number of results returned.
     :attr int total_docs_examined: Number of documents fetched from the index.
     :attr int total_keys_examined: Number of rows scanned in the index.
     :attr int total_quorum_docs_examined: Number of documents fetched from the
           primary index with the specified read quorum.
     """
 
-    def __init__(self,
-                 execution_time_ms: float,
-                 results_returned: int,
-                 total_docs_examined: int,
-                 total_keys_examined: int,
-                 total_quorum_docs_examined: int) -> None:
+    def __init__(
+        self,
+        execution_time_ms: float,
+        results_returned: int,
+        total_docs_examined: int,
+        total_keys_examined: int,
+        total_quorum_docs_examined: int,
+    ) -> None:
         """
         Initialize a ExecutionStats object.
 
         :param float execution_time_ms: Time to execute the query.
         :param int results_returned: Number of results returned.
         :param int total_docs_examined: Number of documents fetched from the index.
         :param int total_keys_examined: Number of rows scanned in the index.
@@ -12098,15 +12647,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ExecutionStats') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ExplainResult():
+
+class ExplainResult:
     """
     Schema for information about the index used for a find query.
 
     :attr str dbname: dbname.
     :attr List[str] fields: fields.
     :attr IndexInformation index: Schema for information about an index.
     :attr int limit: limit.
@@ -12140,24 +12690,26 @@
           of these in a selector.
           For further reference see
           [selector
           syntax](https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-query#selector-syntax).
     :attr int skip: skip.
     """
 
-    def __init__(self,
-                 dbname: str,
-                 fields: List[str],
-                 index: 'IndexInformation',
-                 limit: int,
-                 opts: dict,
-                 selector: dict,
-                 skip: int,
-                 *,
-                 range: 'ExplainResultRange' = None) -> None:
+    def __init__(
+        self,
+        dbname: str,
+        fields: List[str],
+        index: 'IndexInformation',
+        limit: int,
+        opts: dict,
+        selector: dict,
+        skip: int,
+        *,
+        range: 'ExplainResultRange' = None,
+    ) -> None:
         """
         Initialize a ExplainResult object.
 
         :param str dbname: dbname.
         :param List[str] fields: fields.
         :param IndexInformation index: Schema for information about an index.
         :param int limit: limit.
@@ -12287,26 +12839,29 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ExplainResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ExplainResultRange():
+
+class ExplainResultRange:
     """
     range.
 
     :attr List[object] end_key: (optional) end_key.
     :attr List[object] start_key: (optional) start_key.
     """
 
-    def __init__(self,
-                 *,
-                 end_key: List[object] = None,
-                 start_key: List[object] = None) -> None:
+    def __init__(
+        self,
+        *,
+        end_key: List[object] = None,
+        start_key: List[object] = None,
+    ) -> None:
         """
         Initialize a ExplainResultRange object.
 
         :param List[object] end_key: (optional) end_key.
         :param List[object] start_key: (optional) start_key.
         """
         self.end_key = end_key
@@ -12350,31 +12905,34 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ExplainResultRange') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class FindResult():
+
+class FindResult:
     """
     Schema for the result of a query find operation.
 
     :attr str bookmark: Opaque bookmark token used when paginating results.
     :attr List[Document] docs: Documents matching the selector.
     :attr ExecutionStats execution_stats: (optional) Schema for find query execution
           statistics.
     :attr str warning: (optional) warning.
     """
 
-    def __init__(self,
-                 bookmark: str,
-                 docs: List['Document'],
-                 *,
-                 execution_stats: 'ExecutionStats' = None,
-                 warning: str = None) -> None:
+    def __init__(
+        self,
+        bookmark: str,
+        docs: List['Document'],
+        *,
+        execution_stats: 'ExecutionStats' = None,
+        warning: str = None,
+    ) -> None:
         """
         Initialize a FindResult object.
 
         :param str bookmark: Opaque bookmark token used when paginating results.
         :param List[Document] docs: Documents matching the selector.
         :param ExecutionStats execution_stats: (optional) Schema for find query
                execution statistics.
@@ -12444,15 +13002,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'FindResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class IndexDefinition():
+
+class IndexDefinition:
     """
     Schema for a `json` or `text` query index definition. Indexes of type `text` have
     additional configuration properties that do not apply to `json` indexes, these are:
     * `default_analyzer` - the default text analyzer to use * `default_field` - whether to
     index the text in all document fields and what analyzer to use for that purpose.
 
     :attr Analyzer default_analyzer: (optional) Schema for a full text search
@@ -12500,21 +13059,23 @@
           not `$ne`) can be used as the basis of a query. You should include at least one
           of these in a selector.
           For further reference see
           [selector
           syntax](https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-query#selector-syntax).
     """
 
-    def __init__(self,
-                 *,
-                 default_analyzer: 'Analyzer' = None,
-                 default_field: 'IndexTextOperatorDefaultField' = None,
-                 fields: List['IndexField'] = None,
-                 index_array_lengths: bool = None,
-                 partial_filter_selector: dict = None) -> None:
+    def __init__(
+        self,
+        *,
+        default_analyzer: 'Analyzer' = None,
+        default_field: 'IndexTextOperatorDefaultField' = None,
+        fields: List['IndexField'] = None,
+        index_array_lengths: bool = None,
+        partial_filter_selector: dict = None,
+    ) -> None:
         """
         Initialize a IndexDefinition object.
 
         :param Analyzer default_analyzer: (optional) Schema for a full text search
                analyzer.
         :param IndexTextOperatorDefaultField default_field: (optional) Schema for
                the text index default field configuration. The default field is used to
@@ -12635,30 +13196,33 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'IndexDefinition') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class IndexField():
+
+class IndexField:
     """
     Schema for indexed fields for use with declarative JSON query.
 
     :attr str name: (optional) Name of the field.
     :attr str type: (optional) The type of the named field.
     """
 
     # The set of defined properties for the class
     _properties = frozenset(['name', 'type'])
 
-    def __init__(self,
-                 *,
-                 name: str = None,
-                 type: str = None,
-                 **kwargs) -> None:
+    def __init__(
+        self,
+        *,
+        name: str = None,
+        type: str = None,
+        **kwargs,
+    ) -> None:
         """
         Initialize a IndexField object.
 
         :param str name: (optional) Name of the field.
         :param str type: (optional) The type of the named field.
         :param **kwargs: (optional) Any additional properties.
         """
@@ -12671,15 +13235,15 @@
     def from_dict(cls, _dict: Dict) -> 'IndexField':
         """Initialize a IndexField object from a json dictionary."""
         args = {}
         if 'name' in _dict:
             args['name'] = _dict.get('name')
         if 'type' in _dict:
             args['type'] = _dict.get('type')
-        args.update({k:v for (k, v) in _dict.items() if k not in cls._properties})
+        args.update({k: v for (k, v) in _dict.items() if k not in cls._properties})
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a IndexField object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -12729,39 +13293,43 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class TypeEnum(str, Enum):
         """
         The type of the named field.
         """
+
         BOOLEAN = 'boolean'
         NUMBER = 'number'
         STRING = 'string'
 
 
-class IndexInformation():
+
+class IndexInformation:
     """
     Schema for information about an index.
 
     :attr str ddoc: Design document ID.
     :attr IndexDefinition def_: Schema for a `json` or `text` query index
           definition. Indexes of type `text` have additional configuration properties that
           do not apply to `json` indexes, these are:
           * `default_analyzer` - the default text analyzer to use * `default_field` -
           whether to index the text in all document fields and what analyzer to use for
           that purpose.
     :attr str name: Index name.
     :attr str type: Schema for the type of an index.
     """
 
-    def __init__(self,
-                 ddoc: str,
-                 def_: 'IndexDefinition',
-                 name: str,
-                 type: str) -> None:
+    def __init__(
+        self,
+        ddoc: str,
+        def_: 'IndexDefinition',
+        name: str,
+        type: str,
+    ) -> None:
         """
         Initialize a IndexInformation object.
 
         :param str ddoc: Design document ID.
         :param IndexDefinition def_: Schema for a `json` or `text` query index
                definition. Indexes of type `text` have additional configuration properties
                that do not apply to `json` indexes, these are:
@@ -12837,33 +13405,37 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class TypeEnum(str, Enum):
         """
         Schema for the type of an index.
         """
+
         JSON = 'json'
         SPECIAL = 'special'
         TEXT = 'text'
 
 
-class IndexResult():
+
+class IndexResult:
     """
     Schema for the result of creating an index.
 
     :attr str id: Id of the design document the index was created in.
     :attr str name: Name of the index created.
     :attr str result: Flag to show whether the index was created or one already
           exists.
     """
 
-    def __init__(self,
-                 id: str,
-                 name: str,
-                 result: str) -> None:
+    def __init__(
+        self,
+        id: str,
+        name: str,
+        result: str,
+    ) -> None:
         """
         Initialize a IndexResult object.
 
         :param str id: Id of the design document the index was created in.
         :param str name: Name of the index created.
         :param str result: Flag to show whether the index was created or one
                already exists.
@@ -12924,31 +13496,35 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class ResultEnum(str, Enum):
         """
         Flag to show whether the index was created or one already exists.
         """
+
         CREATED = 'created'
         EXISTS = 'exists'
 
 
-class IndexTextOperatorDefaultField():
+
+class IndexTextOperatorDefaultField:
     """
     Schema for the text index default field configuration. The default field is used to
     index the text of all fields within a document for use with the `$text` operator.
 
     :attr Analyzer analyzer: (optional) Schema for a full text search analyzer.
     :attr bool enabled: (optional) Whether or not the default_field is enabled.
     """
 
-    def __init__(self,
-                 *,
-                 analyzer: 'Analyzer' = None,
-                 enabled: bool = None) -> None:
+    def __init__(
+        self,
+        *,
+        analyzer: 'Analyzer' = None,
+        enabled: bool = None,
+    ) -> None:
         """
         Initialize a IndexTextOperatorDefaultField object.
 
         :param Analyzer analyzer: (optional) Schema for a full text search
                analyzer.
         :param bool enabled: (optional) Whether or not the default_field is
                enabled.
@@ -12997,25 +13573,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'IndexTextOperatorDefaultField') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class IndexesInformation():
+
+class IndexesInformation:
     """
     Schema for information about the indexes in a database.
 
     :attr int total_rows: Number of total rows.
     :attr List[IndexInformation] indexes: Indexes.
     """
 
-    def __init__(self,
-                 total_rows: int,
-                 indexes: List['IndexInformation']) -> None:
+    def __init__(
+        self,
+        total_rows: int,
+        indexes: List['IndexInformation'],
+    ) -> None:
         """
         Initialize a IndexesInformation object.
 
         :param int total_rows: Number of total rows.
         :param List[IndexInformation] indexes: Indexes.
         """
         self.total_rows = total_rows
@@ -13069,26 +13648,29 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'IndexesInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class MembershipInformation():
+
+class MembershipInformation:
     """
     Schema for information about known nodes and cluster membership.
 
     :attr List[str] all_nodes: List of nodes this node knows about, including the
           ones that are part of the cluster.
     :attr List[str] cluster_nodes: All cluster nodes.
     """
 
-    def __init__(self,
-                 all_nodes: List[str],
-                 cluster_nodes: List[str]) -> None:
+    def __init__(
+        self,
+        all_nodes: List[str],
+        cluster_nodes: List[str],
+    ) -> None:
         """
         Initialize a MembershipInformation object.
 
         :param List[str] all_nodes: List of nodes this node knows about, including
                the ones that are part of the cluster.
         :param List[str] cluster_nodes: All cluster nodes.
         """
@@ -13137,24 +13719,27 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'MembershipInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Ok():
+
+class Ok:
     """
     Schema for an OK result.
 
     :attr bool ok: (optional) ok.
     """
 
-    def __init__(self,
-                 *,
-                 ok: bool = None) -> None:
+    def __init__(
+        self,
+        *,
+        ok: bool = None,
+    ) -> None:
         """
         Initialize a Ok object.
 
         :param bool ok: (optional) ok.
         """
         self.ok = ok
 
@@ -13192,37 +13777,40 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Ok') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class PartitionInformation():
+
+class PartitionInformation:
     """
     Schema for information about a database partition.
 
     :attr str db_name: The name of the database.
     :attr int doc_count: A count of the documents in the specified database
           partition.
     :attr int doc_del_count: Number of deleted documents.
     :attr str partition: The name of the partition in the database.
     :attr PartitionInformationIndexes partitioned_indexes: (optional) Schema for
           information about the partition index count and limit in a database.
     :attr PartitionInformationSizes sizes: The size of active and external data, in
           bytes.
     """
 
-    def __init__(self,
-                 db_name: str,
-                 doc_count: int,
-                 doc_del_count: int,
-                 partition: str,
-                 sizes: 'PartitionInformationSizes',
-                 *,
-                 partitioned_indexes: 'PartitionInformationIndexes' = None) -> None:
+    def __init__(
+        self,
+        db_name: str,
+        doc_count: int,
+        doc_del_count: int,
+        partition: str,
+        sizes: 'PartitionInformationSizes',
+        *,
+        partitioned_indexes: 'PartitionInformationIndexes' = None,
+    ) -> None:
         """
         Initialize a PartitionInformation object.
 
         :param str db_name: The name of the database.
         :param int doc_count: A count of the documents in the specified database
                partition.
         :param int doc_del_count: Number of deleted documents.
@@ -13309,29 +13897,32 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'PartitionInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class PartitionInformationIndexes():
+
+class PartitionInformationIndexes:
     """
     Schema for information about the partition index count and limit in a database.
 
     :attr int count: (optional) Total count of the partitioned indexes.
     :attr PartitionInformationIndexesIndexes indexes: (optional) The count breakdown
           of partitioned indexes.
     :attr int limit: (optional) The partitioned index limit.
     """
 
-    def __init__(self,
-                 *,
-                 count: int = None,
-                 indexes: 'PartitionInformationIndexesIndexes' = None,
-                 limit: int = None) -> None:
+    def __init__(
+        self,
+        *,
+        count: int = None,
+        indexes: 'PartitionInformationIndexesIndexes' = None,
+        limit: int = None,
+    ) -> None:
         """
         Initialize a PartitionInformationIndexes object.
 
         :param int count: (optional) Total count of the partitioned indexes.
         :param PartitionInformationIndexesIndexes indexes: (optional) The count
                breakdown of partitioned indexes.
         :param int limit: (optional) The partitioned index limit.
@@ -13385,26 +13976,29 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'PartitionInformationIndexes') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class PartitionInformationIndexesIndexes():
+
+class PartitionInformationIndexesIndexes:
     """
     The count breakdown of partitioned indexes.
 
     :attr int search: (optional) Number of partitioned search indexes.
     :attr int view: (optional) Number of partitioned view indexes.
     """
 
-    def __init__(self,
-                 *,
-                 search: int = None,
-                 view: int = None) -> None:
+    def __init__(
+        self,
+        *,
+        search: int = None,
+        view: int = None,
+    ) -> None:
         """
         Initialize a PartitionInformationIndexesIndexes object.
 
         :param int search: (optional) Number of partitioned search indexes.
         :param int view: (optional) Number of partitioned view indexes.
         """
         self.search = search
@@ -13448,28 +14042,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'PartitionInformationIndexesIndexes') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class PartitionInformationSizes():
+
+class PartitionInformationSizes:
     """
     The size of active and external data, in bytes.
 
     :attr int active: (optional) The size of live data inside the database, in
           bytes.
     :attr int external: (optional) The uncompressed size of database contents in
           bytes.
     """
 
-    def __init__(self,
-                 *,
-                 active: int = None,
-                 external: int = None) -> None:
+    def __init__(
+        self,
+        *,
+        active: int = None,
+        external: int = None,
+    ) -> None:
         """
         Initialize a PartitionInformationSizes object.
 
         :param int active: (optional) The size of live data inside the database, in
                bytes.
         :param int external: (optional) The uncompressed size of database contents
                in bytes.
@@ -13515,31 +14112,34 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'PartitionInformationSizes') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ReplicationCreateTargetParameters():
+
+class ReplicationCreateTargetParameters:
     """
     Request parameters to use during target database creation.
 
     :attr int n: (optional) Schema for the number of replicas of a database in a
           cluster.
     :attr bool partitioned: (optional) Parameter to specify whether to enable
           database partitions when creating the target database.
     :attr int q: (optional) Schema for the number of shards in a database. Each
           shard is a partition of the hash value range.
     """
 
-    def __init__(self,
-                 *,
-                 n: int = None,
-                 partitioned: bool = None,
-                 q: int = None) -> None:
+    def __init__(
+        self,
+        *,
+        n: int = None,
+        partitioned: bool = None,
+        q: int = None,
+    ) -> None:
         """
         Initialize a ReplicationCreateTargetParameters object.
 
         :param int n: (optional) Schema for the number of replicas of a database in
                a cluster.
         :param bool partitioned: (optional) Parameter to specify whether to enable
                database partitions when creating the target database.
@@ -13592,29 +14192,32 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ReplicationCreateTargetParameters') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ReplicationDatabase():
+
+class ReplicationDatabase:
     """
     Schema for a replication source or target database.
 
     :attr ReplicationDatabaseAuth auth: (optional) Schema for replication source or
           target database authentication.
     :attr dict headers_: (optional) Replication request headers.
     :attr str url: Replication database URL.
     """
 
-    def __init__(self,
-                 url: str,
-                 *,
-                 auth: 'ReplicationDatabaseAuth' = None,
-                 headers_: dict = None) -> None:
+    def __init__(
+        self,
+        url: str,
+        *,
+        auth: 'ReplicationDatabaseAuth' = None,
+        headers_: dict = None,
+    ) -> None:
         """
         Initialize a ReplicationDatabase object.
 
         :param str url: Replication database URL.
         :param ReplicationDatabaseAuth auth: (optional) Schema for replication
                source or target database authentication.
         :param dict headers_: (optional) Replication request headers.
@@ -13670,28 +14273,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ReplicationDatabase') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ReplicationDatabaseAuth():
+
+class ReplicationDatabaseAuth:
     """
     Schema for replication source or target database authentication.
 
     :attr ReplicationDatabaseAuthBasic basic: (optional) Schema for basic
           authentication of replication source or target database.
     :attr ReplicationDatabaseAuthIam iam: (optional) Schema for an IAM API key for
           replication database authentication.
     """
 
-    def __init__(self,
-                 *,
-                 basic: 'ReplicationDatabaseAuthBasic' = None,
-                 iam: 'ReplicationDatabaseAuthIam' = None) -> None:
+    def __init__(
+        self,
+        *,
+        basic: 'ReplicationDatabaseAuthBasic' = None,
+        iam: 'ReplicationDatabaseAuthIam' = None,
+    ) -> None:
         """
         Initialize a ReplicationDatabaseAuth object.
 
         :param ReplicationDatabaseAuthBasic basic: (optional) Schema for basic
                authentication of replication source or target database.
         :param ReplicationDatabaseAuthIam iam: (optional) Schema for an IAM API key
                for replication database authentication.
@@ -13743,25 +14349,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ReplicationDatabaseAuth') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ReplicationDatabaseAuthBasic():
+
+class ReplicationDatabaseAuthBasic:
     """
     Schema for basic authentication of replication source or target database.
 
     :attr str password: The password associated with the username.
     :attr str username: The username.
     """
 
-    def __init__(self,
-                 password: str,
-                 username: str) -> None:
+    def __init__(
+        self,
+        password: str,
+        username: str,
+    ) -> None:
         """
         Initialize a ReplicationDatabaseAuthBasic object.
 
         :param str password: The password associated with the username.
         :param str username: The username.
         """
         self.password = password
@@ -13809,23 +14418,26 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ReplicationDatabaseAuthBasic') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ReplicationDatabaseAuthIam():
+
+class ReplicationDatabaseAuthIam:
     """
     Schema for an IAM API key for replication database authentication.
 
     :attr str api_key: IAM API key.
     """
 
-    def __init__(self,
-                 api_key: str) -> None:
+    def __init__(
+        self,
+        api_key: str,
+    ) -> None:
         """
         Initialize a ReplicationDatabaseAuthIam object.
 
         :param str api_key: IAM API key.
         """
         self.api_key = api_key
 
@@ -13865,15 +14477,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ReplicationDatabaseAuthIam') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ReplicationDocument():
+
+class ReplicationDocument:
     """
     Schema for a replication document. Note that `selector`, `doc_ids`, and `filter` are
     incompatible with each other.
 
     :attr dict attachments: (optional) Schema for a map of attachment name to
           attachment metadata.
     :attr List[str] conflicts: (optional) Schema for a list of document revision
@@ -13971,50 +14584,52 @@
           read from the changes manager and write to the target. A higher number can
           improve throughput.
     """
 
     # The set of defined properties for the class
     _properties = frozenset(['attachments', '_attachments', 'conflicts', '_conflicts', 'deleted', '_deleted', 'deleted_conflicts', '_deleted_conflicts', 'id', '_id', 'local_seq', '_local_seq', 'rev', '_rev', 'revisions', '_revisions', 'revs_info', '_revs_info', 'cancel', 'checkpoint_interval', 'connection_timeout', 'continuous', 'create_target', 'create_target_params', 'doc_ids', 'filter', 'http_connections', 'query_params', 'retries_per_request', 'selector', 'since_seq', 'socket_options', 'source', 'source_proxy', 'target', 'target_proxy', 'use_bulk_get', 'use_checkpoints', 'user_ctx', 'winning_revs_only', 'worker_batch_size', 'worker_processes'])
 
-    def __init__(self,
-                 source: 'ReplicationDatabase',
-                 target: 'ReplicationDatabase',
-                 *,
-                 attachments: dict = None,
-                 conflicts: List[str] = None,
-                 deleted: bool = None,
-                 deleted_conflicts: List[str] = None,
-                 id: str = None,
-                 local_seq: str = None,
-                 rev: str = None,
-                 revisions: 'Revisions' = None,
-                 revs_info: List['DocumentRevisionStatus'] = None,
-                 cancel: bool = None,
-                 checkpoint_interval: int = None,
-                 connection_timeout: int = None,
-                 continuous: bool = None,
-                 create_target: bool = None,
-                 create_target_params: 'ReplicationCreateTargetParameters' = None,
-                 doc_ids: List[str] = None,
-                 filter: str = None,
-                 http_connections: int = None,
-                 query_params: dict = None,
-                 retries_per_request: int = None,
-                 selector: dict = None,
-                 since_seq: str = None,
-                 socket_options: str = None,
-                 source_proxy: str = None,
-                 target_proxy: str = None,
-                 use_bulk_get: bool = None,
-                 use_checkpoints: bool = None,
-                 user_ctx: 'UserContext' = None,
-                 winning_revs_only: bool = None,
-                 worker_batch_size: int = None,
-                 worker_processes: int = None,
-                 **kwargs) -> None:
+    def __init__(
+        self,
+        source: 'ReplicationDatabase',
+        target: 'ReplicationDatabase',
+        *,
+        attachments: dict = None,
+        conflicts: List[str] = None,
+        deleted: bool = None,
+        deleted_conflicts: List[str] = None,
+        id: str = None,
+        local_seq: str = None,
+        rev: str = None,
+        revisions: 'Revisions' = None,
+        revs_info: List['DocumentRevisionStatus'] = None,
+        cancel: bool = None,
+        checkpoint_interval: int = None,
+        connection_timeout: int = None,
+        continuous: bool = None,
+        create_target: bool = None,
+        create_target_params: 'ReplicationCreateTargetParameters' = None,
+        doc_ids: List[str] = None,
+        filter: str = None,
+        http_connections: int = None,
+        query_params: dict = None,
+        retries_per_request: int = None,
+        selector: dict = None,
+        since_seq: str = None,
+        socket_options: str = None,
+        source_proxy: str = None,
+        target_proxy: str = None,
+        use_bulk_get: bool = None,
+        use_checkpoints: bool = None,
+        user_ctx: 'UserContext' = None,
+        winning_revs_only: bool = None,
+        worker_batch_size: int = None,
+        worker_processes: int = None,
+        **kwargs,
+    ) -> None:
         """
         Initialize a ReplicationDocument object.
 
         :param ReplicationDatabase source: Schema for a replication source or
                target database.
         :param ReplicationDatabase target: Schema for a replication source or
                target database.
@@ -14158,15 +14773,15 @@
             setattr(self, _key, _value)
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ReplicationDocument':
         """Initialize a ReplicationDocument object from a json dictionary."""
         args = {}
         if '_attachments' in _dict:
-            args['attachments'] = {k : Attachment.from_dict(v) for k, v in _dict.get('_attachments').items()}
+            args['attachments'] = {k: Attachment.from_dict(v) for k, v in _dict.get('_attachments').items()}
         if '_conflicts' in _dict:
             args['conflicts'] = _dict.get('_conflicts')
         if '_deleted' in _dict:
             args['deleted'] = _dict.get('_deleted')
         if '_deleted_conflicts' in _dict:
             args['deleted_conflicts'] = _dict.get('_deleted_conflicts')
         if '_id' in _dict:
@@ -14227,15 +14842,15 @@
             args['user_ctx'] = UserContext.from_dict(_dict.get('user_ctx'))
         if 'winning_revs_only' in _dict:
             args['winning_revs_only'] = _dict.get('winning_revs_only')
         if 'worker_batch_size' in _dict:
             args['worker_batch_size'] = _dict.get('worker_batch_size')
         if 'worker_processes' in _dict:
             args['worker_processes'] = _dict.get('worker_processes')
-        args.update({k:v for (k, v) in _dict.items() if k not in cls._properties})
+        args.update({k: v for (k, v) in _dict.items() if k not in cls._properties})
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ReplicationDocument object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -14370,26 +14985,29 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ReplicationDocument') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Revisions():
+
+class Revisions:
     """
     Schema for list of revision information.
 
     :attr List[str] ids: Array of valid revision IDs, in reverse order (latest
           first).
     :attr int start: Prefix number for the latest revision.
     """
 
-    def __init__(self,
-                 ids: List[str],
-                 start: int) -> None:
+    def __init__(
+        self,
+        ids: List[str],
+        start: int,
+    ) -> None:
         """
         Initialize a Revisions object.
 
         :param List[str] ids: Array of valid revision IDs, in reverse order (latest
                first).
         :param int start: Prefix number for the latest revision.
         """
@@ -14438,27 +15056,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Revisions') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class RevsDiff():
+
+class RevsDiff:
     """
     Schema for information about missing revs and possible ancestors.
 
     :attr List[str] missing: (optional) List of missing revisions.
     :attr List[str] possible_ancestors: (optional) List of possible ancestor
           revisions.
     """
 
-    def __init__(self,
-                 *,
-                 missing: List[str] = None,
-                 possible_ancestors: List[str] = None) -> None:
+    def __init__(
+        self,
+        *,
+        missing: List[str] = None,
+        possible_ancestors: List[str] = None,
+    ) -> None:
         """
         Initialize a RevsDiff object.
 
         :param List[str] missing: (optional) List of missing revisions.
         :param List[str] possible_ancestors: (optional) List of possible ancestor
                revisions.
         """
@@ -14503,25 +15124,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'RevsDiff') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SchedulerDocsResult():
+
+class SchedulerDocsResult:
     """
     Schema for a listing of replication scheduler documents.
 
     :attr int total_rows: Number of total rows.
     :attr List[SchedulerDocument] docs: Array of replication scheduler doc objects.
     """
 
-    def __init__(self,
-                 total_rows: int,
-                 docs: List['SchedulerDocument']) -> None:
+    def __init__(
+        self,
+        total_rows: int,
+        docs: List['SchedulerDocument'],
+    ) -> None:
         """
         Initialize a SchedulerDocsResult object.
 
         :param int total_rows: Number of total rows.
         :param List[SchedulerDocument] docs: Array of replication scheduler doc
                objects.
         """
@@ -14576,15 +15200,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SchedulerDocsResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SchedulerDocument():
+
+class SchedulerDocument:
     """
     Schema for a replication scheduler document.
 
     :attr str database: Database where replication document came from.
     :attr str doc_id: Replication document ID.
     :attr int error_count: Consecutive errors count. Indicates how many times in a
           row this replication has crashed. Replication will be retried with an
@@ -14603,29 +15228,31 @@
     :attr datetime start_time: Timestamp of when the replication was started.
     :attr str state: Schema for replication state.
     :attr str target: (optional) Replication target.
     :attr str target_proxy: (optional) Address of the (http or socks5 protocol)
           proxy server through which replication with the target database occurs.
     """
 
-    def __init__(self,
-                 database: str,
-                 doc_id: str,
-                 error_count: int,
-                 id: str,
-                 info: 'SchedulerInfo',
-                 last_updated: datetime,
-                 start_time: datetime,
-                 state: str,
-                 *,
-                 node: str = None,
-                 source: str = None,
-                 source_proxy: str = None,
-                 target: str = None,
-                 target_proxy: str = None) -> None:
+    def __init__(
+        self,
+        database: str,
+        doc_id: str,
+        error_count: int,
+        id: str,
+        info: 'SchedulerInfo',
+        last_updated: datetime,
+        start_time: datetime,
+        state: str,
+        *,
+        node: str = None,
+        source: str = None,
+        source_proxy: str = None,
+        target: str = None,
+        target_proxy: str = None,
+    ) -> None:
         """
         Initialize a SchedulerDocument object.
 
         :param str database: Database where replication document came from.
         :param str doc_id: Replication document ID.
         :param int error_count: Consecutive errors count. Indicates how many times
                in a row this replication has crashed. Replication will be retried with an
@@ -14768,24 +15395,26 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StateEnum(str, Enum):
         """
         Schema for replication state.
         """
+
         INITIALIZING = 'initializing'
         ERROR = 'error'
         PENDING = 'pending'
         RUNNING = 'running'
         CRASHING = 'crashing'
         COMPLETED = 'completed'
         FAILED = 'failed'
 
 
-class SchedulerInfo():
+
+class SchedulerInfo:
     """
     Schema for scheduler document information. A JSON object that may contain additional
     information about the state. For error states this will contain an error field and
     string value.
 
     :attr int changes_pending: (optional) The count of changes not yet replicated.
     :attr str checkpointed_source_seq: (optional) The source sequence id which was
@@ -14803,26 +15432,28 @@
           checked since this replication began.
     :attr str source_seq: (optional) The last sequence number obtained from the
           source database changes feed.
     :attr str through_seq: (optional) The last sequence number processed by the
           replicator.
     """
 
-    def __init__(self,
-                 *,
-                 changes_pending: int = None,
-                 checkpointed_source_seq: str = None,
-                 doc_write_failures: int = None,
-                 docs_read: int = None,
-                 docs_written: int = None,
-                 error: str = None,
-                 missing_revisions_found: int = None,
-                 revisions_checked: int = None,
-                 source_seq: str = None,
-                 through_seq: str = None) -> None:
+    def __init__(
+        self,
+        *,
+        changes_pending: int = None,
+        checkpointed_source_seq: str = None,
+        doc_write_failures: int = None,
+        docs_read: int = None,
+        docs_written: int = None,
+        error: str = None,
+        missing_revisions_found: int = None,
+        revisions_checked: int = None,
+        source_seq: str = None,
+        through_seq: str = None,
+    ) -> None:
         """
         Initialize a SchedulerInfo object.
 
         :param int changes_pending: (optional) The count of changes not yet
                replicated.
         :param str checkpointed_source_seq: (optional) The source sequence id which
                was last successfully replicated.
@@ -14923,15 +15554,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SchedulerInfo') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SchedulerJob():
+
+class SchedulerJob:
     """
     Schema for a replication scheduler job.
 
     :attr str database: Replication document database.
     :attr str doc_id: Replication document ID.
     :attr List[SchedulerJobEvent] history: Timestamped history of events as a list
           of objects.
@@ -14943,26 +15575,28 @@
     :attr str pid: Replication process ID.
     :attr str source: Replication source.
     :attr datetime start_time: Timestamp of when the replication was started.
     :attr str target: Replication target.
     :attr str user: Name of user running replication.
     """
 
-    def __init__(self,
-                 database: str,
-                 doc_id: str,
-                 history: List['SchedulerJobEvent'],
-                 id: str,
-                 info: 'SchedulerInfo',
-                 node: str,
-                 pid: str,
-                 source: str,
-                 start_time: datetime,
-                 target: str,
-                 user: str) -> None:
+    def __init__(
+        self,
+        database: str,
+        doc_id: str,
+        history: List['SchedulerJobEvent'],
+        id: str,
+        info: 'SchedulerInfo',
+        node: str,
+        pid: str,
+        source: str,
+        start_time: datetime,
+        target: str,
+        user: str,
+    ) -> None:
         """
         Initialize a SchedulerJob object.
 
         :param str database: Replication document database.
         :param str doc_id: Replication document ID.
         :param List[SchedulerJobEvent] history: Timestamped history of events as a
                list of objects.
@@ -15094,28 +15728,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SchedulerJob') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SchedulerJobEvent():
+
+class SchedulerJobEvent:
     """
     Schema for a replication scheduler job event.
 
     :attr str reason: (optional) Reason for current state of event.
     :attr datetime timestamp: Timestamp of the event.
     :attr str type: Type of the event.
     """
 
-    def __init__(self,
-                 timestamp: datetime,
-                 type: str,
-                 *,
-                 reason: str = None) -> None:
+    def __init__(
+        self,
+        timestamp: datetime,
+        type: str,
+        *,
+        reason: str = None,
+    ) -> None:
         """
         Initialize a SchedulerJobEvent object.
 
         :param datetime timestamp: Timestamp of the event.
         :param str type: Type of the event.
         :param str reason: (optional) Reason for current state of event.
         """
@@ -15169,25 +15806,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SchedulerJobEvent') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SchedulerJobsResult():
+
+class SchedulerJobsResult:
     """
     Schema for a listing of replication scheduler jobs.
 
     :attr int total_rows: Number of total rows.
     :attr List[SchedulerJob] jobs: Array of replication job objects.
     """
 
-    def __init__(self,
-                 total_rows: int,
-                 jobs: List['SchedulerJob']) -> None:
+    def __init__(
+        self,
+        total_rows: int,
+        jobs: List['SchedulerJob'],
+    ) -> None:
         """
         Initialize a SchedulerJobsResult object.
 
         :param int total_rows: Number of total rows.
         :param List[SchedulerJob] jobs: Array of replication job objects.
         """
         self.total_rows = total_rows
@@ -15241,23 +15881,26 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SchedulerJobsResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchAnalyzeResult():
+
+class SearchAnalyzeResult:
     """
     Schema for the output of testing search analyzer tokenization.
 
     :attr List[str] tokens: tokens.
     """
 
-    def __init__(self,
-                 tokens: List[str]) -> None:
+    def __init__(
+        self,
+        tokens: List[str],
+    ) -> None:
         """
         Initialize a SearchAnalyzeResult object.
 
         :param List[str] tokens: tokens.
         """
         self.tokens = tokens
 
@@ -15297,15 +15940,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchAnalyzeResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchIndexDefinition():
+
+class SearchIndexDefinition:
     """
     Schema for a search index definition.
 
     :attr AnalyzerConfiguration analyzer: (optional) Schema for a search analyzer
           configuration.
     :attr str index: String form of a JavaScript function that is called for each
           document in the database. The function takes the document as a parameter,
@@ -15323,18 +15967,20 @@
               * `index` - boolean, default `true` - If set to `false`, the data
                 cannot be used for searches, but can still be retrieved from the
                 index if `store` is set to `true`.
               * `store` - boolean, default `true` - If true, the value is returned
                 in the search result; otherwise, the value is not returned.
     """
 
-    def __init__(self,
-                 index: str,
-                 *,
-                 analyzer: 'AnalyzerConfiguration' = None) -> None:
+    def __init__(
+        self,
+        index: str,
+        *,
+        analyzer: 'AnalyzerConfiguration' = None,
+    ) -> None:
         """
         Initialize a SearchIndexDefinition object.
 
         :param str index: String form of a JavaScript function that is called for
                each document in the database. The function takes the document as a
                parameter, extracts some data from it, and then calls the `index` function
                to index that data. The index function takes 2, or optionally 3,
@@ -15402,33 +16048,36 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchIndexDefinition') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchIndexInfo():
+
+class SearchIndexInfo:
     """
     Schema for metadata information about a search index.
 
     :attr int committed_seq: The committed sequence identifier.
     :attr int disk_size: The size of the search index on disk.
     :attr int doc_count: The count of the number of indexed documents.
     :attr int doc_del_count: The number of deleted documents.
     :attr int pending_seq: The pending sequence identifier.
     :attr str signature: Unique signature of the search index.
     """
 
-    def __init__(self,
-                 committed_seq: int,
-                 disk_size: int,
-                 doc_count: int,
-                 doc_del_count: int,
-                 pending_seq: int,
-                 signature: str) -> None:
+    def __init__(
+        self,
+        committed_seq: int,
+        disk_size: int,
+        doc_count: int,
+        doc_del_count: int,
+        pending_seq: int,
+        signature: str,
+    ) -> None:
         """
         Initialize a SearchIndexInfo object.
 
         :param int committed_seq: The committed sequence identifier.
         :param int disk_size: The size of the search index on disk.
         :param int doc_count: The count of the number of indexed documents.
         :param int doc_del_count: The number of deleted documents.
@@ -15508,27 +16157,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchIndexInfo') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchInfoResult():
+
+class SearchInfoResult:
     """
     Schema for search index information.
 
     :attr str name: The name of the search index prefixed by the design document ID
           where the index is stored.
     :attr SearchIndexInfo search_index: Schema for metadata information about a
           search index.
     """
 
-    def __init__(self,
-                 name: str,
-                 search_index: 'SearchIndexInfo') -> None:
+    def __init__(
+        self,
+        name: str,
+        search_index: 'SearchIndexInfo',
+    ) -> None:
         """
         Initialize a SearchInfoResult object.
 
         :param str name: The name of the search index prefixed by the design
                document ID where the index is stored.
         :param SearchIndexInfo search_index: Schema for metadata information about
                a search index.
@@ -15581,15 +16233,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchInfoResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchResult():
+
+class SearchResult:
     """
     Schema for the result of a query search operation.
 
     :attr int total_rows: Number of total rows.
     :attr str bookmark: (optional) Opaque bookmark token used when paginating
           results.
     :attr str by: (optional) Grouped search matches.
@@ -15599,23 +16252,25 @@
           syntax for ranges to return counts of results that fit into each specified
           category.
     :attr List[SearchResultRow] rows: (optional) Array of row objects.
     :attr List[SearchResultProperties] groups: (optional) Array of grouped search
           matches.
     """
 
-    def __init__(self,
-                 total_rows: int,
-                 *,
-                 bookmark: str = None,
-                 by: str = None,
-                 counts: dict = None,
-                 ranges: dict = None,
-                 rows: List['SearchResultRow'] = None,
-                 groups: List['SearchResultProperties'] = None) -> None:
+    def __init__(
+        self,
+        total_rows: int,
+        *,
+        bookmark: str = None,
+        by: str = None,
+        counts: dict = None,
+        ranges: dict = None,
+        rows: List['SearchResultRow'] = None,
+        groups: List['SearchResultProperties'] = None,
+    ) -> None:
         """
         Initialize a SearchResult object.
 
         :param int total_rows: Number of total rows.
         :param str bookmark: (optional) Opaque bookmark token used when paginating
                results.
         :param str by: (optional) Grouped search matches.
@@ -15708,15 +16363,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchResultProperties():
+
+class SearchResultProperties:
     """
     Schema for the result of a query search operation.
 
     :attr int total_rows: Number of total rows.
     :attr str bookmark: (optional) Opaque bookmark token used when paginating
           results.
     :attr str by: (optional) Grouped search matches.
@@ -15724,22 +16380,24 @@
           query results for each unique value of each named field.
     :attr dict ranges: (optional) The range facet syntax reuses the standard Lucene
           syntax for ranges to return counts of results that fit into each specified
           category.
     :attr List[SearchResultRow] rows: (optional) Array of row objects.
     """
 
-    def __init__(self,
-                 total_rows: int,
-                 *,
-                 bookmark: str = None,
-                 by: str = None,
-                 counts: dict = None,
-                 ranges: dict = None,
-                 rows: List['SearchResultRow'] = None) -> None:
+    def __init__(
+        self,
+        total_rows: int,
+        *,
+        bookmark: str = None,
+        by: str = None,
+        counts: dict = None,
+        ranges: dict = None,
+        rows: List['SearchResultRow'] = None,
+    ) -> None:
         """
         Initialize a SearchResultProperties object.
 
         :param int total_rows: Number of total rows.
         :param str bookmark: (optional) Opaque bookmark token used when paginating
                results.
         :param str by: (optional) Grouped search matches.
@@ -15819,32 +16477,35 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchResultProperties') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SearchResultRow():
+
+class SearchResultRow:
     """
     Schema for a row of the result of a query search operation.
 
     :attr Document doc: (optional) Schema for a document.
     :attr dict fields: Schema for the fields returned by a query search operation, a
           map of field name to value.
     :attr dict highlights: (optional) Returns the context in which a search term was
           mentioned so that you can display more emphasized results to a user.
     :attr str id: Schema for a document ID.
     """
 
-    def __init__(self,
-                 fields: dict,
-                 id: str,
-                 *,
-                 doc: 'Document' = None,
-                 highlights: dict = None) -> None:
+    def __init__(
+        self,
+        fields: dict,
+        id: str,
+        *,
+        doc: 'Document' = None,
+        highlights: dict = None,
+    ) -> None:
         """
         Initialize a SearchResultRow object.
 
         :param dict fields: Schema for the fields returned by a query search
                operation, a map of field name to value.
         :param str id: Schema for a document ID.
         :param Document doc: (optional) Schema for a document.
@@ -15910,34 +16571,37 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SearchResultRow') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class Security():
+
+class Security:
     """
     Schema for a security document.
 
     :attr SecurityObject admins: (optional) Schema for names and roles to map to a
           database permission.
     :attr SecurityObject members: (optional) Schema for names and roles to map to a
           database permission.
     :attr dict cloudant: (optional) Database permissions for Cloudant users and/or
           API keys.
     :attr bool couchdb_auth_only: (optional) Manage permissions using the `_users`
           database only.
     """
 
-    def __init__(self,
-                 *,
-                 admins: 'SecurityObject' = None,
-                 members: 'SecurityObject' = None,
-                 cloudant: dict = None,
-                 couchdb_auth_only: bool = None) -> None:
+    def __init__(
+        self,
+        *,
+        admins: 'SecurityObject' = None,
+        members: 'SecurityObject' = None,
+        cloudant: dict = None,
+        couchdb_auth_only: bool = None,
+    ) -> None:
         """
         Initialize a Security object.
 
         :param SecurityObject admins: (optional) Schema for names and roles to map
                to a database permission.
         :param SecurityObject members: (optional) Schema for names and roles to map
                to a database permission.
@@ -16007,36 +16671,40 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class CloudantEnum(str, Enum):
         """
         Database permissions for Cloudant users and/or API keys.
         """
+
         READER = '_reader'
         WRITER = '_writer'
         ADMIN = '_admin'
         REPLICATOR = '_replicator'
         DB_UPDATES = '_db_updates'
         DESIGN = '_design'
         SHARDS = '_shards'
         SECURITY = '_security'
 
 
-class SecurityObject():
+
+class SecurityObject:
     """
     Schema for names and roles to map to a database permission.
 
     :attr List[str] names: (optional) List of usernames.
     :attr List[str] roles: (optional) List of roles.
     """
 
-    def __init__(self,
-                 *,
-                 names: List[str] = None,
-                 roles: List[str] = None) -> None:
+    def __init__(
+        self,
+        *,
+        names: List[str] = None,
+        roles: List[str] = None,
+    ) -> None:
         """
         Initialize a SecurityObject object.
 
         :param List[str] names: (optional) List of usernames.
         :param List[str] roles: (optional) List of roles.
         """
         self.names = names
@@ -16080,31 +16748,34 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SecurityObject') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ServerInformation():
+
+class ServerInformation:
     """
     Schema for information about the server instance.
 
     :attr str couchdb: Welcome message.
     :attr List[str] features: List of enabled optional features.
     :attr ServerVendor vendor: Schema for server vendor information.
     :attr str version: Apache CouchDB version.
     :attr List[str] features_flags: List of feature flags.
     """
 
-    def __init__(self,
-                 couchdb: str,
-                 features: List[str],
-                 vendor: 'ServerVendor',
-                 version: str,
-                 features_flags: List[str]) -> None:
+    def __init__(
+        self,
+        couchdb: str,
+        features: List[str],
+        vendor: 'ServerVendor',
+        version: str,
+        features_flags: List[str],
+    ) -> None:
         """
         Initialize a ServerInformation object.
 
         :param str couchdb: Welcome message.
         :param List[str] features: List of enabled optional features.
         :param ServerVendor vendor: Schema for server vendor information.
         :param str version: Apache CouchDB version.
@@ -16179,28 +16850,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ServerInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ServerVendor():
+
+class ServerVendor:
     """
     Schema for server vendor information.
 
     :attr str name: Vendor name.
     :attr str variant: (optional) Vendor variant.
     :attr str version: (optional) Vendor version.
     """
 
-    def __init__(self,
-                 name: str,
-                 *,
-                 variant: str = None,
-                 version: str = None) -> None:
+    def __init__(
+        self,
+        name: str,
+        *,
+        variant: str = None,
+        version: str = None,
+    ) -> None:
         """
         Initialize a ServerVendor object.
 
         :param str name: Vendor name.
         :param str variant: (optional) Vendor variant.
         :param str version: (optional) Vendor version.
         """
@@ -16252,28 +16926,31 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ServerVendor') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SessionAuthentication():
+
+class SessionAuthentication:
     """
     Schema for session authentication information.
 
     :attr str authenticated: (optional) authenticated.
     :attr str authentication_db: (optional) authentication_db.
     :attr List[str] authentication_handlers: authentication_handlers.
     """
 
-    def __init__(self,
-                 authentication_handlers: List[str],
-                 *,
-                 authenticated: str = None,
-                 authentication_db: str = None) -> None:
+    def __init__(
+        self,
+        authentication_handlers: List[str],
+        *,
+        authenticated: str = None,
+        authentication_db: str = None,
+    ) -> None:
         """
         Initialize a SessionAuthentication object.
 
         :param List[str] authentication_handlers: authentication_handlers.
         :param str authenticated: (optional) authenticated.
         :param str authentication_db: (optional) authentication_db.
         """
@@ -16325,27 +17002,30 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SessionAuthentication') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class SessionInformation():
+
+class SessionInformation:
     """
     Schema for information about a session.
 
     :attr bool ok: ok.
     :attr SessionAuthentication info: Schema for session authentication information.
     :attr UserContext user_ctx: Schema for the user context of a session.
     """
 
-    def __init__(self,
-                 ok: bool,
-                 info: 'SessionAuthentication',
-                 user_ctx: 'UserContext') -> None:
+    def __init__(
+        self,
+        ok: bool,
+        info: 'SessionAuthentication',
+        user_ctx: 'UserContext',
+    ) -> None:
         """
         Initialize a SessionInformation object.
 
         :param bool ok: ok.
         :param SessionAuthentication info: Schema for session authentication
                information.
         :param UserContext user_ctx: Schema for the user context of a session.
@@ -16408,24 +17088,27 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SessionInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ShardsInformation():
+
+class ShardsInformation:
     """
     Schema for a shards object that maps the hash value range for each shard to the array
     of nodes that contain a copy of that shard.
 
     :attr dict shards: Mapping of shard hash value range to a list of nodes.
     """
 
-    def __init__(self,
-                 shards: dict) -> None:
+    def __init__(
+        self,
+        shards: dict,
+    ) -> None:
         """
         Initialize a ShardsInformation object.
 
         :param dict shards: Mapping of shard hash value range to a list of nodes.
         """
         self.shards = shards
 
@@ -16465,32 +17148,35 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ShardsInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ThroughputInformation():
+
+class ThroughputInformation:
     """
     Schema for detailed information about throughput capacity with breakdown by specific
     throughput requests classes.
 
     :attr int blocks: A number of blocks of throughput units. A block consists of
           100 reads/sec, 50 writes/sec, and 5 global queries/sec of provisioned throughput
           capacity.
     :attr int query: Provisioned global queries capacity in operations per second.
     :attr int read: Provisioned reads capacity in operations per second.
     :attr int write: Provisioned writes capacity in operations per second.
     """
 
-    def __init__(self,
-                 blocks: int,
-                 query: int,
-                 read: int,
-                 write: int) -> None:
+    def __init__(
+        self,
+        blocks: int,
+        query: int,
+        read: int,
+        write: int,
+    ) -> None:
         """
         Initialize a ThroughputInformation object.
 
         :param int blocks: A number of blocks of throughput units. A block consists
                of 100 reads/sec, 50 writes/sec, and 5 global queries/sec of provisioned
                throughput capacity.
         :param int query: Provisioned global queries capacity in operations per
@@ -16557,25 +17243,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ThroughputInformation') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class UpInformation():
+
+class UpInformation:
     """
     Schema for information about the up state of the server.
 
     :attr dict seeds: seeds.
     :attr str status: status.
     """
 
-    def __init__(self,
-                 seeds: dict,
-                 status: str) -> None:
+    def __init__(
+        self,
+        seeds: dict,
+        status: str,
+    ) -> None:
         """
         Initialize a UpInformation object.
 
         :param dict seeds: seeds.
         :param str status: status.
         """
         self.seeds = seeds
@@ -16627,33 +17316,121 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class StatusEnum(str, Enum):
         """
         status.
         """
+
         MAINTENANCE_MODE = 'maintenance_mode'
         NOLB = 'nolb'
         OK = 'ok'
 
 
-class UserContext():
+
+class UpdatesPending:
+    """
+    Schema for an ability to tell if view is up-to-date without querying it.
+
+    :attr int minimum: Sum of shard copies with the least amount of work to do.
+    :attr int preferred: Sum of unique shards. This value is zero when at least one
+          copy of every shard range is up-to-date and the view is able to answer a query
+          without index building delays.
+    :attr int total: Sum of all shard copies.
+    """
+
+    def __init__(
+        self,
+        minimum: int,
+        preferred: int,
+        total: int,
+    ) -> None:
+        """
+        Initialize a UpdatesPending object.
+
+        :param int minimum: Sum of shard copies with the least amount of work to
+               do.
+        :param int preferred: Sum of unique shards. This value is zero when at
+               least one copy of every shard range is up-to-date and the view is able to
+               answer a query without index building delays.
+        :param int total: Sum of all shard copies.
+        """
+        self.minimum = minimum
+        self.preferred = preferred
+        self.total = total
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'UpdatesPending':
+        """Initialize a UpdatesPending object from a json dictionary."""
+        args = {}
+        if 'minimum' in _dict:
+            args['minimum'] = _dict.get('minimum')
+        else:
+            raise ValueError('Required property \'minimum\' not present in UpdatesPending JSON')
+        if 'preferred' in _dict:
+            args['preferred'] = _dict.get('preferred')
+        else:
+            raise ValueError('Required property \'preferred\' not present in UpdatesPending JSON')
+        if 'total' in _dict:
+            args['total'] = _dict.get('total')
+        else:
+            raise ValueError('Required property \'total\' not present in UpdatesPending JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a UpdatesPending object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'minimum') and self.minimum is not None:
+            _dict['minimum'] = self.minimum
+        if hasattr(self, 'preferred') and self.preferred is not None:
+            _dict['preferred'] = self.preferred
+        if hasattr(self, 'total') and self.total is not None:
+            _dict['total'] = self.total
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this UpdatesPending object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'UpdatesPending') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'UpdatesPending') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class UserContext:
     """
     Schema for the user context of a session.
 
     :attr str db: (optional) Database name in the context of the provided operation.
     :attr str name: User name.
     :attr List[str] roles: List of user roles.
     """
 
-    def __init__(self,
-                 name: str,
-                 roles: List[str],
-                 *,
-                 db: str = None) -> None:
+    def __init__(
+        self,
+        name: str,
+        roles: List[str],
+        *,
+        db: str = None,
+    ) -> None:
         """
         Initialize a UserContext object.
 
         :param str name: User name.
         :param List[str] roles: List of user roles.
         :param str db: (optional) Database name in the context of the provided
                operation.
@@ -16712,33 +17489,37 @@
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
     class RolesEnum(str, Enum):
         """
         Schema for a security role.
         """
+
         READER = '_reader'
         WRITER = '_writer'
         ADMIN = '_admin'
         REPLICATOR = '_replicator'
         DB_UPDATES = '_db_updates'
         DESIGN = '_design'
         SHARDS = '_shards'
         SECURITY = '_security'
 
 
-class UuidsResult():
+
+class UuidsResult:
     """
     Schema for a set of uuids generated by the server.
 
     :attr List[str] uuids: uuids.
     """
 
-    def __init__(self,
-                 uuids: List[str]) -> None:
+    def __init__(
+        self,
+        uuids: List[str],
+    ) -> None:
         """
         Initialize a UuidsResult object.
 
         :param List[str] uuids: uuids.
         """
         self.uuids = uuids
 
@@ -16778,25 +17559,28 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'UuidsResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ViewQueriesResult():
+
+class ViewQueriesResult:
     """
     Schema for the results of a queries view operation.
 
     :attr List[ViewResult] results: An array of result objects - one for each query.
           Each result object contains the same fields as the response to a regular view
           request.
     """
 
-    def __init__(self,
-                 results: List['ViewResult']) -> None:
+    def __init__(
+        self,
+        results: List['ViewResult'],
+    ) -> None:
         """
         Initialize a ViewQueriesResult object.
 
         :param List[ViewResult] results: An array of result objects - one for each
                query. Each result object contains the same fields as the response to a
                regular view request.
         """
@@ -16844,15 +17628,16 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ViewQueriesResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ViewQuery():
+
+class ViewQuery:
     """
     Schema for a query view operation.
 
     :attr bool att_encoding_info: (optional) Parameter to specify whether to include
           the encoding information in attachment stubs if the particular attachment is
           compressed.
     :attr bool attachments: (optional) Parameter to specify whether to include
@@ -16905,36 +17690,38 @@
           question should be updated prior to responding to the user.
           * `true` - Return results after the view is updated.
           * `false` - Return results without updating the view.
           * `lazy` - Return the view results without waiting for an update, but update
           them immediately after the request.
     """
 
-    def __init__(self,
-                 *,
-                 att_encoding_info: bool = None,
-                 attachments: bool = None,
-                 conflicts: bool = None,
-                 descending: bool = None,
-                 include_docs: bool = None,
-                 inclusive_end: bool = None,
-                 limit: int = None,
-                 skip: int = None,
-                 update_seq: bool = None,
-                 end_key: object = None,
-                 end_key_doc_id: str = None,
-                 group: bool = None,
-                 group_level: int = None,
-                 key: object = None,
-                 keys: List[object] = None,
-                 reduce: bool = None,
-                 stable: bool = None,
-                 start_key: object = None,
-                 start_key_doc_id: str = None,
-                 update: str = None) -> None:
+    def __init__(
+        self,
+        *,
+        att_encoding_info: bool = None,
+        attachments: bool = None,
+        conflicts: bool = None,
+        descending: bool = None,
+        include_docs: bool = None,
+        inclusive_end: bool = None,
+        limit: int = None,
+        skip: int = None,
+        update_seq: bool = None,
+        end_key: object = None,
+        end_key_doc_id: str = None,
+        group: bool = None,
+        group_level: int = None,
+        key: object = None,
+        keys: List[object] = None,
+        reduce: bool = None,
+        stable: bool = None,
+        start_key: object = None,
+        start_key_doc_id: str = None,
+        update: str = None,
+    ) -> None:
         """
         Initialize a ViewQuery object.
 
         :param bool att_encoding_info: (optional) Parameter to specify whether to
                include the encoding information in attachment stubs if the particular
                attachment is compressed.
         :param bool attachments: (optional) Parameter to specify whether to include
@@ -17132,33 +17919,37 @@
         Parameter to specify whether or not the view in question should be updated prior
         to responding to the user.
         * `true` - Return results after the view is updated.
         * `false` - Return results without updating the view.
         * `lazy` - Return the view results without waiting for an update, but update them
         immediately after the request.
         """
+
         TRUE = 'true'
         FALSE = 'false'
         LAZY = 'lazy'
 
 
-class ViewResult():
+
+class ViewResult:
     """
     Schema for the result of a query view operation.
 
     :attr int total_rows: (optional) Number of total rows.
     :attr str update_seq: (optional) Current update sequence for the database.
     :attr List[ViewResultRow] rows: rows.
     """
 
-    def __init__(self,
-                 rows: List['ViewResultRow'],
-                 *,
-                 total_rows: int = None,
-                 update_seq: str = None) -> None:
+    def __init__(
+        self,
+        rows: List['ViewResultRow'],
+        *,
+        total_rows: int = None,
+        update_seq: str = None,
+    ) -> None:
         """
         Initialize a ViewResult object.
 
         :param List[ViewResultRow] rows: rows.
         :param int total_rows: (optional) Number of total rows.
         :param str update_seq: (optional) Current update sequence for the database.
         """
@@ -17216,36 +18007,39 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ViewResult') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
-class ViewResultRow():
+
+class ViewResultRow:
     """
     Schema for a row of a view result.
 
     :attr str caused_by: (optional) The cause of the error (if available).
     :attr str error: (optional) The name of the error.
     :attr str reason: (optional) The reason the error occurred (if available).
     :attr Document doc: (optional) Schema for a document.
     :attr str id: (optional) Schema for a document ID.
     :attr object key: Schema for any JSON type.
     :attr object value: Schema for any JSON type.
     """
 
-    def __init__(self,
-                 key: object,
-                 value: object,
-                 *,
-                 caused_by: str = None,
-                 error: str = None,
-                 reason: str = None,
-                 doc: 'Document' = None,
-                 id: str = None) -> None:
+    def __init__(
+        self,
+        key: object,
+        value: object,
+        *,
+        caused_by: str = None,
+        error: str = None,
+        reason: str = None,
+        doc: 'Document' = None,
+        id: str = None,
+    ) -> None:
         """
         Initialize a ViewResultRow object.
 
         :param object key: Schema for any JSON type.
         :param object value: Schema for any JSON type.
         :param str caused_by: (optional) The cause of the error (if available).
         :param str error: (optional) The name of the error.
```

### Comparing `ibmcloudant-0.4.0/ibmcloudant/common.py` & `ibmcloudant-0.4.1/ibmcloudant/common.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/ibmcloudant/couchdb_session_authenticator.py` & `ibmcloudant-0.4.1/ibmcloudant/couchdb_session_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/ibmcloudant/couchdb_session_get_authenticator_patch.py` & `ibmcloudant-0.4.1/ibmcloudant/couchdb_session_get_authenticator_patch.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/ibmcloudant/couchdb_session_token_manager.py` & `ibmcloudant-0.4.1/ibmcloudant/couchdb_session_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/ibmcloudant/version.py` & `ibmcloudant-0.4.1/ibmcloudant/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibmcloudant
 """
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

### Comparing `ibmcloudant-0.4.0/ibmcloudant.egg-info/PKG-INFO` & `ibmcloudant-0.4.1/ibmcloudant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloudant
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python client library for IBM Cloudant
 Home-page: https://github.com/IBM/cloudant-python-sdk
 Author: IBM
 Author-email: cldtsdks@us.ibm.com
 License: Apache 2.0
 Keywords: ibmcloudant
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.0
+# IBM Cloudant Python SDK Version 0.4.1
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -123,21 +123,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.0"
+pip install --upgrade "ibmcloudant>=0.4.1"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.0"
+easy_install --upgrade "ibmcloudant>=0.4.1"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
```

### Comparing `ibmcloudant-0.4.0/ibmcloudant.egg-info/SOURCES.txt` & `ibmcloudant-0.4.1/ibmcloudant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.0/setup.py` & `ibmcloudant-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 PACKAGE_NAME = 'ibmcloudant'
 PACKAGE_DESC = 'Python client library for IBM Cloudant'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

