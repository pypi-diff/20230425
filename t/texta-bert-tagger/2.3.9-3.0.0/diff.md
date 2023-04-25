# Comparing `tmp/texta-bert-tagger-2.3.9.tar.gz` & `tmp/texta-bert-tagger-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texta-bert-tagger-2.3.9.tar", last modified: Tue Mar  1 16:37:30 2022, max compression
+gzip compressed data, was "texta-bert-tagger-3.0.0.tar", last modified: Tue Apr 25 12:41:37 2023, max compression
```

## Comparing `texta-bert-tagger-2.3.9.tar` & `texta-bert-tagger-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 16:37:30.700533 texta-bert-tagger-2.3.9/
--rw-r--r--   0 root         (0) root         (0)     1750 2022-03-01 16:37:30.700533 texta-bert-tagger-2.3.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1102 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-01 16:37:30.700533 texta-bert-tagger-2.3.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      687 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 16:37:30.700533 texta-bert-tagger-2.3.9/texta_bert_tagger/
--rw-rw-rw-   0 root         (0) root         (0)     3360 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/texta_bert_tagger/config.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/texta_bert_tagger/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37896 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/texta_bert_tagger/tagger.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/texta_bert_tagger/tagging_report.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2022-03-01 16:20:34.000000 texta-bert-tagger-2.3.9/texta_bert_tagger/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-01 16:37:30.700533 texta-bert-tagger-2.3.9/texta_bert_tagger.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1750 2022-03-01 16:37:30.000000 texta-bert-tagger-2.3.9/texta_bert_tagger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2022-03-01 16:37:30.000000 texta-bert-tagger-2.3.9/texta_bert_tagger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-01 16:37:30.000000 texta-bert-tagger-2.3.9/texta_bert_tagger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2022-03-01 16:37:30.000000 texta-bert-tagger-2.3.9/texta_bert_tagger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-03-01 16:37:30.000000 texta-bert-tagger-2.3.9/texta_bert_tagger.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:41:37.190668 texta-bert-tagger-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2023-03-14 13:23:16.000000 texta-bert-tagger-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-25 12:41:37.190668 texta-bert-tagger-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-25 12:41:13.000000 texta-bert-tagger-3.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-25 12:41:13.000000 texta-bert-tagger-3.0.0/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-21 14:35:09.000000 texta-bert-tagger-3.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 12:41:37.190668 texta-bert-tagger-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-03-14 13:23:16.000000 texta-bert-tagger-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:41:37.190668 texta-bert-tagger-3.0.0/texta_bert_tagger/
+-rw-rw-rw-   0 root         (0) root         (0)    11119 2023-04-24 12:12:15.000000 texta-bert-tagger-3.0.0/texta_bert_tagger/attributions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3360 2023-03-14 13:23:16.000000 texta-bert-tagger-3.0.0/texta_bert_tagger/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-14 13:23:16.000000 texta-bert-tagger-3.0.0/texta_bert_tagger/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    42566 2023-04-25 12:41:13.000000 texta-bert-tagger-3.0.0/texta_bert_tagger/tagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-03-14 13:23:16.000000 texta-bert-tagger-3.0.0/texta_bert_tagger/tagging_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-03-14 13:23:16.000000 texta-bert-tagger-3.0.0/texta_bert_tagger/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:41:37.190668 texta-bert-tagger-3.0.0/texta_bert_tagger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-25 12:41:37.000000 texta-bert-tagger-3.0.0/texta_bert_tagger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 12:41:37.000000 texta-bert-tagger-3.0.0/texta_bert_tagger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 12:41:37.000000 texta-bert-tagger-3.0.0/texta_bert_tagger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-04-25 12:41:37.000000 texta-bert-tagger-3.0.0/texta_bert_tagger.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 12:41:37.000000 texta-bert-tagger-3.0.0/texta_bert_tagger.egg-info/top_level.txt
```

### Comparing `texta-bert-tagger-2.3.9/README.md` & `texta-bert-tagger-3.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# TEXTA Bert Tagger Python package
+# TEXTA Bert Tagger
 
+![Py3.8](https://img.shields.io/badge/python-3.8-green.svg)
+![Py3.9](https://img.shields.io/badge/python-3.9-green.svg)
 
 ## Installation
 
 ##### Using built package
 `pip install texta-bert-tagger`
 
 ##### Using Git
@@ -15,32 +17,34 @@
 
 ### Documentation
 
 Documentation for version 1.* is available [here](https://git.texta.ee/texta/texta-bert-tagger-python/-/wikis/Documentation-v1.*).
 
 Documentation for version 2.* is available [here](https://git.texta.ee/texta/texta-bert-tagger-python/-/wikis/Documentation-v2.*).
 
-## Usage (for versions >=2.*.*)
+Documentation for version 3.* is available [here](https://git.texta.ee/texta/texta-bert-tagger-python/-/wikis/Documentation-v3.*).
+
+## Usage (for versions >=3.*.*)
 
 ### Fine-tune BERT model
 
 ```python
 from texta_bert_tagger.tagger import BertTagger
 bert_tagger = BertTagger()
 
 data_sample = {"good": ["It was a nice day.", "All was well."], "bad": ["It was horrible.", "What a disaster."]}
 
 # Train a model
 
 # pos_label - used in metrics (precision, recall, f1-score etc) calculations as true label
-bert_tagger.train(data_sample, pos_label = "bad", n_epochs=2)
+bert_tagger.train(data_sample, pos_label="bad", n_epochs=2)
 
 # Predict
 result = bert_tagger.tag_text("How awful!")
 print(result)
 ```
 
 #### Output
 
 ```
-{"prediction": "bad", "probability": 0.55200404}
+[{"prediction": "bad", "probability": 0.55200404, "attributions": []}]
 ```
```

### Comparing `texta-bert-tagger-2.3.9/setup.py` & `texta-bert-tagger-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-2.3.9/texta_bert_tagger/config.py` & `texta-bert-tagger-3.0.0/texta_bert_tagger/config.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-2.3.9/texta_bert_tagger/tagger.py` & `texta-bert-tagger-3.0.0/texta_bert_tagger/tagger.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from copy import deepcopy
 from pynvml import nvmlInit, nvmlDeviceGetHandleByIndex, nvmlDeviceGetMemoryInfo
 
 from typing import List, Dict, Tuple, Union
 
 from .tagging_report import TaggingReport
 from .config import Config
+from .attributions import BertConnector, Attributions
 
 from .validators import ModelExistingValidator, ModelLoadedValidator
 from .validators import InputValidator, ArgumentValidator
 from . import exceptions
 
 from transformers import AutoModelForSequenceClassification, AutoTokenizer, AutoConfig
 from transformers import AdamW, get_linear_schedule_with_warmup
@@ -78,15 +79,16 @@
         self.device = self._get_device()
 
         self.models_dir = os.path.join(".","saved_models")
 
         self.optimizer = None
         self.scheduler = None
         self.tokenizer = None
-
+        self.bert_connector = None
+        self.attributions = None
 
     def _make_dir(self, _dir: str):
         """ Make directories.
         """
         if not os.path.exists(_dir):
             os.makedirs(_dir)
 
@@ -278,14 +280,15 @@
             model_to_save.save_pretrained(model_dir)
         return model
 
 
     @staticmethod
     def save_pretrained_model(bert_model: str, save_dir: str, state_dict: OrderedDict = None, logger: logging.Logger = None, cache_dir: str = "", num_labels: int = None):
         model_dir = os.path.join(save_dir, BertTagger.normalize_name(bert_model), "model")
+        print(model_dir)
         if not os.path.exists(model_dir) or len(os.listdir(model_dir)) < 1:
             if logger: logger.info(f"Downloading pretrained model {bert_model}...")
 
             model_kwargs = {"state_dict": state_dict}
 
             if num_labels:
                 model_kwargs.update({"num_labels": num_labels})
@@ -853,37 +856,89 @@
 
         if torch.cuda.is_available():
             torch.cuda.empty_cache()
 
         return report
 
 
-    def tag_text(self, text: str) -> Dict[str, Union[str, float]]:
+    def get_attributions(self,
+                      text: str,
+                      visualize: bool = False,
+                      true_class: str = "N/A",
+                      multiclass_output: bool = False,
+                      words: bool = True,
+                      round_digits: int = 3) -> Dict[str, List[dict]]:
+
+        """ Finds attribution scores for every word in the text.
+        If all_classes = True, returns a dict, where key = class name and
+           value = list of attributions (as dicts).
+        If all_classes = False, returns a list of attributions (as dicts).
+        """
+        attributions = {}
+
+        if not self.bert_connector:
+            self.bert_connector = BertConnector(self)
+
+        # Calculate attributions only for the class with the highest probability
+        if not multiclass_output:
+            # If the attributions are calculated only for a single class, store them
+            self.attributions = Attributions(self.bert_connector, text, round_digits=round_digits)
+            pred_class = self.attributions.predicted_class_str
+            # Output attributions only for the predicted class
+            attributions[pred_class] = {
+                "tokens": self.attributions.token_attributions,
+                "words": self.attributions.word_attributions
+            }
+
+            if visualize:
+                self.attributions.visualize(true_class=true_class, words=words)
+
+        # Calculate attributions for all the classes
+        else:
+
+            for indx, c in list(self.config.label_reverse_index.items()):
+                a = Attributions(self.bert_connector, text, target_class=indx, round_digits=round_digits)
+
+                # Output attributions for all classes c_index
+                attributions[c] = {
+                    "tokens": a.token_attributions,
+                    "words": a.word_attributions
+                }
+
+                if visualize:
+                    a.visualize(true_class=true_class, pred_class=c, words=words)
+
+        return attributions
+
+
+    def tag(self, text: str, multiclass_output: bool = False) -> Union[dict, List[dict]]:
         """ Tag text with previously loaded or trained model.
 
         Parameters:
             text - Text to tag.
 
         Returns:
             prediction - Predicted label for the input text.
             probability - Probability of the predicted label.
         """
         ModelLoadedValidator().validate(self.model)
 
         input_ids, attention_masks, labels = self.tokenize([text])
+
         prediction_dataset = self._get_dataset(input_ids, attention_masks)
         prediction_iterator= self._get_iterator(prediction_dataset)
 
         # Put model in evaluation mode
         self.model.eval()
 
         # Tracking variables
         predictions = []
         probabilities = []
 
+
         # Predict
         for batch in prediction_iterator:
             # Add batch to GPU
             batch = tuple(t.to(self.device) for t in batch)
 
             # Unpack the inputs from our dataloader
             b_input_ids, b_input_mask = batch
@@ -891,40 +946,100 @@
             # Telling the model not to compute or store gradients, saving memory and
             # speeding up prediction
             with torch.no_grad():
                 # Forward pass, calculate logit predictions
                 outputs = self.model(b_input_ids, token_type_ids=None,
                                      attention_mask=b_input_mask)
 
-            logits = outputs['logits']
-            #logits = outputs[0]
+            logits = outputs.get("logits")
 
             # Move logits and labels to CPU
-            logits = logits.detach().cpu()#.numpy()
+            logits = logits.detach().cpu()
 
             # Store predictions and true labels
             predictions.append(logits.numpy())
 
             # Add class probabilities
             probabilities.append(logits.softmax(1).numpy().flatten())
 
-
         flat_predictions = np.concatenate(predictions, axis=0)
 
         # For each sample, pick the label (0 or 1) with the higher score.
         flat_predictions = np.argmax(flat_predictions, axis=1).flatten()
 
         prediction = flat_predictions[0]
         probability = probabilities[0][prediction]
+
         predicted_label = self.config.label_reverse_index[prediction]
 
-        return {"prediction": predicted_label, "probability": probability}
+        all_preds = [
+            {
+                "prediction": self.config.label_reverse_index[i],
+                "probability": probabilities[0][i],
+                "attributions": []
+            }
+            for i in range(self.config.n_classes)
+        ]
+
+        all_preds.sort(key = lambda x: x["probability"], reverse=True)
+
+        if multiclass_output:
+            out = all_preds
+        else:
+            # Take only the most probable element, but store it in a list
+            # to maintain unform output
+            out = [all_preds[0]]
+
+        return out
+
+
+    def tag_text(self,
+                 text: str,
+                 multiclass_output: bool = False,
+                 attributions: bool = False,
+                 visualize: bool = False,
+                 words: bool = True,
+                 true_class: str = "N/A",
+                 attributions_round_digits: int = 3) -> List[dict]:
+        """ Wraps tag (previous tag_text) and get_attributions. By default,
+        attributions are not calculated as it makes the whole function a lot slower.
+
+        Parameters:
+            text - Text to tag.
+            highest_only - If enabled, returns only the most probable tag (as dict in list),
+                otherwise returns a list of all tags with corresponding probabilities
+                and attributions (if the latter is enabled).
+            with_attributions - If enabled, adds attribution scores to the output.
+            visualize - If enabled, visualizes the attributions of each word in the input text.
+                NB! Can be used only in Jupyter notebook.
+            true_class - Used only in the visualization, but
+                doesn't serve any other purpose beyond display.
+            attribution_round_digits - The number of decimal places to use for
+                rounding the attributions scores.
+        """
+        # Get tag + probability
+        result = self.tag(text=text, multiclass_output=multiclass_output)
+
+        if attributions or visualize:
+            attrs = self.get_attributions(
+                text=text,
+                visualize=visualize,
+                true_class=true_class,
+                words=words,
+                multiclass_output=multiclass_output
+            )
+
+            for pred_info in result:
+                tag = pred_info.get("prediction")
+                pred_info["attributions"] = attrs.get(tag)
+
+        return result
 
 
-    def tag_doc(self, doc: json) -> Dict[str, Union[str, float]]:
+    def tag_doc(self, doc: json, multiclass_output: bool = False, attributions: bool = False, words: bool = True) ->  List[dict]:
         """
         Tag document with previously loaded or trained model by combining
         all fields in the document into one text.
 
         Parameters:
             doc - JSON document to tag. NB! each input field is used for tagging!
 
@@ -932,15 +1047,15 @@
             prediction - Predicted label for the input document.
             probability - Probability of the predicted label.
         """
         combined_text = []
         for field_content in list(doc.values()):
             combined_text.append(str(field_content))
         combined_text = " ".join(combined_text)
-        predicted_item = self.tag_text(combined_text)
+        predicted_item = self.tag_text(combined_text, multiclass_output=multiclass_output, attributions=attributions, words=words)
         return predicted_item
 
 
     def save(self, path: str):
         """ Save fine-tuned model.
 
         Parameters:
```

### Comparing `texta-bert-tagger-2.3.9/texta_bert_tagger/tagging_report.py` & `texta-bert-tagger-3.0.0/texta_bert_tagger/tagging_report.py`

 * *Files identical despite different names*

### Comparing `texta-bert-tagger-2.3.9/texta_bert_tagger/validators.py` & `texta-bert-tagger-3.0.0/texta_bert_tagger/validators.py`

 * *Files identical despite different names*

