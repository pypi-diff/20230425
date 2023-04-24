# Comparing `tmp/numalogic_prometheus-0.3.0.tar.gz` & `tmp/numalogic_prometheus-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.3.0.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.3.1a0.tar", max compression
```

## Comparing `numalogic_prometheus-0.3.0.tar` & `numalogic_prometheus-0.3.1a0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/LICENSE
--rw-r--r--   0        0        0      847 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/__init__.py
--rw-r--r--   0        0        0      974 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/_config.py
--rw-r--r--   0        0        0      756 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0      950 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2145 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0     4447 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/factory.py
--rw-r--r--   0        0        0     8854 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      741 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/filter.py
--rw-r--r--   0        0        0     3628 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/inference.py
--rw-r--r--   0        0        0     6866 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     1889 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     3476 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4227 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     5514 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udsink/train.py
--rw-r--r--   0        0        0     7731 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5026 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/watcher.py
--rw-r--r--   0        0        0     1592 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 22:45:22.427111 numalogic_prometheus-0.3.1a0/LICENSE
+-rw-r--r--   0        0        0      847 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/__init__.py
+-rw-r--r--   0        0        0      974 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/_config.py
+-rw-r--r--   0        0        0      756 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1316 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     1367 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0     4447 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/factory.py
+-rw-r--r--   0        0        0     8854 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      741 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     3628 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     7014 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     1889 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     3476 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4321 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     5608 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     7795 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5026 2023-04-24 22:45:22.431111 numalogic_prometheus-0.3.1a0/numaprom/watcher.py
+-rw-r--r--   0        0        0     1542 2023-04-24 22:45:22.435111 numalogic_prometheus-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.1a0/PKG-INFO
```

### Comparing `numalogic_prometheus-0.3.0/LICENSE` & `numalogic_prometheus-0.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/__init__.py` & `numalogic_prometheus-0.3.1a0/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/_config.py` & `numalogic_prometheus-0.3.1a0/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/_constants.py` & `numalogic_prometheus-0.3.1a0/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.3.1a0/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/clients/redis.py` & `numalogic_prometheus-0.3.1a0/numaprom/clients/redis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import json
 from typing import Optional
 
 from redis.cluster import RedisCluster
+from redis.backoff import ExponentialBackoff
+from redis.exceptions import RedisClusterException, RedisError
+from redis.retry import Retry
 
 from numaprom import get_logger
 from numaprom.tools import is_host_reachable
 
 _LOGGER = get_logger(__name__)
 redis_client: Optional[RedisCluster] = None
 
@@ -21,15 +24,21 @@
     redis_params = {
         "host": host,
         "port": port,
         "password": password,
         "decode_responses": decode_responses,
         "skip_full_coverage_check": True,
         "dynamic_startup_nodes": False,
+        "cluster_error_retry_attempts": 3,
     }
     _LOGGER.info("Redis params: %s", json.dumps(redis_params, indent=4))
 
     if not is_host_reachable(host, port):
         _LOGGER.error("Redis Cluster is unreachable after retries!")
 
-    redis_client = RedisCluster(**redis_params)
+    retry = Retry(
+        ExponentialBackoff(cap=2, base=1),
+        3,
+        supported_errors=(ConnectionError, TimeoutError, RedisClusterException, RedisError),
+    )
+    redis_client = RedisCluster(**redis_params, retry=retry)
     return redis_client
```

### Comparing `numalogic_prometheus-0.3.0/numaprom/configs/config.yaml` & `numalogic_prometheus-0.3.1a0/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.3.1a0/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/entities.py` & `numalogic_prometheus-0.3.1a0/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/factory.py` & `numalogic_prometheus-0.3.1a0/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/tools.py` & `numalogic_prometheus-0.3.1a0/numaprom/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/udf/filter.py` & `numalogic_prometheus-0.3.1a0/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/udf/inference.py` & `numalogic_prometheus-0.3.1a0/numaprom/udf/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.3.1a0/numaprom/udf/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 import time
 import numpy as np
 from typing import List
 from orjson import orjson
 from redis.exceptions import RedisError, RedisClusterException
 
 from pynumaflow.function import Datum
+from redis.sentinel import MasterNotFoundError
 
 from numaprom import get_logger, UnifiedConf
 from numaprom.entities import Status, PrometheusPayload, StreamPayload, Header
-from numaprom.clients.redis import get_redis_client
+from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import (
     msgs_forward,
     WindowScorer,
 )
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
-PORT = os.getenv("REDIS_PORT")
+PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
+MASTERNAME = os.getenv("REDIS_MASTERNAME")
 
 
 def __save_to_redis(
     payload: StreamPayload, final_score: float, recreate: bool, unified_config: UnifiedConf
 ):
-    r = get_redis_client(HOST, PORT, password=AUTH, recreate=recreate)
+    r = get_redis_client(HOST, PORT, password=AUTH, mastername=MASTERNAME, recreate=recreate)
 
     metric_name = payload.composite_keys["name"]
 
     r_keys = payload.composite_keys
     r_keys.pop("name")
     r_key = f"{':'.join(r_keys.values())}:{payload.end_ts}"
 
@@ -140,15 +142,15 @@
         )
         return [publisher_json]
 
     try:
         unified_anomaly, anomalies = __save_to_redis(
             payload=payload, final_score=final_score, recreate=False, unified_config=unified_config
         )
-    except (RedisError, RedisClusterException) as warn:
+    except (RedisError, RedisClusterException, MasterNotFoundError) as warn:
         _LOGGER.warning(
             "%s - Redis connection failed, recreating the redis client; err: %r", payload.uuid, warn
         )
         unified_anomaly, anomalies = __save_to_redis(
             payload=payload, final_score=final_score, recreate=True, unified_config=unified_config
         )
```

### Comparing `numalogic_prometheus-0.3.0/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.3.1a0/numaprom/udf/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/udf/threshold.py` & `numalogic_prometheus-0.3.1a0/numaprom/udf/threshold.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/numaprom/udf/window.py` & `numalogic_prometheus-0.3.1a0/numaprom/udf/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 import numpy.typing as npt
 from orjson import orjson
 from pynumaflow.function import Datum
 from redis.exceptions import RedisError, RedisClusterException
 
 from numaprom import get_logger
 from numaprom.entities import StreamPayload, Status, Header
-from numaprom.clients.redis import get_redis_client
+from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import msg_forward, create_composite_keys
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
-PORT = os.getenv("REDIS_PORT")
+PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
+MASTERNAME = os.getenv("REDIS_MASTERNAME")
 
 
 # TODO get the replacement value from config
 def _clean_arr(
     id_: str,
     ckeys: dict,
     arr: npt.NDArray[float],
@@ -42,15 +43,17 @@
 ) -> list[tuple[float, float]]:
     """
     Adds an element to the sliding window using a redis sorted set.
 
     Returns an empty list if adding the element does not create a new entry
     to the set.
     """
-    redis_client = get_redis_client(HOST, PORT, password=AUTH, recreate=recreate)
+    redis_client = get_redis_client(
+        HOST, PORT, password=AUTH, mastername=MASTERNAME, recreate=recreate
+    )
     with redis_client.pipeline() as pl:
         pl.zadd(key, {f"{value}::{ts}": ts})
         pl.zremrangebyrank(key, -(buff_size + 10), -buff_size)
         pl.zrange(key, -win_size, -1, withscores=True, score_cast_func=int)
         out = pl.execute()
     _is_new, _, _window = out
     if not _is_new:
```

### Comparing `numalogic_prometheus-0.3.0/numaprom/udsink/train.py` & `numalogic_prometheus-0.3.1a0/numaprom/udsink/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 from numalogic.config import PreprocessFactory, ModelInfo, ThresholdFactory, ModelFactory
 from numalogic.models.autoencoder import AutoencoderTrainer
 from numalogic.tools.data import StreamingDataset
 from pynumaflow.sink import Datum, Responses, Response
 
 from numaprom import get_logger
 from numaprom.entities import TrainerPayload
-from numaprom.clients.redis import get_redis_client
+from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import save_model, fetch_data
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
-PORT = os.getenv("REDIS_PORT")
+PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
+MASTERNAME = os.getenv("REDIS_MASTERNAME")
 EXPIRY = int(os.getenv("REDIS_EXPIRY", 300))
 MIN_TRAIN_SIZE = int(os.getenv("MIN_TRAIN_SIZE", 2000))
 
 
 def clean_data(df: pd.DataFrame, limit=12) -> pd.DataFrame:
     df.replace([np.inf, -np.inf], np.nan, inplace=True)
     df = df.fillna(method="ffill", limit=limit)
@@ -72,15 +73,17 @@
     thresh_factory = ThresholdFactory()
     thresh_clf = thresh_factory.get_instance(thresh_cfg)
     thresh_clf.fit(x_reconerr)
     return thresh_clf
 
 
 def _is_new_request(payload: TrainerPayload) -> bool:
-    redis_client = get_redis_client(HOST, PORT, password=AUTH, recreate=False)
+    redis_client = get_redis_client(
+        HOST, PORT, password=AUTH, mastername=MASTERNAME, recreate=False
+    )
     _ckeys = ":".join([payload.composite_keys["namespace"], payload.composite_keys["name"]])
     r_key = f"train::{_ckeys}"
 
     value = redis_client.get(r_key)
     if value:
         return False
```

### Comparing `numalogic_prometheus-0.3.0/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.3.1a0/numaprom/udsink/train_rollout.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 from orjson import orjson
 from pynumaflow.sink import Datum, Responses, Response
 from sklearn.pipeline import make_pipeline
 from torch.utils.data import DataLoader
 
 from numaprom import get_logger
 from numaprom.entities import TrainerPayload
-from numaprom.clients.redis import get_redis_client
+from numaprom.clients.sentinel import get_redis_client
 from numaprom.tools import save_model, fetch_data
 from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
-PORT = os.getenv("REDIS_PORT")
+PORT = int(os.getenv("REDIS_PORT", 6379))
 AUTH = os.getenv("REDIS_AUTH")
+MASTERNAME = os.getenv("REDIS_MASTERNAME")
 EXPIRY = int(os.getenv("REDIS_EXPIRY", 360))
 MIN_TRAIN_SIZE = int(os.getenv("MIN_TRAIN_SIZE", 2000))
 
 
 # TODO: extract all good hashes, including when there are 2 hashes at a time
 # TODO avoid filling inf with nan, or at least throw warning
 def clean_data(df: pd.DataFrame, hash_col: str, limit=12) -> pd.DataFrame:
@@ -85,15 +86,15 @@
     thresh_factory = ThresholdFactory()
     thresh_clf = thresh_factory.get_instance(thresh_cfg)
     thresh_clf.fit(x_reconerr)
     return thresh_clf
 
 
 def _is_new_request(payload: TrainerPayload) -> bool:
-    redis_client = get_redis_client(HOST, PORT, password=AUTH, recreate=False)
+    redis_client = get_redis_client(HOST, PORT, password=AUTH, mastername=MASTERNAME)
     _ckeys = ":".join([payload.composite_keys["namespace"], payload.composite_keys["name"]])
     r_key = f"trainrollout::{_ckeys}"
     value = redis_client.get(r_key)
     if value:
         return False
 
     redis_client.setex(r_key, time=EXPIRY, value=1)
```

### Comparing `numalogic_prometheus-0.3.0/numaprom/watcher.py` & `numalogic_prometheus-0.3.1a0/numaprom/watcher.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.0/pyproject.toml` & `numalogic_prometheus-0.3.1a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.3.0"
+version = "0.3.1a0"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 repository = "https://github.com/numaproj/numalogic-prometheus"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.11"
+python = "~3.10"
 redis = "^4.3.1"
 pynumaflow = "~0.3"
 numalogic = {version = "~0.3.7", extras = ["mlflow"]}
 boto3 = "^1.25.2"
 orjson = "^3.8.4"
 omegaconf = "^2.3.0"
 watchdog = "^3.0.0"
```

### Comparing `numalogic_prometheus-0.3.0/PKG-INFO` & `numalogic_prometheus-0.3.1a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.3.0
+Version: 0.3.1a0
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: boto3 (>=1.25.2,<2.0.0)
 Requires-Dist: numalogic[mlflow] (>=0.3.7,<0.4.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: orjson (>=3.8.4,<4.0.0)
 Requires-Dist: pynumaflow (>=0.3,<0.4)
```

