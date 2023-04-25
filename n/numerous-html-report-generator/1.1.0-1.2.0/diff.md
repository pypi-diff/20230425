# Comparing `tmp/numerous html-report-generator-1.1.0.tar.gz` & `tmp/numerous html-report-generator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerous html-report-generator-1.1.0.tar", last modified: Tue Apr 18 12:20:34 2023, max compression
+gzip compressed data, was "numerous html-report-generator-1.2.0.tar", last modified: Tue Apr 25 07:10:22 2023, max compression
```

## Comparing `numerous html-report-generator-1.1.0.tar` & `numerous html-report-generator-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.991454 numerous html-report-generator-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3156 2023-04-18 12:20:34.990538 numerous html-report-generator-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2627 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:20:34.992371 numerous html-report-generator-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1231 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.981370 numerous html-report-generator-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.979537 numerous html-report-generator-1.1.0/src/numerous/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.984120 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/block.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/caption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.985954 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/div.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/figure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.986871 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/dataframetable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.986871 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/gofigure.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/section.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/table.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/tabs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.987787 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1715 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/quick_start.py
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.987787 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6319 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/templates/report_template_numerous.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.990538 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3156 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1341 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.636365 numerous html-report-generator-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-04-25 07:10:22.635365 numerous html-report-generator-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 07:10:22.636365 numerous html-report-generator-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.625364 numerous html-report-generator-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.623364 numerous html-report-generator-1.2.0/src/numerous/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.628364 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/block.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/caption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.630365 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/div.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/figure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.631365 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/pandas/dataframetable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.632365 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/plotly/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/plotly/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/plotly/gofigure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/section.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/tabs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.632365 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/examples/quick_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.633365 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6319 2023-04-25 07:10:11.000000 numerous html-report-generator-1.2.0/src/numerous/html_report_generator/templates/report_template_numerous.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:10:22.634365 numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-04-25 07:10:22.000000 numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-04-25 07:10:22.000000 numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:10:22.000000 numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-25 07:10:22.000000 numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-25 07:10:22.000000 numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/top_level.txt
```

### Comparing `numerous html-report-generator-1.1.0/LICENSE` & `numerous html-report-generator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/PKG-INFO` & `numerous html-report-generator-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous html-report-generator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Report generator for html reports
 Home-page: 
 Author: numerous - Tobias Skov Reipuert, Tobias Dokkedal Elmøe, Lasse Nyberg Thomsen, Ósk Björnsdottir
 Author-email: report-generator@numerous.com
 License: O-BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `numerous html-report-generator-1.1.0/README.md` & `numerous html-report-generator-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/setup.py` & `numerous html-report-generator-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/__init__.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/caption.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/caption.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from typing import List
+from typing import Optional
 
 _figure_number = {}
 
 def get_next_figure_number(type:str):
     if type not in _figure_number:
         _figure_number[type]=0
     _figure_number[type] += 1
     return _figure_number[type]
 
 class Caption:
 
-    def __init__(self, caption, notes: List[str], type:str="Figure"):
+    def __init__(self, caption, notes: Optional[list[str]] = None, type: str = "Figure"):
         self.caption = caption
-        self.notes = notes
+        if notes:
+            self.notes = notes
+        else:
+            self.notes = []
         self.type = type
         self.number = get_next_figure_number(type)
 
     def caption_as_html(self):
         notes_str = ''.join([f'<div class="note"> <i>Note: {n} </i></div>' for n in self.notes])
         return f'<div class="caption-section"><div class="caption"><b>{self.type} {self.number}:</b> {self.caption}</div>{notes_str}</div>'
```

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/cards.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/cards.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/dataframetable.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/pandas/dataframetable.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/gofigure.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/plotly/gofigure.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ..figure import Figure
 from plotly import graph_objects as go
-from typing import List
+from plotly.basedatatypes import BaseTraceType
+from typing import Union, Optional
 def wrap_div(html, class_=None):
     if class_:
         return f"<div class='{class_}'>\n{html}\n</div>\n"
     else:
         return f'<div>\n{html}\n</div>\n'
 
 class GoFigure(Figure):
@@ -12,24 +13,23 @@
 
             Args:
                 figure_data (dict):
                 post_script (str):
             Attributes:
                 html (str):
     """
-    def __init__(self, figure_data:dict, caption:str, notes:List[str]=[], post_script: str = ""):
+    def __init__(self, figure_data: Union[list[BaseTraceType], dict], caption:str, notes:Optional[list[str]] = None, post_script: str = ""):
         super(GoFigure, self).__init__(caption, notes)
         self.figure_data = figure_data
         self.post_script = post_script
+        self.figure_obj = go.Figure(self.figure_data)
 
     def _as_html_figure_content(self):
 
-
-
-        html = wrap_div(go.Figure(self.figure_data).to_html(config={"displayModeBar": True},
+        html = wrap_div(self.figure_obj.to_html(config={"displayModeBar": True},
                                                             # show_link=False,
                                                             include_plotlyjs=False,
                                                             # output_type='div',
                                                             full_html=False,
                                                             post_script=self.post_script),
                         class_='figure_div')
```

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/section.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/section.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/tabs.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/components/tabs.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/quick_start.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/examples/quick_start.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/report.py` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/report.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/templates/report_template_numerous.html` & `numerous html-report-generator-1.2.0/src/numerous/html_report_generator/templates/report_template_numerous.html`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/PKG-INFO` & `numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous-html-report-generator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Report generator for html reports
 Home-page: 
 Author: numerous - Tobias Skov Reipuert, Tobias Dokkedal Elmøe, Lasse Nyberg Thomsen, Ósk Björnsdottir
 Author-email: report-generator@numerous.com
 License: O-BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/SOURCES.txt` & `numerous html-report-generator-1.2.0/src/numerous_html_report_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

