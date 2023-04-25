# Comparing `tmp/streamlit-component-dropfilltextarea-0.2.2.tar.gz` & `tmp/streamlit-component-dropfilltextarea-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-component-dropfilltextarea-0.2.2.tar", last modified: Wed Apr 19 18:45:40 2023, max compression
+gzip compressed data, was "streamlit-component-dropfilltextarea-0.2.3.tar", last modified: Tue Apr 25 09:46:11 2023, max compression
```

## Comparing `streamlit-component-dropfilltextarea-0.2.2.tar` & `streamlit-component-dropfilltextarea-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.533434 streamlit-component-dropfilltextarea-0.2.2/
--rwxr-xr-x   0 runner    (1000) runner    (1000)     1069 2023-04-18 10:38:05.000000 streamlit-component-dropfilltextarea-0.2.2/LICENSE
--rwxr-xr-x   0 runner    (1000) runner    (1000)       93 2023-04-18 11:35:11.000000 streamlit-component-dropfilltextarea-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     2570 2023-04-19 18:45:40.529434 streamlit-component-dropfilltextarea-0.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1000) runner    (1000)     2061 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-19 18:45:40.533434 streamlit-component-dropfilltextarea-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1000) runner    (1000)      904 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.517434 streamlit-component-dropfilltextarea-0.2.2/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.521434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/
--rwxr-xr-x   0 runner    (1000) runner    (1000)     3111 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.517434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.521434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.521434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/css/
--rw-r--r--   0 runner    (1000) runner    (1000)     1135 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/css/app.153d1a1e.css
--rw-r--r--   0 runner    (1000) runner    (1000)      725 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.525434 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/
--rw-r--r--   0 runner    (1000) runner    (1000)     8229 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js
--rw-r--r--   0 runner    (1000) runner    (1000)    31077 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js.map
--rw-r--r--   0 runner    (1000) runner    (1000)   865876 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
--rw-r--r--   0 runner    (1000) runner    (1000)  3348860 2023-04-19 18:45:35.000000 streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-19 18:45:40.529434 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2570 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      764 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2023-04-19 18:45:40.000000 streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.708339 streamlit-component-dropfilltextarea-0.2.3/
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     1069 2023-04-18 10:38:05.000000 streamlit-component-dropfilltextarea-0.2.3/LICENSE
+-rwxr-xr-x   0 runner    (1000) runner    (1000)       93 2023-04-18 11:35:11.000000 streamlit-component-dropfilltextarea-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     2570 2023-04-25 09:46:11.708339 streamlit-component-dropfilltextarea-0.2.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     2061 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 09:46:11.708339 streamlit-component-dropfilltextarea-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1000) runner    (1000)      904 2023-04-25 09:44:46.000000 streamlit-component-dropfilltextarea-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.692338 streamlit-component-dropfilltextarea-0.2.3/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.692338 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     3111 2023-04-19 18:44:44.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.692338 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.692338 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.696338 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/css/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1297 2023-04-25 09:46:01.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/css/app.58e9fcbb.css
+-rw-r--r--   0 runner    (1000) runner    (1000)      725 2023-04-25 09:46:01.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.696338 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8229 2023-04-25 09:46:01.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/app.7306c276.js
+-rw-r--r--   0 runner    (1000) runner    (1000)    31200 2023-04-25 09:46:01.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/app.7306c276.js.map
+-rw-r--r--   0 runner    (1000) runner    (1000)   865876 2023-04-25 09:46:01.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
+-rw-r--r--   0 runner    (1000) runner    (1000)  3348860 2023-04-25 09:46:01.000000 streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 09:46:11.708339 streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2570 2023-04-25 09:46:11.000000 streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      764 2023-04-25 09:46:11.000000 streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 09:46:11.000000 streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-04-25 09:46:11.000000 streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2023-04-25 09:46:11.000000 streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/LICENSE` & `streamlit-component-dropfilltextarea-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.2.2/PKG-INFO` & `streamlit-component-dropfilltextarea-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-component-dropfilltextarea
-Version: 0.2.2
+Version: 0.2.3
 Summary: Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.
 Author: Jiayi Chen
 Author-email: chenjiayi_344@hotmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/README.md` & `streamlit-component-dropfilltextarea-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.2.2/setup.py` & `streamlit-component-dropfilltextarea-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-component-dropfilltextarea",
-    version="0.2.2",
+    version="0.2.3",
     author="Jiayi Chen",
     author_email="chenjiayi_344@hotmail.com",
     description="Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/__init__.py` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/css/app.153d1a1e.css` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/css/app.58e9fcbb.css`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-.container[data-v-61db93e8]{display:flex;flex-direction:var(--flex-direction);align-items:var(--align-items);height:var(--container-height)}.label[data-v-61db93e8]{margin-right:var(--margin-right);font:var(--font);white-space:pre}.textarea-container[data-v-61db93e8]{width:100%;display:flex;justify-content:center}textarea[data-v-61db93e8]{width:100%;height:var(--textarea-height);resize:none;padding:16px;border:none;border-radius:6px;color:var(--text-color);background-color:var(--background-color);font:var(--font);scrollbar-width:none;overflow:hidden}textarea[data-v-61db93e8]:focus{outline:1px solid red}textarea[data-v-61db93e8]:hover{scrollbar-width:auto;overflow:auto}textarea[data-v-61db93e8]::-webkit-scrollbar{width:6px;height:6px}textarea[data-v-61db93e8]::-webkit-scrollbar-thumb{border-radius:100px;background-color:rgba(143,141,141,.8)}textarea[data-v-61db93e8]::-webkit-scrollbar-track{border-radius:100px}.err__msg[data-v-bef81972],.err__title[data-v-bef81972]{margin:0}body{margin:0}#app{font-family:Avenir,Helvetica,Arial,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;color:#2c3e50}
+.container[data-v-21265b35]{display:flex;flex-direction:var(--flex-direction);align-items:var(--align-items);height:var(--container-height)}.label[data-v-21265b35]{margin-right:var(--margin-right);font:var(--font);white-space:pre}.textarea-container[data-v-21265b35]{width:100%;display:flex;justify-content:center}textarea[data-v-21265b35]{width:100%;height:var(--textarea-height);resize:none;padding:16px;border:none;border-radius:6px;color:var(--text-color);background-color:var(--background-color);font:var(--font);scrollbar-width:none;overflow:auto}textarea[data-v-21265b35]:focus{outline:1px solid red}textarea[data-v-21265b35]:hover{scrollbar-width:auto}textarea[data-v-21265b35]:not(:hover)::-webkit-scrollbar{background-color:transparent}textarea[data-v-21265b35]:not(:hover)::-webkit-scrollbar-thumb{background-color:transparent}textarea[data-v-21265b35]::-webkit-scrollbar{width:6px;height:6px}textarea[data-v-21265b35]::-webkit-scrollbar-thumb{border-radius:100px;background-color:rgba(143,141,141,.8)}textarea[data-v-21265b35]::-webkit-scrollbar-track{border-radius:100px}.err__msg[data-v-bef81972],.err__title[data-v-bef81972]{margin:0}body{margin:0}#app{font-family:Avenir,Helvetica,Arial,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;color:#2c3e50}
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/index.html` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/index.html`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><title>streamlit_component_template</title><link href=css/app.153d1a1e.css rel=preload as=style><link href=js/app.fd804a62.js rel=preload as=script><link href=js/chunk-vendors.e7772cca.js rel=preload as=script><link href=css/app.153d1a1e.css rel=stylesheet></head><body><noscript><strong>We're sorry but streamlit_component_template doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id=app></div><script src=js/chunk-vendors.e7772cca.js></script><script src=js/app.fd804a62.js></script></body></html>
+<!DOCTYPE html><html lang=en><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><title>streamlit_component_template</title><link href=css/app.58e9fcbb.css rel=preload as=style><link href=js/app.7306c276.js rel=preload as=script><link href=js/chunk-vendors.e7772cca.js rel=preload as=script><link href=css/app.58e9fcbb.css rel=stylesheet></head><body><noscript><strong>We're sorry but streamlit_component_template doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id=app></div><script src=js/chunk-vendors.e7772cca.js></script><script src=js/app.7306c276.js></script></body></html>
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/app.7306c276.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -72,30 +72,29 @@
     var s = l;
     o.push([0, "chunk-vendors"]), n()
 })({
     0: function(e, t, n) {
         e.exports = n("cd49")
     },
     1: function(e, t) {},
+    "16df": function(e, t, n) {
+        "use strict";
+        n("e29d")
+    },
     "1eca": function(e, t, n) {},
     2: function(e, t) {},
     "44dc": function(e, t, n) {
         "use strict";
         n("1eca")
     },
     "4b1c": function(e, t, n) {
         "use strict";
         n("5084")
     },
     5084: function(e, t, n) {},
-    "96e9": function(e, t, n) {
-        "use strict";
-        n("b380")
-    },
-    b380: function(e, t, n) {},
     cd49: function(e, t, n) {
         "use strict";
         n.r(t);
         n("e260"), n("e6cf"), n("cca6"), n("a79d");
         var r = n("830f"),
             a = n("5c40"),
             o = {
@@ -112,16 +111,16 @@
                         args: t
                     }, null, 8, ["args"])]
                 })),
                 _: 1
             })])
         }
         var c = n("9ff4"),
-            l = Object(a["C"])("data-v-61db93e8");
-        Object(a["s"])("data-v-61db93e8");
+            l = Object(a["C"])("data-v-21265b35");
+        Object(a["s"])("data-v-21265b35");
         var u = {
             class: "textarea-container",
             ref: "textarea-container"
         };
         Object(a["r"])();
         var s = l((function(e, t, n, o, i, l) {
                 return Object(a["q"])(), Object(a["d"])("div", {
@@ -170,16 +169,16 @@
          *
          * Unless required by applicable law or agreed to in writing, software
          * distributed under the License is distributed on an "AS IS" BASIS,
          * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
          * See the License for the specific language governing permissions and
          * limitations under the License.
          */
-        var b = n("c343"),
-            v = {
+        var v = n("c343"),
+            b = {
                 name: "DropfillTextarea",
                 props: {
                     args: Object
                 },
                 setup: function() {
                     p()
                 },
@@ -284,15 +283,15 @@
                         var u = o.join("\n");
                         u = u.replace(/(\r\n|\r|\n){2,}/g, "$1\n"), this.updateValue(u)
                     },
                     handleDocx: function(e) {
                         var t = this,
                             n = new FileReader;
                         n.onload = function() {
-                            Object(b["convertToHtml"])({
+                            Object(v["convertToHtml"])({
                                 arrayBuffer: n.result
                             }).then((function(e) {
                                 t.convertToJson(e.value)
                             }))
                         }, n.readAsArrayBuffer(e)
                     },
                     handleHtml: function(e) {
@@ -322,17 +321,17 @@
                         e.preventDefault(), e.stopPropagation();
                         var t = e.dataTransfer.files[0],
                             n = this.fileHandler(t);
                         void 0 !== n ? n(t) : this.updateValue("Dropped file type not supported")
                     }
                 }
             };
-        n("96e9");
-        v.render = s, v.__scopeId = "data-v-61db93e8";
-        var g = v,
+        n("16df");
+        b.render = s, b.__scopeId = "data-v-21265b35";
+        var g = b,
             O = Object(a["C"])("data-v-bef81972");
         Object(a["s"])("data-v-bef81972");
         var j = {
                 key: 0
             },
             m = Object(a["h"])("h1", {
                 class: "err__title"
@@ -381,10 +380,11 @@
                     WithStreamlitConnection: w
                 }
             });
         n("4b1c");
         D.render = i;
         var _ = D;
         Object(r["a"])(_).mount("#app")
-    }
+    },
+    e29d: function(e, t, n) {}
 });
-//# sourceMappingURL=app.fd804a62.js.map
+//# sourceMappingURL=app.7306c276.js.map
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js.map` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/app.7306c276.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8224089635854341%*

 * *Differences: {"'file'": "'js/app.7306c276.js'",*

 * * "'mappings'": "'aACE,SAASA,EAAqBC,GAQ7B,IAPA,IAMIC,EAAUC,EANVC,EAAWH,EAAK,GAChBI,EAAcJ,EAAK,GACnBK,EAAiBL,EAAK,GAIHM,EAAI,EAAGC,EAAW,GACpCD,EAAIH,EAASK,OAAQF,IACzBJ,EAAUC,EAASG,GAChBG,OAAOC,UAAUC,eAAeC,KAAKC,EAAiBX,IAAYW,EAAgBX,IACpFK,EAASO,KAAKD,EAAgBX,GAAS,IAExCW,EAAgBX,GAAW,EAE5B,IAAID,KAAYG,EACZK,OAAOC,UAAUC,eAAeC,KAAKR,EAAaH,KACpDc,EAAQd,GAAYG,EAAYH,IAG/Be,GAAqBA,EAAoBhB,GAE5C,MAAMO,EAASC,OACdD,EAASU,OAATV,GAOD,OAHAW,EAAgBJ,KAAKK,MAAMD,EAAiBb,GAAkB,IAGvDe,IAER,SAASA, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "js/app.fd804a62.js",
-    "mappings": "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",
+    "file": "js/app.7306c276.js",
+    "mappings": "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",
     "names": [
         "webpackJsonpCallback",
         "data",
         "moduleId",
         "chunkId",
         "chunkIds",
         "moreModules",
@@ -164,37 +164,37 @@
         "WithStreamlitConnection",
         "App",
         "mount"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///webpack/bootstrap",
+        "webpack:///./src/DropfillTextarea.vue?996a",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?196c",
         "webpack:///./src/App.vue?3a46",
-        "webpack:///./src/DropfillTextarea.vue?4bbd",
         "webpack:///./src/App.vue",
         "webpack:///./src/DropfillTextarea.vue",
         "webpack:///./src/streamlit/StreamlitVue.ts",
         "webpack:///./src/DropfillTextarea.vue?8ae3",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?69f8",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?07d5",
         "webpack:///./src/App.vue?1d14",
         "webpack:///./src/App.vue?97f5",
         "webpack:///./src/main.ts"
     ],
     "sourcesContent": [
         " \t// install a JSONP callback for chunk loading\n \tfunction webpackJsonpCallback(data) {\n \t\tvar chunkIds = data[0];\n \t\tvar moreModules = data[1];\n \t\tvar executeModules = data[2];\n\n \t\t// add \"moreModules\" to the modules object,\n \t\t// then flag all \"chunkIds\" as loaded and fire callback\n \t\tvar moduleId, chunkId, i = 0, resolves = [];\n \t\tfor(;i < chunkIds.length; i++) {\n \t\t\tchunkId = chunkIds[i];\n \t\t\tif(Object.prototype.hasOwnProperty.call(installedChunks, chunkId) && installedChunks[chunkId]) {\n \t\t\t\tresolves.push(installedChunks[chunkId][0]);\n \t\t\t}\n \t\t\tinstalledChunks[chunkId] = 0;\n \t\t}\n \t\tfor(moduleId in moreModules) {\n \t\t\tif(Object.prototype.hasOwnProperty.call(moreModules, moduleId)) {\n \t\t\t\tmodules[moduleId] = moreModules[moduleId];\n \t\t\t}\n \t\t}\n \t\tif(parentJsonpFunction) parentJsonpFunction(data);\n\n \t\twhile(resolves.length) {\n \t\t\tresolves.shift()();\n \t\t}\n\n \t\t// add entry modules from loaded chunk to deferred list\n \t\tdeferredModules.push.apply(deferredModules, executeModules || []);\n\n \t\t// run deferred modules when all chunks ready\n \t\treturn checkDeferredModules();\n \t};\n \tfunction checkDeferredModules() {\n \t\tvar result;\n \t\tfor(var i = 0; i < deferredModules.length; i++) {\n \t\t\tvar deferredModule = deferredModules[i];\n \t\t\tvar fulfilled = true;\n \t\t\tfor(var j = 1; j < deferredModule.length; j++) {\n \t\t\t\tvar depId = deferredModule[j];\n \t\t\t\tif(installedChunks[depId] !== 0) fulfilled = false;\n \t\t\t}\n \t\t\tif(fulfilled) {\n \t\t\t\tdeferredModules.splice(i--, 1);\n \t\t\t\tresult = __webpack_require__(__webpack_require__.s = deferredModule[0]);\n \t\t\t}\n \t\t}\n\n \t\treturn result;\n \t}\n\n \t// The module cache\n \tvar installedModules = {};\n\n \t// object to store loaded and loading chunks\n \t// undefined = chunk not loaded, null = chunk preloaded/prefetched\n \t// Promise = chunk loading, 0 = chunk loaded\n \tvar installedChunks = {\n \t\t\"app\": 0\n \t};\n\n \tvar deferredModules = [];\n\n \t// The require function\n \tfunction __webpack_require__(moduleId) {\n\n \t\t// Check if module is in cache\n \t\tif(installedModules[moduleId]) {\n \t\t\treturn installedModules[moduleId].exports;\n \t\t}\n \t\t// Create a new module (and put it into the cache)\n \t\tvar module = installedModules[moduleId] = {\n \t\t\ti: moduleId,\n \t\t\tl: false,\n \t\t\texports: {}\n \t\t};\n\n \t\t// Execute the module function\n \t\tmodules[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n \t\t// Flag the module as loaded\n \t\tmodule.l = true;\n\n \t\t// Return the exports of the module\n \t\treturn module.exports;\n \t}\n\n\n \t// expose the modules object (__webpack_modules__)\n \t__webpack_require__.m = modules;\n\n \t// expose the module cache\n \t__webpack_require__.c = installedModules;\n\n \t// define getter function for harmony exports\n \t__webpack_require__.d = function(exports, name, getter) {\n \t\tif(!__webpack_require__.o(exports, name)) {\n \t\t\tObject.defineProperty(exports, name, { enumerable: true, get: getter });\n \t\t}\n \t};\n\n \t// define __esModule on exports\n \t__webpack_require__.r = function(exports) {\n \t\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n \t\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n \t\t}\n \t\tObject.defineProperty(exports, '__esModule', { value: true });\n \t};\n\n \t// create a fake namespace object\n \t// mode & 1: value is a module id, require it\n \t// mode & 2: merge all properties of value into the ns\n \t// mode & 4: return value when already ns object\n \t// mode & 8|1: behave like require\n \t__webpack_require__.t = function(value, mode) {\n \t\tif(mode & 1) value = __webpack_require__(value);\n \t\tif(mode & 8) return value;\n \t\tif((mode & 4) && typeof value === 'object' && value && value.__esModule) return value;\n \t\tvar ns = Object.create(null);\n \t\t__webpack_require__.r(ns);\n \t\tObject.defineProperty(ns, 'default', { enumerable: true, value: value });\n \t\tif(mode & 2 && typeof value != 'string') for(var key in value) __webpack_require__.d(ns, key, function(key) { return value[key]; }.bind(null, key));\n \t\treturn ns;\n \t};\n\n \t// getDefaultExport function for compatibility with non-harmony modules\n \t__webpack_require__.n = function(module) {\n \t\tvar getter = module && module.__esModule ?\n \t\t\tfunction getDefault() { return module['default']; } :\n \t\t\tfunction getModuleExports() { return module; };\n \t\t__webpack_require__.d(getter, 'a', getter);\n \t\treturn getter;\n \t};\n\n \t// Object.prototype.hasOwnProperty.call\n \t__webpack_require__.o = function(object, property) { return Object.prototype.hasOwnProperty.call(object, property); };\n\n \t// __webpack_public_path__\n \t__webpack_require__.p = \"\";\n\n \tvar jsonpArray = window[\"webpackJsonp\"] = window[\"webpackJsonp\"] || [];\n \tvar oldJsonpFunction = jsonpArray.push.bind(jsonpArray);\n \tjsonpArray.push = webpackJsonpCallback;\n \tjsonpArray = jsonpArray.slice();\n \tfor(var i = 0; i < jsonpArray.length; i++) webpackJsonpCallback(jsonpArray[i]);\n \tvar parentJsonpFunction = oldJsonpFunction;\n\n\n \t// add entry module to deferred list\n \tdeferredModules.push([0,\"chunk-vendors\"]);\n \t// run deferred modules when ready\n \treturn checkDeferredModules();\n",
+        "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--0-0!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./DropfillTextarea.vue?vue&type=style&index=0&id=21265b35&scoped=true&lang=css\"",
         "export * from \"-!../../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../../node_modules/cache-loader/dist/cjs.js??ref--0-0!../../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"",
         "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--0-0!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./App.vue?vue&type=style&index=0&id=9d77823c&lang=css\"",
-        "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--6-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--6-oneOf-1-1!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--6-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--0-0!../node_modules/@vue/cli-service/node_modules/vue-loader-v16/dist/index.js??ref--0-1!./DropfillTextarea.vue?vue&type=style&index=0&id=61db93e8&scoped=true&lang=css\"",
         "<!-- \n  We bootstrap our Component to Streamlit with our scoped slot in the top-level App.\n  This is where scoped slot passes Streamlit `args` data from itself to children MyComponent.\n  You should not have to edit this, but are free to do so :)\n-->\n<template>\n  <div id=\"app\">\n    <WithStreamlitConnection v-slot=\"{ args }\">\n      <DropfillTextarea :args=\"args\" />\n    </WithStreamlitConnection>\n  </div>\n</template>\n\n<script lang=\"ts\">\nimport { defineComponent } from \"vue\"\nimport DropfillTextarea from \"./DropfillTextarea.vue\"\n\n// \"withStreamlitConnection\" is a scoped slot. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nimport WithStreamlitConnection from \"./streamlit/WithStreamlitConnection.vue\"\n\nexport default defineComponent({\n  name: \"App\",\n  components: {\n    DropfillTextarea,\n    WithStreamlitConnection,\n  },\n})\n</script>\n\n<style>\nbody {\n  margin: 0;\n}\n#app {\n  font-family: Avenir, Helvetica, Arial, sans-serif;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n  color: #2c3e50;\n}\n</style>\n",
-        "<template>\n  <div class=\"container\" :style=\"cssProps\" ref=\"container\">\n    <div class=\"label\" ref=\"label\">\n      {{ label }}\n    </div>\n    <div class=\"textarea-container\" ref=\"textarea-container\">\n      <textarea\n        ref=\"textarea\"\n        v-model=\"value\"\n        :placeholder=\"args.placeholder\"\n        @change=\"handlesChange\"\n        @drop=\"handleDrop\"\n      />\n    </div>\n  </div>\n</template>\n\n<script>\n  import { ref } from \"vue\";\n  import { Streamlit } from \"streamlit-component-lib\";\n  import { useStreamlit } from \"./streamlit\";\n  import { convertToHtml } from \"mammoth\";\n\n  export default {\n    name: \"DropfillTextarea\",\n    props: {\n      args: Object,\n    }, // Arguments that are passed to the plugin in Python are accessible in prop \"args\"\n    setup() {\n      useStreamlit(); // lifecycle hooks for automatic Streamlit resize\n    },\n\n    data() {\n      const value = ref(\"\");\n      return {\n        value,\n      };\n    },\n\n    mounted() {\n      this.value = ref(this.args.value);\n      this.rerender();\n    },\n\n    computed: {\n      label() {\n        return this.args.label;\n      },\n      cssProps() {\n        const propObj = {\n          \"--flex-direction\": \"column\",\n          \"--margin-right\": \"0px\",\n          \"--container-height\": this.args.height * 1.15 + \"px\",\n          \"--textarea-height\": this.args.height + \"px\",\n          \"--align-items\": \"left\",\n          \"--background-color\": \"#f0f2f6\",\n        };\n        if (this.args.layout !== \"column\") {\n          propObj[\"--flex-direction\"] = \"row\";\n          propObj[\"--margin-right\"] = \"4px\";\n          propObj[\"--align-items\"] = \"center\";\n        }\n        return propObj;\n      },\n    },\n\n    methods: {\n      renderColumn() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const height = labelRef.clientHeight + textareaRef.clientHeight;\n          const width = containerRef.clientWidth - 16 * 2 - 4;\n          containerRef.style.height = height + \"px\";\n          textareaRef.style.width = width + \"px\";\n          textareaRef.style.height = this.args.height - 16 + \"px\";\n        }, 100);\n      },\n      renderRow() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaContainerRef = this.$refs[\"textarea-container\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const labelWidth = this.args.labelWidth;\n          let width;\n          if (labelWidth !== null) {\n            labelRef.style.width = labelWidth + \"px\";\n            width = containerRef.clientWidth - labelWidth - 16 * 2 - 8;\n          } else {\n            width =\n              containerRef.clientWidth - labelRef.clientWidth - 16 * 2 - 8;\n          }\n          const height = textareaContainerRef.clientHeight;\n\n          containerRef.style.height = height + \"px\";\n          textareaContainerRef.style.width = width + \"px\";\n          textareaContainerRef.style.height = this.args.height + \"px\";\n          textareaRef.style.height = this.args.height - 16 * 2 + \"px\";\n        }, 100);\n      },\n\n      rerender() {\n        if (this.args.layout === \"column\") {\n          this.renderColumn();\n        } else {\n          this.renderRow();\n        }\n      },\n      handlesChange() {\n        Streamlit.setComponentValue(this.value);\n      },\n\n      updateValue(newValue) {\n        this.value = newValue;\n        this.handlesChange();\n      },\n\n      getTextFromNode(node) {\n        let text = \"\";\n        if (node.nodeType === Node.TEXT_NODE) {\n          text += node.textContent.trim();\n        } else {\n          let children = [];\n          for (const child of node.childNodes) {\n            children.push(this.getTextFromNode(child));\n          }\n          children = children.filter((child) => child.length > 0);\n          text += children.join(\"\") + \"\\n\";\n        }\n        return text;\n      },\n\n      convertToJson(html) {\n        const parser = new DOMParser();\n        const dom = parser.parseFromString(html, \"text/html\");\n        const body = dom.getElementsByTagName(\"body\")[0];\n        const content = [];\n        for (const node of body.childNodes) {\n          const text = this.getTextFromNode(node);\n          content.push(text);\n        }\n        let text = content.join(\"\\n\");\n        text = text.replace(/(\\r\\n|\\r|\\n){2,}/g, \"$1\\n\");\n        this.updateValue(text);\n      },\n\n      handleDocx(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          convertToHtml({ arrayBuffer: reader.result }).then((result) => {\n            this.convertToJson(result.value);\n          });\n        };\n\n        reader.readAsArrayBuffer(file);\n      },\n\n      handleHtml(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.convertToJson(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      handlPlainText(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.updateValue(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      fileHandler(file) {\n        const files = {\n          \"application/vnd.openxmlformats-officedocument.wordprocessingml.document\": this\n            .handleDocx,\n          \"text/html\": this.handleHtml,\n          \"text/plain\": this.handlPlainText,\n          \"application/json\": this.handlPlainText,\n        };\n        return files[file.type];\n      },\n\n      handleDrop(event) {\n        event.preventDefault();\n        event.stopPropagation(); // stops the browser from redirecting.\n        const file = event.dataTransfer.files[0];\n        const handle = this.fileHandler(file);\n        if (handle !== undefined) handle(file);\n        else this.updateValue(\"Dropped file type not supported\");\n      },\n    },\n  };\n</script>\n\n<style scoped>\n  .container {\n    display: flex;\n    flex-direction: var(--flex-direction);\n    align-items: var(--align-items);\n    height: var(--container-height);\n  }\n  .label {\n    margin-right: var(--margin-right);\n    font: var(--font);\n    white-space: pre;\n  }\n\n  .textarea-container {\n    width: 100%;\n    display: flex;\n    justify-content: center;\n  }\n  textarea {\n    width: 100%;\n    height: var(--textarea-height);\n    resize: none;\n    padding: 16px;\n    border: none;\n    border-radius: 6px;\n    color: var(--text-color);\n    background-color: var(--background-color);\n    font: var(--font);\n    scrollbar-width: none; /* hide the scrollbar when out of focus */\n    overflow: hidden; /* hide the overflow when out of focus */\n  }\n  textarea:focus {\n    outline: 1px solid red;\n  }\n\n  textarea:hover {\n    scrollbar-width: auto; /* show the scrollbar when in focus */\n    overflow: auto; /* show the overflow when in focus */\n  }\n\n  textarea::-webkit-scrollbar {\n    width: 6px;\n    height: 6px;\n  }\n\n  textarea::-webkit-scrollbar-thumb {\n    border-radius: 100px;\n    background-color: rgba(143, 141, 141, 0.8);\n  }\n\n  textarea::-webkit-scrollbar-track {\n    border-radius: 100px;\n  }\n</style>\n",
+        "<template>\n  <div class=\"container\" :style=\"cssProps\" ref=\"container\">\n    <div class=\"label\" ref=\"label\">\n      {{ label }}\n    </div>\n    <div class=\"textarea-container\" ref=\"textarea-container\">\n      <textarea\n        ref=\"textarea\"\n        v-model=\"value\"\n        :placeholder=\"args.placeholder\"\n        @change=\"handlesChange\"\n        @drop=\"handleDrop\"\n      />\n    </div>\n  </div>\n</template>\n\n<script>\n  import { ref } from \"vue\";\n  import { Streamlit } from \"streamlit-component-lib\";\n  import { useStreamlit } from \"./streamlit\";\n  import { convertToHtml } from \"mammoth\";\n\n  export default {\n    name: \"DropfillTextarea\",\n    props: {\n      args: Object,\n    }, // Arguments that are passed to the plugin in Python are accessible in prop \"args\"\n    setup() {\n      useStreamlit(); // lifecycle hooks for automatic Streamlit resize\n    },\n\n    data() {\n      const value = ref(\"\");\n      return {\n        value,\n      };\n    },\n\n    mounted() {\n      this.value = ref(this.args.value);\n      this.rerender();\n    },\n\n    computed: {\n      label() {\n        return this.args.label;\n      },\n      cssProps() {\n        const propObj = {\n          \"--flex-direction\": \"column\",\n          \"--margin-right\": \"0px\",\n          \"--container-height\": this.args.height * 1.15 + \"px\",\n          \"--textarea-height\": this.args.height + \"px\",\n          \"--align-items\": \"left\",\n          \"--background-color\": \"#f0f2f6\",\n        };\n        if (this.args.layout !== \"column\") {\n          propObj[\"--flex-direction\"] = \"row\";\n          propObj[\"--margin-right\"] = \"4px\";\n          propObj[\"--align-items\"] = \"center\";\n        }\n        return propObj;\n      },\n    },\n\n    methods: {\n      renderColumn() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const height = labelRef.clientHeight + textareaRef.clientHeight;\n          const width = containerRef.clientWidth - 16 * 2 - 4;\n          containerRef.style.height = height + \"px\";\n          textareaRef.style.width = width + \"px\";\n          textareaRef.style.height = this.args.height - 16 + \"px\";\n        }, 100);\n      },\n      renderRow() {\n        setTimeout(() => {\n          const containerRef = this.$refs[\"container\"];\n          const labelRef = this.$refs[\"label\"];\n          const textareaContainerRef = this.$refs[\"textarea-container\"];\n          const textareaRef = this.$refs[\"textarea\"];\n          const labelWidth = this.args.labelWidth;\n          let width;\n          if (labelWidth !== null) {\n            labelRef.style.width = labelWidth + \"px\";\n            width = containerRef.clientWidth - labelWidth - 16 * 2 - 8;\n          } else {\n            width =\n              containerRef.clientWidth - labelRef.clientWidth - 16 * 2 - 8;\n          }\n          const height = textareaContainerRef.clientHeight;\n\n          containerRef.style.height = height + \"px\";\n          textareaContainerRef.style.width = width + \"px\";\n          textareaContainerRef.style.height = this.args.height + \"px\";\n          textareaRef.style.height = this.args.height - 16 * 2 + \"px\";\n        }, 100);\n      },\n\n      rerender() {\n        if (this.args.layout === \"column\") {\n          this.renderColumn();\n        } else {\n          this.renderRow();\n        }\n      },\n      handlesChange() {\n        Streamlit.setComponentValue(this.value);\n      },\n\n      updateValue(newValue) {\n        this.value = newValue;\n        this.handlesChange();\n      },\n\n      getTextFromNode(node) {\n        let text = \"\";\n        if (node.nodeType === Node.TEXT_NODE) {\n          text += node.textContent.trim();\n        } else {\n          let children = [];\n          for (const child of node.childNodes) {\n            children.push(this.getTextFromNode(child));\n          }\n          children = children.filter((child) => child.length > 0);\n          text += children.join(\"\") + \"\\n\";\n        }\n        return text;\n      },\n\n      convertToJson(html) {\n        const parser = new DOMParser();\n        const dom = parser.parseFromString(html, \"text/html\");\n        const body = dom.getElementsByTagName(\"body\")[0];\n        const content = [];\n        for (const node of body.childNodes) {\n          const text = this.getTextFromNode(node);\n          content.push(text);\n        }\n        let text = content.join(\"\\n\");\n        text = text.replace(/(\\r\\n|\\r|\\n){2,}/g, \"$1\\n\");\n        this.updateValue(text);\n      },\n\n      handleDocx(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          convertToHtml({ arrayBuffer: reader.result }).then((result) => {\n            this.convertToJson(result.value);\n          });\n        };\n\n        reader.readAsArrayBuffer(file);\n      },\n\n      handleHtml(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.convertToJson(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      handlPlainText(file) {\n        const reader = new FileReader();\n        reader.onload = () => {\n          this.updateValue(reader.result);\n        };\n\n        reader.readAsText(file);\n      },\n\n      fileHandler(file) {\n        const files = {\n          \"application/vnd.openxmlformats-officedocument.wordprocessingml.document\": this\n            .handleDocx,\n          \"text/html\": this.handleHtml,\n          \"text/plain\": this.handlPlainText,\n          \"application/json\": this.handlPlainText,\n        };\n        return files[file.type];\n      },\n\n      handleDrop(event) {\n        event.preventDefault();\n        event.stopPropagation(); // stops the browser from redirecting.\n        const file = event.dataTransfer.files[0];\n        const handle = this.fileHandler(file);\n        if (handle !== undefined) handle(file);\n        else this.updateValue(\"Dropped file type not supported\");\n      },\n    },\n  };\n</script>\n\n<style scoped>\n  .container {\n    display: flex;\n    flex-direction: var(--flex-direction);\n    align-items: var(--align-items);\n    height: var(--container-height);\n  }\n  .label {\n    margin-right: var(--margin-right);\n    font: var(--font);\n    white-space: pre;\n  }\n\n  .textarea-container {\n    width: 100%;\n    display: flex;\n    justify-content: center;\n  }\n  textarea {\n    width: 100%;\n    height: var(--textarea-height);\n    resize: none;\n    padding: 16px;\n    border: none;\n    border-radius: 6px;\n    color: var(--text-color);\n    background-color: var(--background-color);\n    font: var(--font);\n    scrollbar-width: none; /* hide the scrollbar when out of focus */\n    overflow: auto; /* hide the overflow when out of focus */\n  }\n  textarea:focus {\n    outline: 1px solid red;\n  }\n\n  textarea:hover {\n    scrollbar-width: auto; /* show the scrollbar when in focus */\n  }\n\n  textarea:not(:hover)::-webkit-scrollbar {\n    background-color: transparent;\n  }\n\n  textarea:not(:hover)::-webkit-scrollbar-thumb {\n    background-color: transparent;\n  }\n\n  textarea::-webkit-scrollbar {\n    width: 6px;\n    height: 6px;\n  }\n\n  textarea::-webkit-scrollbar-thumb {\n    border-radius: 100px;\n    background-color: rgba(143, 141, 141, 0.8);\n  }\n\n  textarea::-webkit-scrollbar-track {\n    border-radius: 100px;\n  }\n</style>\n",
         "/**\n * Vue.js specific composables\n */\nimport { onMounted, onUpdated } from \"vue\"\nimport { Streamlit } from \"streamlit-component-lib\"\n\nexport function useStreamlit() {\n  /**\n   * Optional Streamlit Vue-based setup.\n   *\n   * You are not required call this function on your Streamlit\n   * component. If you decide not to call it, you should implement the\n   * `onMounted` and `onUpdated` functions in your own component,\n   * so that your plugin properly resizes.\n   */\n\n  onMounted((): void => {\n    // After we're rendered for the first time, tell Streamlit that our height\n    // has changed.\n    Streamlit.setFrameHeight()\n  })\n\n  onUpdated((): void => {\n    // After we're updated, tell Streamlit that our height may have changed.\n    Streamlit.setFrameHeight()\n  })\n}\n",
-        "import { render } from \"./DropfillTextarea.vue?vue&type=template&id=61db93e8&scoped=true\"\nimport script from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\nexport * from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\n\nimport \"./DropfillTextarea.vue?vue&type=style&index=0&id=61db93e8&scoped=true&lang=css\"\nscript.render = render\nscript.__scopeId = \"data-v-61db93e8\"\n\nexport default script",
+        "import { render } from \"./DropfillTextarea.vue?vue&type=template&id=21265b35&scoped=true\"\nimport script from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\nexport * from \"./DropfillTextarea.vue?vue&type=script&lang=js\"\n\nimport \"./DropfillTextarea.vue?vue&type=style&index=0&id=21265b35&scoped=true&lang=css\"\nscript.render = render\nscript.__scopeId = \"data-v-21265b35\"\n\nexport default script",
         "<template>\n  <div>\n    <!--  Error boundary. If our wrapped component threw an error, display it. -->\n    <div v-if=\"componentError != ''\">\n      <h1 class=\"err__title\">Component Error</h1>\n      <div class=\"err__msg\">Message: {{ componentError }}</div>\n    </div>\n    <!-- \n      Else render the component slot and pass Streamlit event data in `args` props to it.\n      Don't render until we've gotten our first RENDER_EVENT from Streamlit.\n      All components get disabled while the app is being re-run, and become re-enabled when the re-run has finished.\n    -->\n    <slot\n      v-else-if=\"renderData != null\"\n      :args=\"renderData.args\"\n      :disabled=\"renderData.disabled\"\n    ></slot>\n  </div>\n</template>\n\n<script lang=\"ts\">\nimport {\n  ref,\n  defineComponent,\n  onMounted,\n  onUpdated,\n  onUnmounted,\n  onErrorCaptured,\n} from \"vue\"\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nexport default defineComponent({\n  name: \"WithStreamlitConnection\",\n  setup() {\n    const renderData = ref<RenderData>((undefined as unknown) as RenderData)\n    const componentError = ref(\"\")\n\n    const onRenderEvent = (event: Event): void => {\n      const renderEvent = event as CustomEvent<RenderData>\n      renderData.value = renderEvent.detail\n      componentError.value = \"\"\n    }\n\n    // Set up event listeners, and signal to Streamlit that we're ready.\n    // We won't render the component until we receive the first RENDER_EVENT.\n    onMounted(() => {\n      Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRenderEvent)\n      Streamlit.setComponentReady()\n    })\n    onUpdated(() => {\n      // If our slot threw an error, we display it in render(). In this\n      // case, the slot won't be mounted and therefore won't call\n      // `setFrameHeight` on its own. We do it here so that the rendered\n      // error will be visible.\n      if (componentError.value != \"\") {\n        Streamlit.setFrameHeight()\n      }\n    })\n    onUnmounted(() => {\n      Streamlit.events.removeEventListener(\n        Streamlit.RENDER_EVENT,\n        onRenderEvent\n      )\n    })\n    onErrorCaptured(err => {\n      componentError.value = String(err)\n    })\n\n    return {\n      renderData,\n      componentError,\n    }\n  },\n})\n</script>\n\n<style scoped>\n.err__title,\n.err__msg {\n  margin: 0;\n}\n</style>\n",
         "\nimport {\n  ref,\n  defineComponent,\n  onMounted,\n  onUpdated,\n  onUnmounted,\n  onErrorCaptured,\n} from \"vue\"\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nexport default defineComponent({\n  name: \"WithStreamlitConnection\",\n  setup() {\n    const renderData = ref<RenderData>((undefined as unknown) as RenderData)\n    const componentError = ref(\"\")\n\n    const onRenderEvent = (event: Event): void => {\n      const renderEvent = event as CustomEvent<RenderData>\n      renderData.value = renderEvent.detail\n      componentError.value = \"\"\n    }\n\n    // Set up event listeners, and signal to Streamlit that we're ready.\n    // We won't render the component until we receive the first RENDER_EVENT.\n    onMounted(() => {\n      Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRenderEvent)\n      Streamlit.setComponentReady()\n    })\n    onUpdated(() => {\n      // If our slot threw an error, we display it in render(). In this\n      // case, the slot won't be mounted and therefore won't call\n      // `setFrameHeight` on its own. We do it here so that the rendered\n      // error will be visible.\n      if (componentError.value != \"\") {\n        Streamlit.setFrameHeight()\n      }\n    })\n    onUnmounted(() => {\n      Streamlit.events.removeEventListener(\n        Streamlit.RENDER_EVENT,\n        onRenderEvent\n      )\n    })\n    onErrorCaptured(err => {\n      componentError.value = String(err)\n    })\n\n    return {\n      renderData,\n      componentError,\n    }\n  },\n})\n",
         "import { render } from \"./WithStreamlitConnection.vue?vue&type=template&id=bef81972&scoped=true\"\nimport script from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\nexport * from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\n\nimport \"./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"\nscript.render = render\nscript.__scopeId = \"data-v-bef81972\"\n\nexport default script",
         "\nimport { defineComponent } from \"vue\"\nimport DropfillTextarea from \"./DropfillTextarea.vue\"\n\n// \"withStreamlitConnection\" is a scoped slot. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nimport WithStreamlitConnection from \"./streamlit/WithStreamlitConnection.vue\"\n\nexport default defineComponent({\n  name: \"App\",\n  components: {\n    DropfillTextarea,\n    WithStreamlitConnection,\n  },\n})\n",
         "import { render } from \"./App.vue?vue&type=template&id=9d77823c\"\nimport script from \"./App.vue?vue&type=script&lang=ts\"\nexport * from \"./App.vue?vue&type=script&lang=ts\"\n\nimport \"./App.vue?vue&type=style&index=0&id=9d77823c&lang=css\"\nscript.render = render\n\nexport default script",
         "import { createApp } from 'vue'\nimport App from './App.vue'\n\ncreateApp(App).mount('#app')\n"
     ],
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map` & `streamlit-component-dropfilltextarea-0.2.3/src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO` & `streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-component-dropfilltextarea
-Version: 0.2.2
+Version: 0.2.3
 Summary: Streamlit's DropFillTextarea lets users drag and drop files onto a text area, filling in text quickly. It populates text areas with pre-existing files, reducing manual input, while offering layout customization. Ideal for simplifying workflows for both developers and users.
 Author: Jiayi Chen
 Author-email: chenjiayi_344@hotmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-component-dropfilltextarea-0.2.2/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt` & `streamlit-component-dropfilltextarea-0.2.3/src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/st_dropfill_textarea/__init__.py
 src/st_dropfill_textarea/frontend/dist/index.html
-src/st_dropfill_textarea/frontend/dist/css/app.153d1a1e.css
-src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js
-src/st_dropfill_textarea/frontend/dist/js/app.fd804a62.js.map
+src/st_dropfill_textarea/frontend/dist/css/app.58e9fcbb.css
+src/st_dropfill_textarea/frontend/dist/js/app.7306c276.js
+src/st_dropfill_textarea/frontend/dist/js/app.7306c276.js.map
 src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js
 src/st_dropfill_textarea/frontend/dist/js/chunk-vendors.e7772cca.js.map
 src/streamlit_component_dropfilltextarea.egg-info/PKG-INFO
 src/streamlit_component_dropfilltextarea.egg-info/SOURCES.txt
 src/streamlit_component_dropfilltextarea.egg-info/dependency_links.txt
 src/streamlit_component_dropfilltextarea.egg-info/requires.txt
 src/streamlit_component_dropfilltextarea.egg-info/top_level.txt
```

