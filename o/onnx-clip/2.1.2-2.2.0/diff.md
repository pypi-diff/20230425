# Comparing `tmp/onnx_clip-2.1.2.tar.gz` & `tmp/onnx_clip-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_clip-2.1.2.tar", max compression
+gzip compressed data, was "onnx_clip-2.2.0.tar", max compression
```

## Comparing `onnx_clip-2.1.2.tar` & `onnx_clip-2.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-03-16 10:15:06.336148 onnx_clip-2.1.2/LICENSE
--rw-r--r--   0        0        0     3521 2023-03-16 10:15:06.336274 onnx_clip-2.1.2/README.md
--rw-r--r--   0        0        0      244 2023-03-16 10:15:06.336677 onnx_clip-2.1.2/onnx_clip/__init__.py
--rw-r--r--   0        0        0       43 2023-03-16 10:15:06.336815 onnx_clip-2.1.2/onnx_clip/data/.gitattributes
--rw-r--r--   0        0        0   252444 2023-03-16 10:15:06.338338 onnx_clip-2.1.2/onnx_clip/data/CLIP.png
--rw-r--r--   0        0        0  1356917 2023-03-16 10:15:06.340139 onnx_clip-2.1.2/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0        0        0   602240 2023-03-16 10:15:06.342232 onnx_clip-2.1.2/onnx_clip/data/expected_preprocessed_image.npy
--rw-r--r--   0        0        0    80530 2023-03-16 10:15:06.342542 onnx_clip-2.1.2/onnx_clip/data/franz-kafka.jpg
--rw-r--r--   0        0        0     9400 2023-03-16 10:16:24.042241 onnx_clip-2.1.2/onnx_clip/model.py
--rw-r--r--   0        0        0     6898 2023-03-16 10:15:06.342829 onnx_clip-2.1.2/onnx_clip/preprocessor.py
--rw-r--r--   0        0        0     7659 2023-03-16 10:15:06.342960 onnx_clip-2.1.2/onnx_clip/tokenizer.py
--rw-r--r--   0        0        0      682 2023-03-16 10:33:01.280331 onnx_clip-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     5482 2023-03-16 10:35:06.781562 onnx_clip-2.1.2/setup.py
--rw-r--r--   0        0        0     4375 2023-03-16 10:35:06.781848 onnx_clip-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-06 16:20:44.660387 onnx_clip-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3521 2023-02-08 12:52:08.334182 onnx_clip-2.2.0/README.md
+-rw-r--r--   0        0        0      244 2023-02-06 16:20:44.660871 onnx_clip-2.2.0/onnx_clip/__init__.py
+-rw-r--r--   0        0        0       43 2023-02-06 16:20:44.660994 onnx_clip-2.2.0/onnx_clip/data/.gitattributes
+-rw-r--r--   0        0        0   252444 2023-02-06 16:20:44.662626 onnx_clip-2.2.0/onnx_clip/data/CLIP.png
+-rw-r--r--   0        0        0  1356917 2023-02-06 16:20:44.664095 onnx_clip-2.2.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0   602240 2023-02-06 16:20:44.666081 onnx_clip-2.2.0/onnx_clip/data/expected_preprocessed_image.npy
+-rw-r--r--   0        0        0    80530 2023-02-06 16:20:44.666325 onnx_clip-2.2.0/onnx_clip/data/franz-kafka.jpg
+-rw-r--r--   0        0        0    10104 2023-04-25 08:59:00.089438 onnx_clip-2.2.0/onnx_clip/model.py
+-rw-r--r--   0        0        0     6898 2023-02-08 12:52:08.334682 onnx_clip-2.2.0/onnx_clip/preprocessor.py
+-rw-r--r--   0        0        0     7659 2023-02-08 12:52:08.335075 onnx_clip-2.2.0/onnx_clip/tokenizer.py
+-rw-r--r--   0        0        0      682 2023-04-25 08:59:00.089808 onnx_clip-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 onnx_clip-2.2.0/setup.py
+-rw-r--r--   0        0        0     4474 1970-01-01 00:00:00.000000 onnx_clip-2.2.0/PKG-INFO
```

### Comparing `onnx_clip-2.1.2/LICENSE` & `onnx_clip-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/README.md` & `onnx_clip-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/onnx_clip/data/CLIP.png` & `onnx_clip-2.2.0/onnx_clip/data/CLIP.png`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz` & `onnx_clip-2.2.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/onnx_clip/data/expected_preprocessed_image.npy` & `onnx_clip-2.2.0/onnx_clip/data/expected_preprocessed_image.npy`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/onnx_clip/data/franz-kafka.jpg` & `onnx_clip-2.2.0/onnx_clip/data/franz-kafka.jpg`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/onnx_clip/model.py` & `onnx_clip-2.2.0/onnx_clip/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,23 +63,40 @@
 
 def get_similarity_scores(
     embeddings_1: np.ndarray, embeddings_2: np.ndarray
 ) -> np.ndarray:
     """Compute pairwise similarity scores between two arrays of embeddings.
 
     For zero-shot classification, these can be used as logits. To do so, call
-    `get_similarity_scores(image_embeddings, text_embeddigs)`.
+    `get_similarity_scores(image_embeddings, text_embeddings)`.
 
     Args:
-        embeddings_1: An array of embeddings of shape (N, D).
-        embeddings_2: An array of embeddings of shape (M, D).
+        embeddings_1: An array of embeddings of shape (N, D) or (D,).
+        embeddings_2: An array of embeddings of shape (M, D) or (D,).
 
     Returns:
-        An array of shape (N, M) with the pairwise similarity scores.
+        An array with the pairwise similarity scores. If both inputs are 2-D,
+            the output will be of shape (N, M). If one input is 1-D, the output
+            will be of shape (N,) or (M,). If both inputs are 1-D, the output
+            will be a scalar.
     """
+    if embeddings_1.ndim == 1:
+        # Convert to 2-D array using x[np.newaxis, :]
+        # and remove the extra dimension at the end.
+        return get_similarity_scores(
+            embeddings_1[np.newaxis, :], embeddings_2
+        )[0]
+
+    if embeddings_2.ndim == 1:
+        # Convert to 2-D array using x[np.newaxis, :]
+        # and remove the extra dimension at the end.
+        return get_similarity_scores(
+            embeddings_1, embeddings_2[np.newaxis, :]
+        )[:, 0]
+
     return cosine_similarity(embeddings_1, embeddings_2) * 100
 
 
 class OnnxClip:
     """
     This class can be utilised to predict the most relevant text snippet, given
     an image, without directly optimizing for the task, similarly to the
```

### Comparing `onnx_clip-2.1.2/onnx_clip/preprocessor.py` & `onnx_clip-2.2.0/onnx_clip/preprocessor.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/onnx_clip/tokenizer.py` & `onnx_clip-2.2.0/onnx_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-2.1.2/pyproject.toml` & `onnx_clip-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "onnx_clip"
-version = "2.1.2"
+version = "2.2.0"
 description = "CLIP with ONNX Runtime and without PyTorch dependencies."
 readme = "README.md"
 authors = ["Lakera AI <dev@lakera.ai>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `onnx_clip-2.1.2/setup.py` & `onnx_clip-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,22 @@
  'onnxruntime>=1.4.0',
  'opencv-python-headless>=4.0.1,<5.0.0',
  'pillow>=8.4.0,<9.0.0',
  'regex']
 
 setup_kwargs = {
     'name': 'onnx-clip',
-    'version': '2.1.2',
+    'version': '2.2.0',
     'description': 'CLIP with ONNX Runtime and without PyTorch dependencies.',
     'long_description': '# onnx_clip\n\nAn [ONNX](https://onnx.ai/)-based implementation of [CLIP](https://github.com/openai/CLIP) that doesn\'t\ndepend on `torch` or `torchvision`.\nIt also has a friendlier API than the original implementation. \n\nThis works by\n- running the text and vision encoders (the ViT-B/32 variant) in [ONNX Runtime](https://onnxruntime.ai/)\n- using a pure NumPy version of the tokenizer\n- using a pure NumPy+PIL version of the [preprocess function](https://github.com/openai/CLIP/blob/3702849800aa56e2223035bccd1c6ef91c704ca8/clip/clip.py#L79).\n  The PIL dependency could also be removed with minimal code changes - see `preprocessor.py`.\n\n## Installation\nTo install, run the following in the root of the repository:\n```bash\npip install .\n```\n\n## Usage\n\nAll you need to do is call the `OnnxClip` model class. An example:\n\n```python\nfrom onnx_clip import OnnxClip, softmax, get_similarity_scores\nfrom PIL import Image\n\nimages = [Image.open("onnx_clip/data/franz-kafka.jpg").convert("RGB")]\ntexts = ["a photo of a man", "a photo of a woman"]\n\n# Your images/texts will get split into batches of this size before being\n# passed to CLIP, to limit memory usage\nonnx_model = OnnxClip(batch_size=16)\n\n# Unlike the original CLIP, there is no need to run tokenization/preprocessing\n# separately - simply run get_image_embeddings directly on PIL images/NumPy\n# arrays, and run get_text_embeddings directly on strings.\nimage_embeddings = onnx_model.get_image_embeddings(images)\ntext_embeddings = onnx_model.get_text_embeddings(texts)\n\n# To use the embeddings for zero-shot classification, you can use these two\n# functions. Here we run on a single image, but any number is supported.\nlogits = get_similarity_scores(image_embeddings, text_embeddings)\nprobabilities = softmax(logits)\n\nprint("Logits:", logits)\n\nfor text, p in zip(texts, probabilities[0]):\n    print(f"Probability that the image is \'{text}\': {p:.3f}")\n```\n\n## Building & developing from source\n\n**Note**: The following may give timeout errors due to the filesizes. If so, this can be fixed with poetry version 1.1.13 - see [this related issue.](https://github.com/python-poetry/poetry/issues/6009)\n\n### Install, run, build and publish with Poetry\n\nInstall [Poetry](https://python-poetry.org/docs/)\n```\ncurl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -\n```\n\nTo setup the project and create a virtual environment run the following command from the project\'s root directory.\n```\npoetry install\n```\n\nTo build a source and wheel distribution of the library run the following command from the project\'s root directory.\n```\npoetry build\n```\n\n#### Publishing a new version to PyPI (for project maintainers)\n\nFirst, remove/move the downloaded LFS files, so that they\'re not packaged with the code.\nOtherwise, this creates a huge `.whl` file that PyPI refuses and it causes confusing errors.\n\nThen, follow [this guide](https://towardsdatascience.com/how-to-publish-a-python-package-to-pypi-using-poetry-aa804533fc6f).\ntl;dr: go to the [PyPI account page](https://pypi.org/manage/account/), generate an API token\nand put it into the `$PYPI_PASSWORD` environment variable. Then run\n```shell\npoetry publish --build --username "__token__" --password $PYPI_PASSWORD\n```\n\n## Help\n\nPlease let us know how we can support you: [earlyaccess@lakera.ai](mailto:earlyaccess@lakera.ai).\n\n## LICENSE\nSee the [LICENSE](./LICENSE) file in this repository.\n\nThe `franz-kafka.jpg` is taken from [here](https://www.knesebeck-verlag.de/franz_kafka/p-1/270).',
     'author': 'Lakera AI',
     'author_email': 'dev@lakera.ai',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6.1,<4.0.0',
 }
```

### Comparing `onnx_clip-2.1.2/PKG-INFO` & `onnx_clip-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: onnx-clip
-Version: 2.1.2
+Version: 2.2.0
 Summary: CLIP with ONNX Runtime and without PyTorch dependencies.
 Author: Lakera AI
 Author-email: dev@lakera.ai
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: boto3 (>=1.23.10,<2.0.0)
 Requires-Dist: ftfy (>=6.0.3,<7.0.0)
 Requires-Dist: numpy (>=1.18.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.4.0)
 Requires-Dist: opencv-python-headless (>=4.0.1,<5.0.0)
 Requires-Dist: pillow (>=8.4.0,<9.0.0)
 Requires-Dist: regex
```

