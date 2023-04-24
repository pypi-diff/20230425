# Comparing `tmp/conductor_py-0.0.1.tar.gz` & `tmp/conductor_py-0.0.2.tar.gz`

## Comparing `conductor_py-0.0.1.tar` & `conductor_py-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 conductor_py-0.0.1/operations.graphql
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 conductor_py-0.0.1/schema.graphql
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 conductor_py-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 conductor_py-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/async_base_client.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/base_model.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/client.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/create_integration_connection.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/enums.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/exceptions.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connection.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connections.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/input_types.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/ping_integration_connection.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/scalars.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/send_integration_request.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/netsuite/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/netsuite/invoice.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 conductor_py-0.0.1/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 conductor_py-0.0.1/LICENSE
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 conductor_py-0.0.1/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conductor_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 conductor_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 conductor_py-0.0.2/operations.graphql
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 conductor_py-0.0.2/schema.graphql
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 conductor_py-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 conductor_py-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/base_client.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/base_model.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/client.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/create_integration_connection.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/enums.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/get_integration_connection.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/get_integration_connections.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/input_types.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/ping_integration_connection.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/scalars.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/graphql_client/send_integration_request.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/netsuite/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 conductor_py-0.0.2/conductor_py/netsuite/invoice.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 conductor_py-0.0.2/tests/test_package.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 conductor_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 conductor_py-0.0.2/LICENSE
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 conductor_py-0.0.2/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 conductor_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 conductor_py-0.0.2/PKG-INFO
```

### Comparing `conductor_py-0.0.1/operations.graphql` & `conductor_py-0.0.2/operations.graphql`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.1/schema.graphql` & `conductor_py-0.0.2/schema.graphql`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.1/.github/workflows/python-publish.yml` & `conductor_py-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/__init__.py` & `conductor_py-0.0.2/conductor_py/graphql_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 
-from .async_base_client import AsyncBaseClient
+from .base_client import BaseClient
 from .base_model import BaseModel
 from .client import Client
 from .create_integration_connection import (
     CreateIntegrationConnection,
     CreateIntegrationConnectionCreateIntegrationConnection,
     CreateIntegrationConnectionCreateIntegrationConnectionIntegrationConnection,
 )
@@ -34,15 +34,15 @@
 )
 from .send_integration_request import (
     SendIntegrationRequest,
     SendIntegrationRequestSendIntegrationRequest,
 )
 
 __all__ = [
-    "AsyncBaseClient",
+    "BaseClient",
     "BaseModel",
     "Client",
     "CreateIntegrationConnection",
     "CreateIntegrationConnectionCreateIntegrationConnection",
     "CreateIntegrationConnectionCreateIntegrationConnectionIntegrationConnection",
     "CreateIntegrationConnectionInput",
     "GetIntegrationConnection",
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/async_base_client.py` & `conductor_py-0.0.2/conductor_py/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/base_model.py` & `conductor_py-0.0.2/conductor_py/graphql_client/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/client.py` & `conductor_py-0.0.2/conductor_py/graphql_client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./operations.graphql
 
-from .async_base_client import AsyncBaseClient
+from .base_client import BaseClient
 from .create_integration_connection import CreateIntegrationConnection
 from .get_integration_connection import GetIntegrationConnection
 from .get_integration_connections import GetIntegrationConnections
 from .input_types import (
     CreateIntegrationConnectionInput,
     PingIntegrationConnectionInput,
     SendIntegrationRequestInput,
@@ -14,16 +14,16 @@
 from .send_integration_request import SendIntegrationRequest
 
 
 def gql(q: str) -> str:
     return q
 
 
-class Client(AsyncBaseClient):
-    async def get_integration_connection(
+class Client(BaseClient):
+    def get_integration_connection(
         self, integration_connection_id: str
     ) -> GetIntegrationConnection:
         query = gql(
             """
             query getIntegrationConnection($integrationConnectionId: ID!) {
               integrationConnection(id: $integrationConnectionId) {
                 ...IntegrationConnection
@@ -39,19 +39,19 @@
               lastHeartbeatAt
             }
             """
         )
         variables: dict[str, object] = {
             "integrationConnectionId": integration_connection_id
         }
-        response = await self.execute(query=query, variables=variables)
+        response = self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetIntegrationConnection.parse_obj(data)
 
-    async def get_integration_connections(self) -> GetIntegrationConnections:
+    def get_integration_connections(self) -> GetIntegrationConnections:
         query = gql(
             """
             query getIntegrationConnections {
               integrationConnections {
                 ...IntegrationConnection
               }
             }
@@ -63,19 +63,19 @@
               endUserEmail
               endUserCompanyName
               lastHeartbeatAt
             }
             """
         )
         variables: dict[str, object] = {}
-        response = await self.execute(query=query, variables=variables)
+        response = self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetIntegrationConnections.parse_obj(data)
 
-    async def create_integration_connection(
+    def create_integration_connection(
         self, input: CreateIntegrationConnectionInput
     ) -> CreateIntegrationConnection:
         query = gql(
             """
             mutation createIntegrationConnection($input: CreateIntegrationConnectionInput!) {
               createIntegrationConnection(input: $input) {
                 integrationConnection {
@@ -91,44 +91,44 @@
               endUserEmail
               endUserCompanyName
               lastHeartbeatAt
             }
             """
         )
         variables: dict[str, object] = {"input": input}
-        response = await self.execute(query=query, variables=variables)
+        response = self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateIntegrationConnection.parse_obj(data)
 
-    async def ping_integration_connection(
+    def ping_integration_connection(
         self, input: PingIntegrationConnectionInput
     ) -> PingIntegrationConnection:
         query = gql(
             """
             mutation pingIntegrationConnection($input: PingIntegrationConnectionInput!) {
               pingIntegrationConnection(input: $input) {
                 duration
               }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
-        response = await self.execute(query=query, variables=variables)
+        response = self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return PingIntegrationConnection.parse_obj(data)
 
-    async def send_integration_request(
+    def send_integration_request(
         self, input: SendIntegrationRequestInput
     ) -> SendIntegrationRequest:
         query = gql(
             """
             mutation sendIntegrationRequest($input: SendIntegrationRequestInput!) {
               sendIntegrationRequest(input: $input) {
                 response
               }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
-        response = await self.execute(query=query, variables=variables)
+        response = self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return SendIntegrationRequest.parse_obj(data)
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/create_integration_connection.py` & `conductor_py-0.0.2/conductor_py/graphql_client/create_integration_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/exceptions.py` & `conductor_py-0.0.2/conductor_py/graphql_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 
 from typing import Any, Dict, List, Optional
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connection.py` & `conductor_py-0.0.2/conductor_py/graphql_client/get_integration_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connections.py` & `conductor_py-0.0.2/conductor_py/graphql_client/get_integration_connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./operations.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/input_types.py` & `conductor_py-0.0.2/conductor_py/graphql_client/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./schema.graphql
 
 from typing import Any
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/ping_integration_connection.py` & `conductor_py-0.0.2/conductor_py/graphql_client/ping_integration_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `conductor_py-0.0.1/conductor_py/graphql_client/send_integration_request.py` & `conductor_py-0.0.2/conductor_py/graphql_client/send_integration_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-04-24 11:14
+# Generated by ariadne-codegen on 2023-04-24 15:32
 # Source: ./operations.graphql
 
 from typing import Any
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `conductor_py-0.0.1/.gitignore` & `conductor_py-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.1/LICENSE` & `conductor_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.1/PKG-INFO` & `conductor_py-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conductor-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python bindings for the Conductor API
 Author-email: Danny Nemer <hi@dannynemer.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -18,13 +18,13 @@
 pip install --upgrade conductor-py
 ```
 
 ## Usage
 
 ```py
 import conductor_py as conductor
-conductor.api_key = "sk_test_..."
+conductor.set_api_key("sk_test_...")
 
 # Fetch all invoices for the specified NetSuite account, which previously
 # connected to our Conductor account.
 invoices = conductor.netsuite.invoice.findMany(connection_id="conn_123...")
 ```
```

