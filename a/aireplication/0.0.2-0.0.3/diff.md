# Comparing `tmp/aireplication-0.0.2.tar.gz` & `tmp/aireplication-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aireplication-0.0.2.tar", last modified: Sun Mar 26 16:01:31 2023, max compression
+gzip compressed data, was "aireplication-0.0.3.tar", last modified: Tue Apr 25 08:07:12 2023, max compression
```

## Comparing `aireplication-0.0.2.tar` & `aireplication-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 16:01:31.048204 aireplication-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-03-26 15:26:31.000000 aireplication-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      601 2023-03-26 16:01:31.048204 aireplication-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-03-26 15:26:31.000000 aireplication-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 16:01:31.027171 aireplication-0.0.2/aireplication/
--rw-rw-rw-   0        0        0       21 2023-03-26 16:01:28.000000 aireplication-0.0.2/aireplication/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:01:31.046703 aireplication-0.0.2/aireplication/ultils/
--rw-rw-rw-   0        0        0      236 2023-03-26 15:50:37.000000 aireplication-0.0.2/aireplication/ultils/__init__.py
--rw-rw-rw-   0        0        0    10843 2023-03-26 16:00:48.000000 aireplication-0.0.2/aireplication/ultils/data.py
--rw-rw-rw-   0        0        0     4867 2023-03-26 15:36:08.000000 aireplication-0.0.2/aireplication/ultils/datasets.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:01:31.042703 aireplication-0.0.2/aireplication.egg-info/
--rw-rw-rw-   0        0        0      601 2023-03-26 16:01:30.000000 aireplication-0.0.2/aireplication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-03-26 16:01:30.000000 aireplication-0.0.2/aireplication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 16:01:30.000000 aireplication-0.0.2/aireplication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-26 16:01:30.000000 aireplication-0.0.2/aireplication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-26 16:01:30.000000 aireplication-0.0.2/aireplication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-03-26 16:01:31.050250 aireplication-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1379 2023-03-26 15:50:49.000000 aireplication-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.423297 aireplication-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-25 07:54:43.000000 aireplication-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2728 2023-04-25 08:07:12.423390 aireplication-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2120 2023-04-25 08:03:15.000000 aireplication-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.393796 aireplication-0.0.3/aireplication/
+-rw-rw-rw-   0        0        0       21 2023-04-25 08:06:39.000000 aireplication-0.0.3/aireplication/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.421793 aireplication-0.0.3/aireplication/ultils/
+-rw-rw-rw-   0        0        0      236 2023-04-25 07:54:43.000000 aireplication-0.0.3/aireplication/ultils/__init__.py
+-rw-rw-rw-   0        0        0    13046 2023-04-25 07:59:53.000000 aireplication-0.0.3/aireplication/ultils/data.py
+-rw-rw-rw-   0        0        0     6724 2023-04-25 07:57:19.000000 aireplication-0.0.3/aireplication/ultils/datasets.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:07:12.416303 aireplication-0.0.3/aireplication.egg-info/
+-rw-rw-rw-   0        0        0     2728 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 08:07:12.000000 aireplication-0.0.3/aireplication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-25 08:07:12.424795 aireplication-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-04-25 07:54:43.000000 aireplication-0.0.3/setup.py
```

### Comparing `aireplication-0.0.2/LICENSE` & `aireplication-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aireplication-0.0.2/aireplication/ultils/data.py` & `aireplication-0.0.3/aireplication/ultils/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,15 +67,28 @@
         self.scaler_y = None
         self.raw_data = data
         self.input_width = config['input_width']
         self.output_length = config['output_length']
         self.shift = shift
         self.shuffle = shuffle
 
-        self.X_train, self.X_test = self.split_data(data, config['train_ratio'])
+        """
+        The procedure of data preparation:
+        1. Split data into TRAIN and TEST
+            [num_record, timeseries-past, feature, timeseries-label]
+                example [16752, X] -> [15076, X], [1676, X]
+        2. Building the Time series data type: 
+            [num_record, timeseries-past, feature, timeseries-label]
+                example (1093, 168, 1, 7)
+        3. Normalize data
+        4. Split train data into TRAIN and VALID
+        5. Normalize data
+        """
+
+        self.X_train, self.X_test = self.split_data(data, config['train_ratio'])  # [16752, X] -> [15076, X], [1676, X]
 
         # ASSUME TRAIN AND TEST DATASET HAVE THE SAME DISTRIBUTION
         self.scaler_engine = None  # This is for the normalization of the TRAIN dataset but apply to test and valid
         if normalize_type is not None:
             self.X_train, self.scaler_engine = self.normalize_dataset(self.X_train, standardization_type=normalize_type)
             if self.X_test is not None:
                 self.X_test, _ = self.normalize_dataset(self.X_test, standardization_type=normalize_type,
@@ -83,18 +96,23 @@
 
         # Split train and valid dataset for TRAINING PROCESS. The distribution of train and valid dataset is the same.
         self.X_train, self.X_valid = self.split_data(self.X_train, 0.9)
         if normalize_type is not None:
             self.X_valid, _ = self.normalize_dataset(self.X_valid, standardization_type=normalize_type,
                                                      scaler=self.scaler_engine)
 
-        self.data_train = self.build_tsd(self.X_train)  # (13568, 2) -> [(13399, 168, 2), (13399, 1, 2)]
-        self.data_valid = self.build_tsd(self.X_valid)  # (1508, 2) -> [(1339, 168, 2), (1339, 1, 2)]
+        # (13568, X) -> [(13399, 168, X), (13399, 1, prediction_step)]
+        self.data_train = self.build_tsd(self.X_train,
+                                         config["features"].index(config["prediction_feature"]))
+        # (1508, X) -> [(1339, 168, X), (1339, prediction_step)]
+        self.data_valid = self.build_tsd(self.X_valid,
+                                         config["features"].index(config["prediction_feature"]))
         if self.X_test is not None:
-            self.data_test = self.build_tsd(self.X_test)
+            self.data_test = self.build_tsd(self.X_test,
+                                            config["features"].index(config["prediction_feature"]))
         else:
             self.data_test = None
 
         # self.normalize_data()
 
     def normalize_dataset(self, dataset, standardization_type, scaler=None):
         """
@@ -147,16 +165,16 @@
             X_train, X_test = train_test_split(dataset, train_size=ratio, shuffle=self.shuffle)
         return X_train, X_test
 
     def inverse_scale_transform(self, y_predicted):
         """
         un-scale predicted output
         """
-        if self.scaler_y is not None:
-            return self.scaler_y.inverse_transform(y_predicted)
+        if self.scaler_engine is not None:
+            return self.scaler_engine.inverse_transform(y_predicted)
         return y_predicted
 
     def re_arrange_sequence(self, config):
         """Arranges the input sequence to support Model1 training"""
         self.data_train = (pattern(datapack=self.data_train[0],
                                    kernel_size=config['kernel_size'],
                                    gap=config['gap']),
@@ -210,15 +228,15 @@
         if self.data_test is not None:
             self.data_test = (
                 scaler_x.transform(self.data_test[0]),
                 scaler_y.transform(self.data_test[1]),
             )
             self.data_test = self.data_test[0][..., np.newaxis], self.data_test[1]
 
-    def build_tsd(self, data):
+    def build_tsd_test(self, data):
         """
         Build time series dataset ==> (VALUES_, LABELS_)
         This function is used to build the time series dataset for training dataset, validation dataset and testing dataset
         :param data: [Number of records, Number of features]
         :return: [Number of records, INPUT_WIDTH, INPUT_DIMENSION], [Number of records, OUTPUT_LENGTH, OUTPUT_DIMENSION]
         """
         X_data, y_label = [], []
@@ -231,16 +249,40 @@
             X_data.append(data[i - self.input_width: i])
             y_label.append(data[i: i + self.output_length])
 
         X_data, y_label = np.array(X_data), np.array(y_label)
 
         return X_data, y_label
 
+    def build_tsd(self, data, feature_order):
+        """
+        Build time series dataset ==> (VALUES_, LABELS_)
+        This function is used to build the time series dataset for training dataset, validation dataset and testing dataset
+        :param data: [Number of records, Number of features]
+        :return: [Number of records, INPUT_WIDTH, INPUT_DIMENSION], [Number of records, OUTPUT_LENGTH, OUTPUT_DIMENSION]
+
+        Args:
+            feature_order: Which feature will be predicted
+        """
+        X_data, y_label = [], []
+        if self.input_width >= len(data) - self.output_length - self.input_width:
+            raise ValueError(
+                f"Cannot devide sequence with length={len(data)}. The dataset is too small to be used input_length= {self.input_width}. Please reduce your input_length"
+            )
+
+        for i in range(self.input_width, len(data) - self.output_length):
+            X_data.append(data[i - self.input_width: i])
+            y_label.append(data[i: i + self.output_length][::, feature_order])
+
+        X_data, y_label = np.array(X_data), np.array(y_label)
+
+        return X_data, y_label
+
 
-from aireplication.ultils.datasets import *
+from utils.datasets import *
 
 
 def get_all_data_supported():
     return list(CONFIG_PATH.keys())
 
 
 class Dataset:
@@ -255,16 +297,25 @@
         if dataset_name not in get_all_data_supported():
             raise f"Dataset name {dataset_name} isn't supported"
         self.dataset_name = dataset_name
         # DataLoader
         self.dataloader = self.__load_data()
 
     def __load_data(self):
-        if self.dataset_name == cnu_str:
-            return CNU()
+        if self.dataset_name == cnu_str or \
+                self.dataset_name == cnu_str_engineering_7:
+            return CNU(data_name=self.dataset_name)
+
         elif self.dataset_name == comed_str:
             return COMED()
-        elif self.dataset_name == household_str:
-            return HouseholdDataLoader(
-                data_path=r'C:\Users\Andrew\Documents\Project\Time Series\dataset\Household_power_consumption\household_power_consumption.txt')
-        elif self.dataset_name == gyeonggi_str:
-            return GYEONGGI()
+
+        elif self.dataset_name == france_household_hour_str:
+            return FRANCEHOUSEHOLD()
+
+        elif self.dataset_name == gyeonggi_str or \
+                self.dataset_name == gyeonggi2955_str:
+            return GYEONGGI(data_name=self.dataset_name)
+
+        elif self.dataset_name == spain_str:
+            return SPAIN()
+
+        return None
```

### Comparing `aireplication-0.0.2/setup.py` & `aireplication-0.0.3/setup.py`

 * *Files identical despite different names*

