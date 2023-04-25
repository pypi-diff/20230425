# Comparing `tmp/armada_airflow-0.2.7-py3-none-any.whl.zip` & `tmp/armada_airflow-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 14396 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 21:52 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 21:54 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2728 b- defN 23-Mar-08 21:54 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Mar-08 21:54 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 21:52 armada/operators/__init__.py
--rw-r--r--  2.0 unx     5907 b- defN 23-Mar-08 21:52 armada/operators/armada.py
--rw-r--r--  2.0 unx     1713 b- defN 23-Mar-08 21:52 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     5622 b- defN 23-Mar-08 21:52 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-08 21:57 armada_airflow-0.2.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     3710 b- defN 23-Mar-08 21:57 armada_airflow-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-08 21:57 armada_airflow-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-08 21:57 armada_airflow-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1099 b- defN 23-Mar-08 21:57 armada_airflow-0.2.7.dist-info/RECORD
-13 files, 36357 bytes uncompressed, 12536 bytes compressed:  65.5%
+Zip file size: 18490 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 00:07 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 00:10 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-Apr-25 00:10 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Apr-25 00:10 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 00:07 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     4579 b- defN 23-Apr-25 00:07 armada/operators/armada.py
+-rw-r--r--  2.0 unx    11285 b- defN 23-Apr-25 00:07 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     1384 b- defN 23-Apr-25 00:07 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     1542 b- defN 23-Apr-25 00:07 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx     9976 b- defN 23-Apr-25 00:07 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3769 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1289 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/RECORD
+15 files, 52130 bytes uncompressed, 16328 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -12,29 +12,35 @@
 
 Filename: armada/operators/__init__.py
 Comment: 
 
 Filename: armada/operators/armada.py
 Comment: 
 
+Filename: armada/operators/armada_deferrable.py
+Comment: 
+
 Filename: armada/operators/jobservice.py
 Comment: 
 
+Filename: armada/operators/jobservice_asyncio.py
+Comment: 
+
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.2.7.dist-info/LICENSE
+Filename: armada_airflow-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.2.7.dist-info/METADATA
+Filename: armada_airflow-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.2.7.dist-info/WHEEL
+Filename: armada_airflow-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.2.7.dist-info/top_level.txt
+Filename: armada_airflow-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.2.7.dist-info/RECORD
+Filename: armada_airflow-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/armada.py

```diff
@@ -13,32 +13,32 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import logging
-import os
-from typing import List, Optional
+from typing import Optional
 
 from airflow.models import BaseOperator
 from airflow.exceptions import AirflowException
 
 from armada_client.client import ArmadaClient
-from armada_client.armada import submit_pb2
 from armada.operators.jobservice import JobServiceClient
 
-from armada.operators.utils import airflow_error, search_for_job_complete
+from armada.operators.utils import (
+    airflow_error,
+    search_for_job_complete,
+    annotate_job_request_items,
+)
 from armada.jobservice import jobservice_pb2
 
 
 armada_logger = logging.getLogger("airflow.task")
 
-ANNOTATION_KEY_PREFIX = "armadaproject.io/"
-
 
 class ArmadaOperator(BaseOperator):
     """
     Implementation of an ArmadaOperator for airflow.
 
     Airflow operators inherit from BaseOperator.
 
@@ -50,15 +50,15 @@
     :param job_request_items: A PodSpec that is used by Armada for submitting a job
     :param lookout_url_template: A URL template to be used to provide users
         a valid link to the related lookout job in this operator's log.
         The format should be:
         "https://lookout.armada.domain/jobs?job_id=<job_id>" where <job_id> will
         be replaced with the actual job ID.
 
-    :return: a job service client instance
+    :return: an armada operator instance
     """
 
     def __init__(
         self,
         name: str,
         armada_client: ArmadaClient,
         job_service_client: JobServiceClient,
@@ -123,47 +123,7 @@
         )
         airflow_error(job_state, self.name, job_id)
 
     def _get_lookout_url(self, job_id: str) -> str:
         if self.lookout_url_template is None:
             return ""
         return self.lookout_url_template.replace("<job_id>", job_id)
-
-
-def annotate_job_request_items(
-    context, job_request_items: List[submit_pb2.JobSubmitRequestItem]
-) -> List[submit_pb2.JobSubmitRequestItem]:
-    """
-    Annotates the inbound job request items with Airflow context elements
-
-    :param context: The airflow context.
-
-    :param job_request_items: The job request items to be sent to armada
-
-    :return: annotated job request items for armada
-    """
-    task_instance = context["ti"]
-    task_id = task_instance.task_id
-    run_id = context["run_id"]
-    dag_id = context["dag"].dag_id
-
-    for item in job_request_items:
-        item.annotations[get_annotation_key_prefix() + "taskId"] = task_id
-        item.annotations[get_annotation_key_prefix() + "taskRunId"] = run_id
-        item.annotations[get_annotation_key_prefix() + "dagId"] = dag_id
-
-    return job_request_items
-
-
-def get_annotation_key_prefix() -> str:
-    """
-    Provides the annotation key perfix,
-    which can be specified in env var ANNOTATION_KEY_PREFIX.
-    A default is provided if the env var is not defined
-
-    :return: string annotation key prefix
-    """
-    env_var_name = "ANNOTATION_KEY_PREFIX"
-    if env_var_name in os.environ:
-        return f"{os.environ.get(env_var_name)}"
-    else:
-        return ANNOTATION_KEY_PREFIX
```

## armada/operators/jobservice.py

```diff
@@ -1,32 +1,25 @@
-from concurrent.futures import ThreadPoolExecutor
-import os
-from typing import Optional
 from armada.jobservice import jobservice_pb2_grpc, jobservice_pb2
 
 from google.protobuf import empty_pb2
 
 
 class JobServiceClient:
     """
     The JobService Client
 
     Implementation of gRPC stubs from JobService
 
     :param channel: gRPC channel used for authentication. See
                     https://grpc.github.io/grpc/python/grpc.html
                     for more information.
-    :param max_workers: number of cores for thread pools, if unset, defaults
-                        to number of CPUs
     :return: a job service client instance
     """
 
-    def __init__(self, channel, max_workers: Optional[int] = None):
-        self.executor = ThreadPoolExecutor(max_workers=max_workers or os.cpu_count())
-
+    def __init__(self, channel):
         self.job_stub = jobservice_pb2_grpc.JobServiceStub(channel)
 
     def get_job_status(
         self, queue: str, job_set_id: str, job_id: str
     ) -> jobservice_pb2.JobServiceResponse:
         """Get job status of a given job in a queue and job_set_id.
```

## armada/operators/utils.py

```diff
@@ -1,17 +1,20 @@
+import asyncio
 import logging
 import os
 import time
 
 from airflow.exceptions import AirflowFailException
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 from enum import Enum
 
 from armada.operators.jobservice import JobServiceClient
+from armada.operators.jobservice_asyncio import JobServiceAsyncIOClient
 from armada.jobservice import jobservice_pb2
+from armada_client.armada import submit_pb2
 
 
 class JobState(Enum):
     SUBMITTED = 0
     DUPLICATE_FOUND = 1
     RUNNING = 2
     FAILED = 3
@@ -147,14 +150,134 @@
             continue
 
         if job_state == JobState.JOB_ID_NOT_FOUND:
             end_time = time.time()
             time_elasped = int(end_time) - int(start_time)
             if time_elasped > time_out_for_failure:
                 job_state = JobState.JOB_ID_NOT_FOUND
+                job_message = (
+                    f"Armada {airflow_task_name}:{job_id} could not find a job id and\n"
+                    f"hit a timeout"
+                )
+                break
+
+    return job_state, job_message
+
+
+def annotate_job_request_items(
+    context, job_request_items: List[submit_pb2.JobSubmitRequestItem]
+) -> List[submit_pb2.JobSubmitRequestItem]:
+    """
+    Annotates the inbound job request items with Airflow context elements
+
+    :param context: The airflow context.
+
+    :param job_request_items: The job request items to be sent to armada
+
+    :return: annotated job request items for armada
+    """
+    task_instance = context["ti"]
+    task_id = task_instance.task_id
+    run_id = context["run_id"]
+    dag_id = context["dag"].dag_id
+
+    for item in job_request_items:
+        item.annotations[get_annotation_key_prefix() + "taskId"] = task_id
+        item.annotations[get_annotation_key_prefix() + "taskRunId"] = run_id
+        item.annotations[get_annotation_key_prefix() + "dagId"] = dag_id
+
+    return job_request_items
+
+
+ANNOTATION_KEY_PREFIX = "armadaproject.io/"
+
+
+def get_annotation_key_prefix() -> str:
+    """
+    Provides the annotation key prefix,
+    which can be specified in env var ANNOTATION_KEY_PREFIX.
+    A default is provided if the env var is not defined
+
+    :return: string annotation key prefix
+    """
+    env_var_name = "ANNOTATION_KEY_PREFIX"
+    if env_var_name in os.environ:
+        return f"{os.environ.get(env_var_name)}"
+    else:
+        return ANNOTATION_KEY_PREFIX
+
+
+async def search_for_job_complete_async(
+    armada_queue: str,
+    job_set_id: str,
+    airflow_task_name: str,
+    job_id: str,
+    job_service_client: JobServiceAsyncIOClient,
+    log,
+    time_out_for_failure: int = 7200,
+) -> Tuple[JobState, str]:
+    """
+
+    Poll JobService cache asyncronously until you get a terminated event.
+
+    A terminated event is SUCCEEDED, FAILED or CANCELLED
+
+    :param armada_queue: The queue for armada
+    :param job_set_id: Your job_set_id
+    :param airflow_task_name: The name of your armada job
+    :param job_id: The name of the job id that armada assigns to it
+    :param job_service_client: A JobServiceClient that is used for polling.
+                                It is optional only for testing
+    :param time_out_for_failure: The amount of time a job
+                                    can be in job_id_not_found
+                                    before we decide it was a invalid job
+    :return: A tuple of JobStateEnum, message
+    """
+    start_time = time.time()
+    # Overwrite time_out_for_failure by environment variable for configuration
+    armada_time_out_env = os.getenv("ARMADA_AIRFLOW_TIME_OUT_JOB_ID")
+    if armada_time_out_env:
+        time_out_for_failure = int(armada_time_out_env)
+    while True:
+        job_status_return = await job_service_client.get_job_status(
+            queue=armada_queue,
+            job_id=job_id,
+            job_set_id=job_set_id,
+        )
+
+        job_state = job_state_from_pb(job_status_return.state)
+        log.debug(f"Got job state '{job_state.name}' for job {job_id}")
+
+        await asyncio.sleep(3)
+
+        if job_state == JobState.SUCCEEDED:
+            job_message = f"Armada {airflow_task_name}:{job_id} succeeded"
+            break
+        if job_state == JobState.FAILED:
+            job_message = (
+                f"Armada {airflow_task_name}:{job_id} failed\n"
+                f"failed with reason {job_status_return.error}"
+            )
+            break
+        if job_state == JobState.CANCELLED:
+            job_message = f"Armada {airflow_task_name}:{job_id} cancelled"
+            break
+        if job_state == JobState.CONNECTION_ERR:
+            log_messages = (
+                f"Armada {airflow_task_name}:{job_id} connection error (will retry)"
+                f"failed with reason {job_status_return.error}"
+            )
+            log.warning(log_messages)
+            continue
+
+        if job_state == JobState.JOB_ID_NOT_FOUND:
+            end_time = time.time()
+            time_elasped = int(end_time) - int(start_time)
+            if time_elasped > time_out_for_failure:
+                job_state = JobState.JOB_ID_NOT_FOUND
                 job_message = (
                     f"Armada {airflow_task_name}:{job_id} could not find a job id and\n"
                     f"hit a timeout"
                 )
                 break
 
     return job_state, job_message
```

## Comparing `armada_airflow-0.2.7.dist-info/LICENSE` & `armada_airflow-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.2.7.dist-info/METADATA` & `armada_airflow-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.2.7
+Version: 0.3.0
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
@@ -12,20 +12,21 @@
 Requires-Dist: grpcio (>=1.46.3)
 Requires-Dist: grpcio-tools (>=1.46.3)
 Requires-Dist: types-protobuf (>=3.19.22)
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinx-jekyll-builder ; extra == 'docs'
 Provides-Extra: format
-Requires-Dist: black (==23.1.0) ; extra == 'format'
+Requires-Dist: black (==23.3.0) ; extra == 'format'
 Requires-Dist: flake8 (==6.0.0) ; extra == 'format'
-Requires-Dist: pylint (==2.16.1) ; extra == 'format'
+Requires-Dist: pylint (==2.17.2) ; extra == 'format'
 Provides-Extra: test
-Requires-Dist: pytest (==7.2.1) ; extra == 'test'
+Requires-Dist: pytest (==7.2.2) ; extra == 'test'
 Requires-Dist: coverage (>=6.5.0) ; extra == 'test'
+Requires-Dist: pytest-asyncio (==0.21.0) ; extra == 'test'
 
 # armada-airflow-operator
 
 An Airflow operator for interfacing with the armada client
 
 ## Background
```

## Comparing `armada_airflow-0.2.7.dist-info/RECORD` & `armada_airflow-0.3.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=qqr5DOfjMVk0nImQPBPoN9tSBVz9oRt2o90VNAxWARI,2728
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-armada/operators/armada.py,sha256=BKC6AoeY1sPcFUpro1eWyvf2tIxp0xNzLB6Rlb9JxdI,5907
-armada/operators/jobservice.py,sha256=Yn4Fp7Xabp1Vm5ApHGa4liUMxNCjASysy0jL7UdWeT4,1713
-armada/operators/utils.py,sha256=8C-k9T4Joe4v9stk-0llEhLZ62S0ePNeEbtOFaJBi9w,5622
-armada_airflow-0.2.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.2.7.dist-info/METADATA,sha256=y7dOMRi_avxNpoHNJby8y8vuwRlGi3WXX6tfz55nQE8,3710
-armada_airflow-0.2.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-armada_airflow-0.2.7.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.2.7.dist-info/RECORD,,
+armada/operators/armada.py,sha256=7scMwIWLDUFaIZEJ6FHkHgul-YnMUSuIaPOBRW0f5IE,4579
+armada/operators/armada_deferrable.py,sha256=TmqP0-Rau7q5C6AgCEtRpWzIBfMkN8iwyWYHfercA9E,11285
+armada/operators/jobservice.py,sha256=3K7aIsu-VU42gwLHPMYLqItV4CEJ6ovwn46hSXQGRgU,1384
+armada/operators/jobservice_asyncio.py,sha256=9dJwTuV0OslVavBJVcf1tzb7uU3tuimou8o35lLEdn0,1542
+armada/operators/utils.py,sha256=WuboRUqCHw-SAaA6NegiudvcC7zGyOXkiY0aa7E4eWQ,9976
+armada_airflow-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.3.0.dist-info/METADATA,sha256=7A6W_hqA1zh8ZNDSaNUPQReCd6DZUCqYeSBwV9KBip8,3769
+armada_airflow-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+armada_airflow-0.3.0.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.3.0.dist-info/RECORD,,
```

