# Comparing `tmp/featurizerai-1.4.5.tar.gz` & `tmp/featurizerai-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.5.tar", last modified: Sun Apr 23 14:46:38 2023, max compression
+gzip compressed data, was "featurizerai-1.4.6.tar", last modified: Mon Apr 24 22:22:42 2023, max compression
```

## Comparing `featurizerai-1.4.5.tar` & `featurizerai-1.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.832386 featurizerai-1.4.5/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.5/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.5/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 14:46:38.832450 featurizerai-1.4.5/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.5/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-23 14:46:38.832660 featurizerai-1.4.5/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-23 14:46:29.000000 featurizerai-1.4.5/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.829067 featurizerai-1.4.5/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.831570 featurizerai-1.4.5/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.5/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.5/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-23 11:29:31.000000 featurizerai-1.4.5/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.5/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4128 2023-04-23 14:39:35.000000 featurizerai-1.4.5/src/features/materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      222 2023-04-23 00:14:52.000000 featurizerai-1.4.5/src/features/test_authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1100 2023-04-23 11:25:26.000000 featurizerai-1.4.5/src/features/test_create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2627 2023-04-23 14:45:41.000000 featurizerai-1.4.5/src/features/test_materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-23 14:46:38.832275 featurizerai-1.4.5/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      496 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-23 14:46:38.000000 featurizerai-1.4.5/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-24 22:22:42.411090 featurizerai-1.4.6/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.6/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.6/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-24 22:22:42.411172 featurizerai-1.4.6/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.6/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-24 22:22:42.411439 featurizerai-1.4.6/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-24 22:21:57.000000 featurizerai-1.4.6/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-24 22:22:42.407620 featurizerai-1.4.6/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-24 22:22:42.410305 featurizerai-1.4.6/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.6/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.6/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-23 11:29:31.000000 featurizerai-1.4.6/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.6/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4523 2023-04-24 22:22:09.000000 featurizerai-1.4.6/src/features/materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1100 2023-04-24 11:20:05.000000 featurizerai-1.4.6/src/features/test_create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2280 2023-04-24 22:18:56.000000 featurizerai-1.4.6/src/features/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1349 2023-04-24 21:56:38.000000 featurizerai-1.4.6/src/features/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-24 22:22:42.410963 featurizerai-1.4.6/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-24 22:22:42.000000 featurizerai-1.4.6/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      492 2023-04-24 22:22:42.000000 featurizerai-1.4.6/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-24 22:22:42.000000 featurizerai-1.4.6/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-24 22:22:42.000000 featurizerai-1.4.6/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-24 22:22:42.000000 featurizerai-1.4.6/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.5/LICENSE` & `featurizerai-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.5/PKG-INFO` & `featurizerai-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.4.5/setup.py` & `featurizerai-1.4.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.5',
+    version='1.4.6',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.4.5/src/features/authenticate.py` & `featurizerai-1.4.6/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.5/src/features/create_stream.py` & `featurizerai-1.4.6/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.5/src/features/custom_schema.py` & `featurizerai-1.4.6/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.5/src/features/materialize.py` & `featurizerai-1.4.6/src/features/materialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
 from pyspark.sql import functions as F
 import certifi
 from pymongo.server_api import ServerApi
 
 
 class materialize:
-    def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql):
+    def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql, partition_column=None):
         self.mongo_connection = mongo_connection
         self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
         self.groupby = groupby_value
         self.groupby_attr = groupby_attr
         self.token = token
         self.schema = schema
         self.sparksql = sparksql
+        self.partition_column = partition_column
 
         self.spark = SparkSession.builder \
             .appName("IncrementalAggregation") \
             .master("local[*]") \
             .getOrCreate()
         self.spark.sparkContext.setLogLevel("ERROR")
 
@@ -56,14 +57,20 @@
         raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
         aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
 
         raw_data = raw_data_collection.find()
         raw_data_list = [doc for doc in raw_data]
         df = self.spark.createDataFrame(raw_data_list, self.schema)
 
+        # Apply partitioning if the partition_column is specified
+        if self.partition_column:
+            print("Partitioning the DataFrame based on the column: " + self.partition_column)
+            raw_data_collection.create_index(self.partition_column)
+            df = df.repartition(col(self.partition_column))
+
         # Filter the DataFrame based on the given device_id
         df = df.filter(col(self.groupby_attr) == self.groupby)
         start_time = self.aggregation_date
         df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
         df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
         df.createOrReplaceTempView("temp_table")
```

### Comparing `featurizerai-1.4.5/src/features/test_create_stream.py` & `featurizerai-1.4.6/src/features/test_create_stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         'collection': 'sparkaggregate'
     }
 
     # Create a new instance of the create_stream class
     featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5", "timestamp")
 
     # Start the Kafka consumer in a separate thread
-    jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiYnVyYWsiLCJleHAiOjE2ODIyNTE0MDB9.keOhdMFQhFwNp5VLHW4UrGHsRrglt7HIdOyJ7p9DdLg"
+    jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiYnVyYWsiLCJleHAiOjE2ODIzMzg3OTN9.VutSPOtM4aRgyEBwdoNh-89jdCfcfC9eDe1D8UU3tAs"
     featurizerai.start(jwt)
 
     # Run the consumer for 60 seconds
     time.sleep(60)
 
     # Stop the consumer and wait for the thread to finish
     featurizerai.stop()
```

### Comparing `featurizerai-1.4.5/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.6/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

