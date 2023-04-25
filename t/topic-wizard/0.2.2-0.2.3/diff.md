# Comparing `tmp/topic_wizard-0.2.2.tar.gz` & `tmp/topic_wizard-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.2.2.tar", max compression
+gzip compressed data, was "topic_wizard-0.2.3.tar", max compression
```

## Comparing `topic_wizard-0.2.2.tar` & `topic_wizard-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.2/LICENSE
--rw-r--r--   0        0        0     2140 2023-03-13 12:27:09.710202 topic_wizard-0.2.2/README.md
--rw-r--r--   0        0        0      599 2023-03-13 12:26:24.086078 topic_wizard-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      129 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/__init__.py
--rw-r--r--   0        0        0     7178 2023-02-19 18:11:00.271490 topic_wizard-0.2.2/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.2/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4020 2023-02-19 17:07:50.945176 topic_wizard-0.2.2/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0     1355 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     5195 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     2777 2023-02-19 17:04:06.096792 topic_wizard-0.2.2/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1852 2023-01-17 16:03:27.727135 topic_wizard-0.2.2/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1319 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.2/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1422 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.2/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2310 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.2/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.2/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     4795 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/plots/topics.py
--rw-r--r--   0        0        0     3422 2023-01-17 16:03:27.731135 topic_wizard-0.2.2/topicwizard/plots/words.py
--rw-r--r--   0        0        0     3271 2023-01-18 17:26:11.263417 topic_wizard-0.2.2/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     4048 2023-01-17 16:03:27.735135 topic_wizard-0.2.2/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.2/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     5032 2023-02-19 16:12:48.483176 topic_wizard-0.2.2/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     3353 1970-01-01 00:00:00.000000 topic_wizard-0.2.2/setup.py
--rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 topic_wizard-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2140 2023-03-13 12:27:09.710202 topic_wizard-0.2.3/README.md
+-rw-r--r--   0        0        0      640 2023-04-25 07:41:20.946715 topic_wizard-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/__init__.py
+-rw-r--r--   0        0        0     7178 2023-02-19 18:11:00.271490 topic_wizard-0.2.3/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.3/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4339 2023-04-24 14:06:16.382303 topic_wizard-0.2.3/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0     1355 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     5195 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3143 2023-04-24 14:37:23.038262 topic_wizard-0.2.3/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:55:26.304691 topic_wizard-0.2.3/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.2.3/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.2.3/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.3/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.2.3/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.3/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.2.3/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.3/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.3/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5178 2023-04-24 14:10:21.226703 topic_wizard-0.2.3/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.2.3/topicwizard/plots/words.py
+-rw-r--r--   0        0        0     2708 2023-04-24 13:29:18.682128 topic_wizard-0.2.3/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     3796 2023-04-24 13:29:24.942145 topic_wizard-0.2.3/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.3/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.2.3/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     3422 1970-01-01 00:00:00.000000 topic_wizard-0.2.3/setup.py
+-rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 topic_wizard-0.2.3/PKG-INFO
```

### Comparing `topic_wizard-0.2.2/LICENSE` & `topic_wizard-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/README.md` & `topic_wizard-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/pyproject.toml` & `topic_wizard-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.2.2"
+version = "0.2.3"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0"
 dash = "~2.7.1"
 dash-extensions = "~0.1.10"
 dash-mantine-components = "~0.11.1"
 dash-iconify = "~0.1.2"
 joblib = "~1.2.0"
 scikit-learn = "~1.2.0"
+scipy = ">=1.8.0"
+umap-learn = ">=0.5.3"
 numpy = ">=1.22.0"
 pandas = "~1.5.2"
 wordcloud = "~1.8.2.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `topic_wizard-0.2.2/topicwizard/app.py` & `topic_wizard-0.2.3/topicwizard/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/assets/favicon.ico` & `topic_wizard-0.2.3/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/blueprints/app.py` & `topic_wizard-0.2.3/topicwizard/blueprints/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/blueprints/documents.py` & `topic_wizard-0.2.3/topicwizard/blueprints/documents.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-from typing import List, Any
+from typing import Any, List
 
 import dash_mantine_components as dmc
 import numpy as np
-from dash_extensions.enrich import (
-    DashBlueprint,
-    dcc,
-    html,
-    html,
-)
+from dash_extensions.enrich import DashBlueprint, dcc, html
+from plotly import colors
 
 import topicwizard.prepare.documents as prepare
 from topicwizard.components.documents.document_map import create_document_map
-from topicwizard.components.documents.window_slider import create_window_slider
 from topicwizard.components.documents.document_pie import create_document_pie
+from topicwizard.components.documents.document_selector import \
+    create_document_selector
 from topicwizard.components.documents.document_timeline import create_timeline
-from topicwizard.components.documents.document_selector import (
-    create_document_selector,
-)
-from topicwizard.components.documents.document_wordcloud import (
-    create_document_wordcloud,
-)
+from topicwizard.components.documents.document_wordcloud import \
+    create_document_wordcloud
+from topicwizard.components.documents.window_slider import create_window_slider
 
 
 def create_blueprint(
     vocab: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
     topic_term_matrix: np.ndarray,
     document_names: List[str],
     corpus: List[str],
     vectorizer: Any,
     topic_model: Any,
     topic_names: List[str],
 ) -> DashBlueprint:
-
     # --------[ Preparing data ]--------
     n_topics = topic_term_matrix.shape[0]
     document_positions = prepare.document_positions(
         document_term_matrix=document_term_matrix
     )
     dominant_topics = prepare.dominant_topic(
         document_topic_matrix=document_topic_matrix
     )
+    # Creating unified color scheme
+    twilight = colors.get_colorscale("Twilight")
+    topic_colors = colors.sample_colorscale(twilight, np.arange(n_topics) / n_topics)
+    topic_colors = np.array(topic_colors)
 
     # --------[ Collecting blueprints ]--------
     document_map = create_document_map(
         document_names=document_names,
         document_positions=document_positions,
         dominant_topic=dominant_topics,
         n_topics=n_topics,
+        topic_colors=topic_colors,
     )
     timeline = create_timeline(
-        corpus=corpus, vectorizer=vectorizer, topic_model=topic_model
+        corpus=corpus,
+        vectorizer=vectorizer,
+        topic_model=topic_model,
+        topic_colors=topic_colors,
     )
     document_wordcloud = create_document_wordcloud(
         document_term_matrix=document_term_matrix, vocab=vocab
     )
     document_selector = create_document_selector(document_names=document_names)
     window_slider = create_window_slider()
     document_pie = create_document_pie(
-        document_topic_matrix=document_topic_matrix
+        document_topic_matrix=document_topic_matrix, topic_colors=topic_colors
     )
     blueprints = [
         document_map,
         document_selector,
         document_wordcloud,
         document_pie,
         timeline,
```

### Comparing `topic_wizard-0.2.2/topicwizard/blueprints/template.py` & `topic_wizard-0.2.3/topicwizard/blueprints/template.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/blueprints/topics.py` & `topic_wizard-0.2.3/topicwizard/blueprints/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/blueprints/words.py` & `topic_wizard-0.2.3/topicwizard/blueprints/words.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-from typing import List, Any
-import numpy as np
-from dash_extensions.enrich import (
-    DashBlueprint,
-    dcc,
-    html,
-)
+from typing import Any, List
+
 import dash_mantine_components as dmc
+import numpy as np
+from dash_extensions.enrich import DashBlueprint, dcc, html
+from plotly import colors
 
 import topicwizard.prepare.words as prepare
+from topicwizard.components.words.association_slider import \
+    create_association_slider
+from topicwizard.components.words.word_barplot import create_word_barplot
 from topicwizard.components.words.word_map import create_word_map
 from topicwizard.components.words.word_selector import create_word_selector
-from topicwizard.components.words.word_barplot import create_word_barplot
-from topicwizard.components.words.association_slider import (
-    create_association_slider,
-)
 
 
 def create_blueprint(
     vocab: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
     topic_term_matrix: np.ndarray,
     document_names: List[str],
     corpus: List[str],
     vectorizer: Any,
     topic_model: Any,
     topic_names: List[str],
 ) -> DashBlueprint:
     # --------[ Preparing data ]--------
-    word_positions = prepare.word_positions(
-        topic_term_matrix=topic_term_matrix
-    )
+    word_positions = prepare.word_positions(topic_term_matrix=topic_term_matrix)
     word_frequencies = prepare.word_importances(document_term_matrix)
+    dominant_topic = prepare.dominant_topic(topic_term_matrix)
+    n_topics = len(topic_names)
+    # Creating unified color scheme
+    tempo = colors.get_colorscale("tempo")
+    topic_colors = colors.sample_colorscale(tempo, np.arange(n_topics) / n_topics)
+    topic_colors = np.array(topic_colors)
 
     # --------[ Collecting blueprints ]--------
     word_map = create_word_map(
         word_positions=word_positions,
         word_frequencies=word_frequencies,
         vocab=vocab,
+        dominant_topic=dominant_topic,
+        topic_colors=topic_colors,
     )
     word_selector = create_word_selector(vocab=vocab)
     association_slider = create_association_slider(
         topic_term_matrix=topic_term_matrix,
     )
     word_barplot = create_word_barplot(topic_term_matrix=topic_term_matrix)
     blueprints = [word_map, word_selector, word_barplot, association_slider]
```

### Comparing `topic_wizard-0.2.2/topicwizard/components/documents/document_map.py` & `topic_wizard-0.2.3/topicwizard/components/documents/document_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-from typing import Tuple, List
+from typing import List, Tuple
 
 import numpy as np
+from dash_extensions.enrich import DashBlueprint, Input, Output, State, dcc
 
-from dash_extensions.enrich import (
-    DashBlueprint,
-    dcc,
-    Input,
-    Output,
-    State,
-)
 import topicwizard.plots.documents as plots
 
 
 def create_document_map(
     document_positions: Tuple[np.ndarray, np.ndarray],
     dominant_topic: np.ndarray,
     document_names: List[str],
     n_topics: int,
+    topic_colors: np.ndarray,
 ):
     x, y = document_positions
 
     document_map = DashBlueprint()
 
     document_map.layout = dcc.Graph(
         id="document_map",
         responsive=True,
         figure=plots.document_map(
             x=x,
             y=y,
             document_names=document_names,
+            dominant_topic=dominant_topic,
+            topic_colors=topic_colors,
         ),
         className="flex-1",
     )
 
     document_map.clientside_callback(
         """
         function(selectedDocument, currentPlot) {
@@ -40,20 +37,21 @@
                 return {'data': [], 'layout': {}};
             }
             const trigerred = window.dash_clientside.callback_context.triggered[0];
             const trigerredId = trigerred.prop_id.split(".")[0];
             const trace = currentPlot.data[0];
             const nDocuments = trace.x.length
             const text = new Array(nDocuments).fill('');
-            const colors = new Array(nDocuments).fill('#a8a29e');
+            // const colors = new Array(nDocuments).fill('#a8a29e');
             if (selectedDocument !== undefined) {
                 text[selectedDocument] = trace.customdata[selectedDocument][1];
-                colors[selectedDocument] = '#5F3DC4';
+                // colors[selectedDocument] = '#5F3DC4';
             }
-            const marker = {...trace.marker, 'color': colors};
+            // const marker = {...trace.marker, 'color': colors};
+            const marker = {...trace.marker}
             const newTrace = {...trace, 'marker': marker, 'text': text};
             const newFigure = {...currentPlot, 'data': [newTrace]};
             return newFigure;
         }
         """,
         Output("document_map", "figure"),
         Input("selected_document", "data"),
```

### Comparing `topic_wizard-0.2.2/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.2.3/topicwizard/components/documents/document_pie.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from typing import List, Union
 
 import numpy as np
 import plotly.graph_objects as go
+from dash_extensions.enrich import (DashBlueprint, Input, Output, State, dcc,
+                                    exceptions)
 
-from dash_extensions.enrich import (
-    DashBlueprint,
-    dcc,
-    Input,
-    Output,
-    State,
-    exceptions,
-)
 import topicwizard.plots.documents as plots
 import topicwizard.prepare.documents as prepare
 
 
-def create_document_pie(document_topic_matrix: np.ndarray) -> DashBlueprint:
+def create_document_pie(
+    document_topic_matrix: np.ndarray, topic_colors: np.ndarray
+) -> DashBlueprint:
     topic_importances = prepare.document_topic_importances(
         document_topic_matrix=document_topic_matrix
     )
 
     document_pie = DashBlueprint()
 
     document_pie.layout = dcc.Graph(
@@ -36,14 +32,15 @@
     def update_plot(
         selected_document: Union[int, str], topic_names: List[str]
     ) -> go.Figure:
         if isinstance(selected_document, str):
             selected_document = selected_document.strip()
             selected_document = int(selected_document)
         return plots.document_topic_plot(
+            topic_colors=topic_colors,
             topic_importances=topic_importances[
                 topic_importances.doc_id == selected_document
             ],
             topic_names=topic_names,
         )
 
     return document_pie
```

### Comparing `topic_wizard-0.2.2/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.2.3/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.2.3/topicwizard/components/documents/document_timeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from typing import Tuple, List, Union, Any
+from typing import Any, List, Tuple, Union
 
 import numpy as np
-
-from dash_extensions.enrich import (
-    DashBlueprint,
-    dcc,
-    Input,
-    Output,
-    State,
-)
 import plotly.graph_objects as go
+from dash_extensions.enrich import DashBlueprint, Input, Output, State, dcc
+
 import topicwizard.plots.documents as plots
 import topicwizard.prepare.documents as prepare
 
 
-def create_timeline(corpus: List[str], vectorizer: Any, topic_model: Any):
+def create_timeline(
+    corpus: List[str], vectorizer: Any, topic_model: Any, topic_colors: np.ndarray
+):
     timeline = DashBlueprint()
 
     timeline.layout = dcc.Graph(
         id="timeline",
         responsive=True,
         className="flex-1",
     )
@@ -42,12 +38,13 @@
             corpus=corpus,
             vectorizer=vectorizer,
             topic_model=topic_model,
             window_size=window_size,
             step=1,
         )
         return plots.document_timeline(
+            topic_colors=topic_colors,
             topic_timeline=topic_timeline,
             topic_names=topic_names,
         )
 
     return timeline
```

### Comparing `topic_wizard-0.2.2/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.2.3/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.2.3/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.2.3/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.2.3/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.2.3/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.2.3/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/words/association_slider.py` & `topic_wizard-0.2.3/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.2.3/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/components/words/word_map.py` & `topic_wizard-0.2.3/topicwizard/components/words/word_map.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from typing import Tuple
 
 import numpy as np
+from dash_extensions.enrich import DashBlueprint, Input, Output, State, dcc
 
-from dash_extensions.enrich import (
-    DashBlueprint,
-    dcc,
-    Input,
-    Output,
-    State,
-)
 import topicwizard.plots.words as plots
 
 
 def create_word_map(
     word_positions: Tuple[np.ndarray, np.ndarray],
     word_frequencies: np.ndarray,
     vocab: np.ndarray,
+    dominant_topic: np.ndarray,
+    topic_colors: np.ndarray,
 ):
     x, y = word_positions
 
     word_map = DashBlueprint()
 
     word_map.layout = dcc.Graph(
         id="word_map",
         responsive=True,
         # config=dict(scrollZoom=True),
         # animate=True,
         figure=plots.word_map(
-            x=x, y=y, word_frequencies=word_frequencies, vocab=vocab
+            x=x,
+            y=y,
+            word_frequencies=word_frequencies,
+            vocab=vocab,
+            dominant_topic=dominant_topic,
+            topic_colors=topic_colors,
         ),
         className="flex-1",
     )
 
     word_map.clientside_callback(
         """
         function(selectedWords, associatedWords, currentPlot, vocab) {
@@ -53,15 +54,16 @@
                 textSize[index] = 22;
             })
             associatedWords.forEach(index => {
                 text[index] = vocab[index];
                 colors[index] = '#89dcc3';
             })
             const textFont = {'color': textColor, 'size': textSize};
-            const marker = {...trace.marker, 'color': colors};
+            // const marker = {...trace.marker, 'color': colors};
+            const marker = {...trace.marker}
             const newTrace = {...trace, 'marker': marker, 'text': text, 'textfont': textFont};
             const newFigure = {...currentPlot, 'data': [newTrace]};
             return newFigure;
         }
         """,
         Output("word_map", "figure"),
         Input("selected_words", "data"),
```

### Comparing `topic_wizard-0.2.2/topicwizard/components/words/word_selector.py` & `topic_wizard-0.2.3/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/plots/documents.py` & `topic_wizard-0.2.3/topicwizard/plots/documents.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Module containing plotting utilities for documents."""
-from typing import Dict, List, Optional, Iterable
+from typing import Dict, Iterable, List, Optional
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import scipy.sparse as spr
 from PIL import Image
 from wordcloud import WordCloud
 
 
 def document_map(
     x: np.ndarray,
     y: np.ndarray,
     document_names: List[str],
+    dominant_topic: np.ndarray,
+    topic_colors: np.ndarray,
 ) -> go.Figure:
     n_documents = x.shape[0]
     customdata = np.array([np.arange(n_documents), document_names]).T
     trace = go.Scattergl(
         x=x,
         y=y,
         mode="markers+text",
         text=[""] * n_documents,
-        marker=dict(color="#a8a29e", line=dict(width=1, color="white")),
+        marker=dict(
+            color=topic_colors[dominant_topic], line=dict(width=1, color="white")
+        ),
         customdata=customdata,
         hovertemplate="%{customdata[1]}",
         name="",
         textfont=dict(size=16),
     )
     fig = go.Figure([trace])
     fig.update_layout(
@@ -60,14 +64,15 @@
     )
     return fig
 
 
 def document_topic_plot(
     topic_importances: pd.DataFrame,
     topic_names: List[str],
+    topic_colors: np.ndarray,
 ) -> go.Figure:
     """Plots topic importances for a selected document.
 
     Parameters
     ----------
     topic_importances: dict of int to float
         Mapping of topic id's to importances.
@@ -76,46 +81,51 @@
 
     Returns
     -------
     Figure
         Pie chart of topic importances for each document.
     """
     name_mapping = pd.Series(topic_names)
+    n_topics = len(topic_names)
+    color_mapping = {topic_names[i]: topic_colors[i] for i in range(n_topics)}
     topic_importances = topic_importances.assign(
         topic_name=topic_importances.topic_id.map(name_mapping)
     )
     fig = px.pie(
         topic_importances,
         values="importance",
         names="topic_name",
-        color_discrete_sequence=px.colors.cyclical.Twilight,
+        color="topic_name",
+        color_discrete_map=color_mapping,
+        # color_discrete_sequence=px.colors.cyclical.Twilight,
     )
     fig.update_traces(textposition="inside", textinfo="label")
     fig.update_layout(
         showlegend=False,
         paper_bgcolor="rgba(1,1,1,0)",
         plot_bgcolor="rgba(1,1,1,0)",
     )
     return fig
 
 
 def document_timeline(
-    topic_timeline: np.ndarray, topic_names: List[str]
+    topic_timeline: np.ndarray, topic_names: List[str], topic_colors: np.ndarray
 ) -> go.Figure:
     topic_timeline = topic_timeline.T
     traces = []
     n_topics = len(topic_names)
     for topic_id in range(n_topics):
         timeline = topic_timeline[topic_id]
         timeline = np.squeeze(np.asarray(timeline))
         trace = go.Scattergl(
             x=np.arange(timeline.shape[0]),
             y=timeline,
             mode="lines",
             name=topic_names[topic_id],
+            marker=dict(color=topic_colors[topic_id]),
         )
         traces.append(trace)
     fig = go.Figure(data=traces)
     fig.update_layout(
         hovermode="closest",
         plot_bgcolor="white",
         margin=dict(l=0, r=0, b=0, t=0, pad=0),
@@ -142,17 +152,15 @@
     return fig
 
 
 def document_wordcloud(
     doc_id: int, document_term_matrix: np.ndarray, vocab: np.ndarray
 ) -> go.Figure:
     coo = spr.coo_array(document_term_matrix[doc_id])
-    term_dict = {
-        vocab[column]: data for column, data in zip(coo.col, coo.data)
-    }
+    term_dict = {vocab[column]: data for column, data in zip(coo.col, coo.data)}
     cloud = WordCloud(
         width=800,
         height=800,
         background_color="white",
         colormap="twilight",
         scale=4,
     ).generate_from_frequencies(term_dict)
```

### Comparing `topic_wizard-0.2.2/topicwizard/plots/topics.py` & `topic_wizard-0.2.3/topicwizard/plots/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/plots/words.py` & `topic_wizard-0.2.3/topicwizard/plots/words.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 
 
 def word_map(
     x: np.ndarray,
     y: np.ndarray,
     word_frequencies: np.ndarray,
     vocab: np.ndarray,
+    dominant_topic: np.ndarray,
+    topic_colors: np.ndarray,
 ) -> go.Figure:
     """Plots all words in relation to each other."""
     n_words = vocab.shape[0]
     customdata = np.array([np.arange(n_words), vocab]).T
     word_trace = go.Scattergl(
         x=x,
         y=y,
         mode="text+markers",
         text=[""] * n_words,
         marker=dict(
             size=word_frequencies,
             sizemode="area",
             sizeref=2.0 * max(word_frequencies) / (100.0**2),
             sizemin=4,
-            color="#a8a29e",
+            color=topic_colors[dominant_topic],
         ),
         customdata=customdata,
         hovertemplate="%{customdata[1]}",
         name="",
     )
     fig = go.Figure([word_trace])
     fig.update_layout(
```

### Comparing `topic_wizard-0.2.2/topicwizard/prepare/documents.py` & `topic_wizard-0.2.3/topicwizard/prepare/documents.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from typing import Tuple, List, Any
+from typing import Any, List, Tuple
 
 import numpy as np
 import pandas as pd
 import scipy.sparse as spr
-from sklearn.manifold import TSNE
-from sklearn.preprocessing import StandardScaler
-from sklearn.decomposition import TruncatedSVD
-from sklearn.pipeline import Pipeline
+import umap
 
 
 def dominant_topic(document_topic_matrix: np.ndarray) -> np.ndarray:
     """Calculates dominant topic for each document.
 
     Parameters
     ----------
@@ -37,35 +34,21 @@
     Returns
     -------
     x: array of shape (n_topics)
     y: array of shape (n_topics)
     """
     # Calculating distances
     n_docs = document_term_matrix.shape[0]
-    svd = TruncatedSVD(10)
-    # Choosing perplexity such that the pipeline never fails
     perplexity = np.min((40, n_docs - 1))
-    manifold = TSNE(
+    manifold = umap.UMAP(
         n_components=2,
-        # affinity="nearest_neighbors",
-        perplexity=perplexity,
-        init="pca",
-        metric="euclidean",
-        learning_rate="auto",
-        n_iter=400,
-        n_iter_without_progress=100,
+        n_neighbors=perplexity,
+        metric="cosine",
     )
-    reduction_pipeline = Pipeline(
-        [
-            ("svd", svd),
-            ("scaler", StandardScaler()),
-            ("manifold", manifold),
-        ]
-    )
-    x, y = reduction_pipeline.fit_transform(document_term_matrix).T
+    x, y = manifold.fit_transform(document_term_matrix).T
     return x, y
 
 
 def document_topic_importances(
     document_topic_matrix: np.ndarray,
 ) -> pd.DataFrame:
     """Rearranges the document topic matrix to a DataFrame.
```

### Comparing `topic_wizard-0.2.2/topicwizard/prepare/topics.py` & `topic_wizard-0.2.3/topicwizard/prepare/topics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Utilities for preparing data for visualization."""
 from typing import Tuple
-import pandas as pd
 
 import numpy as np
-from sklearn.manifold import TSNE
-from sklearn.metrics import pairwise_distances
+import pandas as pd
+import umap
 
 
 def topic_positions(
     topic_term_matrix: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Calculates topic positions from topic-term matrices.
 
@@ -19,28 +18,19 @@
 
     Returns
     -------
     x: array of shape (n_topics)
     y: array of shape (n_topics)
     """
     # Calculating distances
-    topic_distances = pairwise_distances(
-        topic_term_matrix, metric="correlation"
-    )
     n_topics = topic_term_matrix.shape[0]
     # Setting perplexity to 30, or the number of topics minus one
     perplexity = np.min((30, n_topics - 1))
-    tsne = TSNE(
-        n_components=2,
-        perplexity=perplexity,
-        init="random",
-        learning_rate="auto",
-        metric="precomputed",
-    )
-    x, y = tsne.fit_transform(topic_distances).T
+    manifold = umap.UMAP(n_components=2, n_neighbors=perplexity, metric="cosine")
+    x, y = manifold.fit_transform(topic_term_matrix).T
     return x, y
 
 
 def topic_importances(
     topic_term_matrix: np.ndarray,
     document_term_matrix: np.ndarray,
     document_topic_matrix: np.ndarray,
@@ -58,17 +48,15 @@
     topic_importances: array of shape (n_topics, )
     term_importances: array of shape (n_terms, )
     topic_term_importances: array of shape (n_topics, n_terms)
     """
     # Calculating document lengths
     document_lengths = document_term_matrix.sum(axis=1)
     # Calculating an estimate of empirical topic frequencies
-    topic_importances = (document_topic_matrix.T * document_lengths).sum(
-        axis=1
-    )
+    topic_importances = (document_topic_matrix.T * document_lengths).sum(axis=1)
     topic_importances = np.squeeze(np.asarray(topic_importances))
     # Calculating empirical estimate of term-topic frequencies
     topic_term_importances = (topic_term_matrix.T * topic_importances).T
     # Empirical term frequency
     term_importances = topic_term_importances.sum(axis=0)
     term_importances = np.squeeze(np.asarray(term_importances))
     return topic_importances, term_importances, topic_term_importances
```

### Comparing `topic_wizard-0.2.2/topicwizard/prepare/utils.py` & `topic_wizard-0.2.3/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.2/topicwizard/prepare/words.py` & `topic_wizard-0.2.3/topicwizard/prepare/words.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 """Utilities for preparing data about words."""
-from typing import Tuple, List
+from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
-from sklearn.decomposition import PCA
-from sklearn.manifold import TSNE
-from sklearn.preprocessing import StandardScaler
+import umap
 from sklearn.metrics import pairwise_distances
-from sklearn.pipeline import Pipeline
+
+
+def dominant_topic(topic_term_matrix: np.ndarray) -> np.ndarray:
+    """Calculates dominant topic for each word.
+
+    Parameters
+    ----------
+    topic_term_matrix: array of shape (n_topics, n_terms)
+
+    Returns
+    -------
+    array of shape (n_documents)
+        Index of dominant topic for each term.
+    """
+    term_topic_matrix = topic_term_matrix.T
+    dominant_topic = np.argmax(term_topic_matrix, axis=1)
+    return dominant_topic
 
 
 def calculate_word_distances(
     topic_term_matrix: np.ndarray,
 ) -> np.ndarray:
     """Calculates pairwise word distances with correlation in
     topic coefficients as the metric.
@@ -24,17 +38,15 @@
     -------
     array of shape (n_terms, n_terms)
         Word distance matrix.
     """
     # We use the parameters of the topic model as word embeddings
     term_topic_matrix = topic_term_matrix.T
     # Calculating word distances using correlation
-    word_distances = pairwise_distances(
-        term_topic_matrix, metric="correlation"
-    )
+    word_distances = pairwise_distances(term_topic_matrix, metric="correlation")
     return word_distances
 
 
 def word_positions(
     topic_term_matrix: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Calculates word positions with manifold learning.
@@ -48,36 +60,23 @@
     x: array of shape (n_topics)
     y: array of shape (n_topics)
     """
     # Getting number of words in the vocabulary
     n_topics, n_vocab = topic_term_matrix.shape
     # We use the parameters of the topic model as word embeddings
     term_topic_matrix = topic_term_matrix.T
-    # Adding pre-manifold reduction, so that it runs faster
-    pca = PCA(n_components=np.min((n_topics, 10)))
     # Choosing perplexity such that the pipeline never fails
     perplexity = np.min((40, n_vocab - 1))
-    manifold = TSNE(
+    manifold = umap.UMAP(
         n_components=2,
         # affinity="nearest_neighbors",
-        perplexity=perplexity,
-        init="pca",
-        metric="euclidean",
-        learning_rate="auto",
-        n_iter=400,
-        n_iter_without_progress=100,
-    )
-    reduction_pipeline = Pipeline(
-        [
-            ("pca", pca),
-            ("scaler", StandardScaler()),
-            ("manifold", manifold),
-        ]
+        n_neighbors=perplexity,
+        metric="cosine",
     )
-    x, y = reduction_pipeline.fit_transform(term_topic_matrix).T
+    x, y = manifold.fit_transform(term_topic_matrix).T
     return x, y
 
 
 def word_importances(
     document_term_matrix: np.ndarray,
 ) -> np.ndarray:
     """Calculates overall word frequencies.
@@ -137,15 +136,15 @@
 ) -> List[int]:
     """Returns words that are closely associated with the selected ones."""
     term_topic_matrix = topic_term_matrix.T
     # Selecting terms
     selected_terms_matrix = term_topic_matrix[selected_words]
     # Calculating all distances from the selected words
     distances = pairwise_distances(
-        selected_terms_matrix, term_topic_matrix, metric="euclidean"
+        selected_terms_matrix, term_topic_matrix, metric="cosine"
     )
     # Partitions array so that the smallest k elements along axis 1 are at the
     # lowest k dimensions, then I slice the array to only get the top indices
     # We do plus 1, as obviously the closest word is gonna be the word itself
     closest = np.argpartition(distances, kth=n_association + 1, axis=1)[
         :, 1 : n_association + 1
     ]
```

### Comparing `topic_wizard-0.2.2/setup.py` & `topic_wizard-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['topicwizard',
  'topicwizard.blueprints',
+ 'topicwizard.compatibility',
  'topicwizard.components',
  'topicwizard.components.documents',
  'topicwizard.components.topics',
  'topicwizard.components.words',
  'topicwizard.plots',
  'topicwizard.prepare']
 
@@ -19,19 +20,21 @@
  'dash-iconify>=0.1.2,<0.2.0',
  'dash-mantine-components>=0.11.1,<0.12.0',
  'dash>=2.7.1,<2.8.0',
  'joblib>=1.2.0,<1.3.0',
  'numpy>=1.22.0',
  'pandas>=1.5.2,<1.6.0',
  'scikit-learn>=1.2.0,<1.3.0',
+ 'scipy>=1.8.0',
+ 'umap-learn>=0.5.3',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'topic-wizard',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Pretty and opinionated topic model visualization in Python.',
     'long_description': '<img align="left" width="82" height="82" src="assets/logo.svg">\n\n# topicwizard\n\n<br>\n\nPretty and opinionated topic model visualization in Python.\n\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/x-tabdeveloping/topic-wizard/blob/main/examples/basic_usage.ipynb)\n[![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)\n[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)\n<br>\n\n\nhttps://user-images.githubusercontent.com/13087737/219967955-1263c35b-4c5b-4ccc-adb9-23e073e099f0.mp4\n\n\n## Features\n\n-   Investigate complex relations between topics, words and documents\n-   Highly interactive\n-   Name topics\n-   Pretty :art:\n-   Intuitive :cow:\n-   Clean API :candy:\n-   Sklearn compatible :nut_and_bolt:\n-   Easy deployment :earth_africa:\n\n## Installation\n\nInstall from PyPI:\n\n```bash\npip install topic-wizard\n```\n\n## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n\n### Step 1:\n\nTrain a scikit-learn compatible topic model.\n\n```python\nfrom sklearn.decomposition import NMF\nfrom sklearn.feature_extraction.text import CountVectorizer\nfrom sklearn.pipeline import Pipeline\n\ntopic_pipeline = Pipeline(\n    [\n        ("bow", CountVectorizer()),\n        ("nmf", NMF(n_components=10)),\n    ]\n)\ntopic_pipeline.fit(texts)\n```\n\n### Step 2:\n\nVisualize with topicwizard.\n\n```python\nimport topicwizard\n\ntopicwizard.visualize(pipeline=topic_pipeline, corpus=texts)\n```\n\n### Step 3:\n\nInvestigate :eyes: .\n\n#### a) Topics\n\n![topics screenshot](assets/screenshot_topics.png)\n\n#### b) Words\n\n![words screenshot](assets/screenshot_words.png)\n![words screenshot](assets/screenshot_words_zoomed.png)\n\n#### c) Documents\n\n![documents screenshot](assets/screenshot_documents.png)\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `topic_wizard-0.2.2/PKG-INFO` & `topic_wizard-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-wizard
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pretty and opinionated topic model visualization in Python.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,16 @@
 Requires-Dist: dash-extensions (>=0.1.10,<0.2.0)
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
 Requires-Dist: dash-mantine-components (>=0.11.1,<0.12.0)
 Requires-Dist: joblib (>=1.2.0,<1.3.0)
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: pandas (>=1.5.2,<1.6.0)
 Requires-Dist: scikit-learn (>=1.2.0,<1.3.0)
+Requires-Dist: scipy (>=1.8.0)
+Requires-Dist: umap-learn (>=0.5.3)
 Requires-Dist: wordcloud (>=1.8.2.2,<1.9.0.0)
 Description-Content-Type: text/markdown
 
 <img align="left" width="82" height="82" src="assets/logo.svg">
 
 # topicwizard
```

