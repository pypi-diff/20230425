# Comparing `tmp/ml_wrappers-0.4.7.tar.gz` & `tmp/ml_wrappers-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml_wrappers-0.4.7.tar", last modified: Fri Apr 14 19:12:19 2023, max compression
+gzip compressed data, was "dist/ml_wrappers-0.4.8.tar", last modified: Mon Apr 24 21:47:52 2023, max compression
```

## Comparing `ml_wrappers-0.4.7.tar` & `ml_wrappers-0.4.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/gpu_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/warnings_suppressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28409 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/timestamp_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/model/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/base_wrapped_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/endpoint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/fastai_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24120 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/image_model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/predictions_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/pytorch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/tensorflow_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/text_model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_without_proba_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/wrapped_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/gpu_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/common/warnings_suppressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28409 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/dataset/timestamp_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/base_wrapped_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/endpoint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/fastai_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29204 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/image_model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/predictions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/pytorch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/tensorflow_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/text_model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_without_proba_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/model/wrapped_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/ml_wrappers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/ml_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 21:47:52.000000 ml_wrappers-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-24 21:44:19.000000 ml_wrappers-0.4.8/setup.py
```

### Comparing `ml_wrappers-0.4.7/LICENSE.txt` & `ml_wrappers-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/PKG-INFO` & `ml_wrappers-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_wrappers
-Version: 0.4.7
+Version: 0.4.8
 Summary: Machine Learning Wrappers SDK for Python
 Home-page: https://github.com/microsoft/ml-wrappers
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_wrappers-0.4.7/README.md` & `ml_wrappers-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/__init__.py` & `ml_wrappers-0.4.8/ml_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/common/constants.py` & `ml_wrappers-0.4.8/ml_wrappers/common/constants.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/common/gpu_kmeans.py` & `ml_wrappers-0.4.8/ml_wrappers/common/gpu_kmeans.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/common/warnings_suppressor.py` & `ml_wrappers-0.4.8/ml_wrappers/common/warnings_suppressor.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_utils.py` & `ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/dataset/timestamp_featurizer.py` & `ml_wrappers-0.4.8/ml_wrappers/dataset/timestamp_featurizer.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/__init__.py` & `ml_wrappers-0.4.8/ml_wrappers/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/base_wrapped_model.py` & `ml_wrappers-0.4.8/ml_wrappers/model/base_wrapped_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/endpoint_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/endpoint_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/evaluator.py` & `ml_wrappers-0.4.8/ml_wrappers/model/evaluator.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/fastai_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/fastai_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/function_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/image_model_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/image_model_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -177,14 +177,51 @@
 
     return {
         "boxes": Tensor(boxes),
         "labels": Tensor(labels),
         "scores": Tensor(scores)}
 
 
+def expand_class_scores(
+        scores: Tensor,
+        labels: Tensor,
+        number_of_classes: int,
+) -> Tensor:
+    """Extrapolate a full set of class scores.
+
+    Many object detection models don't return a full set of class scores, but
+    rather just a score for the predicted class. This is a helper function
+    that approximates a full set of class scores by dividing the difference
+    between 1.0 and the predicted class score among the remaning classes.
+
+    :param scores: Set of class specific scores. Shape [D] where D is number
+        of detections
+    :type scores: torch.Tensor
+    :param labels: Set of label indices corresponding to predicted class.
+        Shape [D] where D is number of detections
+    :type labels: torch.Tensor (ints)
+    :param number_of_classes: Number of classes model predicts
+    :type number_of_classes: int
+    :return: A set of expanded scores, of shape [D, C], where C is number of
+        classes
+    :type: torch.Tensor
+    """
+    number_of_detections = scores.shape[0]
+
+    expanded_scores = torch.ones(number_of_detections, number_of_classes + 1)
+
+    for i, (score, label) in enumerate(zip(scores, labels)):
+
+        residual = (1. - score.item()) / (number_of_classes)
+        expanded_scores[i, :] *= residual
+        expanded_scores[i, int(label.item())] = score
+
+    return expanded_scores
+
+
 def _wrap_image_model(model, examples, model_task, is_function,
                       number_of_classes: int = None,
                       classes: Union[list, np.array] = None):
     """If needed, wraps the model or function in a common API.
 
     Wraps the model based on model task and prediction function contract.
 
@@ -630,22 +667,118 @@
 
             # Note that FasterRCNN doesn't return a score for each class, only
             # the predicted class. DRISE requires a score for each class.
             # We approximate the score for each class
             # by dividing (class score) evenly among the other classes.
 
             raw_detection = _filter_score(raw_detection, 0.5)
-            expanded_class_scores = od_common.expand_class_scores(
+            expanded_class_scores = expand_class_scores(
                 raw_detection[SCORES],
                 raw_detection[LABELS],
                 self._number_of_classes)
 
             detections.append(
                 od_common.DetectionRecord(
                     bounding_boxes=raw_detection[BOXES],
                     class_scores=expanded_class_scores,
                     objectness_scores=torch.tensor(
                         [1.0]*raw_detection[BOXES].shape[0]),
                 )
             )
 
         return detections
+
+
+class MLflowDRiseWrapper():
+    """Wraps a Mlflow model with a predict API function.
+
+    To be compatible with the D-RISE explainability method,
+    all models must be wrapped to have the same output and input class and a
+    predict function for object detection. This wrapper is customized for the
+    FasterRCNN model from AutoML. Unlike the Pytorch wrapper, this wrapper
+    does not inherit from GeneralObjectDetectionModelWrapper as this super
+    class requires predict to take a tensor input.
+    """
+
+    def __init__(self, model: PyFuncModel,
+                 classes: Union[list, np.ndarray]) -> None:
+        """Initialize the MLflowDRiseWrapper.
+
+        :param model: mlflow model
+        :type model: mlflow.pyfunc.PyFuncModel
+        :param number_of_classes: Number of classes the model is predicting
+        :type number_of_classes: int
+        """
+
+        self._model = model
+        self._classes = classes
+        self._number_of_classes = len(classes)
+        self._label_dict = {label: (i+1) for i, label in enumerate(classes)}
+
+    def _mlflow_predict(self, dataset: pd.DataFrame) -> pd.DataFrame:
+        """Perform the inference using the wrapped MLflow model.
+
+        :param dataset: The dataset to predict on.
+        :type dataset: pandas.DataFrame
+        :return: The predicted data.
+        :rtype: pandas.DataFrame
+        """
+        predictions = self._model.predict(dataset)
+        return predictions
+
+    def predict(self, dataset: pd.DataFrame, iou_thresh: float = 0.25,
+                score_thresh: float = 0.5):
+        """Predict the output value using the wrapped MLflow model.
+
+        :param dataset: The dataset to predict on.
+        :type dataset: pandas.DataFrame
+        :return: The predicted values.
+        :rtype: numpy.ndarray
+        """
+        image_sizes = dataset['image_size']
+
+        dataset = dataset.drop(['image_size'], axis=1)
+
+        predictions = self._mlflow_predict(dataset)
+        if not len(predictions['boxes']) == len(image_sizes):
+            raise ValueError("Internal Error: Number of predictions " +
+                             "does not match number of images")
+
+        if not len(predictions['boxes']) == 1:
+            raise ValueError(
+                "Currently, only 1 image can be passed to predict")
+
+        detections = []
+        for image_detections, img_size in \
+                zip(predictions['boxes'], image_sizes):
+
+            raw_detections = _process_automl_detections_to_raw_detections(
+                image_detections, self._label_dict, img_size)
+
+            # TODO: check if this is needed
+            # No detections found - most likely in masked image
+            if raw_detections[BOXES].nelement() == 0:
+                detections.append(None)
+                continue
+
+            raw_detections = _apply_nms(raw_detections, iou_thresh)
+            raw_detections = _filter_score(raw_detections, score_thresh)
+
+            # Note that FasterRCNN doesn't return a score for each class, only
+            # the predicted class. DRISE requires a score for each class.
+            # We approximate the score for each class
+            # by dividing (class score) evenly among the other classes.
+
+            expanded_class_scores = expand_class_scores(
+                raw_detections[SCORES],
+                raw_detections[LABELS],
+                self._number_of_classes)
+
+            detections.append(
+                od_common.DetectionRecord(
+                    bounding_boxes=raw_detections[BOXES],
+                    class_scores=expanded_class_scores,
+                    objectness_scores=torch.tensor(
+                        [1.0]*raw_detections[BOXES].shape[0]),
+                ))
+
+        return detections
```

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/model_utils.py` & `ml_wrappers-0.4.8/ml_wrappers/model/model_utils.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/model_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/predictions_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/predictions_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/pytorch_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/tensorflow_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/tensorflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/text_model_wrapper.py` & `ml_wrappers-0.4.8/ml_wrappers/model/text_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_model.py` & `ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_without_proba_model.py` & `ml_wrappers-0.4.8/ml_wrappers/model/wrapped_classification_without_proba_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers/model/wrapped_regression_model.py` & `ml_wrappers-0.4.8/ml_wrappers/model/wrapped_regression_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/ml_wrappers.egg-info/PKG-INFO` & `ml_wrappers-0.4.8/ml_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-wrappers
-Version: 0.4.7
+Version: 0.4.8
 Summary: Machine Learning Wrappers SDK for Python
 Home-page: https://github.com/microsoft/ml-wrappers
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_wrappers-0.4.7/ml_wrappers.egg-info/SOURCES.txt` & `ml_wrappers-0.4.8/ml_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.7/setup.py` & `ml_wrappers-0.4.8/setup.py`

 * *Files identical despite different names*

