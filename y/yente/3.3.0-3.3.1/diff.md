# Comparing `tmp/yente-3.3.0.tar.gz` & `tmp/yente-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.3.0.tar", last modified: Mon Mar 20 10:09:45 2023, max compression
+gzip compressed data, was "yente-3.3.1.tar", last modified: Tue Apr 25 13:00:19 2023, max compression
```

## Comparing `yente-3.3.0.tar` & `yente-3.3.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.216766 yente-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-20 10:07:55.000000 yente-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-20 10:07:55.000000 yente-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-20 10:09:45.216766 yente-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-20 10:07:55.000000 yente-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 10:09:45.216766 yente-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-20 10:07:55.000000 yente-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.212766 yente-3.3.0/yente/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 10:07:55.000000 yente-3.3.0/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-20 10:07:55.000000 yente-3.3.0/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-20 10:07:55.000000 yente-3.3.0/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.212766 yente-3.3.0/yente/data/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-20 10:07:55.000000 yente-3.3.0/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-03-20 10:07:55.000000 yente-3.3.0/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-20 10:07:55.000000 yente-3.3.0/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.212766 yente-3.3.0/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-20 10:07:55.000000 yente-3.3.0/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.212766 yente-3.3.0/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 10:07:55.000000 yente-3.3.0/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-20 10:07:55.000000 yente-3.3.0/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-03-20 10:07:55.000000 yente-3.3.0/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-03-20 10:07:55.000000 yente-3.3.0/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-20 10:07:55.000000 yente-3.3.0/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-20 10:07:55.000000 yente-3.3.0/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.216766 yente-3.3.0/yente/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-03-20 10:07:55.000000 yente-3.3.0/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-20 10:07:55.000000 yente-3.3.0/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-03-20 10:07:55.000000 yente-3.3.0/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-20 10:07:55.000000 yente-3.3.0/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 10:09:45.212766 yente-3.3.0/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 10:08:47.000000 yente-3.3.0/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 10:09:45.000000 yente-3.3.0/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.890479 yente-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 12:58:23.000000 yente-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 12:58:23.000000 yente-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 13:00:19.890479 yente-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-25 12:58:23.000000 yente-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:00:19.890479 yente-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-25 12:58:23.000000 yente-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.882479 yente-3.3.1/yente/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:23.000000 yente-3.3.1/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-25 12:58:23.000000 yente-3.3.1/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-25 12:58:23.000000 yente-3.3.1/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.886479 yente-3.3.1/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-25 12:58:23.000000 yente-3.3.1/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 12:58:23.000000 yente-3.3.1/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.886479 yente-3.3.1/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-25 12:58:23.000000 yente-3.3.1/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.890479 yente-3.3.1/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 12:58:23.000000 yente-3.3.1/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.890479 yente-3.3.1/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 12:58:23.000000 yente-3.3.1/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-25 12:58:23.000000 yente-3.3.1/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-25 12:58:23.000000 yente-3.3.1/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.886479 yente-3.3.1/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:58:36.000000 yente-3.3.1/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/top_level.txt
```

### Comparing `yente-3.3.0/LICENSE` & `yente-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/PKG-INFO` & `yente-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.3.0
+Version: 3.3.1
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.3.0/README.md` & `yente-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/setup.py` & `yente-3.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.3.0",
+    version="3.3.1",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
         "followthemoney==3.3.0",
-        "nomenklatura==2.8.1",
-        "asyncstdlib==3.10.5",
+        "nomenklatura==2.9.5",
+        "asyncstdlib==3.10.6",
         "aiocron==1.8",
-        "aiocsv==1.2.3",
+        "aiocsv==1.2.4",
         "aiofiles==23.1.0",
-        "types-aiofiles==23.1.0.0",
+        "types-aiofiles==23.1.0.1",
         "aiohttp[speedups]==3.8.4",
-        "elasticsearch[async]==8.6.2",
-        "fastapi==0.95.0",
+        "elasticsearch[async]==8.7.0",
+        "fastapi==0.95.1",
         "uvicorn[standard]==0.21.1",
         "python-multipart==0.0.6",
-        "email-validator==1.3.1",
-        "structlog==22.3.0",
-        "pyicu==2.10.2",
-        "orjson==3.8.7",
+        "email-validator==2.0.0.post2",
+        "structlog==23.1.0",
+        "pyicu==2.11",
+        "orjson==3.8.10",
         "text-unidecode==1.3",
         "click==8.0.4",
         "normality==2.4.0",
         "languagecodes==1.1.1",
         "countrynames==1.14.3",
         "fingerprints==1.1.0",
         "pantomime==0.6.0",
```

### Comparing `yente-3.3.0/yente/app.py` & `yente-3.3.1/yente/app.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/cli.py` & `yente-3.3.1/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/data/__init__.py` & `yente-3.3.1/yente/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/data/common.py` & `yente-3.3.1/yente/data/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     id: str = Field(..., example="NK-A7z....")
     caption: str = Field(..., example="John Doe")
     schema_: str = Field(..., example="LegalEntity", alias="schema")
     properties: EntityProperties = Field(..., example={"name": ["John Doe"]})
     datasets: List[str] = Field([], example=["us_ofac_sdn"])
     referents: List[str] = Field([], example=["ofac-1234"])
     target: bool = Field(False)
-    first_seen: datetime = Field(..., example=datetime.utcnow())
-    last_seen: datetime = Field(..., example=datetime.utcnow())
+    first_seen: Optional[datetime] = Field(..., example=datetime.utcnow())
+    last_seen: Optional[datetime] = Field(..., example=datetime.utcnow())
 
     @classmethod
     def from_entity(cls, entity: Entity) -> "EntityResponse":
         return cls.construct(
             id=entity.id,
             caption=entity.caption,
             schema=entity.schema.name,
@@ -96,14 +96,15 @@
 
 class SearchResponse(ResultsResponse):
     results: List[EntityResponse]
     facets: Dict[str, SearchFacet]
 
 
 class EntityExample(BaseModel):
+    id: Optional[str] = Field(None, example="my-entity-id")
     schema_: str = Field(..., example=settings.BASE_SCHEMA, alias="schema")
     properties: Dict[str, Union[str, List[str]]] = Field(
         ..., example={"name": ["John Doe"]}
     )
 
 
 class EntityMatchQuery(BaseModel):
```

### Comparing `yente-3.3.0/yente/data/dataset.py` & `yente-3.3.1/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/data/entity.py` & `yente-3.3.1/yente/data/entity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,39 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, TYPE_CHECKING
 from followthemoney import model
 from followthemoney.model import Model
 from followthemoney.types import registry
 from followthemoney.helpers import combine_names
 from nomenklatura.entity import CompositeEntity
 
-from yente import settings
 from yente.logs import get_logger
 
+if TYPE_CHECKING:
+    from yente.data.common import EntityExample
+
 log = get_logger(__name__)
 
 
 class Entity(CompositeEntity):
     """Entity for sanctions list entries and adjacent objects."""
 
     def __init__(self, model: Model, data: Dict[str, Any], cleaned: bool = True):
         super().__init__(model, data, cleaned=cleaned)
         self.target: bool = data.get("target", False)
 
-        # Not sure that impugning this is a good idea, to be seen:
-        first_seen: Optional[str] = data.get("first_seen")
-        last_seen: Optional[str] = data.get("last_seen")
-        self.first_seen: str = first_seen or last_seen or settings.RUN_TIME
-        self.last_seen: str = last_seen or self.first_seen
-
     def to_dict(self) -> Dict[str, Any]:
         data = super().to_dict()
-        data["first_seen"] = self.first_seen
-        data["last_seen"] = self.last_seen
         data["target"] = self.target
-        data["caption"] = self.caption
         return data
 
     @classmethod
-    def from_example(cls, schema: str, properties: Dict[str, Any]) -> "Entity":
-        data = {"id": "example", "schema": schema}
+    def from_example(cls, example: "EntityExample") -> "Entity":
+        data = {"id": example.id, "schema": example.schema_}
         obj = cls(model, data)
-        for prop_name, values in properties.items():
+        for prop_name, values in example.properties.items():
             if prop_name not in obj.schema.properties:
                 log.warning(
                     "Invalid example property",
                     prop=prop_name,
                     value=str(values),
                 )
                 continue
```

### Comparing `yente-3.3.0/yente/data/freebase.py` & `yente-3.3.1/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/data/loader.py` & `yente-3.3.1/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/data/manifest.py` & `yente-3.3.1/yente/data/manifest.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/data/util.py` & `yente-3.3.1/yente/data/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for date in dates:
         for prec in (Precision.DAY, Precision.MONTH, Precision.YEAR):
             if len(date) > prec.value:
                 expanded.add(date[: prec.value])
     return list(expanded)
 
 
-@lru_cache(maxsize=500)
+@lru_cache(maxsize=10000)
 def fingerprint_name(name: str) -> Optional[str]:
     return fingerprints.generate(name)
 
 
 def expand_names(names: List[str]) -> List[str]:
     """Expand names into normalized version."""
     expanded = set(names)
```

### Comparing `yente-3.3.0/yente/logs.py` & `yente-3.3.1/yente/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import logging
 import structlog
 from logging import Filter, LogRecord
-from typing import cast, Any, Dict, List
+from typing import Any, Dict, List
 from structlog.dev import ConsoleRenderer, set_exc_info
 from structlog.contextvars import merge_contextvars
 from structlog.processors import UnicodeDecoder, TimeStamper
 from structlog.processors import format_exc_info, add_log_level
 from structlog.processors import JSONRenderer
 from structlog.stdlib import ProcessorFormatter, add_logger_name
 from structlog.stdlib import BoundLogger, LoggerFactory
```

### Comparing `yente-3.3.0/yente/resources/favicon.ico` & `yente-3.3.1/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/routers/admin.py` & `yente-3.3.1/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/routers/reconcile.py` & `yente-3.3.1/yente/routers/reconcile.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fastapi import APIRouter, Query, Form
 from fastapi import Request, Response
 from fastapi import HTTPException
 from followthemoney import model
 from followthemoney.types import registry
 
 from yente import settings
-from yente.data.common import ErrorResponse
+from yente.data.common import ErrorResponse, EntityExample
 from yente.logs import get_logger
 from yente.data.entity import Entity
 from yente.data.dataset import Dataset
 from yente.data.freebase import (
     FreebaseEntity,
     FreebaseEntityResult,
     FreebaseManifestView,
@@ -146,25 +146,26 @@
 
 async def reconcile_query(
     name: str, dataset: Dataset, query: Dict[str, Any]
 ) -> Tuple[str, FreebaseEntityResult]:
     """Reconcile operation for a single query."""
     limit, offset = limit_window(query.get("limit"), 0, settings.MAX_MATCHES)
     schema = query.get("type", settings.BASE_SCHEMA)
-    properties = {"alias": [query.get("query")]}
+    properties: Dict[str, List[str]] = {"alias": [query.get("query", "")]}
 
     for p in query.get("properties", []):
         prop = model.get_qname(p.get("pid"))
         if prop is None:
             continue
         if prop.name not in properties:
             properties[prop.name] = []
         properties[prop.name].append(p.get("v"))
 
-    proxy = Entity.from_example(schema, properties)
+    example = EntityExample(id=None, schema=schema, properties=dict(properties))
+    proxy = Entity.from_example(example)
     query = entity_query(dataset, proxy)
     resp = await search_entities(query, limit=limit, offset=offset)
     entities = result_entities(resp)
     scoreds = [s for s in score_results(proxy, entities, limit=limit)]
     results = [FreebaseScoredEntity.from_scored(s) for s in scoreds]
     log.info(
         f"/reconcile/{dataset.name}",
```

### Comparing `yente-3.3.0/yente/routers/search.py` & `yente-3.3.1/yente/routers/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     queries = []
     entities = []
     responses: Dict[str, EntityMatches] = {}
 
     for name, example in match.queries.items():
         try:
-            entity = Entity.from_example(example.schema_, example.properties)
+            entity = Entity.from_example(example)
             query = entity_query(ds, entity)
         except Exception as exc:
             log.info("Cannot parse example entity: %s" % str(exc))
             raise HTTPException(
                 status_code=400,
                 detail=f"Cannot parse example entity: {exc}",
             )
```

### Comparing `yente-3.3.0/yente/routers/util.py` & `yente-3.3.1/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/scoring.py` & `yente-3.3.1/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/search/base.py` & `yente-3.3.1/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/search/indexer.py` & `yente-3.3.1/yente/search/indexer.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/search/mapping.py` & `yente-3.3.1/yente/search/mapping.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/search/nested.py` & `yente-3.3.1/yente/search/nested.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from fastapi import HTTPException
-from typing import Dict, List, Set, Tuple, Union
-from elasticsearch import ApiError, TransportError
+from typing import Dict, List, Set, Tuple, Union, Optional
+from elasticsearch import ApiError
 from followthemoney.property import Property
 from followthemoney.types import registry
 
 from yente import settings
 from yente.logs import get_logger
 from yente.data.entity import Entity
 from yente.data.common import EntityResponse
@@ -16,28 +16,29 @@
 
 Value = Union[str, EntityResponse]
 Entities = Dict[str, Entity]
 Inverted = Dict[str, Set[Tuple[Property, str]]]
 
 
 def nest_entity(
-    entity: Entity, entities: Entities, inverted: Inverted, path: Set[str]
+    entity: Entity, entities: Entities, inverted: Inverted, path: Set[Optional[str]]
 ) -> EntityResponse:
     props: Dict[str, List[Value]] = {}
     next_path = set([entity.id]).union(path)
 
     # Find other entities pointing to the one we're processing:
-    for (prop, adj_id) in inverted.get(entity.id, {}):
-        if adj_id in path or len(path) > 1:
-            continue
-        adj = entities.get(adj_id)
-        if adj is not None:
-            nested = nest_entity(adj, entities, inverted, next_path)
-            props.setdefault(prop.name, [])
-            props[prop.name].append(nested)
+    if entity.id is not None:
+        for (prop, adj_id) in inverted.get(entity.id, {}):
+            if adj_id in path or len(path) > 1:
+                continue
+            adj = entities.get(adj_id)
+            if adj is not None:
+                nested = nest_entity(adj, entities, inverted, next_path)
+                props.setdefault(prop.name, [])
+                props[prop.name].append(nested)
 
     # Expand nested entities:
     for prop in entity.iterprops():
         if prop.type != registry.entity:
             continue
         values: List[Value] = []
         for value in entity.get(prop):
@@ -54,15 +55,15 @@
             props.pop(prop.name)
     serialized = EntityResponse.from_entity(entity)
     serialized.properties.update(props)
     return serialized
 
 
 async def serialize_entity(root: Entity, nested: bool = False) -> EntityResponse:
-    if not nested:
+    if not nested or root.id is None:
         return EntityResponse.from_entity(root)
     inverted: Inverted = {}
     reverse = [root.id]
 
     entities: Entities = {root.id: root}
     next_entities = set(root.get_type_values(registry.entity))
 
@@ -100,14 +101,16 @@
                 query_json=json.dumps(query),
             )
             raise HTTPException(status_code=500, detail="Error retrieving entity")
 
         reverse = []
         next_entities.clear()
         for adj in result_entities(resp):
+            if adj.id is None:
+                continue
             entities[adj.id] = adj
 
             for prop, value in adj.itervalues():
                 if prop.type != registry.entity:
                     continue
                 if adj.schema.edge and value not in entities:
                     next_entities.add(value)
```

### Comparing `yente-3.3.0/yente/search/queries.py` & `yente-3.3.1/yente/search/queries.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/search/search.py` & `yente-3.3.1/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente/settings.py` & `yente-3.3.1/yente/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def env_str(name: str, default: Optional[str] = None) -> Optional[str]:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.3.0"
+VERSION = "3.3.1"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE") or "yente"
 DESCRIPTION = """
```

### Comparing `yente-3.3.0/yente/util.py` & `yente-3.3.1/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente.egg-info/PKG-INFO` & `yente-3.3.1/yente.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.3.0
+Version: 3.3.1
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.3.0/yente.egg-info/SOURCES.txt` & `yente-3.3.1/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.3.0/yente.egg-info/requires.txt` & `yente-3.3.1/yente.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 followthemoney==3.3.0
-nomenklatura==2.8.1
-asyncstdlib==3.10.5
+nomenklatura==2.9.5
+asyncstdlib==3.10.6
 aiocron==1.8
-aiocsv==1.2.3
+aiocsv==1.2.4
 aiofiles==23.1.0
-types-aiofiles==23.1.0.0
+types-aiofiles==23.1.0.1
 aiohttp[speedups]==3.8.4
-elasticsearch[async]==8.6.2
-fastapi==0.95.0
+elasticsearch[async]==8.7.0
+fastapi==0.95.1
 uvicorn[standard]==0.21.1
 python-multipart==0.0.6
-email-validator==1.3.1
-structlog==22.3.0
-pyicu==2.10.2
-orjson==3.8.7
+email-validator==2.0.0.post2
+structlog==23.1.0
+pyicu==2.11
+orjson==3.8.10
 text-unidecode==1.3
 click==8.0.4
 normality==2.4.0
 languagecodes==1.1.1
 countrynames==1.14.3
 fingerprints==1.1.0
 pantomime==0.6.0
```

