# Comparing `tmp/streamlit_lang_tts-0.0.3.tar.gz` & `tmp/streamlit_lang_tts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_lang_tts-0.0.3.tar", last modified: Mon Apr 24 22:20:15 2023, max compression
+gzip compressed data, was "streamlit_lang_tts-0.0.4.tar", last modified: Tue Apr 25 13:07:14 2023, max compression
```

## Comparing `streamlit_lang_tts-0.0.3.tar` & `streamlit_lang_tts-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.651797 streamlit_lang_tts-0.0.3/
--rw-r--r--   0 ryanrapp   (501) staff       (20)     1063 2023-04-23 15:06:28.000000 streamlit_lang_tts-0.0.3/LICENSE
--rw-r--r--   0 ryanrapp   (501) staff       (20)       54 2023-04-24 22:06:01.000000 streamlit_lang_tts-0.0.3/MANIFEST.in
--rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-24 22:20:15.651678 streamlit_lang_tts-0.0.3/PKG-INFO
--rw-r--r--   0 ryanrapp   (501) staff       (20)       38 2023-04-24 22:20:15.651829 streamlit_lang_tts-0.0.3/setup.cfg
--rw-r--r--   0 ryanrapp   (501) staff       (20)      636 2023-04-24 22:16:49.000000 streamlit_lang_tts-0.0.3/setup.py
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.648300 streamlit_lang_tts-0.0.3/streamlit_lang_tts/
--rw-r--r--   0 ryanrapp   (501) staff       (20)     3514 2023-04-24 22:06:01.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/__init__.py
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.647526 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.649685 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/
--rw-r--r--   0 ryanrapp   (501) staff       (20)      691 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/asset-manifest.json
--rw-r--r--   0 ryanrapp   (501) staff       (20)   197459 2023-04-24 22:20:12.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/bootstrap.min.css
--rw-r--r--   0 ryanrapp   (501) staff       (20)     2081 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/index.html
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.647630 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.651507 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/
--rw-r--r--   0 ryanrapp   (501) staff       (20)   464201 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js
--rw-r--r--   0 ryanrapp   (501) staff       (20)     2059 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js.LICENSE.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)  1710252 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js.map
--rw-r--r--   0 ryanrapp   (501) staff       (20)     1972 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/main.d75feb69.chunk.js
--rw-r--r--   0 ryanrapp   (501) staff       (20)     6998 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/main.d75feb69.chunk.js.map
--rw-r--r--   0 ryanrapp   (501) staff       (20)     1578 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js
--rw-r--r--   0 ryanrapp   (501) staff       (20)     8363 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map
-drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-24 22:20:15.649160 streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/
--rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/PKG-INFO
--rw-r--r--   0 ryanrapp   (501) staff       (20)      907 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/SOURCES.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)        1 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/dependency_links.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)       16 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/requires.txt
--rw-r--r--   0 ryanrapp   (501) staff       (20)       19 2023-04-24 22:20:15.000000 streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/top_level.txt
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.557221 streamlit_lang_tts-0.0.4/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     1063 2023-04-23 15:06:28.000000 streamlit_lang_tts-0.0.4/LICENSE
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       54 2023-04-24 22:06:01.000000 streamlit_lang_tts-0.0.4/MANIFEST.in
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-25 13:07:14.557099 streamlit_lang_tts-0.0.4/PKG-INFO
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       38 2023-04-25 13:07:14.557257 streamlit_lang_tts-0.0.4/setup.cfg
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      636 2023-04-25 13:06:03.000000 streamlit_lang_tts-0.0.4/setup.py
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.553899 streamlit_lang_tts-0.0.4/streamlit_lang_tts/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     3514 2023-04-24 22:06:01.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/__init__.py
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.553114 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.555077 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      691 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/asset-manifest.json
+-rw-r--r--   0 ryanrapp   (501) staff       (20)   197459 2023-04-25 13:07:11.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/bootstrap.min.css
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     2081 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/index.html
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.553223 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.556917 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)   464710 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     2059 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js.LICENSE.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)  1710313 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js.map
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     2280 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/main.78d08be9.chunk.js
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     7634 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/main.78d08be9.chunk.js.map
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     1578 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js
+-rw-r--r--   0 ryanrapp   (501) staff       (20)     8363 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map
+drwxr-xr-x   0 ryanrapp   (501) staff       (20)        0 2023-04-25 13:07:14.554595 streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      263 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/PKG-INFO
+-rw-r--r--   0 ryanrapp   (501) staff       (20)      907 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)        1 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       16 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/requires.txt
+-rw-r--r--   0 ryanrapp   (501) staff       (20)       19 2023-04-25 13:07:14.000000 streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/top_level.txt
```

### Comparing `streamlit_lang_tts-0.0.3/LICENSE` & `streamlit_lang_tts-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.3/setup.py` & `streamlit_lang_tts-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_lang_tts",
-    version="0.0.3",
+    version="0.0.4",
     author="Ryan Rapp",
     author_email="skies_midair0f@icloud.com",
     description="Streamlit extensions for text-to-speech",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/__init__.py` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/bootstrap.min.css` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/index.html` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],i=t[1],f=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var i=r[a];0!==o[i]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_lang_tts=this.webpackJsonpstreamlit_lang_tts||[],i=a.push.bind(a);a.push=t,a=a.slice();for(var f=0;f<a.length;f++)t(a[f]);var p=i;r()}([])</script><script src="./static/js/2.cfa3d2aa.chunk.js"></script><script src="./static/js/main.d75feb69.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],i=t[1],f=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var i=r[a];0!==o[i]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_lang_tts=this.webpackJsonpstreamlit_lang_tts||[],i=a.push.bind(a);a.push=t,a=a.slice();for(var f=0;f<a.length;f++)t(a[f]);var p=i;r()}([])</script><script src="./static/js/2.38865783.chunk.js"></script><script src="./static/js/main.78d08be9.chunk.js"></script></body></html>
```

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-/*! For license information please see 2.cfa3d2aa.chunk.js.LICENSE.txt */
+/*! For license information please see 2.38865783.chunk.js.LICENSE.txt */
 (this.webpackJsonpstreamlit_lang_tts = this.webpackJsonpstreamlit_lang_tts || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return a
         }));
-        var r = n(12);
+        var r = n(14);
 
         function i(e, t) {
             for (var n = 0; n < t.length; n++) {
                 var i = t[n];
                 i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(e, Object(r.a)(i.key), i)
             }
         }
@@ -30,15 +30,15 @@
             return r
         }))
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
         }));
-        var r = n(10);
+        var r = n(12);
 
         function i(e, t) {
             if ("function" !== typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             e.prototype = Object.create(t && t.prototype, {
                 constructor: {
                     value: e,
                     writable: !0,
@@ -50,16 +50,16 @@
         }
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return o
         }));
         var r = n(4),
-            i = n(11),
-            a = n(8);
+            i = n(13),
+            a = n(10);
 
         function o(e) {
             var t = Object(i.a)();
             return function() {
                 var n, i = Object(r.a)(e);
                 if (t) {
                     var o = Object(r.a)(this).constructor;
@@ -77,18 +77,62 @@
             }, r(e)
         }
         n.d(t, "a", (function() {
             return r
         }))
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(23)
+        n.d(t, "a", (function() {
+            return a
+        }));
+        var r = n(6);
+
+        function i(e, t) {
+            var n = Object.keys(e);
+            if (Object.getOwnPropertySymbols) {
+                var r = Object.getOwnPropertySymbols(e);
+                t && (r = r.filter((function(t) {
+                    return Object.getOwnPropertyDescriptor(e, t).enumerable
+                }))), n.push.apply(n, r)
+            }
+            return n
+        }
+
+        function a(e) {
+            for (var t = 1; t < arguments.length; t++) {
+                var n = null != arguments[t] ? arguments[t] : {};
+                t % 2 ? i(Object(n), !0).forEach((function(t) {
+                    Object(r.a)(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : i(Object(n)).forEach((function(t) {
+                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+                }))
+            }
+            return e
+        }
+    }, function(e, t, n) {
+        "use strict";
+        n.d(t, "a", (function() {
+            return i
+        }));
+        var r = n(14);
+
+        function i(e, t, n) {
+            return (t = Object(r.a)(t)) in e ? Object.defineProperty(e, t, {
+                value: n,
+                enumerable: !0,
+                configurable: !0,
+                writable: !0
+            }) : e[t] = n, e
+        }
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(17)
+        e.exports = n(25)
+    }, function(e, t, n) {
+        "use strict";
+        e.exports = n(19)
     }, function(e, t, n) {
         "use strict";
 
         function r(e) {
             return r = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                 return typeof e
             } : function(e) {
@@ -99,16 +143,16 @@
             return r
         }))
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return a
         }));
-        var r = n(7),
-            i = n(9);
+        var r = n(9),
+            i = n(11);
 
         function a(e, t) {
             if (t && ("object" === Object(r.a)(t) || "function" === typeof t)) return t;
             if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
             return Object(i.a)(e)
         }
     }, function(e, t, n) {
@@ -149,15 +193,15 @@
             return r
         }))
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
         }));
-        var r = n(7);
+        var r = n(9);
 
         function i(e) {
             var t = function(e, t) {
                 if ("object" !== Object(r.a)(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var i = n.call(e, t || "default");
@@ -167,17 +211,17 @@
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
             return "symbol" === Object(r.a)(t) ? t : String(t)
         }
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
-            return bl
+            return yl
         })), n.d(t, "b", (function() {
-            return ml
+            return vl
         }));
         var r = {};
         n.r(r), n.d(r, "memcpy", (function() {
             return Ue
         })), n.d(r, "joinUint8Arrays", (function() {
             return Pe
         })), n.d(r, "toArrayBufferView", (function() {
@@ -247,69 +291,69 @@
         })), n.d(r, "rebaseValueOffsets", (function() {
             return kt
         })), n.d(r, "compareArrayLike", (function() {
             return wt
         }));
         var i = {};
         n.r(i), n.d(i, "getBool", (function() {
-            return nn
+            return Xt
         })), n.d(i, "getBit", (function() {
-            return rn
+            return en
         })), n.d(i, "setBool", (function() {
-            return an
+            return tn
         })), n.d(i, "truncateBitmap", (function() {
-            return on
+            return nn
         })), n.d(i, "packBools", (function() {
-            return un
+            return rn
         })), n.d(i, "iterateBits", (function() {
-            return sn
+            return an
         })), n.d(i, "popcnt_bit_range", (function() {
-            return cn
+            return on
         })), n.d(i, "popcnt_array", (function() {
-            return ln
+            return un
         })), n.d(i, "popcnt_uint32", (function() {
-            return fn
+            return sn
         }));
         var a = {};
         n.r(a), n.d(a, "uint16ToFloat64", (function() {
-            return Br
+            return Ir
         })), n.d(a, "float64ToUint16", (function() {
-            return Dr
+            return Er
         }));
         var o = {};
         n.r(o), n.d(o, "isArrowBigNumSymbol", (function() {
-            return zr
+            return Pr
         })), n.d(o, "bignumToString", (function() {
-            return Rr
+            return Nr
         })), n.d(o, "bignumToBigInt", (function() {
-            return Vr
+            return Ur
         })), n.d(o, "BN", (function() {
-            return Gr
+            return Kr
         }));
         var u = {};
         n.r(u), n.d(u, "clampIndex", (function() {
-            return Mi
+            return Fi
         })), n.d(u, "clampRange", (function() {
-            return Ni
+            return Ci
         })), n.d(u, "createElementComparator", (function() {
-            return Ri
+            return Ui
         }));
         var s = {};
         n.r(s), n.d(s, "BaseInt64", (function() {
-            return no
+            return eo
         })), n.d(s, "Uint64", (function() {
-            return ro
+            return to
         })), n.d(s, "Int64", (function() {
-            return io
+            return no
         })), n.d(s, "Int128", (function() {
-            return ao
+            return ro
         }));
-        var c = n(16),
+        var c = n(18),
             l = n.n(c),
-            f = n(6),
+            f = n(8),
             h = n.n(f),
             d = new WeakMap,
             p = new WeakMap;
 
         function y(e) {
             var t = d.get(e);
             return console.assert(null != t, "'this' is expected an Event object, but got", e), t
@@ -475,43 +519,43 @@
             initEvent: function() {}
         }, Object.defineProperty(b.prototype, "constructor", {
             value: b,
             configurable: !0,
             writable: !0
         }), "undefined" !== typeof window && "undefined" !== typeof window.Event && (Object.setPrototypeOf(b.prototype, window.Event.prototype), p.set(window.Event.prototype, b));
         var O = new WeakMap,
-            x = 3;
+            j = 3;
 
-        function j(e) {
+        function x(e) {
             return null !== e && "object" === typeof e
         }
 
         function S(e) {
             var t = O.get(e);
             if (null == t) throw new TypeError("'this' is expected an EventTarget object, but got another value.");
             return t
         }
 
         function T(e, t) {
             Object.defineProperty(e, "on".concat(t), function(e) {
                 return {
                     get: function() {
                         for (var t = S(this).get(e); null != t;) {
-                            if (t.listenerType === x) return t.listener;
+                            if (t.listenerType === j) return t.listener;
                             t = t.next
                         }
                         return null
                     },
                     set: function(t) {
-                        "function" === typeof t || j(t) || (t = null);
-                        for (var n = S(this), r = null, i = n.get(e); null != i;) i.listenerType === x ? null !== r ? r.next = i.next : null !== i.next ? n.set(e, i.next) : n.delete(e) : r = i, i = i.next;
+                        "function" === typeof t || x(t) || (t = null);
+                        for (var n = S(this), r = null, i = n.get(e); null != i;) i.listenerType === j ? null !== r ? r.next = i.next : null !== i.next ? n.set(e, i.next) : n.delete(e) : r = i, i = i.next;
                         if (null !== t) {
                             var a = {
                                 listener: t,
-                                listenerType: x,
+                                listenerType: j,
                                 passive: !1,
                                 once: !1,
                                 next: null
                             };
                             null === r ? n.set(e, a) : r.next = a
                         }
                     },
@@ -546,17 +590,17 @@
                 throw new TypeError("Cannot call a class as a function")
             }
             O.set(this, new Map)
         }
         E.prototype = {
             addEventListener: function(e, t, n) {
                 if (null != t) {
-                    if ("function" !== typeof t && !j(t)) throw new TypeError("'listener' should be a function or an object.");
+                    if ("function" !== typeof t && !x(t)) throw new TypeError("'listener' should be a function or an object.");
                     var r = S(this),
-                        i = j(n),
+                        i = x(n),
                         a = (i ? Boolean(n.capture) : Boolean(n)) ? 1 : 2,
                         o = {
                             listener: t,
                             listenerType: a,
                             passive: i && Boolean(n.passive),
                             once: i && Boolean(n.once),
                             next: null
@@ -569,15 +613,15 @@
                         }
                         s.next = o
                     } else r.set(e, o)
                 }
             },
             removeEventListener: function(e, t, n) {
                 if (null != t)
-                    for (var r = S(this), i = (j(n) ? Boolean(n.capture) : Boolean(n)) ? 1 : 2, a = null, o = r.get(e); null != o;) {
+                    for (var r = S(this), i = (x(n) ? Boolean(n.capture) : Boolean(n)) ? 1 : 2, a = null, o = r.get(e); null != o;) {
                         if (o.listener === t && o.listenerType === i) return void(null !== a ? a.next = o.next : null !== o.next ? r.set(e, o.next) : r.delete(e));
                         a = o, o = o.next
                     }
             },
             dispatchEvent: function(e) {
                 if (null == e || "string" !== typeof e.type) throw new TypeError('"event.type" should be a string.');
                 var t = S(this),
@@ -587,15 +631,15 @@
                 for (var i = function(e, t) {
                         return new(k(Object.getPrototypeOf(t)))(e, t)
                     }(this, e), a = null; null != r;) {
                     if (r.once ? null !== a ? a.next = r.next : null !== r.next ? t.set(n, r.next) : t.delete(n) : a = r, _(i, r.passive ? r.listener : null), "function" === typeof r.listener) try {
                         r.listener.call(this, i)
                     } catch (o) {
                         "undefined" !== typeof console && "function" === typeof console.error && console.error(o)
-                    } else r.listenerType !== x && "function" === typeof r.listener.handleEvent && r.listener.handleEvent(i);
+                    } else r.listenerType !== j && "function" === typeof r.listener.handleEvent && r.listener.handleEvent(i);
                     if (w(i)) break;
                     r = r.next
                 }
                 return _(i, null),
                     function(e, t) {
                         y(e).eventPhase = t
                     }(i, 0),
@@ -697,15 +741,15 @@
                     }
                     o(void 0)
                 }))
             }
         }
         var C = n(1),
             M = n(0),
-            N = n(7);
+            N = n(9);
 
         function U() {
             U = function() {
                 return e
             };
             var e = {},
                 t = Object.prototype,
@@ -733,15 +777,15 @@
                     return e[t] = n
                 }
             }
 
             function c(e, t, n, i) {
                 var a = t && t.prototype instanceof h ? t : h,
                     o = Object.create(a.prototype),
-                    u = new j(i || []);
+                    u = new x(i || []);
                 return r(o, "_invoke", {
                     value: w(e, n, u)
                 }), o
             }
 
             function l(e, t, n) {
                 try {
@@ -861,20 +905,20 @@
             function O(e) {
                 var t = {
                     tryLoc: e[0]
                 };
                 1 in e && (t.catchLoc = e[1]), 2 in e && (t.finallyLoc = e[2], t.afterLoc = e[3]), this.tryEntries.push(t)
             }
 
-            function x(e) {
+            function j(e) {
                 var t = e.completion || {};
                 t.type = "normal", delete t.arg, e.completion = t
             }
 
-            function j(e) {
+            function x(e) {
                 this.tryEntries = [{
                     tryLoc: "root"
                 }], e.forEach(O, this), this.reset(!0)
             }
 
             function S(e) {
                 if (e) {
@@ -937,18 +981,18 @@
                     function e() {
                         for (; n.length;) {
                             var r = n.pop();
                             if (r in t) return e.value = r, e.done = !1, e
                         }
                         return e.done = !0, e
                     }
-            }, e.values = S, j.prototype = {
-                constructor: j,
+            }, e.values = S, x.prototype = {
+                constructor: x,
                 reset: function(e) {
-                    if (this.prev = 0, this.next = 0, this.sent = this._sent = void 0, this.done = !1, this.delegate = null, this.method = "next", this.arg = void 0, this.tryEntries.forEach(x), !e)
+                    if (this.prev = 0, this.next = 0, this.sent = this._sent = void 0, this.done = !1, this.delegate = null, this.method = "next", this.arg = void 0, this.tryEntries.forEach(j), !e)
                         for (var t in this) "t" === t.charAt(0) && n.call(this, t) && !isNaN(+t.slice(1)) && (this[t] = void 0)
                 },
                 stop: function() {
                     this.done = !0;
                     var e = this.tryEntries[0].completion;
                     if ("throw" === e.type) throw e.arg;
                     return this.rval
@@ -994,25 +1038,25 @@
                 complete: function(e, t) {
                     if ("throw" === e.type) throw e.arg;
                     return "break" === e.type || "continue" === e.type ? this.next = e.arg : "return" === e.type ? (this.rval = this.arg = e.arg, this.method = "return", this.next = "end") : "normal" === e.type && t && (this.next = t), f
                 },
                 finish: function(e) {
                     for (var t = this.tryEntries.length - 1; t >= 0; --t) {
                         var n = this.tryEntries[t];
-                        if (n.finallyLoc === e) return this.complete(n.completion, n.afterLoc), x(n), f
+                        if (n.finallyLoc === e) return this.complete(n.completion, n.afterLoc), j(n), f
                     }
                 },
                 catch: function(e) {
                     for (var t = this.tryEntries.length - 1; t >= 0; --t) {
                         var n = this.tryEntries[t];
                         if (n.tryLoc === e) {
                             var r = n.completion;
                             if ("throw" === r.type) {
                                 var i = r.arg;
-                                x(n)
+                                j(n)
                             }
                             return i
                         }
                     }
                     throw new Error("illegal catch attempt")
                 },
                 delegateYield: function(e, t, n) {
@@ -1942,46 +1986,46 @@
             we = ke[0],
             _e = (ke[1], function(e) {
                 return "number" === typeof e
             }),
             Oe = function(e) {
                 return "boolean" === typeof e
             },
-            xe = function(e) {
+            je = function(e) {
                 return "function" === typeof e
             },
-            je = function(e) {
+            xe = function(e) {
                 return null != e && Object(e) === e
             },
             Se = function(e) {
-                return je(e) && xe(e.then)
+                return xe(e) && je(e.then)
             },
             Te = function(e) {
-                return je(e) && xe(e[Symbol.iterator])
+                return xe(e) && je(e[Symbol.iterator])
             },
             Ie = function(e) {
-                return je(e) && xe(e[Symbol.asyncIterator])
+                return xe(e) && je(e[Symbol.asyncIterator])
             },
             Ee = function(e) {
-                return je(e) && je(e.schema)
+                return xe(e) && xe(e.schema)
             },
             Ae = function(e) {
-                return je(e) && "done" in e && "value" in e
+                return xe(e) && "done" in e && "value" in e
             },
             Be = function(e) {
-                return je(e) && xe(e.stat) && _e(e.fd)
+                return xe(e) && je(e.stat) && _e(e.fd)
             },
             De = function(e) {
-                return je(e) && Le(e.body)
+                return xe(e) && Le(e.body)
             },
             Le = function(e) {
-                return je(e) && xe(e.cancel) && xe(e.getReader) && !(e instanceof de)
+                return xe(e) && je(e.cancel) && je(e.getReader) && !(e instanceof de)
             },
             Fe = function(e) {
-                return je(e) && xe(e.read) && xe(e.pipe) && Oe(e.readable) && !(e instanceof de)
+                return xe(e) && je(e.read) && je(e.pipe) && Oe(e.readable) && !(e instanceof de)
             },
             Ce = U().mark(Xe),
             Me = K.ByteBuffer,
             Ne = "undefined" !== typeof SharedArrayBuffer ? SharedArrayBuffer : ArrayBuffer;
 
         function Ue(e, t) {
             var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0,
@@ -2274,46 +2318,46 @@
             if (r !== t.length) return !1;
             if (r > 0)
                 do {
                     if (e[n] !== t[n]) return !1
                 } while (++n < r);
             return !0
         }
-        var _t = U().mark(jt),
+        var _t = U().mark(xt),
             Ot = {
                 fromIterable: function(e) {
-                    return xt(jt(e))
+                    return jt(xt(e))
                 },
                 fromAsyncIterable: function(e) {
-                    return xt(function(e) {
+                    return jt(function(e) {
                         return St.apply(this, arguments)
                     }(e))
                 },
                 fromDOMStream: function(e) {
-                    return xt(function(e) {
+                    return jt(function(e) {
                         return Tt.apply(this, arguments)
                     }(e))
                 },
                 fromNodeStream: function(e) {
-                    return xt(function(e) {
+                    return jt(function(e) {
                         return Dt.apply(this, arguments)
                     }(e))
                 },
                 toDOMStream: function(e, t) {
                     throw new Error('"toDOMStream" not available in this environment')
                 },
                 toNodeStream: function(e, t) {
                     throw new Error('"toNodeStream" not available in this environment')
                 }
             },
-            xt = function(e) {
+            jt = function(e) {
                 return e.next(), e
             };
 
-        function jt(e) {
+        function xt(e) {
             var t, n, r, i, a, o, u, s, c, l, f, h;
             return U().wrap((function(d) {
                 for (;;) switch (d.prev = d.next) {
                     case 0:
                         return s = function() {
                             if ("peek" === a) return Pe(r, o)[0];
                             var e = P(Pe(r, o), 3);
@@ -2764,145 +2808,113 @@
                             return e.stop()
                     }
                 }), e, null, [
                     [16, , 37, 41]
                 ])
             }))), Dt.apply(this, arguments)
         }
-        var Lt = n(12);
-
-        function Ft(e, t, n) {
-            return (t = Object(Lt.a)(t)) in e ? Object.defineProperty(e, t, {
-                value: n,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : e[t] = n, e
-        }
-
-        function Ct(e, t) {
-            var n = Object.keys(e);
-            if (Object.getOwnPropertySymbols) {
-                var r = Object.getOwnPropertySymbols(e);
-                t && (r = r.filter((function(t) {
-                    return Object.getOwnPropertyDescriptor(e, t).enumerable
-                }))), n.push.apply(n, r)
-            }
-            return n
-        }
-
-        function Mt(e) {
-            for (var t = 1; t < arguments.length; t++) {
-                var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ct(Object(n), !0).forEach((function(t) {
-                    Ft(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ct(Object(n)).forEach((function(t) {
-                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
-                }))
-            }
-            return e
-        }
-        var Nt = n(4);
+        var Lt = n(5),
+            Ft = n(4);
 
-        function Ut() {
-            return Ut = "undefined" !== typeof Reflect && Reflect.get ? Reflect.get.bind() : function(e, t, n) {
+        function Ct() {
+            return Ct = "undefined" !== typeof Reflect && Reflect.get ? Reflect.get.bind() : function(e, t, n) {
                 var r = function(e, t) {
-                    for (; !Object.prototype.hasOwnProperty.call(e, t) && null !== (e = Object(Nt.a)(e)););
+                    for (; !Object.prototype.hasOwnProperty.call(e, t) && null !== (e = Object(Ft.a)(e)););
                     return e
                 }(e, t);
                 if (r) {
                     var i = Object.getOwnPropertyDescriptor(r, t);
                     return i.get ? i.get.call(arguments.length < 3 ? e : n) : i.value
                 }
-            }, Ut.apply(this, arguments)
+            }, Ct.apply(this, arguments)
         }
-        var Pt, Rt, Vt, zt, Wt, Yt, Ht = Object(M.a)((function e() {
+        var Mt, Nt, Ut, Pt, Rt, Vt, zt = Object(M.a)((function e() {
             Object(C.a)(this, e)
         }));
-        Wt = Pt || (Pt = {}), zt = Wt.apache || (Wt.apache = {}), Vt = zt.arrow || (zt.arrow = {}),
+        Rt = Mt || (Mt = {}), Pt = Rt.apache || (Rt.apache = {}), Ut = Pt.arrow || (Pt.arrow = {}),
             function(e) {
                 e[e.V1 = 0] = "V1", e[e.V2 = 1] = "V2", e[e.V3 = 2] = "V3", e[e.V4 = 3] = "V4"
-            }((Rt = Vt.flatbuf || (Vt.flatbuf = {})).MetadataVersion || (Rt.MetadataVersion = {})),
+            }((Nt = Ut.flatbuf || (Ut.flatbuf = {})).MetadataVersion || (Nt.MetadataVersion = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.Sparse = 0] = "Sparse", e[e.Dense = 1] = "Dense"
                             }(e.UnionMode || (e.UnionMode = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.HALF = 0] = "HALF", e[e.SINGLE = 1] = "SINGLE", e[e.DOUBLE = 2] = "DOUBLE"
                             }(e.Precision || (e.Precision = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.DAY = 0] = "DAY", e[e.MILLISECOND = 1] = "MILLISECOND"
                             }(e.DateUnit || (e.DateUnit = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.SECOND = 0] = "SECOND", e[e.MILLISECOND = 1] = "MILLISECOND", e[e.MICROSECOND = 2] = "MICROSECOND", e[e.NANOSECOND = 3] = "NANOSECOND"
                             }(e.TimeUnit || (e.TimeUnit = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.YEAR_MONTH = 0] = "YEAR_MONTH", e[e.DAY_TIME = 1] = "DAY_TIME"
                             }(e.IntervalUnit || (e.IntervalUnit = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.NONE = 0] = "NONE", e[e.Null = 1] = "Null", e[e.Int = 2] = "Int", e[e.FloatingPoint = 3] = "FloatingPoint", e[e.Binary = 4] = "Binary", e[e.Utf8 = 5] = "Utf8", e[e.Bool = 6] = "Bool", e[e.Decimal = 7] = "Decimal", e[e.Date = 8] = "Date", e[e.Time = 9] = "Time", e[e.Timestamp = 10] = "Timestamp", e[e.Interval = 11] = "Interval", e[e.List = 12] = "List", e[e.Struct_ = 13] = "Struct_", e[e.Union = 14] = "Union", e[e.FixedSizeBinary = 15] = "FixedSizeBinary", e[e.FixedSizeList = 16] = "FixedSizeList", e[e.Map = 17] = "Map", e[e.Duration = 18] = "Duration", e[e.LargeBinary = 19] = "LargeBinary", e[e.LargeUtf8 = 20] = "LargeUtf8", e[e.LargeList = 21] = "LargeList"
                             }(e.Type || (e.Type = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.Little = 0] = "Little", e[e.Big = 1] = "Big"
                             }(e.Endianness || (e.Endianness = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -2934,15 +2946,15 @@
                                     }
                                 }]), e
                             }();
                             e.Null = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -2974,15 +2986,15 @@
                                     }
                                 }]), e
                             }();
                             e.Struct_ = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3014,15 +3026,15 @@
                                     }
                                 }]), e
                             }();
                             e.List = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3054,15 +3066,15 @@
                                     }
                                 }]), e
                             }();
                             e.LargeList = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3105,15 +3117,15 @@
                                     }
                                 }]), e
                             }();
                             e.FixedSizeList = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3156,15 +3168,15 @@
                                     }
                                 }]), e
                             }();
                             e.Map = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3242,15 +3254,15 @@
                                     }
                                 }]), t
                             }();
                             t.Union = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3304,15 +3316,15 @@
                                     }
                                 }]), e
                             }();
                             e.Int = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3355,15 +3367,15 @@
                                     }
                                 }]), t
                             }();
                             t.FloatingPoint = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3395,15 +3407,15 @@
                                     }
                                 }]), e
                             }();
                             e.Utf8 = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3435,15 +3447,15 @@
                                     }
                                 }]), e
                             }();
                             e.Binary = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3475,15 +3487,15 @@
                                     }
                                 }]), e
                             }();
                             e.LargeUtf8 = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3515,15 +3527,15 @@
                                     }
                                 }]), e
                             }();
                             e.LargeBinary = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3566,15 +3578,15 @@
                                     }
                                 }]), e
                             }();
                             e.FixedSizeBinary = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3606,15 +3618,15 @@
                                     }
                                 }]), e
                             }();
                             e.Bool = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -3668,15 +3680,15 @@
                                     }
                                 }]), e
                             }();
                             e.Decimal = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3719,15 +3731,15 @@
                                     }
                                 }]), t
                             }();
                             t.Date = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3781,15 +3793,15 @@
                                     }
                                 }]), t
                             }();
                             t.Time = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3843,15 +3855,15 @@
                                     }
                                 }]), t
                             }();
                             t.Timestamp = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3894,15 +3906,15 @@
                                     }
                                 }]), t
                             }();
                             t.Interval = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -3945,15 +3957,15 @@
                                     }
                                 }]), t
                             }();
                             t.Duration = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -4007,15 +4019,15 @@
                                     }
                                 }]), e
                             }();
                             e.KeyValue = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -4080,15 +4092,15 @@
                                     }
                                 }]), t
                             }();
                             t.DictionaryEncoding = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -4233,15 +4245,15 @@
                                     }
                                 }]), t
                             }();
                             t.Field = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -4268,15 +4280,15 @@
                                     }
                                 }]), e
                             }();
                             e.Buffer = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -4382,35 +4394,35 @@
                                     }
                                 }]), t
                             }();
                             t.Schema = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Pt || (Pt = {})),
+            }(Mt || (Mt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
-                            e.Schema = Pt.apache.arrow.flatbuf.Schema
+                            e.Schema = Mt.apache.arrow.flatbuf.Schema
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Yt || (Yt = {})),
+            }(Vt || (Vt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             ! function(e) {
                                 e[e.NONE = 0] = "NONE", e[e.Schema = 1] = "Schema", e[e.DictionaryBatch = 2] = "DictionaryBatch", e[e.RecordBatch = 3] = "RecordBatch", e[e.Tensor = 4] = "Tensor", e[e.SparseTensor = 5] = "SparseTensor"
                             }(e.MessageHeader || (e.MessageHeader = {}))
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Yt || (Yt = {})),
+            }(Vt || (Vt = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -4437,15 +4449,15 @@
                                     }
                                 }]), e
                             }();
                             e.FieldNode = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Yt || (Yt = {})),
+            }(Vt || (Vt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -4473,15 +4485,15 @@
                                         var e = this.bb.__offset(this.bb_pos, 6);
                                         return e ? this.bb.__vector_len(this.bb_pos + e) : 0
                                     }
                                 }, {
                                     key: "buffers",
                                     value: function(e, t) {
                                         var n = this.bb.__offset(this.bb_pos, 8);
-                                        return n ? (t || new Pt.apache.arrow.flatbuf.Buffer).__init(this.bb.__vector(this.bb_pos + n) + 16 * e, this.bb) : null
+                                        return n ? (t || new Mt.apache.arrow.flatbuf.Buffer).__init(this.bb.__vector(this.bb_pos + n) + 16 * e, this.bb) : null
                                     }
                                 }, {
                                     key: "buffersLength",
                                     value: function() {
                                         var e = this.bb.__offset(this.bb_pos, 8);
                                         return e ? this.bb.__vector_len(this.bb_pos + e) : 0
                                     }
@@ -4532,15 +4544,15 @@
                                     }
                                 }]), t
                             }();
                             t.RecordBatch = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Yt || (Yt = {})),
+            }(Vt || (Vt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -4605,15 +4617,15 @@
                                     }
                                 }]), t
                             }();
                             t.DictionaryBatch = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Yt || (Yt = {})),
+            }(Vt || (Vt = {})),
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -4623,15 +4635,15 @@
                                     value: function(e, t) {
                                         return this.bb_pos = e, this.bb = t, this
                                     }
                                 }, {
                                     key: "version",
                                     value: function() {
                                         var e = this.bb.__offset(this.bb_pos, 4);
-                                        return e ? this.bb.readInt16(this.bb_pos + e) : Pt.apache.arrow.flatbuf.MetadataVersion.V1
+                                        return e ? this.bb.readInt16(this.bb_pos + e) : Mt.apache.arrow.flatbuf.MetadataVersion.V1
                                     }
                                 }, {
                                     key: "headerType",
                                     value: function() {
                                         var t = this.bb.__offset(this.bb_pos, 6);
                                         return t ? this.bb.readUint8(this.bb_pos + t) : e.apache.arrow.flatbuf.MessageHeader.NONE
                                     }
@@ -4647,15 +4659,15 @@
                                         var e = this.bb.__offset(this.bb_pos, 10);
                                         return e ? this.bb.readInt64(this.bb_pos + e) : this.bb.createLong(0, 0)
                                     }
                                 }, {
                                     key: "customMetadata",
                                     value: function(e, t) {
                                         var n = this.bb.__offset(this.bb_pos, 12);
-                                        return n ? (t || new Pt.apache.arrow.flatbuf.KeyValue).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * e), this.bb) : null
+                                        return n ? (t || new Mt.apache.arrow.flatbuf.KeyValue).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * e), this.bb) : null
                                     }
                                 }, {
                                     key: "customMetadataLength",
                                     value: function() {
                                         var e = this.bb.__offset(this.bb_pos, 12);
                                         return e ? this.bb.__vector_len(this.bb_pos + e) : 0
                                     }
@@ -4668,15 +4680,15 @@
                                     key: "startMessage",
                                     value: function(e) {
                                         e.startObject(5)
                                     }
                                 }, {
                                     key: "addVersion",
                                     value: function(e, t) {
-                                        e.addFieldInt16(0, t, Pt.apache.arrow.flatbuf.MetadataVersion.V1)
+                                        e.addFieldInt16(0, t, Mt.apache.arrow.flatbuf.MetadataVersion.V1)
                                     }
                                 }, {
                                     key: "addHeaderType",
                                     value: function(t, n) {
                                         t.addFieldInt8(1, n, e.apache.arrow.flatbuf.MessageHeader.NONE)
                                     }
                                 }, {
@@ -4723,53 +4735,53 @@
                                     }
                                 }]), t
                             }();
                             t.Message = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Yt || (Yt = {}));
-        Pt.apache.arrow.flatbuf.Type;
-        var $t, Kt, Qt = Pt.apache.arrow.flatbuf.DateUnit,
-            qt = Pt.apache.arrow.flatbuf.TimeUnit,
-            Gt = Pt.apache.arrow.flatbuf.Precision,
-            Jt = Pt.apache.arrow.flatbuf.UnionMode,
-            Zt = Pt.apache.arrow.flatbuf.IntervalUnit,
-            Xt = Yt.apache.arrow.flatbuf.MessageHeader,
-            en = Pt.apache.arrow.flatbuf.MetadataVersion;
+            }(Vt || (Vt = {}));
+        Mt.apache.arrow.flatbuf.Type;
+        var Wt, Yt, Ht = Mt.apache.arrow.flatbuf.DateUnit,
+            $t = Mt.apache.arrow.flatbuf.TimeUnit,
+            Kt = Mt.apache.arrow.flatbuf.Precision,
+            Qt = Mt.apache.arrow.flatbuf.UnionMode,
+            qt = Mt.apache.arrow.flatbuf.IntervalUnit,
+            Gt = Vt.apache.arrow.flatbuf.MessageHeader,
+            Jt = Mt.apache.arrow.flatbuf.MetadataVersion;
         ! function(e) {
             e[e.NONE = 0] = "NONE", e[e.Null = 1] = "Null", e[e.Int = 2] = "Int", e[e.Float = 3] = "Float", e[e.Binary = 4] = "Binary", e[e.Utf8 = 5] = "Utf8", e[e.Bool = 6] = "Bool", e[e.Decimal = 7] = "Decimal", e[e.Date = 8] = "Date", e[e.Time = 9] = "Time", e[e.Timestamp = 10] = "Timestamp", e[e.Interval = 11] = "Interval", e[e.List = 12] = "List", e[e.Struct = 13] = "Struct", e[e.Union = 14] = "Union", e[e.FixedSizeBinary = 15] = "FixedSizeBinary", e[e.FixedSizeList = 16] = "FixedSizeList", e[e.Map = 17] = "Map", e[e.Dictionary = -1] = "Dictionary", e[e.Int8 = -2] = "Int8", e[e.Int16 = -3] = "Int16", e[e.Int32 = -4] = "Int32", e[e.Int64 = -5] = "Int64", e[e.Uint8 = -6] = "Uint8", e[e.Uint16 = -7] = "Uint16", e[e.Uint32 = -8] = "Uint32", e[e.Uint64 = -9] = "Uint64", e[e.Float16 = -10] = "Float16", e[e.Float32 = -11] = "Float32", e[e.Float64 = -12] = "Float64", e[e.DateDay = -13] = "DateDay", e[e.DateMillisecond = -14] = "DateMillisecond", e[e.TimestampSecond = -15] = "TimestampSecond", e[e.TimestampMillisecond = -16] = "TimestampMillisecond", e[e.TimestampMicrosecond = -17] = "TimestampMicrosecond", e[e.TimestampNanosecond = -18] = "TimestampNanosecond", e[e.TimeSecond = -19] = "TimeSecond", e[e.TimeMillisecond = -20] = "TimeMillisecond", e[e.TimeMicrosecond = -21] = "TimeMicrosecond", e[e.TimeNanosecond = -22] = "TimeNanosecond", e[e.DenseUnion = -23] = "DenseUnion", e[e.SparseUnion = -24] = "SparseUnion", e[e.IntervalDayTime = -25] = "IntervalDayTime", e[e.IntervalYearMonth = -26] = "IntervalYearMonth"
-        }($t || ($t = {})),
+        }(Wt || (Wt = {})),
         function(e) {
             e[e.OFFSET = 0] = "OFFSET", e[e.DATA = 1] = "DATA", e[e.VALIDITY = 2] = "VALIDITY", e[e.TYPE = 3] = "TYPE"
-        }(Kt || (Kt = {}));
-        var tn = U().mark(sn);
+        }(Yt || (Yt = {}));
+        var Zt = U().mark(an);
 
-        function nn(e, t, n, r) {
+        function Xt(e, t, n, r) {
             return 0 !== (n & 1 << r)
         }
 
-        function rn(e, t, n, r) {
+        function en(e, t, n, r) {
             return (n & 1 << r) >> r
         }
 
-        function an(e, t, n) {
+        function tn(e, t, n) {
             return n ? !!(e[t >> 3] |= 1 << t % 8) || !0 : !(e[t >> 3] &= ~(1 << t % 8)) && !1
         }
 
-        function on(e, t, n) {
+        function nn(e, t, n) {
             var r = n.byteLength + 7 & -8;
             if (e > 0 || n.byteLength < r) {
                 var i = new Uint8Array(r);
-                return i.set(e % 8 === 0 ? n.subarray(e >> 3) : un(sn(n, e, t, null, nn)).subarray(0, r)), i
+                return i.set(e % 8 === 0 ? n.subarray(e >> 3) : rn(an(n, e, t, null, Xt)).subarray(0, r)), i
             }
             return n
         }
 
-        function un(e) {
+        function rn(e) {
             var t, n = [],
                 r = 0,
                 i = 0,
                 a = 0,
                 o = D(e);
             try {
                 for (o.s(); !(t = o.n()).done;) {
@@ -4780,15 +4792,15 @@
             } finally {
                 o.f()
             }(0 === r || i > 0) && (n[r++] = a);
             var u = new Uint8Array(n.length + 7 & -8);
             return u.set(n), u
         }
 
-        function sn(e, t, n, r, i) {
+        function an(e, t, n, r, i) {
             var a, o, u, s, c;
             return U().wrap((function(l) {
                 for (;;) switch (l.prev = l.next) {
                     case 0:
                         a = t % 8, o = t >> 3, u = 0, s = n;
                     case 3:
                         if (!(s > 0)) {
@@ -4806,69 +4818,69 @@
                     case 8:
                         a = 0, l.next = 3;
                         break;
                     case 11:
                     case "end":
                         return l.stop()
                 }
-            }), tn)
+            }), Zt)
         }
 
-        function cn(e, t, n) {
+        function on(e, t, n) {
             if (n - t <= 0) return 0;
             if (n - t < 8) {
                 var r, i = 0,
-                    a = D(sn(e, t, n - t, e, rn));
+                    a = D(an(e, t, n - t, e, en));
                 try {
                     for (a.s(); !(r = a.n()).done;) {
                         i += r.value
                     }
                 } catch (s) {
                     a.e(s)
                 } finally {
                     a.f()
                 }
                 return i
             }
             var o = n >> 3 << 3,
                 u = t + (t % 8 === 0 ? 0 : 8 - t % 8);
-            return cn(e, t, u) + cn(e, o, n) + ln(e, u >> 3, o - u >> 3)
+            return on(e, t, u) + on(e, o, n) + un(e, u >> 3, o - u >> 3)
         }
 
-        function ln(e, t, n) {
-            for (var r = 0, i = 0 | t, a = new DataView(e.buffer, e.byteOffset, e.byteLength), o = void 0 === n ? e.byteLength : i + n; o - i >= 4;) r += fn(a.getUint32(i)), i += 4;
-            for (; o - i >= 2;) r += fn(a.getUint16(i)), i += 2;
-            for (; o - i >= 1;) r += fn(a.getUint8(i)), i += 1;
+        function un(e, t, n) {
+            for (var r = 0, i = 0 | t, a = new DataView(e.buffer, e.byteOffset, e.byteLength), o = void 0 === n ? e.byteLength : i + n; o - i >= 4;) r += sn(a.getUint32(i)), i += 4;
+            for (; o - i >= 2;) r += sn(a.getUint16(i)), i += 2;
+            for (; o - i >= 1;) r += sn(a.getUint8(i)), i += 1;
             return r
         }
 
-        function fn(e) {
+        function sn(e) {
             var t = 0 | e;
             return 16843009 * ((t = (858993459 & (t -= t >>> 1 & 1431655765)) + (t >>> 2 & 858993459)) + (t >>> 4) & 252645135) >>> 24
         }
 
-        function hn(e) {
+        function cn(e) {
             return function(e) {
                 if (Array.isArray(e)) return A(e)
             }(e) || function(e) {
                 if ("undefined" !== typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
             }(e) || B(e) || function() {
                 throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }()
         }
-        var dn = function() {
+        var ln = function() {
             function e() {
                 Object(C.a)(this, e)
             }
             return Object(M.a)(e, [{
                 key: "visitMany",
                 value: function(e) {
                     for (var t = this, n = arguments.length, r = new Array(n > 1 ? n - 1 : 0), i = 1; i < n; i++) r[i - 1] = arguments[i];
                     return e.map((function(e, n) {
-                        return t.visit.apply(t, [e].concat(hn(r.map((function(e) {
+                        return t.visit.apply(t, [e].concat(cn(r.map((function(e) {
                             return e[n]
                         })))))
                     }))
                 }
             }, {
                 key: "visit",
                 value: function() {
@@ -4877,151 +4889,151 @@
                 }
             }, {
                 key: "getVisitFn",
                 value: function(e) {
                     return function(e, t) {
                         var n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2],
                             r = null,
-                            i = $t.NONE;
-                        t instanceof sr || t instanceof Ht ? i = pn(t.type) : t instanceof Tn ? i = pn(t) : "number" !== typeof(i = t) && (i = $t[t]);
+                            i = Wt.NONE;
+                        t instanceof ar || t instanceof zt ? i = fn(t.type) : t instanceof jn ? i = fn(t) : "number" !== typeof(i = t) && (i = Wt[t]);
                         switch (i) {
-                            case $t.Null:
+                            case Wt.Null:
                                 r = e.visitNull;
                                 break;
-                            case $t.Bool:
+                            case Wt.Bool:
                                 r = e.visitBool;
                                 break;
-                            case $t.Int:
+                            case Wt.Int:
                                 r = e.visitInt;
                                 break;
-                            case $t.Int8:
+                            case Wt.Int8:
                                 r = e.visitInt8 || e.visitInt;
                                 break;
-                            case $t.Int16:
+                            case Wt.Int16:
                                 r = e.visitInt16 || e.visitInt;
                                 break;
-                            case $t.Int32:
+                            case Wt.Int32:
                                 r = e.visitInt32 || e.visitInt;
                                 break;
-                            case $t.Int64:
+                            case Wt.Int64:
                                 r = e.visitInt64 || e.visitInt;
                                 break;
-                            case $t.Uint8:
+                            case Wt.Uint8:
                                 r = e.visitUint8 || e.visitInt;
                                 break;
-                            case $t.Uint16:
+                            case Wt.Uint16:
                                 r = e.visitUint16 || e.visitInt;
                                 break;
-                            case $t.Uint32:
+                            case Wt.Uint32:
                                 r = e.visitUint32 || e.visitInt;
                                 break;
-                            case $t.Uint64:
+                            case Wt.Uint64:
                                 r = e.visitUint64 || e.visitInt;
                                 break;
-                            case $t.Float:
+                            case Wt.Float:
                                 r = e.visitFloat;
                                 break;
-                            case $t.Float16:
+                            case Wt.Float16:
                                 r = e.visitFloat16 || e.visitFloat;
                                 break;
-                            case $t.Float32:
+                            case Wt.Float32:
                                 r = e.visitFloat32 || e.visitFloat;
                                 break;
-                            case $t.Float64:
+                            case Wt.Float64:
                                 r = e.visitFloat64 || e.visitFloat;
                                 break;
-                            case $t.Utf8:
+                            case Wt.Utf8:
                                 r = e.visitUtf8;
                                 break;
-                            case $t.Binary:
+                            case Wt.Binary:
                                 r = e.visitBinary;
                                 break;
-                            case $t.FixedSizeBinary:
+                            case Wt.FixedSizeBinary:
                                 r = e.visitFixedSizeBinary;
                                 break;
-                            case $t.Date:
+                            case Wt.Date:
                                 r = e.visitDate;
                                 break;
-                            case $t.DateDay:
+                            case Wt.DateDay:
                                 r = e.visitDateDay || e.visitDate;
                                 break;
-                            case $t.DateMillisecond:
+                            case Wt.DateMillisecond:
                                 r = e.visitDateMillisecond || e.visitDate;
                                 break;
-                            case $t.Timestamp:
+                            case Wt.Timestamp:
                                 r = e.visitTimestamp;
                                 break;
-                            case $t.TimestampSecond:
+                            case Wt.TimestampSecond:
                                 r = e.visitTimestampSecond || e.visitTimestamp;
                                 break;
-                            case $t.TimestampMillisecond:
+                            case Wt.TimestampMillisecond:
                                 r = e.visitTimestampMillisecond || e.visitTimestamp;
                                 break;
-                            case $t.TimestampMicrosecond:
+                            case Wt.TimestampMicrosecond:
                                 r = e.visitTimestampMicrosecond || e.visitTimestamp;
                                 break;
-                            case $t.TimestampNanosecond:
+                            case Wt.TimestampNanosecond:
                                 r = e.visitTimestampNanosecond || e.visitTimestamp;
                                 break;
-                            case $t.Time:
+                            case Wt.Time:
                                 r = e.visitTime;
                                 break;
-                            case $t.TimeSecond:
+                            case Wt.TimeSecond:
                                 r = e.visitTimeSecond || e.visitTime;
                                 break;
-                            case $t.TimeMillisecond:
+                            case Wt.TimeMillisecond:
                                 r = e.visitTimeMillisecond || e.visitTime;
                                 break;
-                            case $t.TimeMicrosecond:
+                            case Wt.TimeMicrosecond:
                                 r = e.visitTimeMicrosecond || e.visitTime;
                                 break;
-                            case $t.TimeNanosecond:
+                            case Wt.TimeNanosecond:
                                 r = e.visitTimeNanosecond || e.visitTime;
                                 break;
-                            case $t.Decimal:
+                            case Wt.Decimal:
                                 r = e.visitDecimal;
                                 break;
-                            case $t.List:
+                            case Wt.List:
                                 r = e.visitList;
                                 break;
-                            case $t.Struct:
+                            case Wt.Struct:
                                 r = e.visitStruct;
                                 break;
-                            case $t.Union:
+                            case Wt.Union:
                                 r = e.visitUnion;
                                 break;
-                            case $t.DenseUnion:
+                            case Wt.DenseUnion:
                                 r = e.visitDenseUnion || e.visitUnion;
                                 break;
-                            case $t.SparseUnion:
+                            case Wt.SparseUnion:
                                 r = e.visitSparseUnion || e.visitUnion;
                                 break;
-                            case $t.Dictionary:
+                            case Wt.Dictionary:
                                 r = e.visitDictionary;
                                 break;
-                            case $t.Interval:
+                            case Wt.Interval:
                                 r = e.visitInterval;
                                 break;
-                            case $t.IntervalDayTime:
+                            case Wt.IntervalDayTime:
                                 r = e.visitIntervalDayTime || e.visitInterval;
                                 break;
-                            case $t.IntervalYearMonth:
+                            case Wt.IntervalYearMonth:
                                 r = e.visitIntervalYearMonth || e.visitInterval;
                                 break;
-                            case $t.FixedSizeList:
+                            case Wt.FixedSizeList:
                                 r = e.visitFixedSizeList;
                                 break;
-                            case $t.Map:
+                            case Wt.Map:
                                 r = e.visitMap
                         }
                         if ("function" === typeof r) return r;
                         if (!n) return function() {
                             return null
                         };
-                        throw new Error("Unrecognized type '".concat($t[i], "'"))
+                        throw new Error("Unrecognized type '".concat(Wt[i], "'"))
                     }(this, e, !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1])
                 }
             }, {
                 key: "visitNull",
                 value: function(e) {
                     return null
                 }
@@ -5109,333 +5121,333 @@
                 key: "visitMap",
                 value: function(e) {
                     return null
                 }
             }]), e
         }();
 
-        function pn(e) {
+        function fn(e) {
             switch (e.typeId) {
-                case $t.Null:
-                    return $t.Null;
-                case $t.Int:
+                case Wt.Null:
+                    return Wt.Null;
+                case Wt.Int:
                     var t = e.bitWidth,
                         n = e.isSigned;
                     switch (t) {
                         case 8:
-                            return n ? $t.Int8 : $t.Uint8;
+                            return n ? Wt.Int8 : Wt.Uint8;
                         case 16:
-                            return n ? $t.Int16 : $t.Uint16;
+                            return n ? Wt.Int16 : Wt.Uint16;
                         case 32:
-                            return n ? $t.Int32 : $t.Uint32;
+                            return n ? Wt.Int32 : Wt.Uint32;
                         case 64:
-                            return n ? $t.Int64 : $t.Uint64
+                            return n ? Wt.Int64 : Wt.Uint64
                     }
-                    return $t.Int;
-                case $t.Float:
+                    return Wt.Int;
+                case Wt.Float:
                     switch (e.precision) {
-                        case Gt.HALF:
-                            return $t.Float16;
-                        case Gt.SINGLE:
-                            return $t.Float32;
-                        case Gt.DOUBLE:
-                            return $t.Float64
-                    }
-                    return $t.Float;
-                case $t.Binary:
-                    return $t.Binary;
-                case $t.Utf8:
-                    return $t.Utf8;
-                case $t.Bool:
-                    return $t.Bool;
-                case $t.Decimal:
-                    return $t.Decimal;
-                case $t.Time:
+                        case Kt.HALF:
+                            return Wt.Float16;
+                        case Kt.SINGLE:
+                            return Wt.Float32;
+                        case Kt.DOUBLE:
+                            return Wt.Float64
+                    }
+                    return Wt.Float;
+                case Wt.Binary:
+                    return Wt.Binary;
+                case Wt.Utf8:
+                    return Wt.Utf8;
+                case Wt.Bool:
+                    return Wt.Bool;
+                case Wt.Decimal:
+                    return Wt.Decimal;
+                case Wt.Time:
                     switch (e.unit) {
-                        case qt.SECOND:
-                            return $t.TimeSecond;
-                        case qt.MILLISECOND:
-                            return $t.TimeMillisecond;
-                        case qt.MICROSECOND:
-                            return $t.TimeMicrosecond;
-                        case qt.NANOSECOND:
-                            return $t.TimeNanosecond
+                        case $t.SECOND:
+                            return Wt.TimeSecond;
+                        case $t.MILLISECOND:
+                            return Wt.TimeMillisecond;
+                        case $t.MICROSECOND:
+                            return Wt.TimeMicrosecond;
+                        case $t.NANOSECOND:
+                            return Wt.TimeNanosecond
                     }
-                    return $t.Time;
-                case $t.Timestamp:
+                    return Wt.Time;
+                case Wt.Timestamp:
                     switch (e.unit) {
-                        case qt.SECOND:
-                            return $t.TimestampSecond;
-                        case qt.MILLISECOND:
-                            return $t.TimestampMillisecond;
-                        case qt.MICROSECOND:
-                            return $t.TimestampMicrosecond;
-                        case qt.NANOSECOND:
-                            return $t.TimestampNanosecond
+                        case $t.SECOND:
+                            return Wt.TimestampSecond;
+                        case $t.MILLISECOND:
+                            return Wt.TimestampMillisecond;
+                        case $t.MICROSECOND:
+                            return Wt.TimestampMicrosecond;
+                        case $t.NANOSECOND:
+                            return Wt.TimestampNanosecond
                     }
-                    return $t.Timestamp;
-                case $t.Date:
+                    return Wt.Timestamp;
+                case Wt.Date:
                     switch (e.unit) {
-                        case Qt.DAY:
-                            return $t.DateDay;
-                        case Qt.MILLISECOND:
-                            return $t.DateMillisecond
+                        case Ht.DAY:
+                            return Wt.DateDay;
+                        case Ht.MILLISECOND:
+                            return Wt.DateMillisecond
                     }
-                    return $t.Date;
-                case $t.Interval:
+                    return Wt.Date;
+                case Wt.Interval:
                     switch (e.unit) {
-                        case Zt.DAY_TIME:
-                            return $t.IntervalDayTime;
-                        case Zt.YEAR_MONTH:
-                            return $t.IntervalYearMonth
-                    }
-                    return $t.Interval;
-                case $t.Map:
-                    return $t.Map;
-                case $t.List:
-                    return $t.List;
-                case $t.Struct:
-                    return $t.Struct;
-                case $t.Union:
+                        case qt.DAY_TIME:
+                            return Wt.IntervalDayTime;
+                        case qt.YEAR_MONTH:
+                            return Wt.IntervalYearMonth
+                    }
+                    return Wt.Interval;
+                case Wt.Map:
+                    return Wt.Map;
+                case Wt.List:
+                    return Wt.List;
+                case Wt.Struct:
+                    return Wt.Struct;
+                case Wt.Union:
                     switch (e.mode) {
-                        case Jt.Dense:
-                            return $t.DenseUnion;
-                        case Jt.Sparse:
-                            return $t.SparseUnion
-                    }
-                    return $t.Union;
-                case $t.FixedSizeBinary:
-                    return $t.FixedSizeBinary;
-                case $t.FixedSizeList:
-                    return $t.FixedSizeList;
-                case $t.Dictionary:
-                    return $t.Dictionary
+                        case Qt.Dense:
+                            return Wt.DenseUnion;
+                        case Qt.Sparse:
+                            return Wt.SparseUnion
+                    }
+                    return Wt.Union;
+                case Wt.FixedSizeBinary:
+                    return Wt.FixedSizeBinary;
+                case Wt.FixedSizeList:
+                    return Wt.FixedSizeList;
+                case Wt.Dictionary:
+                    return Wt.Dictionary
             }
-            throw new Error("Unrecognized type '".concat($t[e.typeId], "'"))
+            throw new Error("Unrecognized type '".concat(Wt[e.typeId], "'"))
         }
-        dn.prototype.visitInt8 = null, dn.prototype.visitInt16 = null, dn.prototype.visitInt32 = null, dn.prototype.visitInt64 = null, dn.prototype.visitUint8 = null, dn.prototype.visitUint16 = null, dn.prototype.visitUint32 = null, dn.prototype.visitUint64 = null, dn.prototype.visitFloat16 = null, dn.prototype.visitFloat32 = null, dn.prototype.visitFloat64 = null, dn.prototype.visitDateDay = null, dn.prototype.visitDateMillisecond = null, dn.prototype.visitTimestampSecond = null, dn.prototype.visitTimestampMillisecond = null, dn.prototype.visitTimestampMicrosecond = null, dn.prototype.visitTimestampNanosecond = null, dn.prototype.visitTimeSecond = null, dn.prototype.visitTimeMillisecond = null, dn.prototype.visitTimeMicrosecond = null, dn.prototype.visitTimeNanosecond = null, dn.prototype.visitDenseUnion = null, dn.prototype.visitSparseUnion = null, dn.prototype.visitIntervalDayTime = null, dn.prototype.visitIntervalYearMonth = null;
-        var yn = function(e) {
+        ln.prototype.visitInt8 = null, ln.prototype.visitInt16 = null, ln.prototype.visitInt32 = null, ln.prototype.visitInt64 = null, ln.prototype.visitUint8 = null, ln.prototype.visitUint16 = null, ln.prototype.visitUint32 = null, ln.prototype.visitUint64 = null, ln.prototype.visitFloat16 = null, ln.prototype.visitFloat32 = null, ln.prototype.visitFloat64 = null, ln.prototype.visitDateDay = null, ln.prototype.visitDateMillisecond = null, ln.prototype.visitTimestampSecond = null, ln.prototype.visitTimestampMillisecond = null, ln.prototype.visitTimestampMicrosecond = null, ln.prototype.visitTimestampNanosecond = null, ln.prototype.visitTimeSecond = null, ln.prototype.visitTimeMillisecond = null, ln.prototype.visitTimeMicrosecond = null, ln.prototype.visitTimeNanosecond = null, ln.prototype.visitDenseUnion = null, ln.prototype.visitSparseUnion = null, ln.prototype.visitIntervalDayTime = null, ln.prototype.visitIntervalYearMonth = null;
+        var hn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n() {
                 return Object(C.a)(this, n), t.apply(this, arguments)
             }
             return Object(M.a)(n, [{
                 key: "compareSchemas",
                 value: function(e, t) {
-                    return e === t || t instanceof e.constructor && Sn.compareFields(e.fields, t.fields)
+                    return e === t || t instanceof e.constructor && On.compareFields(e.fields, t.fields)
                 }
             }, {
                 key: "compareFields",
                 value: function(e, t) {
                     return e === t || Array.isArray(e) && Array.isArray(t) && e.length === t.length && e.every((function(e, n) {
-                        return Sn.compareField(e, t[n])
+                        return On.compareField(e, t[n])
                     }))
                 }
             }, {
                 key: "compareField",
                 value: function(e, t) {
-                    return e === t || t instanceof e.constructor && e.name === t.name && e.nullable === t.nullable && Sn.visit(e.type, t.type)
+                    return e === t || t instanceof e.constructor && e.name === t.name && e.nullable === t.nullable && On.visit(e.type, t.type)
                 }
             }]), n
-        }(dn);
+        }(ln);
 
-        function vn(e, t) {
+        function dn(e, t) {
             return t instanceof e.constructor
         }
 
-        function bn(e, t) {
-            return e === t || vn(e, t)
+        function pn(e, t) {
+            return e === t || dn(e, t)
         }
 
-        function mn(e, t) {
-            return e === t || vn(e, t) && e.bitWidth === t.bitWidth && e.isSigned === t.isSigned
+        function yn(e, t) {
+            return e === t || dn(e, t) && e.bitWidth === t.bitWidth && e.isSigned === t.isSigned
         }
 
-        function gn(e, t) {
-            return e === t || vn(e, t) && e.precision === t.precision
+        function vn(e, t) {
+            return e === t || dn(e, t) && e.precision === t.precision
         }
 
-        function kn(e, t) {
-            return e === t || vn(e, t) && e.unit === t.unit
+        function bn(e, t) {
+            return e === t || dn(e, t) && e.unit === t.unit
         }
 
-        function wn(e, t) {
-            return e === t || vn(e, t) && e.unit === t.unit && e.timezone === t.timezone
+        function mn(e, t) {
+            return e === t || dn(e, t) && e.unit === t.unit && e.timezone === t.timezone
         }
 
-        function _n(e, t) {
-            return e === t || vn(e, t) && e.unit === t.unit && e.bitWidth === t.bitWidth
+        function gn(e, t) {
+            return e === t || dn(e, t) && e.unit === t.unit && e.bitWidth === t.bitWidth
         }
 
-        function On(e, t) {
-            return e === t || vn(e, t) && e.mode === t.mode && e.typeIds.every((function(e, n) {
+        function kn(e, t) {
+            return e === t || dn(e, t) && e.mode === t.mode && e.typeIds.every((function(e, n) {
                 return e === t.typeIds[n]
-            })) && Sn.compareFields(e.children, t.children)
+            })) && On.compareFields(e.children, t.children)
         }
 
-        function xn(e, t) {
-            return e === t || vn(e, t) && e.unit === t.unit
+        function wn(e, t) {
+            return e === t || dn(e, t) && e.unit === t.unit
         }
-        yn.prototype.visitNull = bn, yn.prototype.visitBool = bn, yn.prototype.visitInt = mn, yn.prototype.visitInt8 = mn, yn.prototype.visitInt16 = mn, yn.prototype.visitInt32 = mn, yn.prototype.visitInt64 = mn, yn.prototype.visitUint8 = mn, yn.prototype.visitUint16 = mn, yn.prototype.visitUint32 = mn, yn.prototype.visitUint64 = mn, yn.prototype.visitFloat = gn, yn.prototype.visitFloat16 = gn, yn.prototype.visitFloat32 = gn, yn.prototype.visitFloat64 = gn, yn.prototype.visitUtf8 = bn, yn.prototype.visitBinary = bn, yn.prototype.visitFixedSizeBinary = function(e, t) {
-            return e === t || vn(e, t) && e.byteWidth === t.byteWidth
-        }, yn.prototype.visitDate = kn, yn.prototype.visitDateDay = kn, yn.prototype.visitDateMillisecond = kn, yn.prototype.visitTimestamp = wn, yn.prototype.visitTimestampSecond = wn, yn.prototype.visitTimestampMillisecond = wn, yn.prototype.visitTimestampMicrosecond = wn, yn.prototype.visitTimestampNanosecond = wn, yn.prototype.visitTime = _n, yn.prototype.visitTimeSecond = _n, yn.prototype.visitTimeMillisecond = _n, yn.prototype.visitTimeMicrosecond = _n, yn.prototype.visitTimeNanosecond = _n, yn.prototype.visitDecimal = bn, yn.prototype.visitList = function(e, t) {
-            return e === t || vn(e, t) && e.children.length === t.children.length && Sn.compareFields(e.children, t.children)
-        }, yn.prototype.visitStruct = function(e, t) {
-            return e === t || vn(e, t) && e.children.length === t.children.length && Sn.compareFields(e.children, t.children)
-        }, yn.prototype.visitUnion = On, yn.prototype.visitDenseUnion = On, yn.prototype.visitSparseUnion = On, yn.prototype.visitDictionary = function(e, t) {
-            return e === t || vn(e, t) && e.id === t.id && e.isOrdered === t.isOrdered && Sn.visit(e.indices, t.indices) && Sn.visit(e.dictionary, t.dictionary)
-        }, yn.prototype.visitInterval = xn, yn.prototype.visitIntervalDayTime = xn, yn.prototype.visitIntervalYearMonth = xn, yn.prototype.visitFixedSizeList = function(e, t) {
-            return e === t || vn(e, t) && e.listSize === t.listSize && e.children.length === t.children.length && Sn.compareFields(e.children, t.children)
-        }, yn.prototype.visitMap = function(e, t) {
-            return e === t || vn(e, t) && e.keysSorted === t.keysSorted && e.children.length === t.children.length && Sn.compareFields(e.children, t.children)
+        hn.prototype.visitNull = pn, hn.prototype.visitBool = pn, hn.prototype.visitInt = yn, hn.prototype.visitInt8 = yn, hn.prototype.visitInt16 = yn, hn.prototype.visitInt32 = yn, hn.prototype.visitInt64 = yn, hn.prototype.visitUint8 = yn, hn.prototype.visitUint16 = yn, hn.prototype.visitUint32 = yn, hn.prototype.visitUint64 = yn, hn.prototype.visitFloat = vn, hn.prototype.visitFloat16 = vn, hn.prototype.visitFloat32 = vn, hn.prototype.visitFloat64 = vn, hn.prototype.visitUtf8 = pn, hn.prototype.visitBinary = pn, hn.prototype.visitFixedSizeBinary = function(e, t) {
+            return e === t || dn(e, t) && e.byteWidth === t.byteWidth
+        }, hn.prototype.visitDate = bn, hn.prototype.visitDateDay = bn, hn.prototype.visitDateMillisecond = bn, hn.prototype.visitTimestamp = mn, hn.prototype.visitTimestampSecond = mn, hn.prototype.visitTimestampMillisecond = mn, hn.prototype.visitTimestampMicrosecond = mn, hn.prototype.visitTimestampNanosecond = mn, hn.prototype.visitTime = gn, hn.prototype.visitTimeSecond = gn, hn.prototype.visitTimeMillisecond = gn, hn.prototype.visitTimeMicrosecond = gn, hn.prototype.visitTimeNanosecond = gn, hn.prototype.visitDecimal = pn, hn.prototype.visitList = function(e, t) {
+            return e === t || dn(e, t) && e.children.length === t.children.length && On.compareFields(e.children, t.children)
+        }, hn.prototype.visitStruct = function(e, t) {
+            return e === t || dn(e, t) && e.children.length === t.children.length && On.compareFields(e.children, t.children)
+        }, hn.prototype.visitUnion = kn, hn.prototype.visitDenseUnion = kn, hn.prototype.visitSparseUnion = kn, hn.prototype.visitDictionary = function(e, t) {
+            return e === t || dn(e, t) && e.id === t.id && e.isOrdered === t.isOrdered && On.visit(e.indices, t.indices) && On.visit(e.dictionary, t.dictionary)
+        }, hn.prototype.visitInterval = wn, hn.prototype.visitIntervalDayTime = wn, hn.prototype.visitIntervalYearMonth = wn, hn.prototype.visitFixedSizeList = function(e, t) {
+            return e === t || dn(e, t) && e.listSize === t.listSize && e.children.length === t.children.length && On.compareFields(e.children, t.children)
+        }, hn.prototype.visitMap = function(e, t) {
+            return e === t || dn(e, t) && e.keysSorted === t.keysSorted && e.children.length === t.children.length && On.compareFields(e.children, t.children)
         };
-        var jn, Sn = new yn,
-            Tn = function() {
+        var _n, On = new hn,
+            jn = function() {
                 function e() {
                     Object(C.a)(this, e)
                 }
                 return Object(M.a)(e, [{
                     key: "typeId",
                     get: function() {
-                        return $t.NONE
+                        return Wt.NONE
                     }
                 }, {
                     key: "compareTo",
                     value: function(e) {
-                        return Sn.visit(this, e)
+                        return On.visit(this, e)
                     }
                 }], [{
                     key: "isNull",
                     value: function(e) {
-                        return e && e.typeId === $t.Null
+                        return e && e.typeId === Wt.Null
                     }
                 }, {
                     key: "isInt",
                     value: function(e) {
-                        return e && e.typeId === $t.Int
+                        return e && e.typeId === Wt.Int
                     }
                 }, {
                     key: "isFloat",
                     value: function(e) {
-                        return e && e.typeId === $t.Float
+                        return e && e.typeId === Wt.Float
                     }
                 }, {
                     key: "isBinary",
                     value: function(e) {
-                        return e && e.typeId === $t.Binary
+                        return e && e.typeId === Wt.Binary
                     }
                 }, {
                     key: "isUtf8",
                     value: function(e) {
-                        return e && e.typeId === $t.Utf8
+                        return e && e.typeId === Wt.Utf8
                     }
                 }, {
                     key: "isBool",
                     value: function(e) {
-                        return e && e.typeId === $t.Bool
+                        return e && e.typeId === Wt.Bool
                     }
                 }, {
                     key: "isDecimal",
                     value: function(e) {
-                        return e && e.typeId === $t.Decimal
+                        return e && e.typeId === Wt.Decimal
                     }
                 }, {
                     key: "isDate",
                     value: function(e) {
-                        return e && e.typeId === $t.Date
+                        return e && e.typeId === Wt.Date
                     }
                 }, {
                     key: "isTime",
                     value: function(e) {
-                        return e && e.typeId === $t.Time
+                        return e && e.typeId === Wt.Time
                     }
                 }, {
                     key: "isTimestamp",
                     value: function(e) {
-                        return e && e.typeId === $t.Timestamp
+                        return e && e.typeId === Wt.Timestamp
                     }
                 }, {
                     key: "isInterval",
                     value: function(e) {
-                        return e && e.typeId === $t.Interval
+                        return e && e.typeId === Wt.Interval
                     }
                 }, {
                     key: "isList",
                     value: function(e) {
-                        return e && e.typeId === $t.List
+                        return e && e.typeId === Wt.List
                     }
                 }, {
                     key: "isStruct",
                     value: function(e) {
-                        return e && e.typeId === $t.Struct
+                        return e && e.typeId === Wt.Struct
                     }
                 }, {
                     key: "isUnion",
                     value: function(e) {
-                        return e && e.typeId === $t.Union
+                        return e && e.typeId === Wt.Union
                     }
                 }, {
                     key: "isFixedSizeBinary",
                     value: function(e) {
-                        return e && e.typeId === $t.FixedSizeBinary
+                        return e && e.typeId === Wt.FixedSizeBinary
                     }
                 }, {
                     key: "isFixedSizeList",
                     value: function(e) {
-                        return e && e.typeId === $t.FixedSizeList
+                        return e && e.typeId === Wt.FixedSizeList
                     }
                 }, {
                     key: "isMap",
                     value: function(e) {
-                        return e && e.typeId === $t.Map
+                        return e && e.typeId === Wt.Map
                     }
                 }, {
                     key: "isDictionary",
                     value: function(e) {
-                        return e && e.typeId === $t.Dictionary
+                        return e && e.typeId === Wt.Dictionary
                     }
                 }]), e
             }();
-        Tn[Symbol.toStringTag] = ((jn = Tn.prototype).children = null, jn.ArrayType = Array, jn[Symbol.toStringTag] = "DataType");
-        var In = function(e) {
+        jn[Symbol.toStringTag] = ((_n = jn.prototype).children = null, _n.ArrayType = Array, _n[Symbol.toStringTag] = "DataType");
+        var xn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n() {
                 return Object(C.a)(this, n), t.apply(this, arguments)
             }
             return Object(M.a)(n, [{
                 key: "toString",
                 value: function() {
                     return "Null"
                 }
             }, {
                 key: "typeId",
                 get: function() {
-                    return $t.Null
+                    return Wt.Null
                 }
             }]), n
-        }(Tn);
-        In[Symbol.toStringTag] = function(e) {
+        }(jn);
+        xn[Symbol.toStringTag] = function(e) {
             return e[Symbol.toStringTag] = "Null"
-        }(In.prototype);
-        var En = function(e) {
+        }(xn.prototype);
+        var Sn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e, r) {
                 var i;
                 return Object(C.a)(this, n), (i = t.call(this)).isSigned = e, i.bitWidth = r, i
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Int
+                    return Wt.Int
                 }
             }, {
                 key: "ArrayType",
                 get: function() {
                     switch (this.bitWidth) {
                         case 8:
                             return this.isSigned ? Int8Array : Uint8Array;
@@ -5449,388 +5461,388 @@
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "".concat(this.isSigned ? "I" : "Ui", "nt").concat(this.bitWidth)
                 }
             }]), n
-        }(Tn);
-        En[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Sn[Symbol.toStringTag] = function(e) {
             return e.isSigned = null, e.bitWidth = null, e[Symbol.toStringTag] = "Int"
-        }(En.prototype);
-        var An = function(e) {
+        }(Sn.prototype);
+        var Tn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !0, 8)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Bn = function(e) {
+            }(Sn),
+            In = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !0, 16)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Dn = function(e) {
+            }(Sn),
+            En = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !0, 32)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Ln = function(e) {
+            }(Sn),
+            An = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !0, 64)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Fn = function(e) {
+            }(Sn),
+            Bn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !1, 8)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Cn = function(e) {
+            }(Sn),
+            Dn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !1, 16)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Mn = function(e) {
+            }(Sn),
+            Ln = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !1, 32)
                 }
                 return Object(M.a)(n)
-            }(En),
-            Nn = function(e) {
+            }(Sn),
+            Fn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.call(this, !1, 64)
                 }
                 return Object(M.a)(n)
-            }(En);
-        Object.defineProperty(An.prototype, "ArrayType", {
+            }(Sn);
+        Object.defineProperty(Tn.prototype, "ArrayType", {
             value: Int8Array
-        }), Object.defineProperty(Bn.prototype, "ArrayType", {
+        }), Object.defineProperty(In.prototype, "ArrayType", {
             value: Int16Array
-        }), Object.defineProperty(Dn.prototype, "ArrayType", {
+        }), Object.defineProperty(En.prototype, "ArrayType", {
             value: Int32Array
-        }), Object.defineProperty(Ln.prototype, "ArrayType", {
+        }), Object.defineProperty(An.prototype, "ArrayType", {
             value: Int32Array
-        }), Object.defineProperty(Fn.prototype, "ArrayType", {
+        }), Object.defineProperty(Bn.prototype, "ArrayType", {
             value: Uint8Array
-        }), Object.defineProperty(Cn.prototype, "ArrayType", {
+        }), Object.defineProperty(Dn.prototype, "ArrayType", {
             value: Uint16Array
-        }), Object.defineProperty(Mn.prototype, "ArrayType", {
+        }), Object.defineProperty(Ln.prototype, "ArrayType", {
             value: Uint32Array
-        }), Object.defineProperty(Nn.prototype, "ArrayType", {
+        }), Object.defineProperty(Fn.prototype, "ArrayType", {
             value: Uint32Array
         });
-        var Un = function(e) {
+        var Cn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r;
                 return Object(C.a)(this, n), (r = t.call(this)).precision = e, r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Float
+                    return Wt.Float
                 }
             }, {
                 key: "ArrayType",
                 get: function() {
                     switch (this.precision) {
-                        case Gt.HALF:
+                        case Kt.HALF:
                             return Uint16Array;
-                        case Gt.SINGLE:
+                        case Kt.SINGLE:
                             return Float32Array;
-                        case Gt.DOUBLE:
+                        case Kt.DOUBLE:
                             return Float64Array
                     }
                     throw new Error("Unrecognized ".concat(this[Symbol.toStringTag], " type"))
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "Float".concat(this.precision << 5 || 16)
                 }
             }]), n
-        }(Tn);
-        Un[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Cn[Symbol.toStringTag] = function(e) {
             return e.precision = null, e[Symbol.toStringTag] = "Float"
-        }(Un.prototype);
-        var Pn = function(e) {
+        }(Cn.prototype);
+        var Mn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
-                    return Object(C.a)(this, n), t.call(this, Gt.HALF)
+                    return Object(C.a)(this, n), t.call(this, Kt.HALF)
                 }
                 return Object(M.a)(n)
-            }(Un),
-            Rn = function(e) {
+            }(Cn),
+            Nn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
-                    return Object(C.a)(this, n), t.call(this, Gt.SINGLE)
+                    return Object(C.a)(this, n), t.call(this, Kt.SINGLE)
                 }
                 return Object(M.a)(n)
-            }(Un),
-            Vn = function(e) {
+            }(Cn),
+            Un = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
-                    return Object(C.a)(this, n), t.call(this, Gt.DOUBLE)
+                    return Object(C.a)(this, n), t.call(this, Kt.DOUBLE)
                 }
                 return Object(M.a)(n)
-            }(Un);
-        Object.defineProperty(Pn.prototype, "ArrayType", {
+            }(Cn);
+        Object.defineProperty(Mn.prototype, "ArrayType", {
             value: Uint16Array
-        }), Object.defineProperty(Rn.prototype, "ArrayType", {
+        }), Object.defineProperty(Nn.prototype, "ArrayType", {
             value: Float32Array
-        }), Object.defineProperty(Vn.prototype, "ArrayType", {
+        }), Object.defineProperty(Un.prototype, "ArrayType", {
             value: Float64Array
         });
-        var zn = function(e) {
+        var Pn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n() {
                 return Object(C.a)(this, n), t.call(this)
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Binary
+                    return Wt.Binary
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "Binary"
                 }
             }]), n
-        }(Tn);
-        zn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Pn[Symbol.toStringTag] = function(e) {
             return e.ArrayType = Uint8Array, e[Symbol.toStringTag] = "Binary"
-        }(zn.prototype);
-        var Wn = function(e) {
+        }(Pn.prototype);
+        var Rn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n() {
                 return Object(C.a)(this, n), t.call(this)
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Utf8
+                    return Wt.Utf8
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "Utf8"
                 }
             }]), n
-        }(Tn);
-        Wn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Rn[Symbol.toStringTag] = function(e) {
             return e.ArrayType = Uint8Array, e[Symbol.toStringTag] = "Utf8"
-        }(Wn.prototype);
-        var Yn = function(e) {
+        }(Rn.prototype);
+        var Vn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n() {
                 return Object(C.a)(this, n), t.call(this)
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Bool
+                    return Wt.Bool
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "Bool"
                 }
             }]), n
-        }(Tn);
-        Yn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Vn[Symbol.toStringTag] = function(e) {
             return e.ArrayType = Uint8Array, e[Symbol.toStringTag] = "Bool"
-        }(Yn.prototype);
-        var Hn = function(e) {
+        }(Vn.prototype);
+        var zn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e, r) {
                 var i;
                 return Object(C.a)(this, n), (i = t.call(this)).scale = e, i.precision = r, i
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Decimal
+                    return Wt.Decimal
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "Decimal[".concat(this.precision, "e").concat(this.scale > 0 ? "+" : "").concat(this.scale, "]")
                 }
             }]), n
-        }(Tn);
-        Hn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        zn[Symbol.toStringTag] = function(e) {
             return e.scale = null, e.precision = null, e.ArrayType = Uint32Array, e[Symbol.toStringTag] = "Decimal"
-        }(Hn.prototype);
-        var $n = function(e) {
+        }(zn.prototype);
+        var Wn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r;
                 return Object(C.a)(this, n), (r = t.call(this)).unit = e, r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Date
+                    return Wt.Date
                 }
             }, {
                 key: "toString",
                 value: function() {
-                    return "Date".concat(32 * (this.unit + 1), "<").concat(Qt[this.unit], ">")
+                    return "Date".concat(32 * (this.unit + 1), "<").concat(Ht[this.unit], ">")
                 }
             }]), n
-        }(Tn);
-        $n[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Wn[Symbol.toStringTag] = function(e) {
             return e.unit = null, e.ArrayType = Int32Array, e[Symbol.toStringTag] = "Date"
-        }($n.prototype);
-        var Kn = function(e) {
+        }(Wn.prototype);
+        var Yn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
-                    return Object(C.a)(this, n), t.call(this, Qt.DAY)
+                    return Object(C.a)(this, n), t.call(this, Ht.DAY)
                 }
                 return Object(M.a)(n)
-            }($n),
-            Qn = function(e) {
+            }(Wn),
+            Hn = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
-                    return Object(C.a)(this, n), t.call(this, Qt.MILLISECOND)
+                    return Object(C.a)(this, n), t.call(this, Ht.MILLISECOND)
                 }
                 return Object(M.a)(n)
-            }($n),
-            qn = function(e) {
+            }(Wn),
+            $n = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     var i;
                     return Object(C.a)(this, n), (i = t.call(this)).unit = e, i.bitWidth = r, i
                 }
                 return Object(M.a)(n, [{
                     key: "typeId",
                     get: function() {
-                        return $t.Time
+                        return Wt.Time
                     }
                 }, {
                     key: "toString",
                     value: function() {
-                        return "Time".concat(this.bitWidth, "<").concat(qt[this.unit], ">")
+                        return "Time".concat(this.bitWidth, "<").concat($t[this.unit], ">")
                     }
                 }]), n
-            }(Tn);
-        qn[Symbol.toStringTag] = function(e) {
+            }(jn);
+        $n[Symbol.toStringTag] = function(e) {
             return e.unit = null, e.bitWidth = null, e.ArrayType = Int32Array, e[Symbol.toStringTag] = "Time"
-        }(qn.prototype);
-        var Gn = function(e) {
+        }($n.prototype);
+        var Kn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e, r) {
                 var i;
                 return Object(C.a)(this, n), (i = t.call(this)).unit = e, i.timezone = r, i
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Timestamp
+                    return Wt.Timestamp
                 }
             }, {
                 key: "toString",
                 value: function() {
-                    return "Timestamp<".concat(qt[this.unit]).concat(this.timezone ? ", ".concat(this.timezone) : "", ">")
+                    return "Timestamp<".concat($t[this.unit]).concat(this.timezone ? ", ".concat(this.timezone) : "", ">")
                 }
             }]), n
-        }(Tn);
-        Gn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Kn[Symbol.toStringTag] = function(e) {
             return e.unit = null, e.timezone = null, e.ArrayType = Int32Array, e[Symbol.toStringTag] = "Timestamp"
-        }(Gn.prototype);
-        var Jn = function(e) {
+        }(Kn.prototype);
+        var Qn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r;
                 return Object(C.a)(this, n), (r = t.call(this)).unit = e, r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Interval
+                    return Wt.Interval
                 }
             }, {
                 key: "toString",
                 value: function() {
-                    return "Interval<".concat(Zt[this.unit], ">")
+                    return "Interval<".concat(qt[this.unit], ">")
                 }
             }]), n
-        }(Tn);
-        Jn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Qn[Symbol.toStringTag] = function(e) {
             return e.unit = null, e.ArrayType = Int32Array, e[Symbol.toStringTag] = "Interval"
-        }(Jn.prototype);
-        var Zn = function(e) {
+        }(Qn.prototype);
+        var qn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r;
                 return Object(C.a)(this, n), (r = t.call(this)).children = [e], r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.List
+                    return Wt.List
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "List<".concat(this.valueType, ">")
                 }
             }, {
@@ -5845,105 +5857,105 @@
                 }
             }, {
                 key: "ArrayType",
                 get: function() {
                     return this.valueType.ArrayType
                 }
             }]), n
-        }(Tn);
-        Zn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        qn[Symbol.toStringTag] = function(e) {
             return e.children = null, e[Symbol.toStringTag] = "List"
-        }(Zn.prototype);
-        var Xn = function(e) {
+        }(qn.prototype);
+        var Gn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r;
                 return Object(C.a)(this, n), (r = t.call(this)).children = e, r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Struct
+                    return Wt.Struct
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "Struct<{".concat(this.children.map((function(e) {
                         return "".concat(e.name, ":").concat(e.type)
                     })).join(", "), "}>")
                 }
             }]), n
-        }(Tn);
-        Xn[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Gn[Symbol.toStringTag] = function(e) {
             return e.children = null, e[Symbol.toStringTag] = "Struct"
-        }(Xn.prototype);
-        var er = function(e) {
+        }(Gn.prototype);
+        var Jn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e, r, i) {
                 var a;
                 return Object(C.a)(this, n), (a = t.call(this)).mode = e, a.children = i, a.typeIds = r = Int32Array.from(r), a.typeIdToChildIndex = r.reduce((function(e, t, n) {
                     return (e[t] = n) && e || e
                 }), Object.create(null)), a
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Union
+                    return Wt.Union
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "".concat(this[Symbol.toStringTag], "<").concat(this.children.map((function(e) {
                         return "".concat(e.type)
                     })).join(" | "), ">")
                 }
             }]), n
-        }(Tn);
-        er[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Jn[Symbol.toStringTag] = function(e) {
             return e.mode = null, e.typeIds = null, e.children = null, e.typeIdToChildIndex = null, e.ArrayType = Int8Array, e[Symbol.toStringTag] = "Union"
-        }(er.prototype);
-        var tr = function(e) {
+        }(Jn.prototype);
+        var Zn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r;
                 return Object(C.a)(this, n), (r = t.call(this)).byteWidth = e, r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.FixedSizeBinary
+                    return Wt.FixedSizeBinary
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "FixedSizeBinary[".concat(this.byteWidth, "]")
                 }
             }]), n
-        }(Tn);
-        tr[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Zn[Symbol.toStringTag] = function(e) {
             return e.byteWidth = null, e.ArrayType = Uint8Array, e[Symbol.toStringTag] = "FixedSizeBinary"
-        }(tr.prototype);
-        var nr = function(e) {
+        }(Zn.prototype);
+        var Xn = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e, r) {
                 var i;
                 return Object(C.a)(this, n), (i = t.call(this)).listSize = e, i.children = [r], i
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.FixedSizeList
+                    return Wt.FixedSizeList
                 }
             }, {
                 key: "valueType",
                 get: function() {
                     return this.children[0].type
                 }
             }, {
@@ -5958,30 +5970,30 @@
                 }
             }, {
                 key: "toString",
                 value: function() {
                     return "FixedSizeList[".concat(this.listSize, "]<").concat(this.valueType, ">")
                 }
             }]), n
-        }(Tn);
-        nr[Symbol.toStringTag] = function(e) {
+        }(jn);
+        Xn[Symbol.toStringTag] = function(e) {
             return e.children = null, e.listSize = null, e[Symbol.toStringTag] = "FixedSizeList"
-        }(nr.prototype);
-        var rr = function(e) {
+        }(Xn.prototype);
+        var er = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n(e) {
                 var r, i = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                 return Object(C.a)(this, n), (r = t.call(this)).children = [e], r.keysSorted = i, r
             }
             return Object(M.a)(n, [{
                 key: "typeId",
                 get: function() {
-                    return $t.Map
+                    return Wt.Map
                 }
             }, {
                 key: "keyType",
                 get: function() {
                     return this.children[0].type.children[0].type
                 }
             }, {
@@ -5993,33 +6005,33 @@
                 key: "toString",
                 value: function() {
                     return "Map<{".concat(this.children[0].type.children.map((function(e) {
                         return "".concat(e.name, ":").concat(e.type)
                     })).join(", "), "}>")
                 }
             }]), n
-        }(Tn);
-        rr[Symbol.toStringTag] = function(e) {
+        }(jn);
+        er[Symbol.toStringTag] = function(e) {
             return e.children = null, e.keysSorted = null, e[Symbol.toStringTag] = "Map_"
-        }(rr.prototype);
-        var ir, ar = (ir = -1, function() {
-                return ++ir
+        }(er.prototype);
+        var tr, nr = (tr = -1, function() {
+                return ++tr
             }),
-            or = function(e) {
+            rr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r, i, a) {
                     var o;
-                    return Object(C.a)(this, n), (o = t.call(this)).indices = r, o.dictionary = e, o.isOrdered = a || !1, o.id = null == i ? ar() : "number" === typeof i ? i : i.low, o
+                    return Object(C.a)(this, n), (o = t.call(this)).indices = r, o.dictionary = e, o.isOrdered = a || !1, o.id = null == i ? nr() : "number" === typeof i ? i : i.low, o
                 }
                 return Object(M.a)(n, [{
                     key: "typeId",
                     get: function() {
-                        return $t.Dictionary
+                        return Wt.Dictionary
                     }
                 }, {
                     key: "children",
                     get: function() {
                         return this.dictionary.children
                     }
                 }, {
@@ -6034,46 +6046,46 @@
                     }
                 }, {
                     key: "toString",
                     value: function() {
                         return "Dictionary<".concat(this.indices, ", ").concat(this.dictionary, ">")
                     }
                 }]), n
-            }(Tn);
+            }(jn);
 
-        function ur(e) {
+        function ir(e) {
             var t = e;
             switch (e.typeId) {
-                case $t.Decimal:
+                case Wt.Decimal:
                     return 4;
-                case $t.Timestamp:
+                case Wt.Timestamp:
                     return 2;
-                case $t.Date:
-                case $t.Interval:
+                case Wt.Date:
+                case Wt.Interval:
                     return 1 + t.unit;
-                case $t.Int:
-                case $t.Time:
+                case Wt.Int:
+                case Wt.Time:
                     return +(t.bitWidth > 32) + 1;
-                case $t.FixedSizeList:
+                case Wt.FixedSizeList:
                     return t.listSize;
-                case $t.FixedSizeBinary:
+                case Wt.FixedSizeBinary:
                     return t.byteWidth;
                 default:
                     return 1
             }
         }
-        or[Symbol.toStringTag] = function(e) {
+        rr[Symbol.toStringTag] = function(e) {
             return e.id = null, e.indices = null, e.isOrdered = null, e.dictionary = null, e[Symbol.toStringTag] = "Dictionary"
-        }(or.prototype);
-        var sr = function() {
+        }(rr.prototype);
+        var ar = function() {
             function e(t, n, r, i, a, o, u) {
                 var s;
                 Object(C.a)(this, e), this.type = t, this.dictionary = u, this.offset = Math.floor(Math.max(n || 0, 0)), this.length = Math.floor(Math.max(r || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), this.childData = (o || []).map((function(t) {
                     return t instanceof e ? t : t.data
-                })), a instanceof e ? (this.stride = a.stride, this.values = a.values, this.typeIds = a.typeIds, this.nullBitmap = a.nullBitmap, this.valueOffsets = a.valueOffsets) : (this.stride = ur(t), a && ((s = a[0]) && (this.valueOffsets = s), (s = a[1]) && (this.values = s), (s = a[2]) && (this.nullBitmap = s), (s = a[3]) && (this.typeIds = s)))
+                })), a instanceof e ? (this.stride = a.stride, this.values = a.values, this.typeIds = a.typeIds, this.nullBitmap = a.nullBitmap, this.valueOffsets = a.valueOffsets) : (this.stride = ir(t), a && ((s = a[0]) && (this.valueOffsets = s), (s = a[1]) && (this.values = s), (s = a[2]) && (this.nullBitmap = s), (s = a[3]) && (this.typeIds = s)))
             }
             return Object(M.a)(e, [{
                 key: "typeId",
                 get: function() {
                     return this.type.typeId
                 }
             }, {
@@ -6098,15 +6110,15 @@
                         return e + t.byteLength
                     }), e)
                 }
             }, {
                 key: "nullCount",
                 get: function() {
                     var e, t = this._nullCount;
-                    return t <= -1 && (e = this.nullBitmap) && (this._nullCount = t = this.length - cn(e, this.offset, this.offset + this.length)), t
+                    return t <= -1 && (e = this.nullBitmap) && (this._nullCount = t = this.length - on(e, this.offset, this.offset + this.length)), t
                 }
             }, {
                 key: "clone",
                 value: function(t) {
                     return new e(t, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.offset, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.length, arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : this._nullCount, arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : this, arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : this.childData, this.dictionary)
                 }
             }, {
@@ -6119,75 +6131,75 @@
                         o = 16 === r ? n : 1,
                         u = this._sliceBuffers(e, t, n, r);
                     return this.clone(this.type, this.offset + e, t, a, u, !i.length || this.valueOffsets ? i : this._sliceChildren(i, o * e, o * t))
                 }
             }, {
                 key: "_changeLengthAndBackfillNullBitmap",
                 value: function(e) {
-                    if (this.typeId === $t.Null) return this.clone(this.type, 0, e, 0);
+                    if (this.typeId === Wt.Null) return this.clone(this.type, 0, e, 0);
                     var t = this.length,
                         n = this.nullCount,
                         r = new Uint8Array((e + 63 & -64) >> 3).fill(255, 0, t >> 3);
-                    r[t >> 3] = (1 << t - (-8 & t)) - 1, n > 0 && r.set(on(this.offset, t, this.nullBitmap), 0);
+                    r[t >> 3] = (1 << t - (-8 & t)) - 1, n > 0 && r.set(nn(this.offset, t, this.nullBitmap), 0);
                     var i = this.buffers;
-                    return i[Kt.VALIDITY] = r, this.clone(this.type, 0, e, n + (e - t), i)
+                    return i[Yt.VALIDITY] = r, this.clone(this.type, 0, e, n + (e - t), i)
                 }
             }, {
                 key: "_sliceBuffers",
                 value: function(e, t, n, r) {
                     var i, a = this.buffers;
-                    return (i = a[Kt.TYPE]) && (a[Kt.TYPE] = i.subarray(e, e + t)), (i = a[Kt.OFFSET]) && (a[Kt.OFFSET] = i.subarray(e, e + t + 1)) || (i = a[Kt.DATA]) && (a[Kt.DATA] = 6 === r ? i : i.subarray(n * e, n * (e + t))), a
+                    return (i = a[Yt.TYPE]) && (a[Yt.TYPE] = i.subarray(e, e + t)), (i = a[Yt.OFFSET]) && (a[Yt.OFFSET] = i.subarray(e, e + t + 1)) || (i = a[Yt.DATA]) && (a[Yt.DATA] = 6 === r ? i : i.subarray(n * e, n * (e + t))), a
                 }
             }, {
                 key: "_sliceChildren",
                 value: function(e, t, n) {
                     return e.map((function(e) {
                         return e.slice(t, n)
                     }))
                 }
             }], [{
                 key: "new",
                 value: function(t, n, r, i, a, o, u) {
                     switch (a instanceof e ? a = a.buffers : a || (a = []), t.typeId) {
-                        case $t.Null:
+                        case Wt.Null:
                             return e.Null(t, n, r);
-                        case $t.Int:
-                            return e.Int(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Dictionary:
-                            return e.Dictionary(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || [], u);
-                        case $t.Float:
-                            return e.Float(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Bool:
-                            return e.Bool(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Decimal:
-                            return e.Decimal(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Date:
-                            return e.Date(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Time:
-                            return e.Time(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Timestamp:
-                            return e.Timestamp(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Interval:
-                            return e.Interval(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.FixedSizeBinary:
-                            return e.FixedSizeBinary(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.DATA] || []);
-                        case $t.Binary:
-                            return e.Binary(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.OFFSET] || [], a[Kt.DATA] || []);
-                        case $t.Utf8:
-                            return e.Utf8(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.OFFSET] || [], a[Kt.DATA] || []);
-                        case $t.List:
-                            return e.List(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.OFFSET] || [], (o || [])[0]);
-                        case $t.FixedSizeList:
-                            return e.FixedSizeList(t, n, r, i || 0, a[Kt.VALIDITY], (o || [])[0]);
-                        case $t.Struct:
-                            return e.Struct(t, n, r, i || 0, a[Kt.VALIDITY], o || []);
-                        case $t.Map:
-                            return e.Map(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.OFFSET] || [], (o || [])[0]);
-                        case $t.Union:
-                            return e.Union(t, n, r, i || 0, a[Kt.VALIDITY], a[Kt.TYPE] || [], a[Kt.OFFSET] || o, o)
+                        case Wt.Int:
+                            return e.Int(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Dictionary:
+                            return e.Dictionary(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || [], u);
+                        case Wt.Float:
+                            return e.Float(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Bool:
+                            return e.Bool(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Decimal:
+                            return e.Decimal(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Date:
+                            return e.Date(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Time:
+                            return e.Time(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Timestamp:
+                            return e.Timestamp(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Interval:
+                            return e.Interval(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.FixedSizeBinary:
+                            return e.FixedSizeBinary(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.DATA] || []);
+                        case Wt.Binary:
+                            return e.Binary(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.OFFSET] || [], a[Yt.DATA] || []);
+                        case Wt.Utf8:
+                            return e.Utf8(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.OFFSET] || [], a[Yt.DATA] || []);
+                        case Wt.List:
+                            return e.List(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.OFFSET] || [], (o || [])[0]);
+                        case Wt.FixedSizeList:
+                            return e.FixedSizeList(t, n, r, i || 0, a[Yt.VALIDITY], (o || [])[0]);
+                        case Wt.Struct:
+                            return e.Struct(t, n, r, i || 0, a[Yt.VALIDITY], o || []);
+                        case Wt.Map:
+                            return e.Map(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.OFFSET] || [], (o || [])[0]);
+                        case Wt.Union:
+                            return e.Union(t, n, r, i || 0, a[Yt.VALIDITY], a[Yt.TYPE] || [], a[Yt.OFFSET] || o, o)
                     }
                     throw new Error("Unrecognized typeId ".concat(t.typeId))
                 }
             }, {
                 key: "Null",
                 value: function(t, n, r) {
                     return new e(t, n, r, 0)
@@ -6272,54 +6284,54 @@
                 value: function(t, n, r, i, a, o, u) {
                     return new e(t, n, r, i, [We(o), void 0, He(a)], [u])
                 }
             }, {
                 key: "Union",
                 value: function(t, n, r, i, a, o, u, s) {
                     var c = [void 0, void 0, He(a), Re(t.ArrayType, o)];
-                    return t.mode === Jt.Sparse ? new e(t, n, r, i, c, u) : (c[Kt.OFFSET] = We(u), new e(t, n, r, i, c, s))
+                    return t.mode === Qt.Sparse ? new e(t, n, r, i, c, u) : (c[Yt.OFFSET] = We(u), new e(t, n, r, i, c, s))
                 }
             }]), e
         }();
-        sr.prototype.childData = Object.freeze([]);
-        var cr = void 0;
+        ar.prototype.childData = Object.freeze([]);
+        var or = void 0;
 
-        function lr(e) {
+        function ur(e) {
             if (null === e) return "null";
-            if (e === cr) return "undefined";
+            if (e === or) return "undefined";
             switch (typeof e) {
                 case "number":
                 case "bigint":
                     return "".concat(e);
                 case "string":
                     return '"'.concat(e, '"')
             }
             return "function" === typeof e[Symbol.toPrimitive] ? e[Symbol.toPrimitive]("string") : ArrayBuffer.isView(e) ? "[".concat(e, "]") : JSON.stringify(e)
         }
 
-        function fr(e) {
+        function sr(e) {
             if (!e || e.length <= 0) return function(e) {
                 return !0
             };
             var t = "",
                 n = e.filter((function(e) {
                     return e === e
                 }));
             return n.length > 0 && (t = "\n    switch (x) {".concat(n.map((function(e) {
                 return "\n        case ".concat(function(e) {
-                    if ("bigint" !== typeof e) return lr(e);
-                    if (be) return "".concat(lr(e), "n");
-                    return '"'.concat(lr(e), '"')
+                    if ("bigint" !== typeof e) return ur(e);
+                    if (be) return "".concat(ur(e), "n");
+                    return '"'.concat(ur(e), '"')
                 }(e), ":")
             })).join(""), "\n            return false;\n    }")), e.length !== n.length && (t = "if (x !== x) return false;\n".concat(t)), new Function("x", "".concat(t, "\nreturn true;"))
         }
-        var hr = function(e, t) {
+        var cr = function(e, t) {
                 return (e * t + 63 & -64 || 64) / t
             },
-            dr = function() {
+            lr = function() {
                 function e(t) {
                     var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 1;
                     Object(C.a)(this, e), this.buffer = t, this.stride = n, this.BYTES_PER_ELEMENT = t.BYTES_PER_ELEMENT, this.ArrayType = t.constructor, this._resize(this.length = t.length / n | 0)
                 }
                 return Object(M.a)(e, [{
                     key: "byteLength",
                     get: function() {
@@ -6349,23 +6361,23 @@
                     key: "reserve",
                     value: function(e) {
                         if (e > 0) {
                             this.length += e;
                             var t = this.stride,
                                 n = this.length * t,
                                 r = this.buffer.length;
-                            n >= r && this._resize(hr(0 === r ? 1 * n : 2 * n, this.BYTES_PER_ELEMENT))
+                            n >= r && this._resize(cr(0 === r ? 1 * n : 2 * n, this.BYTES_PER_ELEMENT))
                         }
                         return this
                     }
                 }, {
                     key: "flush",
                     value: function() {
                         var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.length;
-                        e = hr(e * this.stride, this.BYTES_PER_ELEMENT);
+                        e = cr(e * this.stride, this.BYTES_PER_ELEMENT);
                         var t = function(e) {
                             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
                             return e.length >= t ? e.subarray(0, t) : Ue(new e.constructor(t), e, 0)
                         }(this.buffer, e);
                         return this.clear(), t
                     }
                 }, {
@@ -6376,16 +6388,16 @@
                 }, {
                     key: "_resize",
                     value: function(e) {
                         return this.buffer = Ue(new this.ArrayType(e), this.buffer)
                     }
                 }]), e
             }();
-        dr.prototype.offset = 0;
-        var pr = function(e) {
+        lr.prototype.offset = 0;
+        var fr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -6400,16 +6412,16 @@
                     }
                 }, {
                     key: "set",
                     value: function(e, t) {
                         return this.reserve(e - this.length + 1), this.buffer[e * this.stride] = t, this
                     }
                 }]), n
-            }(dr),
-            yr = function(e) {
+            }(lr),
+            hr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e, r = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : new Uint8Array(0);
                     return Object(C.a)(this, n), (e = t.call(this, r, 1 / 8)).numValid = 0, e
                 }
@@ -6431,19 +6443,19 @@
                             i = e % 8,
                             a = n[r] >> i & 1;
                         return t ? 0 === a && (n[r] |= 1 << i, ++this.numValid) : 1 === a && (n[r] &= ~(1 << i), --this.numValid), this
                     }
                 }, {
                     key: "clear",
                     value: function() {
-                        return this.numValid = 0, Ut(Object(Nt.a)(n.prototype), "clear", this).call(this)
+                        return this.numValid = 0, Ct(Object(Ft.a)(n.prototype), "clear", this).call(this)
                     }
                 }]), n
-            }(pr),
-            vr = function(e) {
+            }(fr),
+            dr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : new Int32Array(1);
                     return Object(C.a)(this, n), t.call(this, e, 1)
                 }
@@ -6459,19 +6471,19 @@
                             r = this.reserve(e - n + 1).buffer;
                         return n < e++ && r.fill(r[n], n, e), r[e] = r[e - 1] + t, this
                     }
                 }, {
                     key: "flush",
                     value: function() {
                         var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.length - 1;
-                        return e > this.length && this.set(e - 1, 0), Ut(Object(Nt.a)(n.prototype), "flush", this).call(this, e + 1)
+                        return e > this.length && this.set(e - 1, 0), Ct(Object(Ft.a)(n.prototype), "flush", this).call(this, e + 1)
                     }
                 }]), n
-            }(pr),
-            br = function(e) {
+            }(fr),
+            pr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -6493,30 +6505,30 @@
                                 this.buffer.set(t, e * this.stride)
                         }
                         return this
                     }
                 }, {
                     key: "_resize",
                     value: function(e) {
-                        var t = Ut(Object(Nt.a)(n.prototype), "_resize", this).call(this, e),
+                        var t = Ct(Object(Ft.a)(n.prototype), "_resize", this).call(this, e),
                             r = t.byteLength / (this.BYTES_PER_ELEMENT * this.stride);
                         return be && (this.buffer64 = new this.ArrayType64(t.buffer, t.byteOffset, r)), t
                     }
                 }]), n
-            }(dr),
-            mr = function() {
+            }(lr),
+            yr = function() {
                 function e(t) {
                     var n = t.type,
                         r = t.nullValues;
-                    Object(C.a)(this, e), this.length = 0, this.finished = !1, this.type = n, this.children = [], this.nullValues = r, this.stride = ur(n), this._nulls = new yr, r && r.length > 0 && (this._isValid = fr(r))
+                    Object(C.a)(this, e), this.length = 0, this.finished = !1, this.type = n, this.children = [], this.nullValues = r, this.stride = ir(n), this._nulls = new hr, r && r.length > 0 && (this._isValid = sr(r))
                 }
                 return Object(M.a)(e, [{
                     key: "toVector",
                     value: function() {
-                        return Ht.new(this.flush())
+                        return zt.new(this.flush())
                     }
                 }, {
                     key: "ArrayType",
                     get: function() {
                         return this.type.ArrayType
                     }
                 }, {
@@ -6611,16 +6623,16 @@
                     value: function() {
                         var e = [],
                             t = this._values,
                             n = this._offsets,
                             r = this._typeIds,
                             i = this.length,
                             a = this.nullCount;
-                        r ? (e[Kt.TYPE] = r.flush(i), n && (e[Kt.OFFSET] = n.flush(i))) : n ? (t && (e[Kt.DATA] = t.flush(n.last())), e[Kt.OFFSET] = n.flush(i)) : t && (e[Kt.DATA] = t.flush(i)), a > 0 && (e[Kt.VALIDITY] = this._nulls.flush(i));
-                        var o = sr.new(this.type, 0, i, a, e, this.children.map((function(e) {
+                        r ? (e[Yt.TYPE] = r.flush(i), n && (e[Yt.OFFSET] = n.flush(i))) : n ? (t && (e[Yt.DATA] = t.flush(n.last())), e[Yt.OFFSET] = n.flush(i)) : t && (e[Yt.DATA] = t.flush(i)), a > 0 && (e[Yt.VALIDITY] = this._nulls.flush(i));
+                        var o = ar.new(this.type, 0, i, a, e, this.children.map((function(e) {
                             return e.flush()
                         })));
                         return this.clear(), o
                     }
                 }, {
                     key: "finish",
                     value: function() {
@@ -6658,15 +6670,15 @@
                                 i = void 0 === r ? "bytes" !== n ? 1e3 : Math.pow(2, 14) : r,
                                 a = "bytes" !== n ? "length" : "byteLength";
                             return U().mark((function t(n) {
                                 var r, o, u, s, c;
                                 return U().wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
-                                            r = 0, o = mr.new(e), u = D(n), t.prev = 3, u.s();
+                                            r = 0, o = yr.new(e), u = D(n), t.prev = 3, u.s();
                                         case 5:
                                             if ((s = u.n()).done) {
                                                 t.next = 14;
                                                 break
                                             }
                                             if (c = s.value, !(o.append(c)[a] >= i)) {
                                                 t.next = 12;
@@ -6714,15 +6726,15 @@
                                 a = "bytes" !== n ? "length" : "byteLength";
                             return function() {
                                 var t = W(U().mark((function t(n) {
                                     var r, o, u, s, c, l, f, h;
                                     return U().wrap((function(t) {
                                         for (;;) switch (t.prev = t.next) {
                                             case 0:
-                                                r = 0, o = mr.new(e), u = !1, s = !1, t.prev = 4, l = H(n);
+                                                r = 0, o = yr.new(e), u = !1, s = !1, t.prev = 4, l = H(n);
                                             case 6:
                                                 return t.next = 8, V(l.next());
                                             case 8:
                                                 if (!(u = !(f = t.sent).done)) {
                                                     t.next = 18;
                                                     break
                                                 }
@@ -6778,93 +6790,93 @@
                                     return t.apply(this, arguments)
                                 }
                             }()
                         }(e)
                     }
                 }]), e
             }();
-        mr.prototype.length = 1, mr.prototype.stride = 1, mr.prototype.children = null, mr.prototype.finished = !1, mr.prototype.nullValues = null, mr.prototype._isValid = function() {
+        yr.prototype.length = 1, yr.prototype.stride = 1, yr.prototype.children = null, yr.prototype.finished = !1, yr.prototype.nullValues = null, yr.prototype._isValid = function() {
             return !0
         };
-        var gr = function(e) {
+        var vr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new pr(new r.ArrayType(0), r.stride), r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new fr(new r.ArrayType(0), r.stride), r
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
                         var r = this._values;
-                        return r.reserve(e - r.length + 1), Ut(Object(Nt.a)(n.prototype), "setValue", this).call(this, e, t)
+                        return r.reserve(e - r.length + 1), Ct(Object(Ft.a)(n.prototype), "setValue", this).call(this, e, t)
                     }
                 }]), n
-            }(mr),
-            kr = function(e) {
+            }(yr),
+            br = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._pendingLength = 0, r._offsets = new vr, r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._pendingLength = 0, r._offsets = new dr, r
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
                         var n = this._pending || (this._pending = new Map),
                             r = n.get(e);
                         r && (this._pendingLength -= r.length), this._pendingLength += t.length, n.set(e, t)
                     }
                 }, {
                     key: "setValid",
                     value: function(e, t) {
-                        return !!Ut(Object(Nt.a)(n.prototype), "setValid", this).call(this, e, t) || ((this._pending || (this._pending = new Map)).set(e, void 0), !1)
+                        return !!Ct(Object(Ft.a)(n.prototype), "setValid", this).call(this, e, t) || ((this._pending || (this._pending = new Map)).set(e, void 0), !1)
                     }
                 }, {
                     key: "clear",
                     value: function() {
-                        return this._pendingLength = 0, this._pending = void 0, Ut(Object(Nt.a)(n.prototype), "clear", this).call(this)
+                        return this._pendingLength = 0, this._pending = void 0, Ct(Object(Ft.a)(n.prototype), "clear", this).call(this)
                     }
                 }, {
                     key: "flush",
                     value: function() {
-                        return this._flush(), Ut(Object(Nt.a)(n.prototype), "flush", this).call(this)
+                        return this._flush(), Ct(Object(Ft.a)(n.prototype), "flush", this).call(this)
                     }
                 }, {
                     key: "finish",
                     value: function() {
-                        return this._flush(), Ut(Object(Nt.a)(n.prototype), "finish", this).call(this)
+                        return this._flush(), Ct(Object(Ft.a)(n.prototype), "finish", this).call(this)
                     }
                 }, {
                     key: "_flush",
                     value: function() {
                         var e = this._pending,
                             t = this._pendingLength;
                         return this._pendingLength = 0, this._pending = void 0, e && e.size > 0 && this._flushPending(e, t), this
                     }
                 }]), n
-            }(mr);
-        var wr = function(e) {
+            }(yr);
+        var mr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new yr, r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new hr, r
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
                         this._values.set(e, +t)
                     }
                 }]), n
-            }(mr),
-            _r = function(e) {
+            }(yr),
+            gr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -6872,65 +6884,65 @@
                     value: function(e, t) {}
                 }, {
                     key: "setValid",
                     value: function(e, t) {
                         return this.length = Math.max(e + 1, this.length), t
                     }
                 }]), n
-            }(mr),
-            Or = function(e) {
+            }(yr),
+            kr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            xr = function(e) {
+            }(vr),
+            wr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Or),
-            jr = function(e) {
+            }(kr),
+            _r = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Or),
-            Sr = function(e) {
+            }(kr),
+            Or = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            Tr = function(e) {
+            }(vr),
+            jr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r, i = e.type,
                         a = e.nullValues,
                         o = e.dictionaryHashFunction;
                     return Object(C.a)(this, n), (r = t.call(this, {
-                        type: new or(i.dictionary, i.indices, i.id, i.isOrdered)
-                    }))._nulls = null, r._dictionaryOffset = 0, r._keysToIndices = Object.create(null), r.indices = mr.new({
+                        type: new rr(i.dictionary, i.indices, i.id, i.isOrdered)
+                    }))._nulls = null, r._dictionaryOffset = 0, r._keysToIndices = Object.create(null), r.indices = yr.new({
                         type: r.type.indices,
                         nullValues: a
-                    }), r.dictionary = mr.new({
+                    }), r.dictionary = yr.new({
                         type: r.type.dictionary,
                         nullValues: null
                     }), "function" === typeof o && (r.valueToKey = o), r
                 }
                 return Object(M.a)(n, [{
                     key: "values",
                     get: function() {
@@ -6988,486 +7000,486 @@
                             n = this.dictionary.toVector(),
                             r = this.indices.flush().clone(e);
                         return r.dictionary = t ? t.concat(n) : n, this.finished || (this._dictionaryOffset += n.length), this._dictionary = r.dictionary, this.clear(), r
                     }
                 }, {
                     key: "finish",
                     value: function() {
-                        return this.indices.finish(), this.dictionary.finish(), this._dictionaryOffset = 0, this._keysToIndices = Object.create(null), Ut(Object(Nt.a)(n.prototype), "finish", this).call(this)
+                        return this.indices.finish(), this.dictionary.finish(), this._dictionaryOffset = 0, this._keysToIndices = Object.create(null), Ct(Object(Ft.a)(n.prototype), "finish", this).call(this)
                     }
                 }, {
                     key: "clear",
                     value: function() {
-                        return this.indices.clear(), this.dictionary.clear(), Ut(Object(Nt.a)(n.prototype), "clear", this).call(this)
+                        return this.indices.clear(), this.dictionary.clear(), Ct(Object(Ft.a)(n.prototype), "clear", this).call(this)
                     }
                 }, {
                     key: "valueToKey",
                     value: function(e) {
                         return "string" === typeof e ? e : "".concat(e)
                     }
                 }]), n
-            }(mr),
-            Ir = function(e) {
+            }(yr),
+            xr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            Er = new Float64Array(1),
-            Ar = new Uint32Array(Er.buffer);
+            }(vr),
+            Sr = new Float64Array(1),
+            Tr = new Uint32Array(Sr.buffer);
 
-        function Br(e) {
+        function Ir(e) {
             var t = (31744 & e) >> 10,
                 n = (1023 & e) / 1024,
                 r = Math.pow(-1, (32768 & e) >> 15);
             switch (t) {
                 case 31:
                     return r * (n ? NaN : 1 / 0);
                 case 0:
                     return r * (n ? 6103515625e-14 * n : 0)
             }
             return r * Math.pow(2, t - 15) * (1 + n)
         }
 
-        function Dr(e) {
+        function Er(e) {
             if (e !== e) return 32256;
-            Er[0] = e;
-            var t = (2147483648 & Ar[1]) >> 16 & 65535,
-                n = 2146435072 & Ar[1],
+            Sr[0] = e;
+            var t = (2147483648 & Tr[1]) >> 16 & 65535,
+                n = 2146435072 & Tr[1],
                 r = 0;
-            return n >= 1089470464 ? Ar[0] > 0 ? n = 31744 : (n = (2080374784 & n) >> 16, r = (1048575 & Ar[1]) >> 10) : n <= 1056964608 ? (r = 1048576 + ((r = 1048576 + (1048575 & Ar[1])) << (n >> 20) - 998) >> 21, n = 0) : (n = n - 1056964608 >> 10, r = 512 + (1048575 & Ar[1]) >> 10), t | n | 65535 & r
+            return n >= 1089470464 ? Tr[0] > 0 ? n = 31744 : (n = (2080374784 & n) >> 16, r = (1048575 & Tr[1]) >> 10) : n <= 1056964608 ? (r = 1048576 + ((r = 1048576 + (1048575 & Tr[1])) << (n >> 20) - 998) >> 21, n = 0) : (n = n - 1056964608 >> 10, r = 512 + (1048575 & Tr[1]) >> 10), t | n | 65535 & r
         }
-        var Lr = function(e) {
+        var Ar = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            Fr = function(e) {
+            }(vr),
+            Br = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
-                        this._values.set(e, Dr(t))
+                        this._values.set(e, Er(t))
                     }
                 }]), n
-            }(Lr),
-            Cr = function(e) {
+            }(Ar),
+            Dr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
                         this._values.set(e, t)
                     }
                 }]), n
-            }(Lr),
-            Mr = function(e) {
+            }(Ar),
+            Lr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
                         this._values.set(e, t)
                     }
                 }]), n
-            }(Lr),
-            Nr = n(10),
-            Ur = n(11);
+            }(Ar),
+            Fr = n(12),
+            Cr = n(13);
 
-        function Pr(e, t, n) {
-            return Pr = Object(Ur.a)() ? Reflect.construct.bind() : function(e, t, n) {
+        function Mr(e, t, n) {
+            return Mr = Object(Cr.a)() ? Reflect.construct.bind() : function(e, t, n) {
                 var r = [null];
                 r.push.apply(r, t);
                 var i = new(Function.bind.apply(e, r));
-                return n && Object(Nr.a)(i, n.prototype), i
-            }, Pr.apply(null, arguments)
+                return n && Object(Fr.a)(i, n.prototype), i
+            }, Mr.apply(null, arguments)
         }
-        var Rr, Vr, zr = Symbol.for("isArrowBigNum");
+        var Nr, Ur, Pr = Symbol.for("isArrowBigNum");
 
-        function Wr(e) {
+        function Rr(e) {
             for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
-            return 0 === n.length ? Object.setPrototypeOf(Re(this.TypedArray, e), this.constructor.prototype) : Object.setPrototypeOf(Pr(this.TypedArray, [e].concat(n)), this.constructor.prototype)
+            return 0 === n.length ? Object.setPrototypeOf(Re(this.TypedArray, e), this.constructor.prototype) : Object.setPrototypeOf(Mr(this.TypedArray, [e].concat(n)), this.constructor.prototype)
         }
 
-        function Yr() {
+        function Vr() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-            return Wr.apply(this, t)
+            return Rr.apply(this, t)
         }
 
-        function Hr() {
+        function zr() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-            return Wr.apply(this, t)
+            return Rr.apply(this, t)
         }
 
-        function $r() {
+        function Wr() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-            return Wr.apply(this, t)
+            return Rr.apply(this, t)
         }
 
-        function Kr(e) {
+        function Yr(e) {
             for (var t, n, r = e.buffer, i = e.byteOffset, a = e.length, o = e.signed, u = new Int32Array(r, i, a), s = 0, c = 0, l = u.length; c < l;) n = u[c++], t = u[c++], o || (t >>>= 0), s += (n >>> 0) + t * Math.pow(c, 32);
             return s
         }
 
-        function Qr(e) {
+        function Hr(e) {
             var t = "",
                 n = new Uint32Array(2),
                 r = new Uint16Array(e.buffer, e.byteOffset, e.byteLength / 2),
                 i = new Uint32Array((r = new Uint16Array(r).reverse()).buffer),
                 a = -1,
                 o = r.length - 1;
             do {
                 for (n[0] = r[a = 0]; a < o;) r[a++] = n[1] = n[0] / 10, n[0] = (n[0] - 10 * n[1] << 16) + r[a];
                 r[a] = n[1] = n[0] / 10, n[0] = n[0] - 10 * n[1], t = "".concat(n[0]).concat(t)
             } while (i[0] || i[1] || i[2] || i[3]);
             return t || "0"
         }
-        Wr.prototype[zr] = !0, Wr.prototype.toJSON = function() {
-            return '"'.concat(Rr(this), '"')
-        }, Wr.prototype.valueOf = function() {
-            return Kr(this)
-        }, Wr.prototype.toString = function() {
-            return Rr(this)
-        }, Wr.prototype[Symbol.toPrimitive] = function() {
+        Rr.prototype[Pr] = !0, Rr.prototype.toJSON = function() {
+            return '"'.concat(Nr(this), '"')
+        }, Rr.prototype.valueOf = function() {
+            return Yr(this)
+        }, Rr.prototype.toString = function() {
+            return Nr(this)
+        }, Rr.prototype[Symbol.toPrimitive] = function() {
             switch (arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "default") {
                 case "number":
-                    return Kr(this);
+                    return Yr(this);
                 case "string":
-                    return Rr(this);
+                    return Nr(this);
                 case "default":
-                    return Vr(this)
+                    return Ur(this)
             }
-            return Rr(this)
-        }, Object.setPrototypeOf(Yr.prototype, Object.create(Int32Array.prototype)), Object.setPrototypeOf(Hr.prototype, Object.create(Uint32Array.prototype)), Object.setPrototypeOf($r.prototype, Object.create(Uint32Array.prototype)), Object.assign(Yr.prototype, Wr.prototype, {
-            constructor: Yr,
+            return Nr(this)
+        }, Object.setPrototypeOf(Vr.prototype, Object.create(Int32Array.prototype)), Object.setPrototypeOf(zr.prototype, Object.create(Uint32Array.prototype)), Object.setPrototypeOf(Wr.prototype, Object.create(Uint32Array.prototype)), Object.assign(Vr.prototype, Rr.prototype, {
+            constructor: Vr,
             signed: !0,
             TypedArray: Int32Array,
             BigIntArray: ge
-        }), Object.assign(Hr.prototype, Wr.prototype, {
-            constructor: Hr,
+        }), Object.assign(zr.prototype, Rr.prototype, {
+            constructor: zr,
             signed: !1,
             TypedArray: Uint32Array,
             BigIntArray: we
-        }), Object.assign($r.prototype, Wr.prototype, {
-            constructor: $r,
+        }), Object.assign(Wr.prototype, Rr.prototype, {
+            constructor: Wr,
             signed: !0,
             TypedArray: Uint32Array,
             BigIntArray: we
-        }), be ? (Vr = function(e) {
-            return 8 === e.byteLength ? new e.BigIntArray(e.buffer, e.byteOffset, 1)[0] : Qr(e)
-        }, Rr = function(e) {
-            return 8 === e.byteLength ? "".concat(new e.BigIntArray(e.buffer, e.byteOffset, 1)[0]) : Qr(e)
-        }) : Vr = Rr = Qr;
-        var qr, Gr = function() {
+        }), be ? (Ur = function(e) {
+            return 8 === e.byteLength ? new e.BigIntArray(e.buffer, e.byteOffset, 1)[0] : Hr(e)
+        }, Nr = function(e) {
+            return 8 === e.byteLength ? "".concat(new e.BigIntArray(e.buffer, e.byteOffset, 1)[0]) : Hr(e)
+        }) : Ur = Nr = Hr;
+        var $r, Kr = function() {
                 function e(t, n) {
                     return Object(C.a)(this, e), e.new(t, n)
                 }
                 return Object(M.a)(e, null, [{
                     key: "new",
                     value: function(e, t) {
                         switch (t) {
                             case !0:
-                                return new Yr(e);
+                                return new Vr(e);
                             case !1:
-                                return new Hr(e)
+                                return new zr(e)
                         }
                         switch (e.constructor) {
                             case Int8Array:
                             case Int16Array:
                             case Int32Array:
                             case ge:
-                                return new Yr(e)
+                                return new Vr(e)
                         }
-                        return 16 === e.byteLength ? new $r(e) : new Hr(e)
+                        return 16 === e.byteLength ? new Wr(e) : new zr(e)
                     }
                 }, {
                     key: "signed",
                     value: function(e) {
-                        return new Yr(e)
+                        return new Vr(e)
                     }
                 }, {
                     key: "unsigned",
                     value: function(e) {
-                        return new Hr(e)
+                        return new zr(e)
                     }
                 }, {
                     key: "decimal",
                     value: function(e) {
-                        return new $r(e)
+                        return new Wr(e)
                     }
                 }]), e
             }(),
-            Jr = function(e) {
+            Qr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
                         this._values.set(e, t)
                     }
                 }]), n
-            }(gr),
-            Zr = function(e) {
+            }(vr),
+            qr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Jr),
-            Xr = function(e) {
+            }(Qr),
+            Gr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Jr),
-            ei = function(e) {
+            }(Qr),
+            Jr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Jr),
-            ti = function(e) {
+            }(Qr),
+            Zr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), e.nullValues && (e.nullValues = e.nullValues.map(oi)), (r = t.call(this, e))._values = new br(new Int32Array(0), 2), r
+                    return Object(C.a)(this, n), e.nullValues && (e.nullValues = e.nullValues.map(ri)), (r = t.call(this, e))._values = new pr(new Int32Array(0), 2), r
                 }
                 return Object(M.a)(n, [{
                     key: "values64",
                     get: function() {
                         return this._values.buffer64
                     }
                 }, {
                     key: "isValid",
                     value: function(e) {
-                        return Ut(Object(Nt.a)(n.prototype), "isValid", this).call(this, oi(e))
+                        return Ct(Object(Ft.a)(n.prototype), "isValid", this).call(this, ri(e))
                     }
                 }]), n
-            }(Jr),
-            ni = function(e) {
+            }(Qr),
+            Xr = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Jr),
-            ri = function(e) {
+            }(Qr),
+            ei = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Jr),
-            ii = function(e) {
+            }(Qr),
+            ti = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Jr),
-            ai = function(e) {
+            }(Qr),
+            ni = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), e.nullValues && (e.nullValues = e.nullValues.map(oi)), (r = t.call(this, e))._values = new br(new Uint32Array(0), 2), r
+                    return Object(C.a)(this, n), e.nullValues && (e.nullValues = e.nullValues.map(ri)), (r = t.call(this, e))._values = new pr(new Uint32Array(0), 2), r
                 }
                 return Object(M.a)(n, [{
                     key: "values64",
                     get: function() {
                         return this._values.buffer64
                     }
                 }, {
                     key: "isValid",
                     value: function(e) {
-                        return Ut(Object(Nt.a)(n.prototype), "isValid", this).call(this, oi(e))
+                        return Ct(Object(Ft.a)(n.prototype), "isValid", this).call(this, ri(e))
                     }
                 }]), n
-            }(Jr),
-            oi = (qr = {
+            }(Qr),
+            ri = ($r = {
                 BigIntArray: ge
             }, function(e) {
-                return ArrayBuffer.isView(e) && (qr.buffer = e.buffer, qr.byteOffset = e.byteOffset, qr.byteLength = e.byteLength, e = Vr(qr), qr.buffer = null), e
+                return ArrayBuffer.isView(e) && ($r.buffer = e.buffer, $r.byteOffset = e.byteOffset, $r.byteLength = e.byteLength, e = Ur($r), $r.buffer = null), e
             }),
-            ui = function(e) {
+            ii = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            si = function(e) {
+            }(vr),
+            ai = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ui),
-            ci = function(e) {
+            }(ii),
+            oi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ui),
-            li = function(e) {
+            }(ii),
+            ui = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ui),
-            fi = function(e) {
+            }(ii),
+            si = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ui),
-            hi = function(e) {
+            }(ii),
+            ci = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            di = function(e) {
+            }(vr),
+            li = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(hi),
-            pi = function(e) {
+            }(ci),
+            fi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(hi),
-            yi = function(e) {
+            }(ci),
+            hi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(hi),
-            vi = function(e) {
+            }(ci),
+            di = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(hi),
-            bi = function(e) {
+            }(ci),
+            pi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(gr),
-            mi = function(e) {
+            }(vr),
+            yi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(bi),
-            gi = function(e) {
+            }(pi),
+            vi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(bi),
-            ki = function(e) {
+            }(pi),
+            bi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new dr(new Uint8Array(0)), r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new lr(new Uint8Array(0)), r
                 }
                 return Object(M.a)(n, [{
                     key: "byteLength",
                     get: function() {
                         var e = this._pendingLength + 4 * this.length;
                         return this._offsets && (e += this._offsets.byteLength), this._values && (e += this._values.byteLength), this._nulls && (e += this._nulls.byteLength), e
                     }
                 }, {
                     key: "setValue",
                     value: function(e, t) {
-                        return Ut(Object(Nt.a)(n.prototype), "setValue", this).call(this, e, He(t))
+                        return Ct(Object(Ft.a)(n.prototype), "setValue", this).call(this, e, He(t))
                     }
                 }, {
                     key: "_flushPending",
                     value: function(e, t) {
                         var n, r, i = this._offsets,
                             a = this._values.reserve(t).buffer,
                             o = 0,
@@ -7482,41 +7494,41 @@
                         } catch (f) {
                             c.e(f)
                         } finally {
                             c.f()
                         }
                     }
                 }]), n
-            }(kr),
-            wi = function(e) {
+            }(br),
+            mi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new dr(new Uint8Array(0)), r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._values = new lr(new Uint8Array(0)), r
                 }
                 return Object(M.a)(n, [{
                     key: "byteLength",
                     get: function() {
                         var e = this._pendingLength + 4 * this.length;
                         return this._offsets && (e += this._offsets.byteLength), this._values && (e += this._values.byteLength), this._nulls && (e += this._nulls.byteLength), e
                     }
                 }, {
                     key: "setValue",
                     value: function(e, t) {
-                        return Ut(Object(Nt.a)(n.prototype), "setValue", this).call(this, e, se(t))
+                        return Ct(Object(Ft.a)(n.prototype), "setValue", this).call(this, e, se(t))
                     }
                 }, {
                     key: "_flushPending",
                     value: function(e, t) {}
                 }]), n
-            }(kr);
-        wi.prototype._flushPending = ki.prototype._flushPending;
-        var _i = function() {
+            }(br);
+        mi.prototype._flushPending = bi.prototype._flushPending;
+        var gi = function() {
                 function e() {
                     Object(C.a)(this, e)
                 }
                 return Object(M.a)(e, [{
                     key: "length",
                     get: function() {
                         return this._values.length
@@ -7530,28 +7542,29 @@
                     key: "clear",
                     value: function() {
                         return this._values = null, this
                     }
                 }, {
                     key: "bind",
                     value: function(e) {
-                        return e instanceof Ht ? e : (this._values = e, this)
+                        return e instanceof zt ? e : (this._values = e, this)
                     }
                 }]), e
             }(),
-            Oi = n(8),
-            xi = n(9),
-            ji = Symbol.for("parent"),
-            Si = Symbol.for("rowIndex"),
-            Ti = Symbol.for("keyToIdx"),
-            Ii = Symbol.for("idxToVal"),
-            Ei = Symbol.for("nodejs.util.inspect.custom"),
-            Ai = function(e) {
+            ki = n(10),
+            wi = n(11),
+            _i = n(6),
+            Oi = Symbol.for("parent"),
+            ji = Symbol.for("rowIndex"),
+            xi = Symbol.for("keyToIdx"),
+            Si = Symbol.for("idxToVal"),
+            Ti = Symbol.for("nodejs.util.inspect.custom"),
+            Ii = function(e) {
                 function t(e, n) {
-                    Object(C.a)(this, t), this[ji] = e, this.size = n
+                    Object(C.a)(this, t), this[Oi] = e, this.size = n
                 }
                 return Object(M.a)(t, [{
                     key: "entries",
                     value: function() {
                         return this[Symbol.iterator]()
                     }
                 }, {
@@ -7560,34 +7573,34 @@
                         return void 0 !== this.get(e)
                     }
                 }, {
                     key: "get",
                     value: function(e) {
                         var t = void 0;
                         if (null !== e && void 0 !== e) {
-                            var n = this[Ti] || (this[Ti] = new Map),
+                            var n = this[xi] || (this[xi] = new Map),
                                 r = n.get(e);
                             if (void 0 !== r) {
-                                var i = this[Ii] || (this[Ii] = new Array(this.size));
+                                var i = this[Si] || (this[Si] = new Array(this.size));
                                 void 0 !== (t = i[r]) || (i[r] = t = this.getValue(r))
                             } else if ((r = this.getIndex(e)) > -1) {
                                 n.set(e, r);
-                                var a = this[Ii] || (this[Ii] = new Array(this.size));
+                                var a = this[Si] || (this[Si] = new Array(this.size));
                                 void 0 !== (t = a[r]) || (a[r] = t = this.getValue(r))
                             }
                         }
                         return t
                     }
                 }, {
                     key: "set",
                     value: function(e, t) {
                         if (null !== e && void 0 !== e) {
-                            var n = this[Ti] || (this[Ti] = new Map),
+                            var n = this[xi] || (this[xi] = new Map),
                                 r = n.get(e);
-                            if (void 0 === r && n.set(e, r = this.getIndex(e)), r > -1)(this[Ii] || (this[Ii] = new Array(this.size)))[r] = this.setValue(r, t)
+                            if (void 0 === r && n.set(e, r = this.getIndex(e)), r > -1)(this[Si] || (this[Si] = new Array(this.size)))[r] = this.setValue(r, t)
                         }
                         return this
                     }
                 }, {
                     key: "clear",
                     value: function() {
                         throw new Error("Clearing ".concat(this[Symbol.toStringTag], " not supported."))
@@ -7600,15 +7613,15 @@
                 }, {
                     key: e,
                     value: U().mark((function e() {
                         var t, n, r, i, a, o, u, s, c;
                         return U().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
-                                    t = this.keys(), n = this.values(), r = this[Ti] || (this[Ti] = new Map), i = this[Ii] || (this[Ii] = new Array(this.size)), u = 0;
+                                    t = this.keys(), n = this.values(), r = this[xi] || (this[xi] = new Map), i = this[Si] || (this[Si] = new Array(this.size)), u = 0;
                                 case 5:
                                     if ((s = t.next()).done || (c = n.next()).done) {
                                         e.next = 15;
                                         break
                                     }
                                     return a = s.value, o = c.value, i[u] = o, r.has(a) || r.set(a, u), e.next = 12, [a, o];
                                 case 12:
@@ -7621,20 +7634,20 @@
                         }), e, this)
                     }))
                 }, {
                     key: "forEach",
                     value: function(e, t) {
                         for (var n, r, i, a, o = this.keys(), u = this.values(), s = void 0 === t ? e : function(n, r, i) {
                                 return e.call(t, n, r, i)
-                            }, c = this[Ti] || (this[Ti] = new Map), l = this[Ii] || (this[Ii] = new Array(this.size)), f = 0; !(i = o.next()).done && !(a = u.next()).done; ++f) n = i.value, r = a.value, l[f] = r, c.has(n) || c.set(n, f), s(r, n, this)
+                            }, c = this[xi] || (this[xi] = new Map), l = this[Si] || (this[Si] = new Array(this.size)), f = 0; !(i = o.next()).done && !(a = u.next()).done; ++f) n = i.value, r = a.value, l[f] = r, c.has(n) || c.set(n, f), s(r, n, this)
                     }
                 }, {
                     key: "toArray",
                     value: function() {
-                        return hn(this.values())
+                        return cn(this.values())
                     }
                 }, {
                     key: "toJSON",
                     value: function() {
                         var e = {};
                         return this.forEach((function(t, n) {
                             return e[n] = t
@@ -7642,105 +7655,105 @@
                     }
                 }, {
                     key: "inspect",
                     value: function() {
                         return this.toString()
                     }
                 }, {
-                    key: Ei,
+                    key: Ti,
                     value: function() {
                         return this.toString()
                     }
                 }, {
                     key: "toString",
                     value: function() {
                         var e = [];
                         return this.forEach((function(t, n) {
-                            n = lr(n), t = lr(t), e.push("".concat(n, ": ").concat(t))
+                            n = ur(n), t = ur(t), e.push("".concat(n, ": ").concat(t))
                         })), "{ ".concat(e.join(", "), " }")
                     }
                 }]), t
             }(Symbol.iterator);
-        Ai[Symbol.toStringTag] = function(e) {
+        Ii[Symbol.toStringTag] = function(e) {
             var t;
-            return Object.defineProperties(e, (Ft(t = {
+            return Object.defineProperties(e, (t = {
                 size: {
                     writable: !0,
                     enumerable: !1,
                     configurable: !1,
                     value: 0
                 }
-            }, ji, {
+            }, Object(_i.a)(t, Oi, {
                 writable: !0,
                 enumerable: !1,
                 configurable: !1,
                 value: null
-            }), Ft(t, Si, {
+            }), Object(_i.a)(t, ji, {
                 writable: !0,
                 enumerable: !1,
                 configurable: !1,
                 value: -1
             }), t)), e[Symbol.toStringTag] = "Row"
-        }(Ai.prototype);
-        var Bi = function(e) {
+        }(Ii.prototype);
+        var Ei = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), r = t.call(this, e, e.length), Object(Oi.a)(r, Ci(Object(xi.a)(r)))
+                    return Object(C.a)(this, n), r = t.call(this, e, e.length), Object(ki.a)(r, Li(Object(wi.a)(r)))
                 }
                 return Object(M.a)(n, [{
                     key: "keys",
                     value: function() {
-                        return this[ji].getChildAt(0)[Symbol.iterator]()
+                        return this[Oi].getChildAt(0)[Symbol.iterator]()
                     }
                 }, {
                     key: "values",
                     value: function() {
-                        return this[ji].getChildAt(1)[Symbol.iterator]()
+                        return this[Oi].getChildAt(1)[Symbol.iterator]()
                     }
                 }, {
                     key: "getKey",
                     value: function(e) {
-                        return this[ji].getChildAt(0).get(e)
+                        return this[Oi].getChildAt(0).get(e)
                     }
                 }, {
                     key: "getIndex",
                     value: function(e) {
-                        return this[ji].getChildAt(0).indexOf(e)
+                        return this[Oi].getChildAt(0).indexOf(e)
                     }
                 }, {
                     key: "getValue",
                     value: function(e) {
-                        return this[ji].getChildAt(1).get(e)
+                        return this[Oi].getChildAt(1).get(e)
                     }
                 }, {
                     key: "setValue",
                     value: function(e, t) {
-                        this[ji].getChildAt(1).set(e, t)
+                        this[Oi].getChildAt(1).set(e, t)
                     }
                 }]), n
-            }(Ai),
-            Di = function(e) {
+            }(Ii),
+            Ai = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), r = t.call(this, e, e.type.children.length), Object(Oi.a)(r, Fi(Object(xi.a)(r)))
+                    return Object(C.a)(this, n), r = t.call(this, e, e.type.children.length), Object(ki.a)(r, Di(Object(wi.a)(r)))
                 }
                 return Object(M.a)(n, [{
                     key: "keys",
                     value: U().mark((function e() {
                         var t, n, r;
                         return U().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
-                                    t = D(this[ji].type.children), e.prev = 1, t.s();
+                                    t = D(this[Oi].type.children), e.prev = 1, t.s();
                                 case 3:
                                     if ((n = t.n()).done) {
                                         e.next = 9;
                                         break
                                     }
                                     return r = n.value, e.next = 7, r.name;
                                 case 7:
@@ -7764,15 +7777,15 @@
                 }, {
                     key: "values",
                     value: U().mark((function e() {
                         var t, n, r;
                         return U().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
-                                    t = D(this[ji].type.children), e.prev = 1, t.s();
+                                    t = D(this[Oi].type.children), e.prev = 1, t.s();
                                 case 3:
                                     if ((n = t.n()).done) {
                                         e.next = 9;
                                         break
                                     }
                                     return r = n.value, e.next = 7, this[r.name];
                                 case 7:
@@ -7792,46 +7805,46 @@
                         }), e, this, [
                             [1, 11, 14, 17]
                         ])
                     }))
                 }, {
                     key: "getKey",
                     value: function(e) {
-                        return this[ji].type.children[e].name
+                        return this[Oi].type.children[e].name
                     }
                 }, {
                     key: "getIndex",
                     value: function(e) {
-                        return this[ji].type.children.findIndex((function(t) {
+                        return this[Oi].type.children.findIndex((function(t) {
                             return t.name === e
                         }))
                     }
                 }, {
                     key: "getValue",
                     value: function(e) {
-                        return this[ji].getChildAt(e).get(this[Si])
+                        return this[Oi].getChildAt(e).get(this[ji])
                     }
                 }, {
                     key: "setValue",
                     value: function(e, t) {
-                        return this[ji].getChildAt(e).set(this[Si], t)
+                        return this[Oi].getChildAt(e).set(this[ji], t)
                     }
                 }]), n
-            }(Ai);
-        Object.setPrototypeOf(Ai.prototype, Map.prototype);
-        var Li, Fi = function() {
+            }(Ii);
+        Object.setPrototypeOf(Ii.prototype, Map.prototype);
+        var Bi, Di = function() {
                 var e = {
                     enumerable: !0,
                     configurable: !1,
                     get: null,
                     set: null
                 };
                 return function(t) {
                     var n, r = -1,
-                        i = t[Ti] || (t[Ti] = new Map),
+                        i = t[xi] || (t[xi] = new Map),
                         a = function(e) {
                             return function() {
                                 return this.get(e)
                             }
                         },
                         o = function(e) {
                             return function(t) {
@@ -7848,32 +7861,32 @@
                         u.e(c)
                     } finally {
                         u.f()
                     }
                     return e.get = e.set = null, t
                 }
             }(),
-            Ci = function() {
-                if ("undefined" === typeof Proxy) return Fi;
-                var e = Ai.prototype.has,
-                    t = Ai.prototype.get,
-                    n = Ai.prototype.set,
-                    r = Ai.prototype.getKey,
+            Li = function() {
+                if ("undefined" === typeof Proxy) return Di;
+                var e = Ii.prototype.has,
+                    t = Ii.prototype.get,
+                    n = Ii.prototype.set,
+                    r = Ii.prototype.getKey,
                     i = {
                         isExtensible: function() {
                             return !1
                         },
                         deleteProperty: function() {
                             return !1
                         },
                         preventExtensions: function() {
                             return !0
                         },
                         ownKeys: function(e) {
-                            return hn(e.keys()).map((function(e) {
+                            return cn(e.keys()).map((function(e) {
                                 return "".concat(e)
                             }))
                         },
                         has: function(e, t) {
                             switch (t) {
                                 case "getKey":
                                 case "getIndex":
@@ -7902,19 +7915,19 @@
                                 case "__defineGetter__":
                                 case "__defineSetter__":
                                 case "hasOwnProperty":
                                 case "__lookupGetter__":
                                 case "__lookupSetter__":
                                 case Symbol.iterator:
                                 case Symbol.toStringTag:
+                                case Oi:
                                 case ji:
                                 case Si:
-                                case Ii:
+                                case xi:
                                 case Ti:
-                                case Ei:
                                     return !0
                             }
                             return "number" !== typeof t || e.has(t) || (t = e.getKey(t)), e.has(t)
                         },
                         get: function(n, i, a) {
                             switch (i) {
                                 case "getKey":
@@ -7944,29 +7957,29 @@
                                 case "__defineGetter__":
                                 case "__defineSetter__":
                                 case "hasOwnProperty":
                                 case "__lookupGetter__":
                                 case "__lookupSetter__":
                                 case Symbol.iterator:
                                 case Symbol.toStringTag:
+                                case Oi:
                                 case ji:
                                 case Si:
-                                case Ii:
+                                case xi:
                                 case Ti:
-                                case Ei:
                                     return Reflect.get(n, i, a)
                             }
                             return "number" !== typeof i || e.call(a, i) || (i = r.call(a, i)), t.call(a, i)
                         },
                         set: function(t, i, a, o) {
                             switch (i) {
+                                case Oi:
                                 case ji:
                                 case Si:
-                                case Ii:
-                                case Ti:
+                                case xi:
                                     return Reflect.set(t, i, a, o);
                                 case "getKey":
                                 case "getIndex":
                                 case "getValue":
                                 case "setValue":
                                 case "toArray":
                                 case "toJSON":
@@ -8001,104 +8014,104 @@
                         }
                     };
                 return function(e) {
                     return new Proxy(e, i)
                 }
             }();
 
-        function Mi(e, t, n) {
+        function Fi(e, t, n) {
             var r = e.length,
                 i = t > -1 ? t : r + t % r;
             return n ? n(e, i) : i
         }
 
-        function Ni(e, t, n, r) {
+        function Ci(e, t, n, r) {
             var i = e.length,
                 a = void 0 === i ? 0 : i,
                 o = "number" !== typeof t ? 0 : t,
                 u = "number" !== typeof n ? a : n;
-            return o < 0 && (o = (o % a + a) % a), u < 0 && (u = (u % a + a) % a), u < o && (Li = o, o = u, u = Li), u > a && (u = a), r ? r(e, o, u) : [o, u]
+            return o < 0 && (o = (o % a + a) % a), u < 0 && (u = (u % a + a) % a), u < o && (Bi = o, o = u, u = Bi), u > a && (u = a), r ? r(e, o, u) : [o, u]
         }
-        var Ui = be ? ve(0) : 0,
-            Pi = function(e) {
+        var Mi = be ? ve(0) : 0,
+            Ni = function(e) {
                 return e !== e
             };
 
-        function Ri(e) {
+        function Ui(e) {
             var t = typeof e;
-            if ("object" !== t || null === e) return Pi(e) ? Pi : "bigint" !== t ? function(t) {
+            if ("object" !== t || null === e) return Ni(e) ? Ni : "bigint" !== t ? function(t) {
                 return t === e
             } : function(t) {
-                return Ui + t === e
+                return Mi + t === e
             };
             if (e instanceof Date) {
                 var n = e.valueOf();
                 return function(e) {
                     return e instanceof Date && e.valueOf() === n
                 }
             }
             return ArrayBuffer.isView(e) ? function(t) {
                 return !!t && wt(e, t)
             } : e instanceof Map ? function(e) {
                 var t = -1,
                     n = [];
                 return e.forEach((function(e) {
-                    return n[++t] = Ri(e)
-                })), Vi(n)
+                    return n[++t] = Ui(e)
+                })), Pi(n)
             }(e) : Array.isArray(e) ? function(e) {
-                for (var t = [], n = -1, r = e.length; ++n < r;) t[n] = Ri(e[n]);
-                return Vi(t)
-            }(e) : e instanceof Ht ? function(e) {
-                for (var t = [], n = -1, r = e.length; ++n < r;) t[n] = Ri(e.get(n));
-                return Vi(t)
+                for (var t = [], n = -1, r = e.length; ++n < r;) t[n] = Ui(e[n]);
+                return Pi(t)
+            }(e) : e instanceof zt ? function(e) {
+                for (var t = [], n = -1, r = e.length; ++n < r;) t[n] = Ui(e.get(n));
+                return Pi(t)
             }(e) : function(e) {
                 var t = Object.keys(e);
                 if (0 === t.length) return function() {
                     return !1
                 };
-                for (var n = [], r = -1, i = t.length; ++r < i;) n[r] = Ri(e[t[r]]);
-                return Vi(n, t)
+                for (var n = [], r = -1, i = t.length; ++r < i;) n[r] = Ui(e[t[r]]);
+                return Pi(n, t)
             }(e)
         }
 
-        function Vi(e, t) {
+        function Pi(e, t) {
             return function(n) {
                 if (!n || "object" !== typeof n) return !1;
                 switch (n.constructor) {
                     case Array:
                         return function(e, t) {
                             var n = e.length;
                             if (t.length !== n) return !1;
                             for (var r = -1; ++r < n;)
                                 if (!e[r](t[r])) return !1;
                             return !0
                         }(e, n);
                     case Map:
-                    case Bi:
-                    case Di:
-                        return zi(e, n, n.keys());
+                    case Ei:
+                    case Ai:
+                        return Ri(e, n, n.keys());
                     case Object:
                     case void 0:
-                        return zi(e, n, t || Object.keys(n))
+                        return Ri(e, n, t || Object.keys(n))
                 }
-                return n instanceof Ht && function(e, t) {
+                return n instanceof zt && function(e, t) {
                     var n = e.length;
                     if (t.length !== n) return !1;
                     for (var r = -1; ++r < n;)
                         if (!e[r](t.get(r))) return !1;
                     return !0
                 }(e, n)
             }
         }
 
-        function zi(e, t, n) {
+        function Ri(e, t, n) {
             for (var r = n[Symbol.iterator](), i = t instanceof Map ? t.keys() : Object.keys(t)[Symbol.iterator](), a = t instanceof Map ? t.values() : Object.values(t)[Symbol.iterator](), o = 0, u = e.length, s = a.next(), c = r.next(), l = i.next(); o < u && !c.done && !l.done && !s.done && (c.value === l.value && e[o](s.value)); ++o, c = r.next(), l = i.next(), s = a.next());
             return !!(o === u && c.done && l.done && s.done) || (r.return && r.return(), i.return && i.return(), a.return && a.return(), !1)
         }
-        var Wi = function(e, t) {
+        var Vi = function(e, t) {
             Object(ce.a)(r, e);
             var n = Object(le.a)(r);
 
             function r(e) {
                 var t, i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [],
                     a = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : function(e) {
                         for (var t = new Uint32Array((e || []).length + 1), n = t[0] = 0, r = t.length, i = 0; ++i < r;) t[i] = n += e[i - 1].length;
@@ -8165,29 +8178,29 @@
                     return e < 0 && (this._nullCount = e = this._chunks.reduce((function(e, t) {
                         return e + t.nullCount
                     }), 0)), e
                 }
             }, {
                 key: "indices",
                 get: function() {
-                    if (Tn.isDictionary(this._type)) {
+                    if (jn.isDictionary(this._type)) {
                         if (!this._indices) {
                             var e = this._chunks;
-                            this._indices = 1 === e.length ? e[0].indices : r.concat.apply(r, hn(e.map((function(e) {
+                            this._indices = 1 === e.length ? e[0].indices : r.concat.apply(r, cn(e.map((function(e) {
                                 return e.indices
                             }))))
                         }
                         return this._indices
                     }
                     return null
                 }
             }, {
                 key: "dictionary",
                 get: function() {
-                    return Tn.isDictionary(this._type) ? this._chunks[this._chunks.length - 1].data.dictionary : null
+                    return jn.isDictionary(this._type) ? this._chunks[this._chunks.length - 1].data.dictionary : null
                 }
             }, {
                 key: t,
                 value: U().mark((function e() {
                     var t, n, r;
                     return U().wrap((function(e) {
                         for (;;) switch (e.prev = e.next) {
@@ -8228,15 +8241,15 @@
                 value: function() {
                     for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                     return this.clone(r.flatten.apply(r, [this].concat(t)))
                 }
             }, {
                 key: "slice",
                 value: function(e, t) {
-                    return Ni(this, e, t, this._sliceInternal)
+                    return Ci(this, e, t, this._sliceInternal)
                 }
             }, {
                 key: "getChildAt",
                 value: function(e) {
                     if (e < 0 || e >= this._numChildren) return null;
                     var t, n, i, a = this._children || (this._children = []);
                     return (t = a[e]) ? t : (n = (this._type.children || [])[e]) && (i = this._chunks.map((function(t) {
@@ -8294,15 +8307,15 @@
                     var e = this.chunks,
                         t = e.length,
                         n = this._type.ArrayType;
                     if (t <= 0) return new n(0);
                     if (t <= 1) return e[0].toArray();
                     for (var r = 0, i = new Array(t), a = -1; ++a < t;) r += (i[a] = e[a].toArray()).length;
                     n !== i[0].constructor && (n = i[0].constructor);
-                    for (var o = new n(r), u = n === Array ? Hi : Yi, s = -1, c = 0; ++s < t;) c = u(i[s], o, c);
+                    for (var o = new n(r), u = n === Array ? Wi : zi, s = -1, c = 0; ++s < t;) c = u(i[s], o, c);
                     return o
                 }
             }, {
                 key: "getInternal",
                 value: function(e, t, n) {
                     return e._chunks[t].get(n)
                 }
@@ -8338,39 +8351,39 @@
                     }
                     return e.clone(r)
                 }
             }], [{
                 key: "flatten",
                 value: function() {
                     for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                    return Ji(Ht, t)
+                    return qi(zt, t)
                 }
             }, {
                 key: "concat",
                 value: function() {
                     var e = r.flatten.apply(r, arguments);
                     return new r(e[0].type, e)
                 }
             }]), r
-        }(Ht, Symbol.iterator);
-        var Yi = function(e, t, n) {
+        }(zt, Symbol.iterator);
+        var zi = function(e, t, n) {
                 return t.set(e, n), n + e.length
             },
-            Hi = function(e, t, n) {
+            Wi = function(e, t, n) {
                 for (var r = n, i = -1, a = e.length; ++i < a;) t[r++] = e[i];
                 return r
             },
-            $i = function(e) {
+            Yi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r, i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [],
                         a = arguments.length > 2 ? arguments[2] : void 0;
-                    return Object(C.a)(this, n), i = Wi.flatten.apply(Wi, hn(i)), (r = t.call(this, e.type, i, a))._field = e, 1 !== i.length || Object(xi.a)(r) instanceof Ki ? r : Object(Oi.a)(r, new Ki(e, i[0], r._chunkOffsets))
+                    return Object(C.a)(this, n), i = Vi.flatten.apply(Vi, cn(i)), (r = t.call(this, e.type, i, a))._field = e, 1 !== i.length || Object(wi.a)(r) instanceof Hi ? r : Object(ki.a)(r, new Hi(e, i[0], r._chunkOffsets))
                 }
                 return Object(M.a)(n, [{
                     key: "field",
                     get: function() {
                         return this._field
                     }
                 }, {
@@ -8405,28 +8418,28 @@
                             return null != e
                         }))).length > 0 ? a[e] = new n(r, i) : null
                     }
                 }], [{
                     key: "new",
                     value: function(e, t) {
                         for (var r = arguments.length, i = new Array(r > 2 ? r - 2 : 0), a = 2; a < r; a++) i[a - 2] = arguments[a];
-                        var o = Wi.flatten(Array.isArray(t) ? [].concat(hn(t), i) : t instanceof Ht ? [t].concat(i) : [Ht.new.apply(Ht, [t].concat(i))]);
+                        var o = Vi.flatten(Array.isArray(t) ? [].concat(cn(t), i) : t instanceof zt ? [t].concat(i) : [zt.new.apply(zt, [t].concat(i))]);
                         if ("string" === typeof e) {
                             var u = o[0].data.type;
-                            e = new aa(e, u, !0)
+                            e = new ra(e, u, !0)
                         } else !e.nullable && o.some((function(e) {
                             return e.nullCount > 0
                         })) && (e = e.clone({
                             nullable: !0
                         }));
                         return new n(e, o)
                     }
                 }]), n
-            }(Wi),
-            Ki = function(e) {
+            }(Vi),
+            Hi = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r, i) {
                     var a;
                     return Object(C.a)(this, n), (a = t.call(this, e, [r], i))._chunk = r, a
                 }
@@ -8452,84 +8465,84 @@
                     }
                 }, {
                     key: "indexOf",
                     value: function(e, t) {
                         return this._chunk.indexOf(e, t)
                     }
                 }]), n
-            }($i),
-            Qi = Array.isArray,
-            qi = function(e, t) {
-                return Xi(e, t, [], 0)
+            }(Yi),
+            $i = Array.isArray,
+            Ki = function(e, t) {
+                return Ji(e, t, [], 0)
             },
-            Gi = function(e) {
-                return ra(e, [
+            Qi = function(e) {
+                return ta(e, [
                     [],
                     []
                 ])
             },
-            Ji = function(e, t) {
-                return ea(e, t, [], 0)
+            qi = function(e, t) {
+                return Zi(e, t, [], 0)
             },
-            Zi = function(e, t) {
-                return ta(e, t, [], 0)
+            Gi = function(e, t) {
+                return Xi(e, t, [], 0)
             };
 
-        function Xi(e, t, n, r) {
-            for (var i, a = r, o = -1, u = t.length; ++o < u;) Qi(i = t[o]) ? a = Xi(e, i, n, a).length : i instanceof e && (n[a++] = i);
+        function Ji(e, t, n, r) {
+            for (var i, a = r, o = -1, u = t.length; ++o < u;) $i(i = t[o]) ? a = Ji(e, i, n, a).length : i instanceof e && (n[a++] = i);
             return n
         }
 
-        function ea(e, t, n, r) {
-            for (var i, a = r, o = -1, u = t.length; ++o < u;) Qi(i = t[o]) ? a = ea(e, i, n, a).length : i instanceof Wi ? a = ea(e, i.chunks, n, a).length : i instanceof e && (n[a++] = i);
+        function Zi(e, t, n, r) {
+            for (var i, a = r, o = -1, u = t.length; ++o < u;) $i(i = t[o]) ? a = Zi(e, i, n, a).length : i instanceof Vi ? a = Zi(e, i.chunks, n, a).length : i instanceof e && (n[a++] = i);
             return n
         }
 
-        function ta(e, t, n, r) {
-            for (var i, a = r, o = -1, u = t.length; ++o < u;) Qi(i = t[o]) ? a = ta(e, i, n, a).length : i instanceof e ? a = Xi(Ht, i.schema.fields.map((function(e, t) {
+        function Xi(e, t, n, r) {
+            for (var i, a = r, o = -1, u = t.length; ++o < u;) $i(i = t[o]) ? a = Xi(e, i, n, a).length : i instanceof e ? a = Ji(zt, i.schema.fields.map((function(e, t) {
                 return i.getChildAt(t)
-            })), n, a).length : i instanceof Ht && (n[a++] = i);
+            })), n, a).length : i instanceof zt && (n[a++] = i);
             return n
         }
-        var na = function(e, t, n) {
+        var ea = function(e, t, n) {
             var r = P(t, 2),
                 i = r[0],
                 a = r[1];
             return e[0][n] = i, e[1][n] = a, e
         };
 
-        function ra(e, t) {
+        function ta(e, t) {
             var n, r;
             switch (r = e.length) {
                 case 0:
                     return t;
                 case 1:
                     if (n = t[0], !e[0]) return t;
-                    if (Qi(e[0])) return ra(e[0], t);
-                    if (!(e[0] instanceof sr || e[0] instanceof Ht || e[0] instanceof Tn)) {
-                        var i = P(Object.entries(e[0]).reduce(na, t), 2);
+                    if ($i(e[0])) return ta(e[0], t);
+                    if (!(e[0] instanceof ar || e[0] instanceof zt || e[0] instanceof jn)) {
+                        var i = P(Object.entries(e[0]).reduce(ea, t), 2);
                         n = i[0], e = i[1]
                     }
                     break;
                 default:
-                    Qi(n = e[r - 1]) ? e = Qi(e[0]) ? e[0] : e.slice(0, r - 1) : (e = Qi(e[0]) ? e[0] : e, n = [])
+                    $i(n = e[r - 1]) ? e = $i(e[0]) ? e[0] : e.slice(0, r - 1) : (e = $i(e[0]) ? e[0] : e, n = [])
             }
             for (var a, o, u = -1, s = -1, c = -1, l = e.length, f = P(t, 2), h = f[0], d = f[1]; ++c < l;)
-                if ((o = e[c]) instanceof $i && (d[++s] = o)) h[++u] = o.field.clone(n[c], o.type, !0);
+                if ((o = e[c]) instanceof Yi && (d[++s] = o)) h[++u] = o.field.clone(n[c], o.type, !0);
                 else {
                     var p = n[c];
-                    a = void 0 === p ? c : p, o instanceof Tn && (d[++s] = o) ? h[++u] = aa.new(a, o, !0) : o && o.type && (d[++s] = o) && (o instanceof sr && (d[s] = o = Ht.new(o)), h[++u] = aa.new(a, o.type, !0))
+                    a = void 0 === p ? c : p, o instanceof jn && (d[++s] = o) ? h[++u] = ra.new(a, o, !0) : o && o.type && (d[++s] = o) && (o instanceof ar && (d[s] = o = zt.new(o)), h[++u] = ra.new(a, o.type, !0))
                 } return t
         }
-        var ia = function(e) {
+        var na = function(e) {
                 function t() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [],
                         n = arguments.length > 1 ? arguments[1] : void 0,
                         r = arguments.length > 2 ? arguments[2] : void 0;
-                    Object(C.a)(this, t), this.fields = e || [], this.metadata = n || new Map, r || (r = ua(e)), this.dictionaries = r
+                    Object(C.a)(this, t), this.fields = e || [], this.metadata = n || new Map, r || (r = aa(e)), this.dictionaries = r
                 }
                 return Object(M.a)(t, [{
                     key: e,
                     get: function() {
                         return "Schema"
                     }
                 }, {
@@ -8538,15 +8551,15 @@
                         return "Schema<{ ".concat(this.fields.map((function(e, t) {
                             return "".concat(t, ": ").concat(e)
                         })).join(", "), " }>")
                     }
                 }, {
                     key: "compareTo",
                     value: function(e) {
-                        return Sn.compareSchemas(this, e)
+                        return On.compareSchemas(this, e)
                     }
                 }, {
                     key: "select",
                     value: function() {
                         for (var e = arguments.length, n = new Array(e), r = 0; r < e; r++) n[r] = arguments[r];
                         var i = n.reduce((function(e, t) {
                             return (e[t] = !0) && e
@@ -8563,42 +8576,42 @@
                             return e.fields[t]
                         })).filter(Boolean), this.metadata)
                     }
                 }, {
                     key: "assign",
                     value: function() {
                         for (var e = arguments.length, n = new Array(e), r = 0; r < e; r++) n[r] = arguments[r];
-                        var i = n[0] instanceof t ? n[0] : new t(qi(aa, n)),
-                            a = hn(this.fields),
-                            o = oa(oa(new Map, this.metadata), i.metadata),
+                        var i = n[0] instanceof t ? n[0] : new t(Ki(ra, n)),
+                            a = cn(this.fields),
+                            o = ia(ia(new Map, this.metadata), i.metadata),
                             u = i.fields.filter((function(e) {
                                 var t = a.findIndex((function(t) {
                                     return t.name === e.name
                                 }));
                                 return !~t || (a[t] = e.clone({
-                                    metadata: oa(oa(new Map, a[t].metadata), e.metadata)
+                                    metadata: ia(ia(new Map, a[t].metadata), e.metadata)
                                 })) && !1
                             })),
-                            s = ua(u, new Map);
-                        return new t([].concat(hn(a), hn(u)), o, new Map([].concat(hn(this.dictionaries), hn(s))))
+                            s = aa(u, new Map);
+                        return new t([].concat(cn(a), cn(u)), o, new Map([].concat(cn(this.dictionaries), cn(s))))
                     }
                 }], [{
                     key: "from",
                     value: function() {
                         return t.new(arguments.length <= 0 ? void 0 : arguments[0], arguments.length <= 1 ? void 0 : arguments[1])
                     }
                 }, {
                     key: "new",
                     value: function() {
                         for (var e = arguments.length, n = new Array(e), r = 0; r < e; r++) n[r] = arguments[r];
-                        return new t(Gi(n)[0])
+                        return new t(Qi(n)[0])
                     }
                 }]), t
             }(Symbol.toStringTag),
-            aa = function(e) {
+            ra = function(e) {
                 function t(e, n) {
                     var r = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
                         i = arguments.length > 3 ? arguments[3] : void 0;
                     Object(C.a)(this, t), this.name = e, this.type = n, this.nullable = r, this.metadata = i || new Map
                 }
                 return Object(M.a)(t, [{
                     key: "typeId",
@@ -8614,15 +8627,15 @@
                     key: "toString",
                     value: function() {
                         return "".concat(this.name, ": ").concat(this.type)
                     }
                 }, {
                     key: "compareTo",
                     value: function(e) {
-                        return Sn.compareField(this, e)
+                        return On.compareField(this, e)
                     }
                 }, {
                     key: "clone",
                     value: function() {
                         for (var e, n, r, i, a, o, u, s, c, l, f = arguments.length, h = new Array(f), d = 0; d < f; d++) h[d] = arguments[d];
                         var p = h[0],
                             y = h[1],
@@ -8639,49 +8652,49 @@
                             o = n[2],
                             u = n[3];
                         return n[0] && "object" === typeof n[0] && (i = n[0].name, void 0 === a && (a = n[0].type), void 0 === o && (o = n[0].nullable), void 0 === u && (u = n[0].metadata)), new t("".concat(i), a, o, u)
                     }
                 }]), t
             }(Symbol.toStringTag);
 
-        function oa(e, t) {
-            return new Map([].concat(hn(e || new Map), hn(t || new Map)))
+        function ia(e, t) {
+            return new Map([].concat(cn(e || new Map), cn(t || new Map)))
         }
 
-        function ua(e) {
+        function aa(e) {
             for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map, n = -1, r = e.length; ++n < r;) {
                 var i = e[n].type;
-                if (Tn.isDictionary(i))
+                if (jn.isDictionary(i))
                     if (t.has(i.id)) {
                         if (t.get(i.id) !== i.dictionary) throw new Error("Cannot create Schema containing two different dictionaries with the same Id")
                     } else t.set(i.id, i.dictionary);
-                i.children && i.children.length > 0 && ua(i.children, t)
+                i.children && i.children.length > 0 && aa(i.children, t)
             }
             return t
         }
-        ia.prototype.fields = null, ia.prototype.metadata = null, ia.prototype.dictionaries = null, aa.prototype.type = null, aa.prototype.name = null, aa.prototype.nullable = null, aa.prototype.metadata = null;
-        var sa = function(e) {
+        na.prototype.fields = null, na.prototype.metadata = null, na.prototype.dictionaries = null, ra.prototype.type = null, ra.prototype.name = null, ra.prototype.nullable = null, ra.prototype.metadata = null;
+        var oa = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._run = new _i, r._offsets = new vr, r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._run = new gi, r._offsets = new dr, r
                 }
                 return Object(M.a)(n, [{
                     key: "addChild",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "0";
                         if (this.numChildren > 0) throw new Error("ListBuilder can only have one child.");
-                        return this.children[this.numChildren] = e, this.type = new Zn(new aa(t, e.type, !0)), this.numChildren - 1
+                        return this.children[this.numChildren] = e, this.type = new qn(new ra(t, e.type, !0)), this.numChildren - 1
                     }
                 }, {
                     key: "clear",
                     value: function() {
-                        return this._run.clear(), Ut(Object(Nt.a)(n.prototype), "clear", this).call(this)
+                        return this._run.clear(), Ct(Object(Ft.a)(n.prototype), "clear", this).call(this)
                     }
                 }, {
                     key: "_flushPending",
                     value: function(e) {
                         var t, n, r = this._run,
                             i = this._offsets,
                             a = this._setValue,
@@ -8695,105 +8708,105 @@
                         } catch (c) {
                             u.e(c)
                         } finally {
                             u.f()
                         }
                     }
                 }]), n
-            }(kr),
-            ca = function(e) {
+            }(br),
+            ua = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e;
-                    return Object(C.a)(this, n), (e = t.apply(this, arguments))._run = new _i, e
+                    return Object(C.a)(this, n), (e = t.apply(this, arguments))._run = new gi, e
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t) {
-                        Ut(Object(Nt.a)(n.prototype), "setValue", this).call(this, e, this._run.bind(t))
+                        Ct(Object(Ft.a)(n.prototype), "setValue", this).call(this, e, this._run.bind(t))
                     }
                 }, {
                     key: "addChild",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "0";
                         if (this.numChildren > 0) throw new Error("FixedSizeListBuilder can only have one child.");
                         var n = this.children.push(e);
-                        return this.type = new nr(this.type.listSize, new aa(t, e.type, !0)), n
+                        return this.type = new Xn(this.type.listSize, new ra(t, e.type, !0)), n
                     }
                 }, {
                     key: "clear",
                     value: function() {
-                        return this._run.clear(), Ut(Object(Nt.a)(n.prototype), "clear", this).call(this)
+                        return this._run.clear(), Ct(Object(Ft.a)(n.prototype), "clear", this).call(this)
                     }
                 }]), n
-            }(mr),
-            la = function(e) {
+            }(yr),
+            sa = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "set",
                     value: function(e, t) {
-                        return Ut(Object(Nt.a)(n.prototype), "set", this).call(this, e, t)
+                        return Ct(Object(Ft.a)(n.prototype), "set", this).call(this, e, t)
                     }
                 }, {
                     key: "setValue",
                     value: function(e, t) {
                         t = t instanceof Map ? t : new Map(Object.entries(t));
                         var n = this._pending || (this._pending = new Map),
                             r = n.get(e);
                         r && (this._pendingLength -= r.size), this._pendingLength += t.size, n.set(e, t)
                     }
                 }, {
                     key: "addChild",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "".concat(this.numChildren);
                         if (this.numChildren > 0) throw new Error("ListBuilder can only have one child.");
-                        return this.children[this.numChildren] = e, this.type = new rr(new aa(t, e.type, !0), this.type.keysSorted), this.numChildren - 1
+                        return this.children[this.numChildren] = e, this.type = new er(new ra(t, e.type, !0), this.type.keysSorted), this.numChildren - 1
                     }
                 }, {
                     key: "_flushPending",
                     value: function(e) {
                         var t = this,
                             n = this._offsets,
                             r = this._setValue;
                         e.forEach((function(e, i) {
                             void 0 === e ? n.set(i, 0) : (n.set(i, e.size), r(t, i, e))
                         }))
                     }
                 }]), n
-            }(kr),
-            fa = function(e) {
+            }(br),
+            ca = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "addChild",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "".concat(this.numChildren),
                             n = this.children.push(e);
-                        return this.type = new Xn([].concat(hn(this.type.children), [new aa(t, e.type, !0)])), n
+                        return this.type = new Gn([].concat(cn(this.type.children), [new ra(t, e.type, !0)])), n
                     }
                 }]), n
-            }(mr),
-            ha = function(e) {
+            }(yr),
+            la = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._typeIds = new pr(new Int8Array(0), 1), "function" === typeof e.valueToChildTypeId && (r._valueToChildTypeId = e.valueToChildTypeId), r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._typeIds = new fr(new Int8Array(0), 1), "function" === typeof e.valueToChildTypeId && (r._valueToChildTypeId = e.valueToChildTypeId), r
                 }
                 return Object(M.a)(n, [{
                     key: "typeIdToChildIndex",
                     get: function() {
                         return this.type.typeIdToChildIndex
                     }
                 }, {
@@ -8805,207 +8818,207 @@
                     key: "set",
                     value: function(e, t, n) {
                         return void 0 === n && (n = this._valueToChildTypeId(this, t, e)), this.setValid(e, this.isValid(t)) && this.setValue(e, t, n), this
                     }
                 }, {
                     key: "setValue",
                     value: function(e, t, r) {
-                        this._typeIds.set(e, r), Ut(Object(Nt.a)(n.prototype), "setValue", this).call(this, e, t)
+                        this._typeIds.set(e, r), Ct(Object(Ft.a)(n.prototype), "setValue", this).call(this, e, t)
                     }
                 }, {
                     key: "addChild",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "".concat(this.children.length),
                             n = this.children.push(e),
                             r = this.type,
                             i = r.children,
                             a = r.mode,
                             o = r.typeIds,
-                            u = [].concat(hn(i), [new aa(t, e.type)]);
-                        return this.type = new er(a, [].concat(hn(o), [n]), u), n
+                            u = [].concat(cn(i), [new ra(t, e.type)]);
+                        return this.type = new Jn(a, [].concat(cn(o), [n]), u), n
                     }
                 }, {
                     key: "_valueToChildTypeId",
                     value: function(e, t, n) {
                         throw new Error("Cannot map UnionBuilder value to child typeId. Pass the `childTypeId` as the second argument to unionBuilder.append(), or supply a `valueToChildTypeId` function as part of the UnionBuilder constructor options.")
                     }
                 }]), n
-            }(mr),
-            da = function(e) {
+            }(yr),
+            fa = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ha),
-            pa = function(e) {
+            }(la),
+            ha = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e))._offsets = new pr(new Int32Array(0)), r
+                    return Object(C.a)(this, n), (r = t.call(this, e))._offsets = new fr(new Int32Array(0)), r
                 }
                 return Object(M.a)(n, [{
                     key: "setValue",
                     value: function(e, t, r) {
                         var i = this.type.typeIdToChildIndex[r];
-                        return this._offsets.set(e, this.getChildAt(i).length), Ut(Object(Nt.a)(n.prototype), "setValue", this).call(this, e, t, r)
+                        return this._offsets.set(e, this.getChildAt(i).length), Ct(Object(Ft.a)(n.prototype), "setValue", this).call(this, e, t, r)
                     }
                 }]), n
-            }(ha),
-            ya = function(e) {
+            }(la),
+            da = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(dn),
-            va = function(e, t, n) {
+            }(ln),
+            pa = function(e, t, n) {
                 e[t] = n % 4294967296 | 0, e[t + 1] = n / 4294967296 | 0
             },
-            ba = function(e, t, n, r) {
+            ya = function(e, t, n, r) {
                 var i = t[n],
                     a = t[n + 1];
                 null != i && null != a && e.set(r.subarray(0, a - i), i)
             },
-            ma = function(e, t, n) {
+            va = function(e, t, n) {
                 ! function(e, t, n) {
                     e[t] = n / 864e5 | 0
                 }(e.values, t, n.valueOf())
             },
-            ga = function(e, t, n) {
+            ba = function(e, t, n) {
                 var r = e.values;
-                va(r, 2 * t, n.valueOf())
+                pa(r, 2 * t, n.valueOf())
             },
-            ka = function(e, t, n) {
+            ma = function(e, t, n) {
                 var r = e.stride;
                 e.values[r * t] = n
             },
-            wa = function(e, t, n) {
+            ga = function(e, t, n) {
                 var r = e.stride;
-                e.values[r * t] = Dr(n)
+                e.values[r * t] = Er(n)
             },
-            _a = function(e, t, n) {
+            ka = function(e, t, n) {
                 switch (typeof n) {
                     case "bigint":
                         e.values64[t] = n;
                         break;
                     case "number":
                         e.values[t * e.stride] = n;
                         break;
                     default:
                         var r = n,
                             i = e.stride,
                             a = Re(e.ArrayType, r);
                         e.values.set(a.subarray(0, i), i * t)
                 }
             },
-            Oa = function(e, t, n) {
+            wa = function(e, t, n) {
                 var r = e.values;
-                return va(r, 2 * t, n / 1e3)
+                return pa(r, 2 * t, n / 1e3)
             },
-            xa = function(e, t, n) {
+            _a = function(e, t, n) {
                 var r = e.values;
-                return va(r, 2 * t, n)
+                return pa(r, 2 * t, n)
             },
-            ja = function(e, t, n) {
+            Oa = function(e, t, n) {
                 return function(e, t, n) {
                     e[t] = 1e3 * n % 4294967296 | 0, e[t + 1] = 1e3 * n / 4294967296 | 0
                 }(e.values, 2 * t, n)
             },
-            Sa = function(e, t, n) {
+            ja = function(e, t, n) {
                 return function(e, t, n) {
                     e[t] = 1e6 * n % 4294967296 | 0, e[t + 1] = 1e6 * n / 4294967296 | 0
                 }(e.values, 2 * t, n)
             },
-            Ta = function(e, t, n) {
+            xa = function(e, t, n) {
                 e.values[e.stride * t] = n
             },
-            Ia = function(e, t, n) {
+            Sa = function(e, t, n) {
                 e.values[e.stride * t] = n
             },
-            Ea = function(e, t, n) {
+            Ta = function(e, t, n) {
                 e.values.set(n.subarray(0, 2), 2 * t)
             },
-            Aa = function(e, t, n) {
+            Ia = function(e, t, n) {
                 e.values.set(n.subarray(0, 2), 2 * t)
             },
-            Ba = function(e, t, n) {
+            Ea = function(e, t, n) {
                 var r = e.typeIdToChildIndex[e.typeIds[t]],
                     i = e.getChildAt(r);
                 i && i.set(e.valueOffsets[t], n)
             },
-            Da = function(e, t, n) {
+            Aa = function(e, t, n) {
                 var r = e.typeIdToChildIndex[e.typeIds[t]],
                     i = e.getChildAt(r);
                 i && i.set(t, n)
             },
-            La = function(e, t, n) {
+            Ba = function(e, t, n) {
                 e.values.set(n.subarray(0, 2), 2 * t)
             },
-            Fa = function(e, t, n) {
+            Da = function(e, t, n) {
                 e.values[t] = 12 * n[0] + n[1] % 12
             };
-        ya.prototype.visitBool = function(e, t, n) {
+        da.prototype.visitBool = function(e, t, n) {
             var r = e.offset,
                 i = e.values,
                 a = r + t;
             n ? i[a >> 3] |= 1 << a % 8 : i[a >> 3] &= ~(1 << a % 8)
-        }, ya.prototype.visitInt = function(e, t, n) {
-            e.type.bitWidth < 64 ? ka(e, t, n) : _a(e, t, n)
-        }, ya.prototype.visitInt8 = ka, ya.prototype.visitInt16 = ka, ya.prototype.visitInt32 = ka, ya.prototype.visitInt64 = _a, ya.prototype.visitUint8 = ka, ya.prototype.visitUint16 = ka, ya.prototype.visitUint32 = ka, ya.prototype.visitUint64 = _a, ya.prototype.visitFloat = function(e, t, n) {
-            e.type.precision !== Gt.HALF ? ka(e, t, n) : wa(e, t, n)
-        }, ya.prototype.visitFloat16 = wa, ya.prototype.visitFloat32 = ka, ya.prototype.visitFloat64 = ka, ya.prototype.visitUtf8 = function(e, t, n) {
+        }, da.prototype.visitInt = function(e, t, n) {
+            e.type.bitWidth < 64 ? ma(e, t, n) : ka(e, t, n)
+        }, da.prototype.visitInt8 = ma, da.prototype.visitInt16 = ma, da.prototype.visitInt32 = ma, da.prototype.visitInt64 = ka, da.prototype.visitUint8 = ma, da.prototype.visitUint16 = ma, da.prototype.visitUint32 = ma, da.prototype.visitUint64 = ka, da.prototype.visitFloat = function(e, t, n) {
+            e.type.precision !== Kt.HALF ? ma(e, t, n) : ga(e, t, n)
+        }, da.prototype.visitFloat16 = ga, da.prototype.visitFloat32 = ma, da.prototype.visitFloat64 = ma, da.prototype.visitUtf8 = function(e, t, n) {
             var r = e.values,
                 i = e.valueOffsets;
-            ba(r, i, t, se(n))
-        }, ya.prototype.visitBinary = function(e, t, n) {
+            ya(r, i, t, se(n))
+        }, da.prototype.visitBinary = function(e, t, n) {
             var r = e.values,
                 i = e.valueOffsets;
-            return ba(r, i, t, n)
-        }, ya.prototype.visitFixedSizeBinary = function(e, t, n) {
+            return ya(r, i, t, n)
+        }, da.prototype.visitFixedSizeBinary = function(e, t, n) {
             var r = e.stride;
             e.values.set(n.subarray(0, r), r * t)
-        }, ya.prototype.visitDate = function(e, t, n) {
-            e.type.unit === Qt.DAY ? ma(e, t, n) : ga(e, t, n)
-        }, ya.prototype.visitDateDay = ma, ya.prototype.visitDateMillisecond = ga, ya.prototype.visitTimestamp = function(e, t, n) {
+        }, da.prototype.visitDate = function(e, t, n) {
+            e.type.unit === Ht.DAY ? va(e, t, n) : ba(e, t, n)
+        }, da.prototype.visitDateDay = va, da.prototype.visitDateMillisecond = ba, da.prototype.visitTimestamp = function(e, t, n) {
             switch (e.type.unit) {
-                case qt.SECOND:
+                case $t.SECOND:
+                    return wa(e, t, n);
+                case $t.MILLISECOND:
+                    return _a(e, t, n);
+                case $t.MICROSECOND:
                     return Oa(e, t, n);
-                case qt.MILLISECOND:
-                    return xa(e, t, n);
-                case qt.MICROSECOND:
-                    return ja(e, t, n);
-                case qt.NANOSECOND:
-                    return Sa(e, t, n)
+                case $t.NANOSECOND:
+                    return ja(e, t, n)
             }
-        }, ya.prototype.visitTimestampSecond = Oa, ya.prototype.visitTimestampMillisecond = xa, ya.prototype.visitTimestampMicrosecond = ja, ya.prototype.visitTimestampNanosecond = Sa, ya.prototype.visitTime = function(e, t, n) {
+        }, da.prototype.visitTimestampSecond = wa, da.prototype.visitTimestampMillisecond = _a, da.prototype.visitTimestampMicrosecond = Oa, da.prototype.visitTimestampNanosecond = ja, da.prototype.visitTime = function(e, t, n) {
             switch (e.type.unit) {
-                case qt.SECOND:
+                case $t.SECOND:
+                    return xa(e, t, n);
+                case $t.MILLISECOND:
+                    return Sa(e, t, n);
+                case $t.MICROSECOND:
                     return Ta(e, t, n);
-                case qt.MILLISECOND:
-                    return Ia(e, t, n);
-                case qt.MICROSECOND:
-                    return Ea(e, t, n);
-                case qt.NANOSECOND:
-                    return Aa(e, t, n)
+                case $t.NANOSECOND:
+                    return Ia(e, t, n)
             }
-        }, ya.prototype.visitTimeSecond = Ta, ya.prototype.visitTimeMillisecond = Ia, ya.prototype.visitTimeMicrosecond = Ea, ya.prototype.visitTimeNanosecond = Aa, ya.prototype.visitDecimal = function(e, t, n) {
+        }, da.prototype.visitTimeSecond = xa, da.prototype.visitTimeMillisecond = Sa, da.prototype.visitTimeMicrosecond = Ta, da.prototype.visitTimeNanosecond = Ia, da.prototype.visitDecimal = function(e, t, n) {
             e.values.set(n.subarray(0, 4), 4 * t)
-        }, ya.prototype.visitList = function(e, t, n) {
+        }, da.prototype.visitList = function(e, t, n) {
             for (var r = e.getChildAt(0), i = e.valueOffsets, a = -1, o = i[t], u = i[t + 1]; o < u;) r.set(o++, n.get(++a))
-        }, ya.prototype.visitStruct = function(e, t, n) {
+        }, da.prototype.visitStruct = function(e, t, n) {
             var r, i, a = n instanceof Map ? (r = t, i = n, function(e, t, n) {
                 return e && e.set(r, i.get(t.name))
-            }) : n instanceof Ht ? function(e, t) {
+            }) : n instanceof zt ? function(e, t) {
                 return function(n, r, i) {
                     return n && n.set(e, t.get(i))
                 }
             }(t, n) : Array.isArray(n) ? function(e, t) {
                 return function(n, r, i) {
                     return n && n.set(e, t[i])
                 }
@@ -9013,282 +9026,282 @@
                 return function(n, r, i) {
                     return n && n.set(e, t[r.name])
                 }
             }(t, n);
             e.type.children.forEach((function(t, n) {
                 return a(e.getChildAt(n), t, n)
             }))
-        }, ya.prototype.visitUnion = function(e, t, n) {
-            e.type.mode === Jt.Dense ? Ba(e, t, n) : Da(e, t, n)
-        }, ya.prototype.visitDenseUnion = Ba, ya.prototype.visitSparseUnion = Da, ya.prototype.visitDictionary = function(e, t, n) {
+        }, da.prototype.visitUnion = function(e, t, n) {
+            e.type.mode === Qt.Dense ? Ea(e, t, n) : Aa(e, t, n)
+        }, da.prototype.visitDenseUnion = Ea, da.prototype.visitSparseUnion = Aa, da.prototype.visitDictionary = function(e, t, n) {
             var r = e.getKey(t);
             null !== r && e.setValue(r, n)
-        }, ya.prototype.visitInterval = function(e, t, n) {
-            e.type.unit === Zt.DAY_TIME ? La(e, t, n) : Fa(e, t, n)
-        }, ya.prototype.visitIntervalDayTime = La, ya.prototype.visitIntervalYearMonth = Fa, ya.prototype.visitFixedSizeList = function(e, t, n) {
+        }, da.prototype.visitInterval = function(e, t, n) {
+            e.type.unit === qt.DAY_TIME ? Ba(e, t, n) : Da(e, t, n)
+        }, da.prototype.visitIntervalDayTime = Ba, da.prototype.visitIntervalYearMonth = Da, da.prototype.visitFixedSizeList = function(e, t, n) {
             for (var r = e.getChildAt(0), i = e.stride, a = -1, o = t * i; ++a < i;) r.set(o + a, n.get(a))
-        }, ya.prototype.visitMap = function(e, t, n) {
-            for (var r = e.getChildAt(0), i = e.valueOffsets, a = n instanceof Map ? hn(n) : Object.entries(n), o = -1, u = i[t], s = i[t + 1]; u < s;) r.set(u++, a[++o])
+        }, da.prototype.visitMap = function(e, t, n) {
+            for (var r = e.getChildAt(0), i = e.valueOffsets, a = n instanceof Map ? cn(n) : Object.entries(n), o = -1, u = i[t], s = i[t + 1]; u < s;) r.set(u++, a[++o])
         };
-        var Ca, Ma = new ya,
-            Na = function(e) {
+        var La, Fa = new da,
+            Ca = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "visitNull",
                     value: function() {
-                        return _r
+                        return gr
                     }
                 }, {
                     key: "visitBool",
                     value: function() {
-                        return wr
+                        return mr
                     }
                 }, {
                     key: "visitInt",
                     value: function() {
-                        return Jr
+                        return Qr
                     }
                 }, {
                     key: "visitInt8",
                     value: function() {
-                        return Zr
+                        return qr
                     }
                 }, {
                     key: "visitInt16",
                     value: function() {
-                        return Xr
+                        return Gr
                     }
                 }, {
                     key: "visitInt32",
                     value: function() {
-                        return ei
+                        return Jr
                     }
                 }, {
                     key: "visitInt64",
                     value: function() {
-                        return ti
+                        return Zr
                     }
                 }, {
                     key: "visitUint8",
                     value: function() {
-                        return ni
+                        return Xr
                     }
                 }, {
                     key: "visitUint16",
                     value: function() {
-                        return ri
+                        return ei
                     }
                 }, {
                     key: "visitUint32",
                     value: function() {
-                        return ii
+                        return ti
                     }
                 }, {
                     key: "visitUint64",
                     value: function() {
-                        return ai
+                        return ni
                     }
                 }, {
                     key: "visitFloat",
                     value: function() {
-                        return Lr
+                        return Ar
                     }
                 }, {
                     key: "visitFloat16",
                     value: function() {
-                        return Fr
+                        return Br
                     }
                 }, {
                     key: "visitFloat32",
                     value: function() {
-                        return Cr
+                        return Dr
                     }
                 }, {
                     key: "visitFloat64",
                     value: function() {
-                        return Mr
+                        return Lr
                     }
                 }, {
                     key: "visitUtf8",
                     value: function() {
-                        return wi
+                        return mi
                     }
                 }, {
                     key: "visitBinary",
                     value: function() {
-                        return ki
+                        return bi
                     }
                 }, {
                     key: "visitFixedSizeBinary",
                     value: function() {
-                        return Ir
+                        return xr
                     }
                 }, {
                     key: "visitDate",
                     value: function() {
-                        return Or
+                        return kr
                     }
                 }, {
                     key: "visitDateDay",
                     value: function() {
-                        return xr
+                        return wr
                     }
                 }, {
                     key: "visitDateMillisecond",
                     value: function() {
-                        return jr
+                        return _r
                     }
                 }, {
                     key: "visitTimestamp",
                     value: function() {
-                        return hi
+                        return ci
                     }
                 }, {
                     key: "visitTimestampSecond",
                     value: function() {
-                        return di
+                        return li
                     }
                 }, {
                     key: "visitTimestampMillisecond",
                     value: function() {
-                        return pi
+                        return fi
                     }
                 }, {
                     key: "visitTimestampMicrosecond",
                     value: function() {
-                        return yi
+                        return hi
                     }
                 }, {
                     key: "visitTimestampNanosecond",
                     value: function() {
-                        return vi
+                        return di
                     }
                 }, {
                     key: "visitTime",
                     value: function() {
-                        return ui
+                        return ii
                     }
                 }, {
                     key: "visitTimeSecond",
                     value: function() {
-                        return si
+                        return ai
                     }
                 }, {
                     key: "visitTimeMillisecond",
                     value: function() {
-                        return ci
+                        return oi
                     }
                 }, {
                     key: "visitTimeMicrosecond",
                     value: function() {
-                        return li
+                        return ui
                     }
                 }, {
                     key: "visitTimeNanosecond",
                     value: function() {
-                        return fi
+                        return si
                     }
                 }, {
                     key: "visitDecimal",
                     value: function() {
-                        return Sr
+                        return Or
                     }
                 }, {
                     key: "visitList",
                     value: function() {
-                        return sa
+                        return oa
                     }
                 }, {
                     key: "visitStruct",
                     value: function() {
-                        return fa
+                        return ca
                     }
                 }, {
                     key: "visitUnion",
                     value: function() {
-                        return ha
+                        return la
                     }
                 }, {
                     key: "visitDenseUnion",
                     value: function() {
-                        return pa
+                        return ha
                     }
                 }, {
                     key: "visitSparseUnion",
                     value: function() {
-                        return da
+                        return fa
                     }
                 }, {
                     key: "visitDictionary",
                     value: function() {
-                        return Tr
+                        return jr
                     }
                 }, {
                     key: "visitInterval",
                     value: function() {
-                        return bi
+                        return pi
                     }
                 }, {
                     key: "visitIntervalDayTime",
                     value: function() {
-                        return mi
+                        return yi
                     }
                 }, {
                     key: "visitIntervalYearMonth",
                     value: function() {
-                        return gi
+                        return vi
                     }
                 }, {
                     key: "visitFixedSizeList",
                     value: function() {
-                        return ca
+                        return ua
                     }
                 }, {
                     key: "visitMap",
                     value: function() {
-                        return la
+                        return sa
                     }
                 }]), n
-            }(dn),
-            Ua = new Na;
-        mr.new = function e(t) {
+            }(ln),
+            Ma = new Ca;
+        yr.new = function e(t) {
                 var n = t.type,
-                    r = new(Ua.getVisitFn(n)())(t);
+                    r = new(Ma.getVisitFn(n)())(t);
                 if (n.children && n.children.length > 0) {
                     var i = t.children || [],
                         a = {
                             nullValues: t.nullValues
                         },
                         o = Array.isArray(i) ? function(e, t) {
                             return i[t] || a
                         } : function(e) {
                             var t = e.name;
                             return i[t] || a
                         };
                     n.children.forEach((function(t, n) {
                         var i = t.type,
                             a = o(t, n);
-                        r.children.push(e(Mt(Mt({}, a), {}, {
+                        r.children.push(e(Object(Lt.a)(Object(Lt.a)({}, a), {}, {
                             type: i
                         })))
                     }))
                 }
                 return r
-            }, Object.keys($t).map((function(e) {
-                return $t[e]
+            }, Object.keys(Wt).map((function(e) {
+                return Wt[e]
             })).filter((function(e) {
-                return "number" === typeof e && e !== $t.NONE
+                return "number" === typeof e && e !== Wt.NONE
             })).forEach((function(e) {
-                Ua.visit(e).prototype._setValue = Ma.getVisitFn(e)
-            })), wi.prototype._setValue = Ma.visitBinary,
+                Ma.visit(e).prototype._setValue = Fa.getVisitFn(e)
+            })), mi.prototype._setValue = Fa.visitBinary,
             function(e) {
                 ! function(t) {
                     ! function(t) {
                         ! function(t) {
                             var n = function() {
                                 function t() {
                                     Object(C.a)(this, t), this.bb = null, this.bb_pos = 0
@@ -9298,21 +9311,21 @@
                                     value: function(e, t) {
                                         return this.bb_pos = e, this.bb = t, this
                                     }
                                 }, {
                                     key: "version",
                                     value: function() {
                                         var e = this.bb.__offset(this.bb_pos, 4);
-                                        return e ? this.bb.readInt16(this.bb_pos + e) : Pt.apache.arrow.flatbuf.MetadataVersion.V1
+                                        return e ? this.bb.readInt16(this.bb_pos + e) : Mt.apache.arrow.flatbuf.MetadataVersion.V1
                                     }
                                 }, {
                                     key: "schema",
                                     value: function(e) {
                                         var t = this.bb.__offset(this.bb_pos, 6);
-                                        return t ? (e || new Pt.apache.arrow.flatbuf.Schema).__init(this.bb.__indirect(this.bb_pos + t), this.bb) : null
+                                        return t ? (e || new Mt.apache.arrow.flatbuf.Schema).__init(this.bb.__indirect(this.bb_pos + t), this.bb) : null
                                     }
                                 }, {
                                     key: "dictionaries",
                                     value: function(t, n) {
                                         var r = this.bb.__offset(this.bb_pos, 8);
                                         return r ? (n || new e.apache.arrow.flatbuf.Block).__init(this.bb.__vector(this.bb_pos + r) + 24 * t, this.bb) : null
                                     }
@@ -9343,15 +9356,15 @@
                                     key: "startFooter",
                                     value: function(e) {
                                         e.startObject(4)
                                     }
                                 }, {
                                     key: "addVersion",
                                     value: function(e, t) {
-                                        e.addFieldInt16(0, t, Pt.apache.arrow.flatbuf.MetadataVersion.V1)
+                                        e.addFieldInt16(0, t, Mt.apache.arrow.flatbuf.MetadataVersion.V1)
                                     }
                                 }, {
                                     key: "addSchema",
                                     value: function(e, t) {
                                         e.addFieldOffset(1, t, 0)
                                     }
                                 }, {
@@ -9391,15 +9404,15 @@
                                     }
                                 }]), t
                             }();
                             t.Footer = n
                         }(t.flatbuf || (t.flatbuf = {}))
                     }(t.arrow || (t.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Ca || (Ca = {})),
+            }(La || (La = {})),
             function(e) {
                 ! function(e) {
                     ! function(e) {
                         ! function(e) {
                             var t = function() {
                                 function e() {
                                     Object(C.a)(this, e), this.bb = null, this.bb_pos = 0
@@ -9431,23 +9444,23 @@
                                     }
                                 }]), e
                             }();
                             e.Block = t
                         }(e.flatbuf || (e.flatbuf = {}))
                     }(e.arrow || (e.arrow = {}))
                 }(e.apache || (e.apache = {}))
-            }(Ca || (Ca = {}));
-        var Pa = K.Long,
-            Ra = K.Builder,
-            Va = K.ByteBuffer,
-            za = Ca.apache.arrow.flatbuf.Block,
-            Wa = Ca.apache.arrow.flatbuf.Footer,
-            Ya = function() {
+            }(La || (La = {}));
+        var Na = K.Long,
+            Ua = K.Builder,
+            Pa = K.ByteBuffer,
+            Ra = La.apache.arrow.flatbuf.Block,
+            Va = La.apache.arrow.flatbuf.Footer,
+            za = function() {
                 function e(t) {
-                    var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : en.V4,
+                    var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Jt.V4,
                         r = arguments.length > 2 ? arguments[2] : void 0,
                         i = arguments.length > 3 ? arguments[3] : void 0;
                     Object(C.a)(this, e), this.schema = t, this.version = n, r && (this._recordBatches = r), i && (this._dictionaryBatches = i)
                 }
                 return Object(M.a)(e, [{
                     key: "numRecordBatches",
                     get: function() {
@@ -9521,37 +9534,37 @@
                     key: "getDictionaryBatch",
                     value: function(e) {
                         return e >= 0 && e < this.numDictionaries && this._dictionaryBatches[e] || null
                     }
                 }], [{
                     key: "decode",
                     value: function(e) {
-                        e = new Va(He(e));
-                        var t = Wa.getRootAsFooter(e),
-                            n = ia.decode(t.schema());
-                        return new Ha(n, t)
+                        e = new Pa(He(e));
+                        var t = Va.getRootAsFooter(e),
+                            n = na.decode(t.schema());
+                        return new Wa(n, t)
                     }
                 }, {
                     key: "encode",
                     value: function(e) {
-                        var t = new Ra,
-                            n = ia.encode(t, e.schema);
-                        Wa.startRecordBatchesVector(t, e.numRecordBatches), hn(e.recordBatches()).slice().reverse().forEach((function(e) {
-                            return $a.encode(t, e)
+                        var t = new Ua,
+                            n = na.encode(t, e.schema);
+                        Va.startRecordBatchesVector(t, e.numRecordBatches), cn(e.recordBatches()).slice().reverse().forEach((function(e) {
+                            return Ya.encode(t, e)
                         }));
                         var r = t.endVector();
-                        Wa.startDictionariesVector(t, e.numDictionaries), hn(e.dictionaryBatches()).slice().reverse().forEach((function(e) {
-                            return $a.encode(t, e)
+                        Va.startDictionariesVector(t, e.numDictionaries), cn(e.dictionaryBatches()).slice().reverse().forEach((function(e) {
+                            return Ya.encode(t, e)
                         }));
                         var i = t.endVector();
-                        return Wa.startFooter(t), Wa.addSchema(t, n), Wa.addVersion(t, en.V4), Wa.addRecordBatches(t, r), Wa.addDictionaries(t, i), Wa.finishFooterBuffer(t, Wa.endFooter(t)), t.asUint8Array()
+                        return Va.startFooter(t), Va.addSchema(t, n), Va.addVersion(t, Jt.V4), Va.addRecordBatches(t, r), Va.addDictionaries(t, i), Va.finishFooterBuffer(t, Va.endFooter(t)), t.asUint8Array()
                     }
                 }]), e
             }(),
-            Ha = function(e) {
+            Wa = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     var i;
                     return Object(C.a)(this, n), (i = t.call(this, e, r.version()))._footer = r, i
                 }
@@ -9566,59 +9579,59 @@
                         return this._footer.dictionariesLength()
                     }
                 }, {
                     key: "getRecordBatch",
                     value: function(e) {
                         if (e >= 0 && e < this.numRecordBatches) {
                             var t = this._footer.recordBatches(e);
-                            if (t) return $a.decode(t)
+                            if (t) return Ya.decode(t)
                         }
                         return null
                     }
                 }, {
                     key: "getDictionaryBatch",
                     value: function(e) {
                         if (e >= 0 && e < this.numDictionaries) {
                             var t = this._footer.dictionaries(e);
-                            if (t) return $a.decode(t)
+                            if (t) return Ya.decode(t)
                         }
                         return null
                     }
                 }]), n
-            }(Ya),
-            $a = function() {
+            }(za),
+            Ya = function() {
                 function e(t, n, r) {
                     Object(C.a)(this, e), this.metaDataLength = t, this.offset = "number" === typeof r ? r : r.low, this.bodyLength = "number" === typeof n ? n : n.low
                 }
                 return Object(M.a)(e, null, [{
                     key: "decode",
                     value: function(t) {
                         return new e(t.metaDataLength(), t.bodyLength(), t.offset())
                     }
                 }, {
                     key: "encode",
                     value: function(e, t) {
                         var n = t.metaDataLength,
-                            r = new Pa(t.offset, 0),
-                            i = new Pa(t.bodyLength, 0);
-                        return za.createBlock(e, r, n, i)
+                            r = new Na(t.offset, 0),
+                            i = new Na(t.bodyLength, 0);
+                        return Ra.createBlock(e, r, n, i)
                     }
                 }]), e
             }(),
-            Ka = function(e) {
+            Ha = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "write",
                     value: function(e) {
-                        if ((e = He(e)).byteLength > 0) return Ut(Object(Nt.a)(n.prototype), "write", this).call(this, e)
+                        if ((e = He(e)).byteLength > 0) return Ct(Object(Ft.a)(n.prototype), "write", this).call(this, e)
                     }
                 }, {
                     key: "toString",
                     value: function() {
                         return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? ue(this.toUint8Array(!0)) : this.toUint8Array(!1).then(ue)
                     }
                 }, {
@@ -9673,17 +9686,17 @@
                                 [3, 16, 20, 30],
                                 [21, , 25, 29]
                             ])
                         })))()
                     }
                 }]), n
             }(pe),
-            Qa = function(e) {
+            $a = function(e) {
                 function t(e) {
-                    Object(C.a)(this, t), e && (this.source = new Ga(Ot.fromIterable(e)))
+                    Object(C.a)(this, t), e && (this.source = new Qa(Ot.fromIterable(e)))
                 }
                 return Object(M.a)(t, [{
                     key: e,
                     value: function() {
                         return this
                     }
                 }, {
@@ -9709,17 +9722,17 @@
                 }, {
                     key: "read",
                     value: function(e) {
                         return this.source.read(e)
                     }
                 }]), t
             }(Symbol.iterator),
-            qa = function(e) {
+            Ka = function(e) {
                 function t(e) {
-                    Object(C.a)(this, t), e instanceof t ? this.source = e.source : e instanceof Ka ? this.source = new Ja(Ot.fromAsyncIterable(e)) : Fe(e) ? this.source = new Ja(Ot.fromNodeStream(e)) : Le(e) ? this.source = new Ja(Ot.fromDOMStream(e)) : De(e) ? this.source = new Ja(Ot.fromDOMStream(e.body)) : Te(e) ? this.source = new Ja(Ot.fromIterable(e)) : (Se(e) || Ie(e)) && (this.source = new Ja(Ot.fromAsyncIterable(e)))
+                    Object(C.a)(this, t), e instanceof t ? this.source = e.source : e instanceof Ha ? this.source = new qa(Ot.fromAsyncIterable(e)) : Fe(e) ? this.source = new qa(Ot.fromNodeStream(e)) : Le(e) ? this.source = new qa(Ot.fromDOMStream(e)) : De(e) ? this.source = new qa(Ot.fromDOMStream(e.body)) : Te(e) ? this.source = new qa(Ot.fromIterable(e)) : (Se(e) || Ie(e)) && (this.source = new qa(Ot.fromAsyncIterable(e)))
                 }
                 return Object(M.a)(t, [{
                     key: e,
                     value: function() {
                         return this
                     }
                 }, {
@@ -9755,15 +9768,15 @@
                 }, {
                     key: "read",
                     value: function(e) {
                         return this.source.read(e)
                     }
                 }]), t
             }(Symbol.asyncIterator),
-            Ga = function() {
+            Qa = function() {
                 function e(t) {
                     Object(C.a)(this, e), this.source = t
                 }
                 return Object(M.a)(e, [{
                     key: "cancel",
                     value: function(e) {
                         this.return(e)
@@ -9795,15 +9808,15 @@
                 }, {
                     key: "return",
                     value: function(e) {
                         return Object.create(this.source.return && this.source.return(e) || fe)
                     }
                 }]), e
             }(),
-            Ja = function() {
+            qa = function() {
                 function e(t) {
                     var n = this;
                     Object(C.a)(this, e), this.source = t, this._closedPromise = new Promise((function(e) {
                         return n._closedPromiseResolve = e
                     }))
                 }
                 return Object(M.a)(e, [{
@@ -9957,15 +9970,15 @@
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 }]), e
             }(),
-            Za = function(e) {
+            Ga = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     var i;
                     return Object(C.a)(this, n), (i = t.call(this)).position = 0, i.buffer = He(e), i.size = "undefined" === typeof r ? i.buffer.byteLength : r, i
                 }
@@ -10015,16 +10028,16 @@
                     value: function(e) {
                         return this.close(), {
                             done: !0,
                             value: e
                         }
                     }
                 }]), n
-            }(Qa),
-            Xa = function(e) {
+            }($a),
+            Ja = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     var i;
                     return Object(C.a)(this, n), (i = t.call(this)).position = 0, i._handle = e, "number" === typeof r ? i.size = r : i._pending = F(U().mark((function t() {
                         return U().wrap((function(t) {
@@ -10226,21 +10239,21 @@
                             }), e, this)
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 }]), n
-            }(qa);
+            }(Ka);
 
-        function eo(e) {
+        function Za(e) {
             return e < 0 && (e = 4294967295 + e + 1), "0x".concat(e.toString(16))
         }
-        var to = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8],
-            no = function() {
+        var Xa = [1, 10, 100, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8],
+            eo = function() {
                 function e(t) {
                     Object(C.a)(this, e), this.buffer = t
                 }
                 return Object(M.a)(e, [{
                     key: "high",
                     value: function() {
                         return this.buffer[1]
@@ -10280,19 +10293,19 @@
                     key: "greaterThan",
                     value: function(e) {
                         return e.lessThan(this)
                     }
                 }, {
                     key: "hex",
                     value: function() {
-                        return "".concat(eo(this.buffer[1]), " ").concat(eo(this.buffer[0]))
+                        return "".concat(Za(this.buffer[1]), " ").concat(Za(this.buffer[0]))
                     }
                 }]), e
             }(),
-            ro = function(e) {
+            to = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -10319,15 +10332,15 @@
                     }
                 }, {
                     key: "fromString",
                     value: function(e) {
                         for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2), r = e.length, i = new n(t), a = 0; a < r;) {
                             var o = 8 < r - a ? 8 : r - a,
                                 u = new n(new Uint32Array([parseInt(e.substr(a, o), 10), 0])),
-                                s = new n(new Uint32Array([to[o], 0]));
+                                s = new n(new Uint32Array([Xa[o], 0]));
                             i.times(s), i.plus(u), a += o
                         }
                         return i
                     }
                 }, {
                     key: "convertArray",
                     value: function(e) {
@@ -10341,16 +10354,16 @@
                     }
                 }, {
                     key: "add",
                     value: function(e, t) {
                         return new n(new Uint32Array(e.buffer)).plus(t)
                     }
                 }]), n
-            }(no),
-            io = function(e) {
+            }(eo),
+            no = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -10389,15 +10402,15 @@
                     }
                 }, {
                     key: "fromString",
                     value: function(e) {
                         for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(2), r = e.startsWith("-"), i = e.length, a = new n(t), o = r ? 1 : 0; o < i;) {
                             var u = 8 < i - o ? 8 : i - o,
                                 s = new n(new Uint32Array([parseInt(e.substr(o, u), 10), 0])),
-                                c = new n(new Uint32Array([to[u], 0]));
+                                c = new n(new Uint32Array([Xa[u], 0]));
                             a.times(c), a.plus(s), o += u
                         }
                         return r ? a.negate() : a
                     }
                 }, {
                     key: "convertArray",
                     value: function(e) {
@@ -10411,60 +10424,60 @@
                     }
                 }, {
                     key: "add",
                     value: function(e, t) {
                         return new n(new Uint32Array(e.buffer)).plus(t)
                     }
                 }]), n
-            }(no),
-            ao = function() {
+            }(eo),
+            ro = function() {
                 function e(t) {
                     Object(C.a)(this, e), this.buffer = t
                 }
                 return Object(M.a)(e, [{
                     key: "high",
                     value: function() {
-                        return new io(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
+                        return new no(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2))
                     }
                 }, {
                     key: "low",
                     value: function() {
-                        return new io(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset, 2))
+                        return new no(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset, 2))
                     }
                 }, {
                     key: "negate",
                     value: function() {
                         return this.buffer[0] = 1 + ~this.buffer[0], this.buffer[1] = ~this.buffer[1], this.buffer[2] = ~this.buffer[2], this.buffer[3] = ~this.buffer[3], 0 == this.buffer[0] && ++this.buffer[1], 0 == this.buffer[1] && ++this.buffer[2], 0 == this.buffer[2] && ++this.buffer[3], this
                     }
                 }, {
                     key: "times",
                     value: function(e) {
-                        var t = new ro(new Uint32Array([this.buffer[3], 0])),
-                            n = new ro(new Uint32Array([this.buffer[2], 0])),
-                            r = new ro(new Uint32Array([this.buffer[1], 0])),
-                            i = new ro(new Uint32Array([this.buffer[0], 0])),
-                            a = new ro(new Uint32Array([e.buffer[3], 0])),
-                            o = new ro(new Uint32Array([e.buffer[2], 0])),
-                            u = new ro(new Uint32Array([e.buffer[1], 0])),
-                            s = new ro(new Uint32Array([e.buffer[0], 0])),
-                            c = ro.multiply(i, s);
+                        var t = new to(new Uint32Array([this.buffer[3], 0])),
+                            n = new to(new Uint32Array([this.buffer[2], 0])),
+                            r = new to(new Uint32Array([this.buffer[1], 0])),
+                            i = new to(new Uint32Array([this.buffer[0], 0])),
+                            a = new to(new Uint32Array([e.buffer[3], 0])),
+                            o = new to(new Uint32Array([e.buffer[2], 0])),
+                            u = new to(new Uint32Array([e.buffer[1], 0])),
+                            s = new to(new Uint32Array([e.buffer[0], 0])),
+                            c = to.multiply(i, s);
                         this.buffer[0] = c.low();
-                        var l = new ro(new Uint32Array([c.high(), 0]));
-                        return c = ro.multiply(r, s), l.plus(c), c = ro.multiply(i, u), l.plus(c), this.buffer[1] = l.low(), this.buffer[3] = l.lessThan(c) ? 1 : 0, this.buffer[2] = l.high(), new ro(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(ro.multiply(n, s)).plus(ro.multiply(r, u)).plus(ro.multiply(i, o)), this.buffer[3] += ro.multiply(t, s).plus(ro.multiply(n, u)).plus(ro.multiply(r, o)).plus(ro.multiply(i, a)).low(), this
+                        var l = new to(new Uint32Array([c.high(), 0]));
+                        return c = to.multiply(r, s), l.plus(c), c = to.multiply(i, u), l.plus(c), this.buffer[1] = l.low(), this.buffer[3] = l.lessThan(c) ? 1 : 0, this.buffer[2] = l.high(), new to(new Uint32Array(this.buffer.buffer, this.buffer.byteOffset + 8, 2)).plus(to.multiply(n, s)).plus(to.multiply(r, u)).plus(to.multiply(i, o)), this.buffer[3] += to.multiply(t, s).plus(to.multiply(n, u)).plus(to.multiply(r, o)).plus(to.multiply(i, a)).low(), this
                     }
                 }, {
                     key: "plus",
                     value: function(e) {
                         var t = new Uint32Array(4);
                         return t[3] = this.buffer[3] + e.buffer[3] >>> 0, t[2] = this.buffer[2] + e.buffer[2] >>> 0, t[1] = this.buffer[1] + e.buffer[1] >>> 0, t[0] = this.buffer[0] + e.buffer[0] >>> 0, t[0] < this.buffer[0] >>> 0 && ++t[1], t[1] < this.buffer[1] >>> 0 && ++t[2], t[2] < this.buffer[2] >>> 0 && ++t[3], this.buffer[3] = t[3], this.buffer[2] = t[2], this.buffer[1] = t[1], this.buffer[0] = t[0], this
                     }
                 }, {
                     key: "hex",
                     value: function() {
-                        return "".concat(eo(this.buffer[3]), " ").concat(eo(this.buffer[2]), " ").concat(eo(this.buffer[1]), " ").concat(eo(this.buffer[0]))
+                        return "".concat(Za(this.buffer[3]), " ").concat(Za(this.buffer[2]), " ").concat(Za(this.buffer[1]), " ").concat(Za(this.buffer[0]))
                     }
                 }], [{
                     key: "multiply",
                     value: function(t, n) {
                         return new e(new Uint32Array(t.buffer)).times(n)
                     }
                 }, {
@@ -10486,194 +10499,194 @@
                     }
                 }, {
                     key: "fromString",
                     value: function(t) {
                         for (var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Uint32Array(4), r = t.startsWith("-"), i = t.length, a = new e(n), o = r ? 1 : 0; o < i;) {
                             var u = 8 < i - o ? 8 : i - o,
                                 s = new e(new Uint32Array([parseInt(t.substr(o, u), 10), 0, 0, 0])),
-                                c = new e(new Uint32Array([to[u], 0, 0, 0]));
+                                c = new e(new Uint32Array([Xa[u], 0, 0, 0]));
                             a.times(c), a.plus(s), o += u
                         }
                         return r ? a.negate() : a
                     }
                 }, {
                     key: "convertArray",
                     value: function(t) {
                         for (var n = new Uint32Array(4 * t.length), r = -1, i = t.length; ++r < i;) e.from(t[r], new Uint32Array(n.buffer, n.byteOffset + 16 * r, 4));
                         return n
                     }
                 }]), e
             }(),
-            oo = function(e) {
+            io = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r, i, a) {
                     var o;
                     return Object(C.a)(this, n), (o = t.call(this)).nodesIndex = -1, o.buffersIndex = -1, o.bytes = e, o.nodes = r, o.buffers = i, o.dictionaries = a, o
                 }
                 return Object(M.a)(n, [{
                     key: "visit",
                     value: function(e) {
-                        return Ut(Object(Nt.a)(n.prototype), "visit", this).call(this, e instanceof aa ? e.type : e)
+                        return Ct(Object(Ft.a)(n.prototype), "visit", this).call(this, e instanceof ra ? e.type : e)
                     }
                 }, {
                     key: "visitNull",
                     value: function(e) {
                         var t = (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode()).length;
-                        return sr.Null(e, 0, t)
+                        return ar.Null(e, 0, t)
                     }
                 }, {
                     key: "visitBool",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Bool(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Bool(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitInt",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Int(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Int(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitFloat",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Float(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Float(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitUtf8",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Utf8(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.readData(e))
+                        return ar.Utf8(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.readData(e))
                     }
                 }, {
                     key: "visitBinary",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Binary(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.readData(e))
+                        return ar.Binary(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.readData(e))
                     }
                 }, {
                     key: "visitFixedSizeBinary",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.FixedSizeBinary(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.FixedSizeBinary(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitDate",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Date(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Date(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitTimestamp",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Timestamp(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Timestamp(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitTime",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Time(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Time(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitDecimal",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Decimal(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Decimal(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitList",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.List(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.visit(e.children[0]))
+                        return ar.List(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.visit(e.children[0]))
                     }
                 }, {
                     key: "visitStruct",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Struct(e, 0, n, r, this.readNullBitmap(e, r), this.visitMany(e.children))
+                        return ar.Struct(e, 0, n, r, this.readNullBitmap(e, r), this.visitMany(e.children))
                     }
                 }, {
                     key: "visitUnion",
                     value: function(e) {
-                        return e.mode === Jt.Sparse ? this.visitSparseUnion(e) : this.visitDenseUnion(e)
+                        return e.mode === Qt.Sparse ? this.visitSparseUnion(e) : this.visitDenseUnion(e)
                     }
                 }, {
                     key: "visitDenseUnion",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Union(e, 0, n, r, this.readNullBitmap(e, r), this.readTypeIds(e), this.readOffsets(e), this.visitMany(e.children))
+                        return ar.Union(e, 0, n, r, this.readNullBitmap(e, r), this.readTypeIds(e), this.readOffsets(e), this.visitMany(e.children))
                     }
                 }, {
                     key: "visitSparseUnion",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Union(e, 0, n, r, this.readNullBitmap(e, r), this.readTypeIds(e), this.visitMany(e.children))
+                        return ar.Union(e, 0, n, r, this.readNullBitmap(e, r), this.readTypeIds(e), this.visitMany(e.children))
                     }
                 }, {
                     key: "visitDictionary",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Dictionary(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e.indices), this.readDictionary(e))
+                        return ar.Dictionary(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e.indices), this.readDictionary(e))
                     }
                 }, {
                     key: "visitInterval",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Interval(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
+                        return ar.Interval(e, 0, n, r, this.readNullBitmap(e, r), this.readData(e))
                     }
                 }, {
                     key: "visitFixedSizeList",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.FixedSizeList(e, 0, n, r, this.readNullBitmap(e, r), this.visit(e.children[0]))
+                        return ar.FixedSizeList(e, 0, n, r, this.readNullBitmap(e, r), this.visit(e.children[0]))
                     }
                 }, {
                     key: "visitMap",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextFieldNode(),
                             n = t.length,
                             r = t.nullCount;
-                        return sr.Map(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.visit(e.children[0]))
+                        return ar.Map(e, 0, n, r, this.readNullBitmap(e, r), this.readOffsets(e), this.visit(e.children[0]))
                     }
                 }, {
                     key: "nextFieldNode",
                     value: function() {
                         return this.nodes[++this.nodesIndex]
                     }
                 }, {
@@ -10707,28 +10720,28 @@
                     }
                 }, {
                     key: "readDictionary",
                     value: function(e) {
                         return this.dictionaries.get(e.id)
                     }
                 }]), n
-            }(dn),
-            uo = function(e) {
+            }(ln),
+            ao = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r, i, a) {
                     var o;
                     return Object(C.a)(this, n), (o = t.call(this, new Uint8Array(0), r, i, a)).sources = e, o
                 }
                 return Object(M.a)(n, [{
                     key: "readNullBitmap",
                     value: function(e, t) {
                         var n = (arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.nextBufferRange()).offset;
-                        return t <= 0 ? new Uint8Array(0) : un(this.sources[n])
+                        return t <= 0 ? new Uint8Array(0) : rn(this.sources[n])
                     }
                 }, {
                     key: "readOffsets",
                     value: function(e) {
                         var t = (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange()).offset;
                         return Re(Uint8Array, Re(Int32Array, this.sources[t]))
                     }
@@ -10739,256 +10752,256 @@
                         return Re(Uint8Array, Re(e.ArrayType, this.sources[t]))
                     }
                 }, {
                     key: "readData",
                     value: function(e) {
                         var t = (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange()).offset,
                             n = this.sources;
-                        return Tn.isTimestamp(e) || (Tn.isInt(e) || Tn.isTime(e)) && 64 === e.bitWidth || Tn.isDate(e) && e.unit === Qt.MILLISECOND ? Re(Uint8Array, io.convertArray(n[t])) : Tn.isDecimal(e) ? Re(Uint8Array, ao.convertArray(n[t])) : Tn.isBinary(e) || Tn.isFixedSizeBinary(e) ? function(e) {
+                        return jn.isTimestamp(e) || (jn.isInt(e) || jn.isTime(e)) && 64 === e.bitWidth || jn.isDate(e) && e.unit === Ht.MILLISECOND ? Re(Uint8Array, no.convertArray(n[t])) : jn.isDecimal(e) ? Re(Uint8Array, ro.convertArray(n[t])) : jn.isBinary(e) || jn.isFixedSizeBinary(e) ? function(e) {
                             for (var t = e.join(""), n = new Uint8Array(t.length / 2), r = 0; r < t.length; r += 2) n[r >> 1] = parseInt(t.substr(r, 2), 16);
                             return n
-                        }(n[t]) : Tn.isBool(e) ? un(n[t]) : Tn.isUtf8(e) ? se(n[t].join("")) : Re(Uint8Array, Re(e.ArrayType, n[t].map((function(e) {
+                        }(n[t]) : jn.isBool(e) ? rn(n[t]) : jn.isUtf8(e) ? se(n[t].join("")) : Re(Uint8Array, Re(e.ArrayType, n[t].map((function(e) {
                             return +e
                         }))))
                     }
                 }]), n
-            }(oo);
-        var so = K.Long,
-            co = Pt.apache.arrow.flatbuf.Null,
-            lo = Pt.apache.arrow.flatbuf.Int,
-            fo = Pt.apache.arrow.flatbuf.FloatingPoint,
-            ho = Pt.apache.arrow.flatbuf.Binary,
-            po = Pt.apache.arrow.flatbuf.Bool,
-            yo = Pt.apache.arrow.flatbuf.Utf8,
-            vo = Pt.apache.arrow.flatbuf.Decimal,
-            bo = Pt.apache.arrow.flatbuf.Date,
-            mo = Pt.apache.arrow.flatbuf.Time,
-            go = Pt.apache.arrow.flatbuf.Timestamp,
-            ko = Pt.apache.arrow.flatbuf.Interval,
-            wo = Pt.apache.arrow.flatbuf.List,
-            _o = Pt.apache.arrow.flatbuf.Struct_,
-            Oo = Pt.apache.arrow.flatbuf.Union,
-            xo = Pt.apache.arrow.flatbuf.DictionaryEncoding,
-            jo = Pt.apache.arrow.flatbuf.FixedSizeBinary,
-            So = Pt.apache.arrow.flatbuf.FixedSizeList,
-            To = Pt.apache.arrow.flatbuf.Map,
-            Io = function(e) {
+            }(io);
+        var oo = K.Long,
+            uo = Mt.apache.arrow.flatbuf.Null,
+            so = Mt.apache.arrow.flatbuf.Int,
+            co = Mt.apache.arrow.flatbuf.FloatingPoint,
+            lo = Mt.apache.arrow.flatbuf.Binary,
+            fo = Mt.apache.arrow.flatbuf.Bool,
+            ho = Mt.apache.arrow.flatbuf.Utf8,
+            po = Mt.apache.arrow.flatbuf.Decimal,
+            yo = Mt.apache.arrow.flatbuf.Date,
+            vo = Mt.apache.arrow.flatbuf.Time,
+            bo = Mt.apache.arrow.flatbuf.Timestamp,
+            mo = Mt.apache.arrow.flatbuf.Interval,
+            go = Mt.apache.arrow.flatbuf.List,
+            ko = Mt.apache.arrow.flatbuf.Struct_,
+            wo = Mt.apache.arrow.flatbuf.Union,
+            _o = Mt.apache.arrow.flatbuf.DictionaryEncoding,
+            Oo = Mt.apache.arrow.flatbuf.FixedSizeBinary,
+            jo = Mt.apache.arrow.flatbuf.FixedSizeList,
+            xo = Mt.apache.arrow.flatbuf.Map,
+            So = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "visit",
                     value: function(e, t) {
-                        return null == e || null == t ? void 0 : Ut(Object(Nt.a)(n.prototype), "visit", this).call(this, e, t)
+                        return null == e || null == t ? void 0 : Ct(Object(Ft.a)(n.prototype), "visit", this).call(this, e, t)
                     }
                 }, {
                     key: "visitNull",
                     value: function(e, t) {
-                        return co.startNull(t), co.endNull(t)
+                        return uo.startNull(t), uo.endNull(t)
                     }
                 }, {
                     key: "visitInt",
                     value: function(e, t) {
-                        return lo.startInt(t), lo.addBitWidth(t, e.bitWidth), lo.addIsSigned(t, e.isSigned), lo.endInt(t)
+                        return so.startInt(t), so.addBitWidth(t, e.bitWidth), so.addIsSigned(t, e.isSigned), so.endInt(t)
                     }
                 }, {
                     key: "visitFloat",
                     value: function(e, t) {
-                        return fo.startFloatingPoint(t), fo.addPrecision(t, e.precision), fo.endFloatingPoint(t)
+                        return co.startFloatingPoint(t), co.addPrecision(t, e.precision), co.endFloatingPoint(t)
                     }
                 }, {
                     key: "visitBinary",
                     value: function(e, t) {
-                        return ho.startBinary(t), ho.endBinary(t)
+                        return lo.startBinary(t), lo.endBinary(t)
                     }
                 }, {
                     key: "visitBool",
                     value: function(e, t) {
-                        return po.startBool(t), po.endBool(t)
+                        return fo.startBool(t), fo.endBool(t)
                     }
                 }, {
                     key: "visitUtf8",
                     value: function(e, t) {
-                        return yo.startUtf8(t), yo.endUtf8(t)
+                        return ho.startUtf8(t), ho.endUtf8(t)
                     }
                 }, {
                     key: "visitDecimal",
                     value: function(e, t) {
-                        return vo.startDecimal(t), vo.addScale(t, e.scale), vo.addPrecision(t, e.precision), vo.endDecimal(t)
+                        return po.startDecimal(t), po.addScale(t, e.scale), po.addPrecision(t, e.precision), po.endDecimal(t)
                     }
                 }, {
                     key: "visitDate",
                     value: function(e, t) {
-                        return bo.startDate(t), bo.addUnit(t, e.unit), bo.endDate(t)
+                        return yo.startDate(t), yo.addUnit(t, e.unit), yo.endDate(t)
                     }
                 }, {
                     key: "visitTime",
                     value: function(e, t) {
-                        return mo.startTime(t), mo.addUnit(t, e.unit), mo.addBitWidth(t, e.bitWidth), mo.endTime(t)
+                        return vo.startTime(t), vo.addUnit(t, e.unit), vo.addBitWidth(t, e.bitWidth), vo.endTime(t)
                     }
                 }, {
                     key: "visitTimestamp",
                     value: function(e, t) {
                         var n = e.timezone && t.createString(e.timezone) || void 0;
-                        return go.startTimestamp(t), go.addUnit(t, e.unit), void 0 !== n && go.addTimezone(t, n), go.endTimestamp(t)
+                        return bo.startTimestamp(t), bo.addUnit(t, e.unit), void 0 !== n && bo.addTimezone(t, n), bo.endTimestamp(t)
                     }
                 }, {
                     key: "visitInterval",
                     value: function(e, t) {
-                        return ko.startInterval(t), ko.addUnit(t, e.unit), ko.endInterval(t)
+                        return mo.startInterval(t), mo.addUnit(t, e.unit), mo.endInterval(t)
                     }
                 }, {
                     key: "visitList",
                     value: function(e, t) {
-                        return wo.startList(t), wo.endList(t)
+                        return go.startList(t), go.endList(t)
                     }
                 }, {
                     key: "visitStruct",
                     value: function(e, t) {
-                        return _o.startStruct_(t), _o.endStruct_(t)
+                        return ko.startStruct_(t), ko.endStruct_(t)
                     }
                 }, {
                     key: "visitUnion",
                     value: function(e, t) {
-                        Oo.startTypeIdsVector(t, e.typeIds.length);
-                        var n = Oo.createTypeIdsVector(t, e.typeIds);
-                        return Oo.startUnion(t), Oo.addMode(t, e.mode), Oo.addTypeIds(t, n), Oo.endUnion(t)
+                        wo.startTypeIdsVector(t, e.typeIds.length);
+                        var n = wo.createTypeIdsVector(t, e.typeIds);
+                        return wo.startUnion(t), wo.addMode(t, e.mode), wo.addTypeIds(t, n), wo.endUnion(t)
                     }
                 }, {
                     key: "visitDictionary",
                     value: function(e, t) {
                         var n = this.visit(e.indices, t);
-                        return xo.startDictionaryEncoding(t), xo.addId(t, new so(e.id, 0)), xo.addIsOrdered(t, e.isOrdered), void 0 !== n && xo.addIndexType(t, n), xo.endDictionaryEncoding(t)
+                        return _o.startDictionaryEncoding(t), _o.addId(t, new oo(e.id, 0)), _o.addIsOrdered(t, e.isOrdered), void 0 !== n && _o.addIndexType(t, n), _o.endDictionaryEncoding(t)
                     }
                 }, {
                     key: "visitFixedSizeBinary",
                     value: function(e, t) {
-                        return jo.startFixedSizeBinary(t), jo.addByteWidth(t, e.byteWidth), jo.endFixedSizeBinary(t)
+                        return Oo.startFixedSizeBinary(t), Oo.addByteWidth(t, e.byteWidth), Oo.endFixedSizeBinary(t)
                     }
                 }, {
                     key: "visitFixedSizeList",
                     value: function(e, t) {
-                        return So.startFixedSizeList(t), So.addListSize(t, e.listSize), So.endFixedSizeList(t)
+                        return jo.startFixedSizeList(t), jo.addListSize(t, e.listSize), jo.endFixedSizeList(t)
                     }
                 }, {
                     key: "visitMap",
                     value: function(e, t) {
-                        return To.startMap(t), To.addKeysSorted(t, e.keysSorted), To.endMap(t)
+                        return xo.startMap(t), xo.addKeysSorted(t, e.keysSorted), xo.endMap(t)
                     }
                 }]), n
-            }(dn),
-            Eo = new Io;
+            }(ln),
+            To = new So;
 
-        function Ao(e) {
-            return new Jo(e.count, Do(e.columns), Lo(e.columns))
+        function Io(e) {
+            return new qo(e.count, Ao(e.columns), Bo(e.columns))
         }
 
-        function Bo(e, t) {
+        function Eo(e, t) {
             return (e.children || []).filter(Boolean).map((function(e) {
-                return aa.fromJSON(e, t)
+                return ra.fromJSON(e, t)
             }))
         }
 
-        function Do(e) {
+        function Ao(e) {
             return (e || []).reduce((function(e, t) {
-                return [].concat(hn(e), [new eu(t.count, (n = t.VALIDITY, (n || []).reduce((function(e, t) {
+                return [].concat(cn(e), [new Zo(t.count, (n = t.VALIDITY, (n || []).reduce((function(e, t) {
                     return e + +(0 === t)
-                }), 0)))], hn(Do(t.children)));
+                }), 0)))], cn(Ao(t.children)));
                 var n
             }), [])
         }
 
-        function Lo(e) {
+        function Bo(e) {
             for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [], n = -1, r = (e || []).length; ++n < r;) {
                 var i = e[n];
-                i.VALIDITY && t.push(new Xo(t.length, i.VALIDITY.length)), i.TYPE && t.push(new Xo(t.length, i.TYPE.length)), i.OFFSET && t.push(new Xo(t.length, i.OFFSET.length)), i.DATA && t.push(new Xo(t.length, i.DATA.length)), t = Lo(i.children, t)
+                i.VALIDITY && t.push(new Jo(t.length, i.VALIDITY.length)), i.TYPE && t.push(new Jo(t.length, i.TYPE.length)), i.OFFSET && t.push(new Jo(t.length, i.OFFSET.length)), i.DATA && t.push(new Jo(t.length, i.DATA.length)), t = Bo(i.children, t)
             }
             return t
         }
 
-        function Fo(e) {
+        function Do(e) {
             return new Map(Object.entries(e || {}))
         }
 
-        function Co(e) {
-            return new En(e.isSigned, e.bitWidth)
+        function Lo(e) {
+            return new Sn(e.isSigned, e.bitWidth)
         }
 
-        function Mo(e, t) {
+        function Fo(e, t) {
             var n = e.type.name;
             switch (n) {
                 case "NONE":
                 case "null":
-                    return new In;
+                    return new xn;
                 case "binary":
-                    return new zn;
+                    return new Pn;
                 case "utf8":
-                    return new Wn;
+                    return new Rn;
                 case "bool":
-                    return new Yn;
+                    return new Vn;
                 case "list":
-                    return new Zn((t || [])[0]);
+                    return new qn((t || [])[0]);
                 case "struct":
                 case "struct_":
-                    return new Xn(t || [])
+                    return new Gn(t || [])
             }
             switch (n) {
                 case "int":
                     var r = e.type;
-                    return new En(r.isSigned, r.bitWidth);
+                    return new Sn(r.isSigned, r.bitWidth);
                 case "floatingpoint":
                     var i = e.type;
-                    return new Un(Gt[i.precision]);
+                    return new Cn(Kt[i.precision]);
                 case "decimal":
                     var a = e.type;
-                    return new Hn(a.scale, a.precision);
+                    return new zn(a.scale, a.precision);
                 case "date":
                     var o = e.type;
-                    return new $n(Qt[o.unit]);
+                    return new Wn(Ht[o.unit]);
                 case "time":
                     var u = e.type;
-                    return new qn(qt[u.unit], u.bitWidth);
+                    return new $n($t[u.unit], u.bitWidth);
                 case "timestamp":
                     var s = e.type;
-                    return new Gn(qt[s.unit], s.timezone);
+                    return new Kn($t[s.unit], s.timezone);
                 case "interval":
                     var c = e.type;
-                    return new Jn(Zt[c.unit]);
+                    return new Qn(qt[c.unit]);
                 case "union":
                     var l = e.type;
-                    return new er(Jt[l.mode], l.typeIds || [], t || []);
+                    return new Jn(Qt[l.mode], l.typeIds || [], t || []);
                 case "fixedsizebinary":
                     var f = e.type;
-                    return new tr(f.byteWidth);
+                    return new Zn(f.byteWidth);
                 case "fixedsizelist":
                     var h = e.type;
-                    return new nr(h.listSize, (t || [])[0]);
+                    return new Xn(h.listSize, (t || [])[0]);
                 case "map":
                     var d = e.type;
-                    return new rr((t || [])[0], d.keysSorted)
+                    return new er((t || [])[0], d.keysSorted)
             }
             throw new Error('Unrecognized type: "'.concat(n, '"'))
         }
-        var No = K.Long,
-            Uo = K.Builder,
-            Po = K.ByteBuffer,
-            Ro = Pt.apache.arrow.flatbuf.Type,
-            Vo = Pt.apache.arrow.flatbuf.Field,
-            zo = Pt.apache.arrow.flatbuf.Schema,
-            Wo = Pt.apache.arrow.flatbuf.Buffer,
-            Yo = Yt.apache.arrow.flatbuf.Message,
-            Ho = Pt.apache.arrow.flatbuf.KeyValue,
-            $o = Yt.apache.arrow.flatbuf.FieldNode,
-            Ko = Pt.apache.arrow.flatbuf.Endianness,
-            Qo = Yt.apache.arrow.flatbuf.RecordBatch,
-            qo = Yt.apache.arrow.flatbuf.DictionaryBatch,
-            Go = function() {
+        var Co = K.Long,
+            Mo = K.Builder,
+            No = K.ByteBuffer,
+            Uo = Mt.apache.arrow.flatbuf.Type,
+            Po = Mt.apache.arrow.flatbuf.Field,
+            Ro = Mt.apache.arrow.flatbuf.Schema,
+            Vo = Mt.apache.arrow.flatbuf.Buffer,
+            zo = Vt.apache.arrow.flatbuf.Message,
+            Wo = Mt.apache.arrow.flatbuf.KeyValue,
+            Yo = Vt.apache.arrow.flatbuf.FieldNode,
+            Ho = Mt.apache.arrow.flatbuf.Endianness,
+            $o = Vt.apache.arrow.flatbuf.RecordBatch,
+            Ko = Vt.apache.arrow.flatbuf.DictionaryBatch,
+            Qo = function() {
                 function e(t, n, r, i) {
                     Object(C.a)(this, e), this._version = n, this._headerType = r, this.body = new Uint8Array(0), i && (this._createHeader = function() {
                         return i
                     }), this._bodyLength = "number" === typeof t ? t : t.low
                 }
                 return Object(M.a)(e, [{
                     key: "type",
@@ -11014,86 +11027,86 @@
                     key: "header",
                     value: function() {
                         return this._createHeader()
                     }
                 }, {
                     key: "isSchema",
                     value: function() {
-                        return this.headerType === Xt.Schema
+                        return this.headerType === Gt.Schema
                     }
                 }, {
                     key: "isRecordBatch",
                     value: function() {
-                        return this.headerType === Xt.RecordBatch
+                        return this.headerType === Gt.RecordBatch
                     }
                 }, {
                     key: "isDictionaryBatch",
                     value: function() {
-                        return this.headerType === Xt.DictionaryBatch
+                        return this.headerType === Gt.DictionaryBatch
                     }
                 }], [{
                     key: "fromJSON",
                     value: function(t, n) {
-                        var r = new e(0, en.V4, n);
+                        var r = new e(0, Jt.V4, n);
                         return r._createHeader = function(e, t) {
                             return function() {
                                 switch (t) {
-                                    case Xt.Schema:
-                                        return ia.fromJSON(e);
-                                    case Xt.RecordBatch:
-                                        return Jo.fromJSON(e);
-                                    case Xt.DictionaryBatch:
-                                        return Zo.fromJSON(e)
+                                    case Gt.Schema:
+                                        return na.fromJSON(e);
+                                    case Gt.RecordBatch:
+                                        return qo.fromJSON(e);
+                                    case Gt.DictionaryBatch:
+                                        return Go.fromJSON(e)
                                 }
-                                throw new Error("Unrecognized Message type: { name: ".concat(Xt[t], ", type: ").concat(t, " }"))
+                                throw new Error("Unrecognized Message type: { name: ".concat(Gt[t], ", type: ").concat(t, " }"))
                             }
                         }(t, n), r
                     }
                 }, {
                     key: "decode",
                     value: function(t) {
-                        t = new Po(He(t));
-                        var n = Yo.getRootAsMessage(t),
+                        t = new No(He(t));
+                        var n = zo.getRootAsMessage(t),
                             r = n.bodyLength(),
                             i = n.version(),
                             a = n.headerType(),
                             o = new e(r, i, a);
                         return o._createHeader = function(e, t) {
                             return function() {
                                 switch (t) {
-                                    case Xt.Schema:
-                                        return ia.decode(e.header(new zo));
-                                    case Xt.RecordBatch:
-                                        return Jo.decode(e.header(new Qo), e.version());
-                                    case Xt.DictionaryBatch:
-                                        return Zo.decode(e.header(new qo), e.version())
+                                    case Gt.Schema:
+                                        return na.decode(e.header(new Ro));
+                                    case Gt.RecordBatch:
+                                        return qo.decode(e.header(new $o), e.version());
+                                    case Gt.DictionaryBatch:
+                                        return Go.decode(e.header(new Ko), e.version())
                                 }
-                                throw new Error("Unrecognized Message type: { name: ".concat(Xt[t], ", type: ").concat(t, " }"))
+                                throw new Error("Unrecognized Message type: { name: ".concat(Gt[t], ", type: ").concat(t, " }"))
                             }
                         }(n, a), o
                     }
                 }, {
                     key: "encode",
                     value: function(e) {
-                        var t = new Uo,
+                        var t = new Mo,
                             n = -1;
-                        return e.isSchema() ? n = ia.encode(t, e.header()) : e.isRecordBatch() ? n = Jo.encode(t, e.header()) : e.isDictionaryBatch() && (n = Zo.encode(t, e.header())), Yo.startMessage(t), Yo.addVersion(t, en.V4), Yo.addHeader(t, n), Yo.addHeaderType(t, e.headerType), Yo.addBodyLength(t, new No(e.bodyLength, 0)), Yo.finishMessageBuffer(t, Yo.endMessage(t)), t.asUint8Array()
+                        return e.isSchema() ? n = na.encode(t, e.header()) : e.isRecordBatch() ? n = qo.encode(t, e.header()) : e.isDictionaryBatch() && (n = Go.encode(t, e.header())), zo.startMessage(t), zo.addVersion(t, Jt.V4), zo.addHeader(t, n), zo.addHeaderType(t, e.headerType), zo.addBodyLength(t, new Co(e.bodyLength, 0)), zo.finishMessageBuffer(t, zo.endMessage(t)), t.asUint8Array()
                     }
                 }, {
                     key: "from",
                     value: function(t) {
                         var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
-                        if (t instanceof ia) return new e(0, en.V4, Xt.Schema, t);
-                        if (t instanceof Jo) return new e(n, en.V4, Xt.RecordBatch, t);
-                        if (t instanceof Zo) return new e(n, en.V4, Xt.DictionaryBatch, t);
+                        if (t instanceof na) return new e(0, Jt.V4, Gt.Schema, t);
+                        if (t instanceof qo) return new e(n, Jt.V4, Gt.RecordBatch, t);
+                        if (t instanceof Go) return new e(n, Jt.V4, Gt.DictionaryBatch, t);
                         throw new Error("Unrecognized Message header: ".concat(t))
                     }
                 }]), e
             }(),
-            Jo = function() {
+            qo = function() {
                 function e(t, n, r) {
                     Object(C.a)(this, e), this._nodes = n, this._buffers = r, this._length = "number" === typeof t ? t : t.low
                 }
                 return Object(M.a)(e, [{
                     key: "nodes",
                     get: function() {
                         return this._nodes
@@ -11106,15 +11119,15 @@
                 }, {
                     key: "buffers",
                     get: function() {
                         return this._buffers
                     }
                 }]), e
             }(),
-            Zo = function() {
+            Go = function() {
                 function e(t, n) {
                     var r = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                     Object(C.a)(this, e), this._data = t, this._isDelta = r, this._id = "number" === typeof n ? n : n.low
                 }
                 return Object(M.a)(e, [{
                     key: "id",
                     get: function() {
@@ -11143,202 +11156,202 @@
                 }, {
                     key: "buffers",
                     get: function() {
                         return this.data.buffers
                     }
                 }]), e
             }(),
-            Xo = Object(M.a)((function e(t, n) {
+            Jo = Object(M.a)((function e(t, n) {
                 Object(C.a)(this, e), this.offset = "number" === typeof t ? t : t.low, this.length = "number" === typeof n ? n : n.low
             })),
-            eu = Object(M.a)((function e(t, n) {
+            Zo = Object(M.a)((function e(t, n) {
                 Object(C.a)(this, e), this.length = "number" === typeof t ? t : t.low, this.nullCount = "number" === typeof n ? n : n.low
             }));
 
-        function tu(e, t) {
-            for (var n, r = [], i = -1, a = -1, o = e.childrenLength(); ++i < o;)(n = e.children(i)) && (r[++a] = aa.decode(n, t));
+        function Xo(e, t) {
+            for (var n, r = [], i = -1, a = -1, o = e.childrenLength(); ++i < o;)(n = e.children(i)) && (r[++a] = ra.decode(n, t));
             return r
         }
 
-        function nu(e) {
+        function eu(e) {
             var t = new Map;
             if (e)
                 for (var n, r, i = -1, a = 0 | e.customMetadataLength(); ++i < a;)(n = e.customMetadata(i)) && null != (r = n.key()) && t.set(r, n.value());
             return t
         }
 
-        function ru(e) {
-            return new En(e.isSigned(), e.bitWidth())
+        function tu(e) {
+            return new Sn(e.isSigned(), e.bitWidth())
         }
 
-        function iu(e, t) {
+        function nu(e, t) {
             var n = e.typeType();
             switch (n) {
-                case Ro.NONE:
-                case Ro.Null:
-                    return new In;
-                case Ro.Binary:
-                    return new zn;
-                case Ro.Utf8:
-                    return new Wn;
-                case Ro.Bool:
-                    return new Yn;
-                case Ro.List:
-                    return new Zn((t || [])[0]);
-                case Ro.Struct_:
-                    return new Xn(t || [])
+                case Uo.NONE:
+                case Uo.Null:
+                    return new xn;
+                case Uo.Binary:
+                    return new Pn;
+                case Uo.Utf8:
+                    return new Rn;
+                case Uo.Bool:
+                    return new Vn;
+                case Uo.List:
+                    return new qn((t || [])[0]);
+                case Uo.Struct_:
+                    return new Gn(t || [])
             }
             switch (n) {
-                case Ro.Int:
-                    var r = e.type(new Pt.apache.arrow.flatbuf.Int);
-                    return new En(r.isSigned(), r.bitWidth());
-                case Ro.FloatingPoint:
-                    var i = e.type(new Pt.apache.arrow.flatbuf.FloatingPoint);
-                    return new Un(i.precision());
-                case Ro.Decimal:
-                    var a = e.type(new Pt.apache.arrow.flatbuf.Decimal);
-                    return new Hn(a.scale(), a.precision());
-                case Ro.Date:
-                    var o = e.type(new Pt.apache.arrow.flatbuf.Date);
-                    return new $n(o.unit());
-                case Ro.Time:
-                    var u = e.type(new Pt.apache.arrow.flatbuf.Time);
-                    return new qn(u.unit(), u.bitWidth());
-                case Ro.Timestamp:
-                    var s = e.type(new Pt.apache.arrow.flatbuf.Timestamp);
-                    return new Gn(s.unit(), s.timezone());
-                case Ro.Interval:
-                    var c = e.type(new Pt.apache.arrow.flatbuf.Interval);
-                    return new Jn(c.unit());
-                case Ro.Union:
-                    var l = e.type(new Pt.apache.arrow.flatbuf.Union);
-                    return new er(l.mode(), l.typeIdsArray() || [], t || []);
-                case Ro.FixedSizeBinary:
-                    var f = e.type(new Pt.apache.arrow.flatbuf.FixedSizeBinary);
-                    return new tr(f.byteWidth());
-                case Ro.FixedSizeList:
-                    var h = e.type(new Pt.apache.arrow.flatbuf.FixedSizeList);
-                    return new nr(h.listSize(), (t || [])[0]);
-                case Ro.Map:
-                    var d = e.type(new Pt.apache.arrow.flatbuf.Map);
-                    return new rr((t || [])[0], d.keysSorted())
+                case Uo.Int:
+                    var r = e.type(new Mt.apache.arrow.flatbuf.Int);
+                    return new Sn(r.isSigned(), r.bitWidth());
+                case Uo.FloatingPoint:
+                    var i = e.type(new Mt.apache.arrow.flatbuf.FloatingPoint);
+                    return new Cn(i.precision());
+                case Uo.Decimal:
+                    var a = e.type(new Mt.apache.arrow.flatbuf.Decimal);
+                    return new zn(a.scale(), a.precision());
+                case Uo.Date:
+                    var o = e.type(new Mt.apache.arrow.flatbuf.Date);
+                    return new Wn(o.unit());
+                case Uo.Time:
+                    var u = e.type(new Mt.apache.arrow.flatbuf.Time);
+                    return new $n(u.unit(), u.bitWidth());
+                case Uo.Timestamp:
+                    var s = e.type(new Mt.apache.arrow.flatbuf.Timestamp);
+                    return new Kn(s.unit(), s.timezone());
+                case Uo.Interval:
+                    var c = e.type(new Mt.apache.arrow.flatbuf.Interval);
+                    return new Qn(c.unit());
+                case Uo.Union:
+                    var l = e.type(new Mt.apache.arrow.flatbuf.Union);
+                    return new Jn(l.mode(), l.typeIdsArray() || [], t || []);
+                case Uo.FixedSizeBinary:
+                    var f = e.type(new Mt.apache.arrow.flatbuf.FixedSizeBinary);
+                    return new Zn(f.byteWidth());
+                case Uo.FixedSizeList:
+                    var h = e.type(new Mt.apache.arrow.flatbuf.FixedSizeList);
+                    return new Xn(h.listSize(), (t || [])[0]);
+                case Uo.Map:
+                    var d = e.type(new Mt.apache.arrow.flatbuf.Map);
+                    return new er((t || [])[0], d.keysSorted())
             }
-            throw new Error('Unrecognized type: "'.concat(Ro[n], '" (').concat(n, ")"))
+            throw new Error('Unrecognized type: "'.concat(Uo[n], '" (').concat(n, ")"))
         }
-        aa.encode = function(e, t) {
+        ra.encode = function(e, t) {
             var n = -1,
                 r = -1,
                 i = -1,
                 a = t.type,
                 o = t.typeId;
-            Tn.isDictionary(a) ? (o = a.dictionary.typeId, i = Eo.visit(a, e), r = Eo.visit(a.dictionary, e)) : r = Eo.visit(a, e);
+            jn.isDictionary(a) ? (o = a.dictionary.typeId, i = To.visit(a, e), r = To.visit(a.dictionary, e)) : r = To.visit(a, e);
             var u = (a.children || []).map((function(t) {
-                    return aa.encode(e, t)
+                    return ra.encode(e, t)
                 })),
-                s = Vo.createChildrenVector(e, u),
-                c = t.metadata && t.metadata.size > 0 ? Vo.createCustomMetadataVector(e, hn(t.metadata).map((function(t) {
+                s = Po.createChildrenVector(e, u),
+                c = t.metadata && t.metadata.size > 0 ? Po.createCustomMetadataVector(e, cn(t.metadata).map((function(t) {
                     var n = P(t, 2),
                         r = n[0],
                         i = n[1],
                         a = e.createString("".concat(r)),
                         o = e.createString("".concat(i));
-                    return Ho.startKeyValue(e), Ho.addKey(e, a), Ho.addValue(e, o), Ho.endKeyValue(e)
+                    return Wo.startKeyValue(e), Wo.addKey(e, a), Wo.addValue(e, o), Wo.endKeyValue(e)
                 }))) : -1;
             t.name && (n = e.createString(t.name));
-            Vo.startField(e), Vo.addType(e, r), Vo.addTypeType(e, o), Vo.addChildren(e, s), Vo.addNullable(e, !!t.nullable), -1 !== n && Vo.addName(e, n); - 1 !== i && Vo.addDictionary(e, i); - 1 !== c && Vo.addCustomMetadata(e, c);
-            return Vo.endField(e)
-        }, aa.decode = function(e, t) {
+            Po.startField(e), Po.addType(e, r), Po.addTypeType(e, o), Po.addChildren(e, s), Po.addNullable(e, !!t.nullable), -1 !== n && Po.addName(e, n); - 1 !== i && Po.addDictionary(e, i); - 1 !== c && Po.addCustomMetadata(e, c);
+            return Po.endField(e)
+        }, ra.decode = function(e, t) {
             var n, r, i, a, o, u;
-            t && (u = e.dictionary()) ? t.has(n = u.id().low) ? (a = (a = u.indexType()) ? ru(a) : new Dn, o = new or(t.get(n), a, n, u.isOrdered()), r = new aa(e.name(), o, e.nullable(), nu(e))) : (a = (a = u.indexType()) ? ru(a) : new Dn, t.set(n, i = iu(e, tu(e, t))), o = new or(i, a, n, u.isOrdered()), r = new aa(e.name(), o, e.nullable(), nu(e))) : (i = iu(e, tu(e, t)), r = new aa(e.name(), i, e.nullable(), nu(e)));
+            t && (u = e.dictionary()) ? t.has(n = u.id().low) ? (a = (a = u.indexType()) ? tu(a) : new En, o = new rr(t.get(n), a, n, u.isOrdered()), r = new ra(e.name(), o, e.nullable(), eu(e))) : (a = (a = u.indexType()) ? tu(a) : new En, t.set(n, i = nu(e, Xo(e, t))), o = new rr(i, a, n, u.isOrdered()), r = new ra(e.name(), o, e.nullable(), eu(e))) : (i = nu(e, Xo(e, t)), r = new ra(e.name(), i, e.nullable(), eu(e)));
             return r || null
-        }, aa.fromJSON = function(e, t) {
+        }, ra.fromJSON = function(e, t) {
             var n, r, i, a, o, u;
-            return t && (a = e.dictionary) ? t.has(n = a.id) ? (r = (r = a.indexType) ? Co(r) : new Dn, u = new or(t.get(n), r, n, a.isOrdered), i = new aa(e.name, u, e.nullable, Fo(e.customMetadata))) : (r = (r = a.indexType) ? Co(r) : new Dn, t.set(n, o = Mo(e, Bo(e, t))), u = new or(o, r, n, a.isOrdered), i = new aa(e.name, u, e.nullable, Fo(e.customMetadata))) : (o = Mo(e, Bo(e, t)), i = new aa(e.name, o, e.nullable, Fo(e.customMetadata))), i || null
-        }, ia.encode = function(e, t) {
+            return t && (a = e.dictionary) ? t.has(n = a.id) ? (r = (r = a.indexType) ? Lo(r) : new En, u = new rr(t.get(n), r, n, a.isOrdered), i = new ra(e.name, u, e.nullable, Do(e.customMetadata))) : (r = (r = a.indexType) ? Lo(r) : new En, t.set(n, o = Fo(e, Eo(e, t))), u = new rr(o, r, n, a.isOrdered), i = new ra(e.name, u, e.nullable, Do(e.customMetadata))) : (o = Fo(e, Eo(e, t)), i = new ra(e.name, o, e.nullable, Do(e.customMetadata))), i || null
+        }, na.encode = function(e, t) {
             var n = t.fields.map((function(t) {
-                return aa.encode(e, t)
+                return ra.encode(e, t)
             }));
-            zo.startFieldsVector(e, n.length);
-            var r = zo.createFieldsVector(e, n),
-                i = t.metadata && t.metadata.size > 0 ? zo.createCustomMetadataVector(e, hn(t.metadata).map((function(t) {
+            Ro.startFieldsVector(e, n.length);
+            var r = Ro.createFieldsVector(e, n),
+                i = t.metadata && t.metadata.size > 0 ? Ro.createCustomMetadataVector(e, cn(t.metadata).map((function(t) {
                     var n = P(t, 2),
                         r = n[0],
                         i = n[1],
                         a = e.createString("".concat(r)),
                         o = e.createString("".concat(i));
-                    return Ho.startKeyValue(e), Ho.addKey(e, a), Ho.addValue(e, o), Ho.endKeyValue(e)
+                    return Wo.startKeyValue(e), Wo.addKey(e, a), Wo.addValue(e, o), Wo.endKeyValue(e)
                 }))) : -1;
-            zo.startSchema(e), zo.addFields(e, r), zo.addEndianness(e, au ? Ko.Little : Ko.Big), -1 !== i && zo.addCustomMetadata(e, i);
-            return zo.endSchema(e)
-        }, ia.decode = function(e) {
+            Ro.startSchema(e), Ro.addFields(e, r), Ro.addEndianness(e, ru ? Ho.Little : Ho.Big), -1 !== i && Ro.addCustomMetadata(e, i);
+            return Ro.endSchema(e)
+        }, na.decode = function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map,
                 n = function(e, t) {
-                    for (var n, r = [], i = -1, a = -1, o = e.fieldsLength(); ++i < o;)(n = e.fields(i)) && (r[++a] = aa.decode(n, t));
+                    for (var n, r = [], i = -1, a = -1, o = e.fieldsLength(); ++i < o;)(n = e.fields(i)) && (r[++a] = ra.decode(n, t));
                     return r
                 }(e, t);
-            return new ia(n, nu(e), t)
-        }, ia.fromJSON = function(e) {
+            return new na(n, eu(e), t)
+        }, na.fromJSON = function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map;
-            return new ia(function(e, t) {
+            return new na(function(e, t) {
                 return (e.fields || []).filter(Boolean).map((function(e) {
-                    return aa.fromJSON(e, t)
+                    return ra.fromJSON(e, t)
                 }))
-            }(e, t), Fo(e.customMetadata), t)
-        }, Jo.encode = function(e, t) {
+            }(e, t), Do(e.customMetadata), t)
+        }, qo.encode = function(e, t) {
             var n = t.nodes || [],
                 r = t.buffers || [];
-            Qo.startNodesVector(e, n.length), n.slice().reverse().forEach((function(t) {
-                return eu.encode(e, t)
+            $o.startNodesVector(e, n.length), n.slice().reverse().forEach((function(t) {
+                return Zo.encode(e, t)
             }));
             var i = e.endVector();
-            Qo.startBuffersVector(e, r.length), r.slice().reverse().forEach((function(t) {
-                return Xo.encode(e, t)
+            $o.startBuffersVector(e, r.length), r.slice().reverse().forEach((function(t) {
+                return Jo.encode(e, t)
             }));
             var a = e.endVector();
-            return Qo.startRecordBatch(e), Qo.addLength(e, new No(t.length, 0)), Qo.addNodes(e, i), Qo.addBuffers(e, a), Qo.endRecordBatch(e)
-        }, Jo.decode = function(e) {
-            var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : en.V4;
-            return new Jo(e.length(), function(e) {
-                for (var t, n = [], r = -1, i = -1, a = e.nodesLength(); ++r < a;)(t = e.nodes(r)) && (n[++i] = eu.decode(t));
+            return $o.startRecordBatch(e), $o.addLength(e, new Co(t.length, 0)), $o.addNodes(e, i), $o.addBuffers(e, a), $o.endRecordBatch(e)
+        }, qo.decode = function(e) {
+            var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Jt.V4;
+            return new qo(e.length(), function(e) {
+                for (var t, n = [], r = -1, i = -1, a = e.nodesLength(); ++r < a;)(t = e.nodes(r)) && (n[++i] = Zo.decode(t));
                 return n
             }(e), function(e, t) {
-                for (var n, r = [], i = -1, a = -1, o = e.buffersLength(); ++i < o;)(n = e.buffers(i)) && (t < en.V4 && (n.bb_pos += 8 * (i + 1)), r[++a] = Xo.decode(n));
+                for (var n, r = [], i = -1, a = -1, o = e.buffersLength(); ++i < o;)(n = e.buffers(i)) && (t < Jt.V4 && (n.bb_pos += 8 * (i + 1)), r[++a] = Jo.decode(n));
                 return r
             }(e, t))
-        }, Jo.fromJSON = Ao, Zo.encode = function(e, t) {
-            var n = Jo.encode(e, t.data);
-            return qo.startDictionaryBatch(e), qo.addId(e, new No(t.id, 0)), qo.addIsDelta(e, t.isDelta), qo.addData(e, n), qo.endDictionaryBatch(e)
+        }, qo.fromJSON = Io, Go.encode = function(e, t) {
+            var n = qo.encode(e, t.data);
+            return Ko.startDictionaryBatch(e), Ko.addId(e, new Co(t.id, 0)), Ko.addIsDelta(e, t.isDelta), Ko.addData(e, n), Ko.endDictionaryBatch(e)
+        }, Go.decode = function(e) {
+            var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Jt.V4;
+            return new Go(qo.decode(e.data(), t), e.id(), e.isDelta())
+        }, Go.fromJSON = function(e) {
+            return new Go(Io(e.data), e.id, e.isDelta)
+        }, Zo.encode = function(e, t) {
+            return Yo.createFieldNode(e, new Co(t.length, 0), new Co(t.nullCount, 0))
         }, Zo.decode = function(e) {
-            var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : en.V4;
-            return new Zo(Jo.decode(e.data(), t), e.id(), e.isDelta())
-        }, Zo.fromJSON = function(e) {
-            return new Zo(Ao(e.data), e.id, e.isDelta)
-        }, eu.encode = function(e, t) {
-            return $o.createFieldNode(e, new No(t.length, 0), new No(t.nullCount, 0))
-        }, eu.decode = function(e) {
-            return new eu(e.length(), e.nullCount())
-        }, Xo.encode = function(e, t) {
-            return Wo.createBuffer(e, new No(t.offset, 0), new No(t.length, 0))
-        }, Xo.decode = function(e) {
-            return new Xo(e.offset(), e.length())
+            return new Zo(e.length(), e.nullCount())
+        }, Jo.encode = function(e, t) {
+            return Vo.createBuffer(e, new Co(t.offset, 0), new Co(t.length, 0))
+        }, Jo.decode = function(e) {
+            return new Jo(e.offset(), e.length())
         };
-        for (var au = function() {
+        for (var ru = function() {
                 var e = new ArrayBuffer(2);
                 return new DataView(e).setInt16(0, 256, !0), 256 === new Int16Array(e)[0]
-            }(), ou = K.ByteBuffer, uu = function(e) {
-                return "Expected ".concat(Xt[e], " Message in stream, but was null or length 0.")
-            }, su = function(e) {
-                return "Header pointer of flatbuffer-encoded ".concat(Xt[e], " Message is null or length 0.")
-            }, cu = function(e, t) {
+            }(), iu = K.ByteBuffer, au = function(e) {
+                return "Expected ".concat(Gt[e], " Message in stream, but was null or length 0.")
+            }, ou = function(e) {
+                return "Header pointer of flatbuffer-encoded ".concat(Gt[e], " Message is null or length 0.")
+            }, uu = function(e, t) {
                 return "Expected to read ".concat(e, " metadata bytes, but only read ").concat(t, ".")
-            }, lu = function(e, t) {
+            }, su = function(e, t) {
                 return "Expected to read ".concat(e, " bytes for message body, but only read ").concat(t, ".")
-            }, fu = function(e) {
+            }, cu = function(e) {
                 function t(e) {
-                    Object(C.a)(this, t), this.source = e instanceof Qa ? e : new Qa(e)
+                    Object(C.a)(this, t), this.source = e instanceof $a ? e : new $a(e)
                 }
                 return Object(M.a)(t, [{
                     key: e,
                     value: function() {
                         return this
                     }
                 }, {
@@ -11358,61 +11371,61 @@
                         return this.source.return(e)
                     }
                 }, {
                     key: "readMessage",
                     value: function(e) {
                         var t;
                         if ((t = this.next()).done) return null;
-                        if (null != e && t.value.headerType !== e) throw new Error(uu(e));
+                        if (null != e && t.value.headerType !== e) throw new Error(au(e));
                         return t.value
                     }
                 }, {
                     key: "readMessageBody",
                     value: function(e) {
                         if (e <= 0) return new Uint8Array(0);
                         var t = He(this.source.read(e));
-                        if (t.byteLength < e) throw new Error(lu(e, t.byteLength));
+                        if (t.byteLength < e) throw new Error(su(e, t.byteLength));
                         return t.byteOffset % 8 === 0 && t.byteOffset + t.byteLength <= t.buffer.byteLength ? t : t.slice()
                     }
                 }, {
                     key: "readSchema",
                     value: function() {
                         var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
-                            t = Xt.Schema,
+                            t = Gt.Schema,
                             n = this.readMessage(t),
                             r = n && n.header();
-                        if (e && !r) throw new Error(su(t));
+                        if (e && !r) throw new Error(ou(t));
                         return r
                     }
                 }, {
                     key: "readMetadataLength",
                     value: function() {
-                        var e = this.source.read(pu),
-                            t = e && new ou(e),
+                        var e = this.source.read(hu),
+                            t = e && new iu(e),
                             n = t && t.readInt32(0) || 0;
                         return {
                             done: 0 === n,
                             value: n
                         }
                     }
                 }, {
                     key: "readMetadata",
                     value: function(e) {
                         var t = this.source.read(e);
                         if (!t) return fe;
-                        if (t.byteLength < e) throw new Error(cu(e, t.byteLength));
+                        if (t.byteLength < e) throw new Error(uu(e, t.byteLength));
                         return {
                             done: !1,
-                            value: Go.decode(t)
+                            value: Qo.decode(t)
                         }
                     }
                 }]), t
-            }(Symbol.iterator), hu = function(e) {
+            }(Symbol.iterator), lu = function(e) {
                 function t(e, n) {
-                    Object(C.a)(this, t), this.source = e instanceof qa ? e : Be(e) ? new Xa(e, n) : new qa(e)
+                    Object(C.a)(this, t), this.source = e instanceof Ka ? e : Be(e) ? new Ja(e, n) : new Ka(e)
                 }
                 return Object(M.a)(t, [{
                     key: e,
                     value: function() {
                         return this
                     }
                 }, {
@@ -11520,15 +11533,15 @@
                                         }
                                         return e.abrupt("return", null);
                                     case 4:
                                         if (null == t || n.value.headerType === t) {
                                             e.next = 6;
                                             break
                                         }
-                                        throw new Error(uu(t));
+                                        throw new Error(au(t));
                                     case 6:
                                         return e.abrupt("return", n.value);
                                     case 7:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, this)
@@ -11553,15 +11566,15 @@
                                     case 2:
                                         return e.t0 = He, e.next = 5, this.source.read(t);
                                     case 5:
                                         if (e.t1 = e.sent, !((n = (0, e.t0)(e.t1)).byteLength < t)) {
                                             e.next = 9;
                                             break
                                         }
-                                        throw new Error(lu(t, n.byteLength));
+                                        throw new Error(su(t, n.byteLength));
                                     case 9:
                                         return e.abrupt("return", n.byteOffset % 8 === 0 && n.byteOffset + n.byteLength <= n.buffer.byteLength ? n : n.slice());
                                     case 10:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, this)
@@ -11574,21 +11587,21 @@
                     key: "readSchema",
                     value: function() {
                         var e = F(U().mark((function e() {
                             var t, n, r, i, a = arguments;
                             return U().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
-                                        return t = a.length > 0 && void 0 !== a[0] && a[0], n = Xt.Schema, e.next = 4, this.readMessage(n);
+                                        return t = a.length > 0 && void 0 !== a[0] && a[0], n = Gt.Schema, e.next = 4, this.readMessage(n);
                                     case 4:
                                         if (r = e.sent, i = r && r.header(), !t || i) {
                                             e.next = 8;
                                             break
                                         }
-                                        throw new Error(su(n));
+                                        throw new Error(ou(n));
                                     case 8:
                                         return e.abrupt("return", i);
                                     case 9:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, this)
@@ -11601,17 +11614,17 @@
                     key: "readMetadataLength",
                     value: function() {
                         var e = F(U().mark((function e() {
                             var t, n, r;
                             return U().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
-                                        return e.next = 2, this.source.read(pu);
+                                        return e.next = 2, this.source.read(hu);
                                     case 2:
-                                        return t = e.sent, n = t && new ou(t), r = n && n.readInt32(0) || 0, e.abrupt("return", {
+                                        return t = e.sent, n = t && new iu(t), r = n && n.readInt32(0) || 0, e.abrupt("return", {
                                             done: 0 === r,
                                             value: r
                                         });
                                     case 6:
                                     case "end":
                                         return e.stop()
                                 }
@@ -11637,119 +11650,119 @@
                                         }
                                         return e.abrupt("return", fe);
                                     case 5:
                                         if (!(n.byteLength < t)) {
                                             e.next = 7;
                                             break
                                         }
-                                        throw new Error(cu(t, n.byteLength));
+                                        throw new Error(uu(t, n.byteLength));
                                     case 7:
                                         return e.abrupt("return", {
                                             done: !1,
-                                            value: Go.decode(n)
+                                            value: Qo.decode(n)
                                         });
                                     case 8:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, this)
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 }]), t
-            }(Symbol.asyncIterator), du = function(e) {
+            }(Symbol.asyncIterator), fu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
                     return Object(C.a)(this, n), (r = t.call(this, new Uint8Array(0)))._schema = !1, r._body = [], r._batchIndex = 0, r._dictionaryIndex = 0, r._json = e instanceof he ? e : new he(e), r
                 }
                 return Object(M.a)(n, [{
                     key: "next",
                     value: function() {
                         var e = this._json;
                         if (!this._schema) return this._schema = !0, {
                             done: !1,
-                            value: Go.fromJSON(e.schema, Xt.Schema)
+                            value: Qo.fromJSON(e.schema, Gt.Schema)
                         };
                         if (this._dictionaryIndex < e.dictionaries.length) {
                             var t = e.dictionaries[this._dictionaryIndex++];
                             return this._body = t.data.columns, {
                                 done: !1,
-                                value: Go.fromJSON(t, Xt.DictionaryBatch)
+                                value: Qo.fromJSON(t, Gt.DictionaryBatch)
                             }
                         }
                         if (this._batchIndex < e.batches.length) {
                             var n = e.batches[this._batchIndex++];
                             return this._body = n.columns, {
                                 done: !1,
-                                value: Go.fromJSON(n, Xt.RecordBatch)
+                                value: Qo.fromJSON(n, Gt.RecordBatch)
                             }
                         }
                         return this._body = [], fe
                     }
                 }, {
                     key: "readMessageBody",
                     value: function(e) {
                         return function e(t) {
                             return (t || []).reduce((function(t, n) {
-                                return [].concat(hn(t), hn(n.VALIDITY && [n.VALIDITY] || []), hn(n.TYPE && [n.TYPE] || []), hn(n.OFFSET && [n.OFFSET] || []), hn(n.DATA && [n.DATA] || []), hn(e(n.children)))
+                                return [].concat(cn(t), cn(n.VALIDITY && [n.VALIDITY] || []), cn(n.TYPE && [n.TYPE] || []), cn(n.OFFSET && [n.OFFSET] || []), cn(n.DATA && [n.DATA] || []), cn(e(n.children)))
                             }), [])
                         }(this._body)
                     }
                 }, {
                     key: "readMessage",
                     value: function(e) {
                         var t;
                         if ((t = this.next()).done) return null;
-                        if (null != e && t.value.headerType !== e) throw new Error(uu(e));
+                        if (null != e && t.value.headerType !== e) throw new Error(au(e));
                         return t.value
                     }
                 }, {
                     key: "readSchema",
                     value: function() {
-                        var e = Xt.Schema,
+                        var e = Gt.Schema,
                             t = this.readMessage(e),
                             n = t && t.header();
-                        if (!t || !n) throw new Error(su(e));
+                        if (!t || !n) throw new Error(ou(e));
                         return n
                     }
                 }]), n
-            }(fu), pu = 4, yu = "ARROW1", vu = new Uint8Array(6), bu = 0; bu < 6; bu += 1) vu[bu] = yu.charCodeAt(bu);
+            }(cu), hu = 4, du = "ARROW1", pu = new Uint8Array(6), yu = 0; yu < 6; yu += 1) pu[yu] = du.charCodeAt(yu);
 
-        function mu(e) {
-            for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0, n = -1, r = vu.length; ++n < r;)
-                if (vu[n] !== e[t + n]) return !1;
+        function vu(e) {
+            for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0, n = -1, r = pu.length; ++n < r;)
+                if (pu[n] !== e[t + n]) return !1;
             return !0
         }
-        var gu = vu.length,
-            ku = gu + pu,
-            wu = 2 * gu + pu,
-            _u = function(e) {
+        var bu = pu.length,
+            mu = bu + hu,
+            gu = 2 * bu + hu,
+            ku = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e;
                     return Object(C.a)(this, n), (e = t.call(this))._byteLength = 0, e._nodes = [], e._buffers = [], e._bufferRegions = [], e
                 }
                 return Object(M.a)(n, [{
                     key: "visit",
                     value: function(e) {
-                        if (!Tn.isDictionary(e.type)) {
+                        if (!jn.isDictionary(e.type)) {
                             var t = e.data,
                                 r = e.length,
                                 i = e.nullCount;
                             if (r > 2147483647) throw new RangeError("Cannot write arrays larger than 2^31 - 1 in length");
-                            Tn.isNull(e.type) || Ou.call(this, i <= 0 ? new Uint8Array(0) : on(t.offset, r, t.nullBitmap)), this.nodes.push(new eu(r, i))
+                            jn.isNull(e.type) || wu.call(this, i <= 0 ? new Uint8Array(0) : nn(t.offset, r, t.nullBitmap)), this.nodes.push(new Zo(r, i))
                         }
-                        return Ut(Object(Nt.a)(n.prototype), "visit", this).call(this, e)
+                        return Ct(Object(Ft.a)(n.prototype), "visit", this).call(this, e)
                     }
                 }, {
                     key: "visitNull",
                     value: function(e) {
                         return this
                     }
                 }, {
@@ -11777,82 +11790,82 @@
                     get: function() {
                         return this._bufferRegions
                     }
                 }], [{
                     key: "assemble",
                     value: function() {
                         for (var e = new n, t = arguments.length, r = new Array(t), i = 0; i < t; i++) r[i] = arguments[i];
-                        var a = Zi(jc, r),
+                        var a = Gi(Oc, r),
                             o = P(e.visitMany(a), 1)[0];
                         return void 0 === o ? e : o
                     }
                 }]), n
-            }(dn);
+            }(ln);
 
-        function Ou(e) {
+        function wu(e) {
             var t = e.byteLength + 7 & -8;
-            return this.buffers.push(e), this.bufferRegions.push(new Xo(this._byteLength, t)), this._byteLength += t, this
+            return this.buffers.push(e), this.bufferRegions.push(new Jo(this._byteLength, t)), this._byteLength += t, this
         }
 
-        function xu(e) {
-            return Ou.call(this, e.values.subarray(0, e.length * e.stride))
+        function _u(e) {
+            return wu.call(this, e.values.subarray(0, e.length * e.stride))
         }
 
-        function ju(e) {
+        function Ou(e) {
             var t = e.length,
                 n = e.values,
                 r = e.valueOffsets,
                 i = r[0],
                 a = r[t],
                 o = Math.min(a - i, n.byteLength - i);
-            return Ou.call(this, kt(-r[0], t, r)), Ou.call(this, n.subarray(i, i + o)), this
+            return wu.call(this, kt(-r[0], t, r)), wu.call(this, n.subarray(i, i + o)), this
         }
 
-        function Su(e) {
+        function ju(e) {
             var t = e.length,
                 n = e.valueOffsets;
-            return n && Ou.call(this, kt(n[0], t, n)), this.visit(e.getChildAt(0))
+            return n && wu.call(this, kt(n[0], t, n)), this.visit(e.getChildAt(0))
         }
 
-        function Tu(e) {
+        function xu(e) {
             return this.visitMany(e.type.children.map((function(t, n) {
                 return e.getChildAt(n)
             })).filter(Boolean))[0]
         }
-        _u.prototype.visitBool = function(e) {
+        ku.prototype.visitBool = function(e) {
             var t;
-            return e.nullCount >= e.length ? Ou.call(this, new Uint8Array(0)) : (t = e.values) instanceof Uint8Array ? Ou.call(this, on(e.offset, e.length, t)) : Ou.call(this, un(e))
-        }, _u.prototype.visitInt = xu, _u.prototype.visitFloat = xu, _u.prototype.visitUtf8 = ju, _u.prototype.visitBinary = ju, _u.prototype.visitFixedSizeBinary = xu, _u.prototype.visitDate = xu, _u.prototype.visitTimestamp = xu, _u.prototype.visitTime = xu, _u.prototype.visitDecimal = xu, _u.prototype.visitList = Su, _u.prototype.visitStruct = Tu, _u.prototype.visitUnion = function(e) {
+            return e.nullCount >= e.length ? wu.call(this, new Uint8Array(0)) : (t = e.values) instanceof Uint8Array ? wu.call(this, nn(e.offset, e.length, t)) : wu.call(this, rn(e))
+        }, ku.prototype.visitInt = _u, ku.prototype.visitFloat = _u, ku.prototype.visitUtf8 = Ou, ku.prototype.visitBinary = Ou, ku.prototype.visitFixedSizeBinary = _u, ku.prototype.visitDate = _u, ku.prototype.visitTimestamp = _u, ku.prototype.visitTime = _u, ku.prototype.visitDecimal = _u, ku.prototype.visitList = ju, ku.prototype.visitStruct = xu, ku.prototype.visitUnion = function(e) {
             var t = e.type,
                 n = e.length,
                 r = e.typeIds,
                 i = e.valueOffsets;
-            if (Ou.call(this, r), t.mode === Jt.Sparse) return Tu.call(this, e);
-            if (t.mode === Jt.Dense) {
-                if (e.offset <= 0) return Ou.call(this, i), Tu.call(this, e);
+            if (wu.call(this, r), t.mode === Qt.Sparse) return xu.call(this, e);
+            if (t.mode === Qt.Dense) {
+                if (e.offset <= 0) return wu.call(this, i), xu.call(this, e);
                 for (var a, o, u = r.reduce((function(e, t) {
                         return Math.max(e, t)
                     }), r[0]), s = new Int32Array(u + 1), c = new Int32Array(u + 1).fill(-1), l = new Int32Array(n), f = kt(-i[0], n, i), h = -1; ++h < n;) - 1 === (o = c[a = r[h]]) && (o = c[a] = f[a]), l[h] = f[h] - o, ++s[a];
-                Ou.call(this, l);
+                wu.call(this, l);
                 for (var d, p = -1, y = t.children.length; ++p < y;)
                     if (d = e.getChildAt(p)) {
                         var v = t.typeIds[p],
                             b = Math.min(n, s[v]);
                         this.visit(d.slice(c[v], b))
                     }
             }
             return this
-        }, _u.prototype.visitInterval = xu, _u.prototype.visitFixedSizeList = Su, _u.prototype.visitMap = Su;
-        var Iu = function(e, t) {
+        }, ku.prototype.visitInterval = _u, ku.prototype.visitFixedSizeList = ju, ku.prototype.visitMap = ju;
+        var Su = function(e, t) {
                 Object(ce.a)(r, e);
                 var n = Object(le.a)(r);
 
                 function r(e) {
                     var t;
-                    return Object(C.a)(this, r), (t = n.call(this))._position = 0, t._started = !1, t._sink = new Ka, t._schema = null, t._dictionaryBlocks = [], t._recordBatchBlocks = [], t._dictionaryDeltaOffsets = new Map, je(e) || (e = {
+                    return Object(C.a)(this, r), (t = n.call(this))._position = 0, t._started = !1, t._sink = new Ha, t._schema = null, t._dictionaryBlocks = [], t._recordBatchBlocks = [], t._dictionaryDeltaOffsets = new Map, xe(e) || (e = {
                         autoDestroy: !0,
                         writeLegacyIpcFormat: !1
                     }), t._autoDestroy = "boolean" !== typeof e.autoDestroy || e.autoDestroy, t._writeLegacyIpcFormat = "boolean" === typeof e.writeLegacyIpcFormat && e.writeLegacyIpcFormat, t
                 }
                 return Object(M.a)(r, [{
                     key: "toString",
                     value: function() {
@@ -11867,15 +11880,15 @@
                     }
                 }, {
                     key: "writeAll",
                     value: function(e) {
                         var t = this;
                         return Se(e) ? e.then((function(e) {
                             return t.writeAll(e)
-                        })) : Ie(e) ? Du(this, e) : Bu(this, e)
+                        })) : Ie(e) ? Au(this, e) : Eu(this, e)
                     }
                 }, {
                     key: "closed",
                     get: function() {
                         return this._sink.closed
                     }
                 }, {
@@ -11909,101 +11922,101 @@
                         return this._autoDestroy ? this.close() : this.reset(this._sink, this._schema), this
                     }
                 }, {
                     key: "reset",
                     value: function() {
                         var e, t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this._sink,
                             n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
-                        return t === this._sink || t instanceof Ka ? this._sink = t : (this._sink = new Ka, t && (je(e = t) && xe(e.abort) && xe(e.getWriter) && !(e instanceof de)) ? this.toDOMStream({
+                        return t === this._sink || t instanceof Ha ? this._sink = t : (this._sink = new Ha, t && (xe(e = t) && je(e.abort) && je(e.getWriter) && !(e instanceof de)) ? this.toDOMStream({
                             type: "bytes"
                         }).pipeTo(t) : t && function(e) {
-                            return je(e) && xe(e.end) && xe(e.write) && Oe(e.writable) && !(e instanceof de)
+                            return xe(e) && je(e.end) && je(e.write) && Oe(e.writable) && !(e instanceof de)
                         }(t) && this.toNodeStream({
                             objectMode: !1
                         }).pipe(t)), this._started && this._schema && this._writeFooter(this._schema), this._started = !1, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, n && n.compareTo(this._schema) || (null === n ? (this._position = 0, this._schema = null) : (this._started = !0, this._schema = n, this._writeSchema(n))), this
                     }
                 }, {
                     key: "write",
                     value: function(e) {
                         var t = null;
                         if (!this._sink) throw new Error("RecordBatchWriter is closed");
                         if (null === e || void 0 === e) return this.finish() && void 0;
-                        if (e instanceof xc && !(t = e.schema)) return this.finish() && void 0;
-                        if (e instanceof jc && !(t = e.schema)) return this.finish() && void 0;
+                        if (e instanceof _c && !(t = e.schema)) return this.finish() && void 0;
+                        if (e instanceof Oc && !(t = e.schema)) return this.finish() && void 0;
                         if (t && !t.compareTo(this._schema)) {
                             if (this._started && this._autoDestroy) return this.close();
                             this.reset(this._sink, t)
                         }
-                        e instanceof jc ? e instanceof Sc || this._writeRecordBatch(e) : e instanceof xc ? this.writeAll(e.chunks) : Te(e) && this.writeAll(e)
+                        e instanceof Oc ? e instanceof jc || this._writeRecordBatch(e) : e instanceof _c ? this.writeAll(e.chunks) : Te(e) && this.writeAll(e)
                     }
                 }, {
                     key: "_writeMessage",
                     value: function(e) {
                         var t = (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8) - 1,
-                            n = Go.encode(e),
+                            n = Qo.encode(e),
                             r = n.byteLength,
                             i = this._writeLegacyIpcFormat ? 4 : 8,
                             a = r + i + t & ~t,
                             o = a - r - i;
-                        return e.headerType === Xt.RecordBatch ? this._recordBatchBlocks.push(new $a(a, e.bodyLength, this._position)) : e.headerType === Xt.DictionaryBatch && this._dictionaryBlocks.push(new $a(a, e.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(a - i)), r > 0 && this._write(n), this._writePadding(o)
+                        return e.headerType === Gt.RecordBatch ? this._recordBatchBlocks.push(new Ya(a, e.bodyLength, this._position)) : e.headerType === Gt.DictionaryBatch && this._dictionaryBlocks.push(new Ya(a, e.bodyLength, this._position)), this._writeLegacyIpcFormat || this._write(Int32Array.of(-1)), this._write(Int32Array.of(a - i)), r > 0 && this._write(n), this._writePadding(o)
                     }
                 }, {
                     key: "_write",
                     value: function(e) {
                         if (this._started) {
                             var t = He(e);
                             t && t.byteLength > 0 && (this._sink.write(t), this._position += t.byteLength)
                         }
                         return this
                     }
                 }, {
                     key: "_writeSchema",
                     value: function(e) {
-                        return this._writeMessage(Go.from(e))
+                        return this._writeMessage(Qo.from(e))
                     }
                 }, {
                     key: "_writeFooter",
                     value: function(e) {
                         return this._writeLegacyIpcFormat ? this._write(Int32Array.of(0)) : this._write(Int32Array.of(-1, 0))
                     }
                 }, {
                     key: "_writeMagic",
                     value: function() {
-                        return this._write(vu)
+                        return this._write(pu)
                     }
                 }, {
                     key: "_writePadding",
                     value: function(e) {
                         return e > 0 ? this._write(new Uint8Array(e)) : this
                     }
                 }, {
                     key: "_writeRecordBatch",
                     value: function(e) {
-                        var t = _u.assemble(e),
+                        var t = ku.assemble(e),
                             n = t.byteLength,
                             r = t.nodes,
                             i = t.bufferRegions,
                             a = t.buffers,
-                            o = new Jo(e.length, r, i),
-                            u = Go.from(o, n);
+                            o = new qo(e.length, r, i),
+                            u = Qo.from(o, n);
                         return this._writeDictionaries(e)._writeMessage(u)._writeBodyBuffers(a)
                     }
                 }, {
                     key: "_writeDictionaryBatch",
                     value: function(e, t) {
                         var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                         this._dictionaryDeltaOffsets.set(t, e.length + (this._dictionaryDeltaOffsets.get(t) || 0));
-                        var r = _u.assemble(e),
+                        var r = ku.assemble(e),
                             i = r.byteLength,
                             a = r.nodes,
                             o = r.bufferRegions,
                             u = r.buffers,
-                            s = new Jo(e.length, a, o),
-                            c = new Zo(s, t, n),
-                            l = Go.from(c, i);
+                            s = new qo(e.length, a, o),
+                            c = new Go(s, t, n),
+                            l = Qo.from(c, i);
                         return this._writeMessage(l)._writeBodyBuffers(u)
                     }
                 }, {
                     key: "_writeBodyBuffers",
                     value: function(e) {
                         for (var t, n, r, i = -1, a = e.length; ++i < a;)(t = e[i]) && (n = t.byteLength) > 0 && (this._write(t), (r = (n + 7 & -8) - n) > 0 && this._writePadding(r));
                         return this
@@ -12047,32 +12060,32 @@
                 }, {
                     key: "throughDOM",
                     value: function(e, t) {
                         throw new Error('"throughDOM" not available in this environment')
                     }
                 }]), r
             }(de, Symbol.asyncIterator),
-            Eu = function(e) {
+            Tu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, null, [{
                     key: "writeAll",
                     value: function(e, t) {
                         var r = new n(t);
                         return Se(e) ? e.then((function(e) {
                             return r.writeAll(e)
-                        })) : Ie(e) ? Du(r, e) : Bu(r, e)
+                        })) : Ie(e) ? Au(r, e) : Eu(r, e)
                     }
                 }]), n
-            }(Iu),
-            Au = function(e) {
+            }(Su),
+            Iu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e;
                     return Object(C.a)(this, n), (e = t.call(this))._autoDestroy = !0, e
                 }
@@ -12080,51 +12093,51 @@
                     key: "_writeSchema",
                     value: function(e) {
                         return this._writeMagic()._writePadding(2)
                     }
                 }, {
                     key: "_writeFooter",
                     value: function(e) {
-                        var t = Ya.encode(new Ya(e, en.V4, this._recordBatchBlocks, this._dictionaryBlocks));
-                        return Ut(Object(Nt.a)(n.prototype), "_writeFooter", this).call(this, e)._write(t)._write(Int32Array.of(t.byteLength))._writeMagic()
+                        var t = za.encode(new za(e, Jt.V4, this._recordBatchBlocks, this._dictionaryBlocks));
+                        return Ct(Object(Ft.a)(n.prototype), "_writeFooter", this).call(this, e)._write(t)._write(Int32Array.of(t.byteLength))._writeMagic()
                     }
                 }], [{
                     key: "writeAll",
                     value: function(e) {
                         var t = new n;
                         return Se(e) ? e.then((function(e) {
                             return t.writeAll(e)
-                        })) : Ie(e) ? Du(t, e) : Bu(t, e)
+                        })) : Ie(e) ? Au(t, e) : Eu(t, e)
                     }
                 }]), n
-            }(Iu);
+            }(Su);
 
-        function Bu(e, t) {
+        function Eu(e, t) {
             var n = t;
-            t instanceof xc && (n = t.chunks, e.reset(void 0, t.schema));
+            t instanceof _c && (n = t.chunks, e.reset(void 0, t.schema));
             var r, i = D(n);
             try {
                 for (i.s(); !(r = i.n()).done;) {
                     var a = r.value;
                     e.write(a)
                 }
             } catch (o) {
                 i.e(o)
             } finally {
                 i.f()
             }
             return e.finish()
         }
 
-        function Du(e, t) {
-            return Lu.apply(this, arguments)
+        function Au(e, t) {
+            return Bu.apply(this, arguments)
         }
 
-        function Lu() {
-            return (Lu = F(U().mark((function e(t, n) {
+        function Bu() {
+            return (Bu = F(U().mark((function e(t, n) {
                 var r, i, a, o, u, s;
                 return U().wrap((function(e) {
                     for (;;) switch (e.prev = e.next) {
                         case 0:
                             r = !1, i = !1, e.prev = 2, o = H(n);
                         case 4:
                             return e.next = 6, o.next();
@@ -12166,70 +12179,70 @@
                     }
                 }), e, null, [
                     [2, 14, 18, 28],
                     [19, , 23, 27]
                 ])
             })))).apply(this, arguments)
         }
-        var Fu = new Uint8Array(0),
-            Cu = function(e) {
-                return [Fu, Fu, new Uint8Array(e), Fu]
+        var Du = new Uint8Array(0),
+            Lu = function(e) {
+                return [Du, Du, new Uint8Array(e), Du]
             };
 
-        function Mu(e, t) {
+        function Fu(e, t) {
             return function(e, t) {
-                var n, r = hn(e.fields),
+                var n, r = cn(e.fields),
                     i = [],
                     a = {
                         numBatches: t.reduce((function(e, t) {
                             return Math.max(e, t.length)
                         }), 0)
                     },
                     o = 0,
                     u = 0,
                     s = -1,
                     c = t.length,
                     l = [];
                 for (; a.numBatches-- > 0;) {
                     for (u = Number.POSITIVE_INFINITY, s = -1; ++s < c;) l[s] = n = t[s].shift(), u = Math.min(u, n ? n.length : u);
-                    isFinite(u) && (l = Nu(r, u, l, t, a), u > 0 && (i[o++] = [u, l.slice()]))
+                    isFinite(u) && (l = Cu(r, u, l, t, a), u > 0 && (i[o++] = [u, l.slice()]))
                 }
-                return [e = new ia(r, e.metadata), i.map((function(t) {
-                    return Pr(jc, [e].concat(hn(t)))
+                return [e = new na(r, e.metadata), i.map((function(t) {
+                    return Mr(Oc, [e].concat(cn(t)))
                 }))]
             }(e, t.map((function(e) {
-                return e instanceof Wi ? e.chunks.map((function(e) {
+                return e instanceof Vi ? e.chunks.map((function(e) {
                     return e.data
                 })) : [e.data]
             })))
         }
 
-        function Nu(e, t, n, r, i) {
+        function Cu(e, t, n, r, i) {
             for (var a, o, u = 0, s = -1, c = r.length, l = (t + 63 & -64) >> 3; ++s < c;)(a = n[s]) && (u = a.length) >= t ? u === t ? n[s] = a : (n[s] = a.slice(0, t), a = a.slice(t, u - t), i.numBatches = Math.max(i.numBatches, r[s].unshift(a))) : ((o = e[s]).nullable || (e[s] = o.clone({
                 nullable: !0
-            })), n[s] = a ? a._changeLengthAndBackfillNullBitmap(t) : sr.new(o.type, 0, t, t, Cu(l)));
+            })), n[s] = a ? a._changeLengthAndBackfillNullBitmap(t) : ar.new(o.type, 0, t, t, Lu(l)));
             return n
         }
 
-        function Uu(e, t) {
+        function Mu(e, t) {
             if (null == e) return {};
             var n, r, i = function(e, t) {
                 if (null == e) return {};
                 var n, r, i = {},
                     a = Object.keys(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || (i[n] = e[n]);
                 return i
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var a = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < a.length; r++) n = a[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (i[n] = e[n])
             }
             return i
         }
-        var Pu = function(e, t) {
+        var Nu = function(e, t) {
             Object(ce.a)(r, e);
             var n = Object(le.a)(r);
 
             function r(e, t) {
                 var i;
                 return Object(C.a)(this, r), (i = n.call(this))._children = t, i.numChildren = e.childData.length, i._bindDataAccessors(i.data = e), i
             }
@@ -12267,15 +12280,15 @@
                 key: "byteLength",
                 get: function() {
                     return this.data.byteLength
                 }
             }, {
                 key: "VectorName",
                 get: function() {
-                    return "".concat($t[this.typeId], "Vector")
+                    return "".concat(Wt[this.typeId], "Vector")
                 }
             }, {
                 key: "ArrayType",
                 get: function() {
                     return this.type.ArrayType
                 }
             }, {
@@ -12303,140 +12316,140 @@
                 get: function() {
                     return "".concat(this.VectorName, "<").concat(this.type[Symbol.toStringTag], ">")
                 }
             }, {
                 key: "clone",
                 value: function(e) {
                     var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this._children;
-                    return Ht.new(e, t)
+                    return zt.new(e, t)
                 }
             }, {
                 key: "concat",
                 value: function() {
                     for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                    return Wi.concat.apply(Wi, [this].concat(t))
+                    return Vi.concat.apply(Vi, [this].concat(t))
                 }
             }, {
                 key: "slice",
                 value: function(e, t) {
-                    return Ni(this, e, t, this._sliceInternal)
+                    return Ci(this, e, t, this._sliceInternal)
                 }
             }, {
                 key: "isValid",
                 value: function(e) {
                     if (this.nullCount > 0) {
                         var t = this.offset + e;
                         return 0 !== (this.nullBitmap[t >> 3] & 1 << t % 8)
                     }
                     return !0
                 }
             }, {
                 key: "getChildAt",
                 value: function(e) {
-                    return e < 0 || e >= this.numChildren ? null : (this._children || (this._children = []))[e] || (this._children[e] = Ht.new(this.data.childData[e]))
+                    return e < 0 || e >= this.numChildren ? null : (this._children || (this._children = []))[e] || (this._children[e] = zt.new(this.data.childData[e]))
                 }
             }, {
                 key: "toJSON",
                 value: function() {
-                    return hn(this)
+                    return cn(this)
                 }
             }, {
                 key: "_sliceInternal",
                 value: function(e, t, n) {
                     return e.clone(e.data.slice(t, n - t), null)
                 }
             }, {
                 key: "_bindDataAccessors",
                 value: function(e) {}
             }]), r
-        }(Ht, Symbol.toStringTag);
-        Pu.prototype[Symbol.isConcatSpreadable] = !0;
-        var Ru = function(e) {
+        }(zt, Symbol.toStringTag);
+        Nu.prototype[Symbol.isConcatSpreadable] = !0;
+        var Uu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "asUtf8",
                     value: function() {
-                        return Ht.new(this.data.clone(new Wn))
+                        return zt.new(this.data.clone(new Rn))
                     }
                 }]), n
-            }(Pu),
-            Vu = function(e) {
+            }(Nu),
+            Pu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, null, [{
                     key: "from",
                     value: function(e) {
-                        return Oc((function() {
-                            return new Yn
+                        return wc((function() {
+                            return new Vn
                         }), e)
                     }
                 }]), n
-            }(Pu),
-            zu = function(e) {
+            }(Nu),
+            Ru = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, null, [{
                     key: "from",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                        return 2 === t.length ? Oc((function() {
-                            return t[1] === Qt.DAY ? new Kn : new Qn
-                        }), t[0]) : Oc((function() {
-                            return new Qn
+                        return 2 === t.length ? wc((function() {
+                            return t[1] === Ht.DAY ? new Yn : new Hn
+                        }), t[0]) : wc((function() {
+                            return new Hn
                         }), t[0])
                     }
                 }]), n
-            }(Pu),
-            Wu = function(e) {
+            }(Nu),
+            Vu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(zu),
-            Yu = function(e) {
+            }(Ru),
+            zu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(zu),
-            Hu = function(e) {
+            }(Ru),
+            Wu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            $u = function(e) {
+            }(Nu),
+            Yu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
-                    return Object(C.a)(this, n), (r = t.call(this, e)).indices = Ht.new(e.clone(r.type.indices)), r
+                    return Object(C.a)(this, n), (r = t.call(this, e)).indices = zt.new(e.clone(r.type.indices)), r
                 }
                 return Object(M.a)(n, [{
                     key: "dictionary",
                     get: function() {
                         return this.data.dictionary
                     }
                 }, {
@@ -12468,70 +12481,70 @@
                     key: "from",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                         if (3 === t.length) {
                             var r = t[0],
                                 i = t[1],
                                 a = t[2],
-                                o = new or(r.type, i, null, null);
-                            return Ht.new(sr.Dictionary(o, 0, a.length, 0, null, a, r))
+                                o = new rr(r.type, i, null, null);
+                            return zt.new(ar.Dictionary(o, 0, a.length, 0, null, a, r))
                         }
-                        return Oc((function() {
+                        return wc((function() {
                             return t[0].type
                         }), t[0])
                     }
                 }]), n
-            }(Pu);
-        $u.prototype.indices = null;
-        var Ku = function(e) {
+            }(Nu);
+        Yu.prototype.indices = null;
+        var Hu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            Qu = function(e) {
+            }(Nu),
+            $u = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            qu = function(e) {
+            }(Nu),
+            Ku = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, null, [{
                     key: "from",
                     value: function(e) {
-                        var t = ts(this);
+                        var t = Xu(this);
                         if (e instanceof ArrayBuffer || ArrayBuffer.isView(e)) {
-                            var n = es(e.constructor) || t;
+                            var n = Zu(e.constructor) || t;
                             if (null === t && (t = n), t && t === n) {
                                 var r = new t,
                                     i = e.byteLength / r.ArrayType.BYTES_PER_ELEMENT;
-                                if (!Xu(t, e.constructor)) return Ht.new(sr.Float(r, 0, i, 0, null, e))
+                                if (!Ju(t, e.constructor)) return zt.new(ar.Float(r, 0, i, 0, null, e))
                             }
                         }
-                        if (t) return Oc((function() {
+                        if (t) return wc((function() {
                             return new t
                         }), e);
                         if (e instanceof DataView || e instanceof ArrayBuffer) throw new TypeError("Cannot infer float type from instance of ".concat(e.constructor.name));
                         throw new TypeError("Unrecognized FloatVector input")
                     }
                 }]), n
-            }(Pu),
-            Gu = function(e) {
+            }(Nu),
+            Qu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -12541,146 +12554,146 @@
                     }
                 }, {
                     key: "toFloat64Array",
                     value: function() {
                         return new Float64Array(this)
                     }
                 }]), n
-            }(qu),
-            Ju = function(e) {
+            }(Ku),
+            qu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(qu),
-            Zu = function(e) {
+            }(Ku),
+            Gu = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(qu),
-            Xu = function(e, t) {
-                return e === Pn && t !== Uint16Array
+            }(Ku),
+            Ju = function(e, t) {
+                return e === Mn && t !== Uint16Array
             },
-            es = function(e) {
+            Zu = function(e) {
                 switch (e) {
                     case Uint16Array:
-                        return Pn;
+                        return Mn;
                     case Float32Array:
-                        return Rn;
+                        return Nn;
                     case Float64Array:
-                        return Vn;
+                        return Un;
                     default:
                         return null
                 }
             },
-            ts = function(e) {
+            Xu = function(e) {
                 switch (e) {
+                    case Qu:
+                        return Mn;
+                    case qu:
+                        return Nn;
                     case Gu:
-                        return Pn;
-                    case Ju:
-                        return Rn;
-                    case Zu:
-                        return Vn;
+                        return Un;
                     default:
                         return null
                 }
             },
-            ns = function(e) {
+            es = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            rs = function(e) {
+            }(Nu),
+            ts = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ns),
-            is = function(e) {
+            }(es),
+            ns = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(ns),
-            as = function(e) {
+            }(es),
+            rs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, null, [{
                     key: "from",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                         var r = t[0],
                             i = t[1],
                             a = void 0 !== i && i,
-                            o = vs(this, a);
+                            o = ps(this, a);
                         if (r instanceof ArrayBuffer || ArrayBuffer.isView(r)) {
-                            var u = ys(r.constructor, a) || o;
+                            var u = ds(r.constructor, a) || o;
                             if (null === o && (o = u), o && o === u) {
                                 var s = new o,
                                     c = r.byteLength / s.ArrayType.BYTES_PER_ELEMENT;
-                                return ps(o, r.constructor) && (c *= .5), Ht.new(sr.Int(s, 0, c, 0, null, r))
+                                return hs(o, r.constructor) && (c *= .5), zt.new(ar.Int(s, 0, c, 0, null, r))
                             }
                         }
-                        if (o) return Oc((function() {
+                        if (o) return wc((function() {
                             return new o
                         }), r);
                         if (r instanceof DataView || r instanceof ArrayBuffer) throw new TypeError("Cannot infer integer type from instance of ".concat(r.constructor.name));
                         throw new TypeError("Unrecognized IntVector input")
                     }
                 }]), n
-            }(Pu),
-            os = function(e) {
+            }(Nu),
+            is = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(as),
-            us = function(e) {
+            }(rs),
+            as = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(as),
-            ss = function(e) {
+            }(rs),
+            os = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(as),
-            cs = function(e) {
+            }(rs),
+            us = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -12690,43 +12703,43 @@
                     }
                 }, {
                     key: "values64",
                     get: function() {
                         return this._values64 || (this._values64 = this.toBigInt64Array())
                     }
                 }]), n
-            }(as),
-            ls = function(e) {
+            }(rs),
+            ss = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(as),
-            fs = function(e) {
+            }(rs),
+            cs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(as),
-            hs = function(e) {
+            }(rs),
+            ls = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(as),
-            ds = function(e) {
+            }(rs),
+            fs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -12736,510 +12749,510 @@
                     }
                 }, {
                     key: "values64",
                     get: function() {
                         return this._values64 || (this._values64 = this.toBigUint64Array())
                     }
                 }]), n
-            }(as),
-            ps = function(e, t) {
-                return (e === Ln || e === Nn) && (t === Int32Array || t === Uint32Array)
+            }(rs),
+            hs = function(e, t) {
+                return (e === An || e === Fn) && (t === Int32Array || t === Uint32Array)
             },
-            ys = function(e, t) {
+            ds = function(e, t) {
                 switch (e) {
                     case Int8Array:
-                        return An;
+                        return Tn;
                     case Int16Array:
-                        return Bn;
+                        return In;
                     case Int32Array:
-                        return t ? Ln : Dn;
+                        return t ? An : En;
                     case ge:
-                        return Ln;
+                        return An;
                     case Uint8Array:
-                        return Fn;
+                        return Bn;
                     case Uint16Array:
-                        return Cn;
+                        return Dn;
                     case Uint32Array:
-                        return t ? Nn : Mn;
+                        return t ? Fn : Ln;
                     case we:
-                        return Nn;
+                        return Fn;
                     default:
                         return null
                 }
             },
-            vs = function(e, t) {
+            ps = function(e, t) {
                 switch (e) {
+                    case is:
+                        return Tn;
+                    case as:
+                        return In;
                     case os:
-                        return An;
+                        return t ? An : En;
                     case us:
-                        return Bn;
+                        return An;
                     case ss:
-                        return t ? Ln : Dn;
+                        return Bn;
                     case cs:
-                        return Ln;
+                        return Dn;
                     case ls:
-                        return Fn;
+                        return t ? Fn : Ln;
                     case fs:
-                        return Cn;
-                    case hs:
-                        return t ? Nn : Mn;
-                    case ds:
-                        return Nn;
+                        return Fn;
                     default:
                         return null
                 }
             },
-            bs = function(e) {
+            ys = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            ms = function(e) {
+            }(Nu),
+            vs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "asList",
                     value: function() {
                         var e = this.type.children[0];
-                        return Ht.new(this.data.clone(new Zn(e)))
+                        return zt.new(this.data.clone(new qn(e)))
                     }
                 }, {
                     key: "bind",
                     value: function(e) {
                         var t = this.getChildAt(0),
                             n = this.valueOffsets,
                             r = n[e],
                             i = n[e + 1];
-                        return new Bi(t.slice(r, i))
+                        return new Ei(t.slice(r, i))
                     }
                 }]), n
-            }(Pu),
-            gs = function(e) {
+            }(Nu),
+            bs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            ks = Symbol.for("rowIndex"),
-            ws = function(e) {
+            }(Nu),
+            ms = Symbol.for("rowIndex"),
+            gs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "bind",
                     value: function(e) {
-                        var t = this._row || (this._row = new Di(this)),
+                        var t = this._row || (this._row = new Ai(this)),
                             n = Object.create(t);
-                        return n[ks] = e, n
+                        return n[ms] = e, n
                     }
                 }]), n
-            }(Pu),
-            _s = function(e) {
+            }(Nu),
+            ks = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            Os = function(e) {
+            }(Nu),
+            ws = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(_s),
-            xs = function(e) {
+            }(ks),
+            _s = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(_s),
-            js = function(e) {
+            }(ks),
+            Os = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(_s),
-            Ss = function(e) {
+            }(ks),
+            js = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(_s),
-            Ts = function(e) {
+            }(ks),
+            xs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Pu),
-            Is = function(e) {
+            }(Nu),
+            Ss = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Ts),
-            Es = function(e) {
+            }(xs),
+            Ts = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Ts),
-            As = function(e) {
+            }(xs),
+            Is = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Ts),
-            Bs = function(e) {
+            }(xs),
+            Es = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Ts),
-            Ds = function(e) {
+            }(xs),
+            As = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "typeIdToChildIndex",
                     get: function() {
                         return this.data.type.typeIdToChildIndex
                     }
                 }]), n
-            }(Pu),
-            Ls = function(e) {
+            }(Nu),
+            Bs = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "valueOffsets",
                     get: function() {
                         return this.data.valueOffsets
                     }
                 }]), n
-            }(Ds),
-            Fs = function(e) {
+            }(As),
+            Ds = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(Ds),
-            Cs = function(e) {
+            }(As),
+            Ls = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "asBinary",
                     value: function() {
-                        return Ht.new(this.data.clone(new zn))
+                        return zt.new(this.data.clone(new Pn))
                     }
                 }], [{
                     key: "from",
                     value: function(e) {
-                        return Oc((function() {
-                            return new Wn
+                        return wc((function() {
+                            return new Rn
                         }), e)
                     }
                 }]), n
-            }(Pu);
+            }(Nu);
 
-        function Ms(e) {
+        function Fs(e) {
             return function() {
                 return e(this)
             }
         }
 
-        function Ns(e) {
+        function Cs(e) {
             return function(t, n) {
                 return e(this, t, n)
             }
         }
-        var Us = function(e) {
+        var Ms = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(dn),
-            Ps = function(e, t) {
+            }(ln),
+            Ns = function(e, t) {
                 return 4294967296 * e[t + 1] + (e[t] >>> 0)
             },
-            Rs = function(e) {
+            Us = function(e) {
                 return new Date(e)
             },
-            Vs = function(e, t, n) {
+            Ps = function(e, t, n) {
                 var r = t[n],
                     i = t[n + 1];
                 return null != r && null != i ? e.subarray(r, i) : null
             },
-            zs = function(e, t) {
+            Rs = function(e, t) {
                 return function(e, t) {
-                    return Rs(function(e, t) {
+                    return Us(function(e, t) {
                         return 864e5 * e[t]
                     }(e, t))
                 }(e.values, t)
             },
-            Ws = function(e, t) {
+            Vs = function(e, t) {
                 return function(e, t) {
-                    return Rs(Ps(e, t))
+                    return Us(Ns(e, t))
                 }(e.values, 2 * t)
             },
-            Ys = function(e, t) {
+            zs = function(e, t) {
                 var n = e.stride;
                 return e.values[n * t]
             },
-            Hs = function(e, t) {
+            Ws = function(e, t) {
                 var n = e.stride;
-                return Br(e.values[n * t])
+                return Ir(e.values[n * t])
             },
-            $s = function(e, t) {
+            Ys = function(e, t) {
                 var n = e.stride,
                     r = e.values,
                     i = e.type;
-                return Gr.new(r.subarray(n * t, n * (t + 1)), i.isSigned)
+                return Kr.new(r.subarray(n * t, n * (t + 1)), i.isSigned)
             },
-            Ks = function(e, t) {
+            Hs = function(e, t) {
                 var n = e.values;
-                return 1e3 * Ps(n, 2 * t)
+                return 1e3 * Ns(n, 2 * t)
             },
-            Qs = function(e, t) {
+            $s = function(e, t) {
                 var n = e.values;
-                return Ps(n, 2 * t)
+                return Ns(n, 2 * t)
             },
-            qs = function(e, t) {
+            Ks = function(e, t) {
                 return function(e, t) {
                     return e[t + 1] / 1e3 * 4294967296 + (e[t] >>> 0) / 1e3
                 }(e.values, 2 * t)
             },
-            Gs = function(e, t) {
+            Qs = function(e, t) {
                 return function(e, t) {
                     return e[t + 1] / 1e6 * 4294967296 + (e[t] >>> 0) / 1e6
                 }(e.values, 2 * t)
             },
-            Js = function(e, t) {
+            qs = function(e, t) {
                 return e.values[e.stride * t]
             },
-            Zs = function(e, t) {
+            Gs = function(e, t) {
                 return e.values[e.stride * t]
             },
-            Xs = function(e, t) {
+            Js = function(e, t) {
                 var n = e.values;
-                return Gr.signed(n.subarray(2 * t, 2 * (t + 1)))
+                return Kr.signed(n.subarray(2 * t, 2 * (t + 1)))
             },
-            ec = function(e, t) {
+            Zs = function(e, t) {
                 var n = e.values;
-                return Gr.signed(n.subarray(2 * t, 2 * (t + 1)))
+                return Kr.signed(n.subarray(2 * t, 2 * (t + 1)))
             },
-            tc = function(e, t) {
+            Xs = function(e, t) {
                 var n = e.typeIdToChildIndex[e.typeIds[t]],
                     r = e.getChildAt(n);
                 return r ? r.get(e.valueOffsets[t]) : null
             },
-            nc = function(e, t) {
+            ec = function(e, t) {
                 var n = e.typeIdToChildIndex[e.typeIds[t]],
                     r = e.getChildAt(n);
                 return r ? r.get(t) : null
             },
-            rc = function(e, t) {
+            tc = function(e, t) {
                 return e.values.subarray(2 * t, 2 * (t + 1))
             },
-            ic = function(e, t) {
+            nc = function(e, t) {
                 var n = e.values[t],
                     r = new Int32Array(2);
                 return r[0] = n / 12 | 0, r[1] = n % 12 | 0, r
             };
-        Us.prototype.visitNull = function(e, t) {
+        Ms.prototype.visitNull = function(e, t) {
             return null
-        }, Us.prototype.visitBool = function(e, t) {
+        }, Ms.prototype.visitBool = function(e, t) {
             var n = e.offset + t;
             return 0 !== (e.values[n >> 3] & 1 << n % 8)
-        }, Us.prototype.visitInt = function(e, t) {
-            return e.type.bitWidth < 64 ? Ys(e, t) : $s(e, t)
-        }, Us.prototype.visitInt8 = Ys, Us.prototype.visitInt16 = Ys, Us.prototype.visitInt32 = Ys, Us.prototype.visitInt64 = $s, Us.prototype.visitUint8 = Ys, Us.prototype.visitUint16 = Ys, Us.prototype.visitUint32 = Ys, Us.prototype.visitUint64 = $s, Us.prototype.visitFloat = function(e, t) {
-            return e.type.precision !== Gt.HALF ? Ys(e, t) : Hs(e, t)
-        }, Us.prototype.visitFloat16 = Hs, Us.prototype.visitFloat32 = Ys, Us.prototype.visitFloat64 = Ys, Us.prototype.visitUtf8 = function(e, t) {
+        }, Ms.prototype.visitInt = function(e, t) {
+            return e.type.bitWidth < 64 ? zs(e, t) : Ys(e, t)
+        }, Ms.prototype.visitInt8 = zs, Ms.prototype.visitInt16 = zs, Ms.prototype.visitInt32 = zs, Ms.prototype.visitInt64 = Ys, Ms.prototype.visitUint8 = zs, Ms.prototype.visitUint16 = zs, Ms.prototype.visitUint32 = zs, Ms.prototype.visitUint64 = Ys, Ms.prototype.visitFloat = function(e, t) {
+            return e.type.precision !== Kt.HALF ? zs(e, t) : Ws(e, t)
+        }, Ms.prototype.visitFloat16 = Ws, Ms.prototype.visitFloat32 = zs, Ms.prototype.visitFloat64 = zs, Ms.prototype.visitUtf8 = function(e, t) {
             var n = e.values,
                 r = e.valueOffsets,
-                i = Vs(n, r, t);
+                i = Ps(n, r, t);
             return null !== i ? ue(i) : null
-        }, Us.prototype.visitBinary = function(e, t) {
+        }, Ms.prototype.visitBinary = function(e, t) {
             var n = e.values,
                 r = e.valueOffsets;
-            return Vs(n, r, t)
-        }, Us.prototype.visitFixedSizeBinary = function(e, t) {
+            return Ps(n, r, t)
+        }, Ms.prototype.visitFixedSizeBinary = function(e, t) {
             var n = e.stride;
             return e.values.subarray(n * t, n * (t + 1))
-        }, Us.prototype.visitDate = function(e, t) {
-            return e.type.unit === Qt.DAY ? zs(e, t) : Ws(e, t)
-        }, Us.prototype.visitDateDay = zs, Us.prototype.visitDateMillisecond = Ws, Us.prototype.visitTimestamp = function(e, t) {
+        }, Ms.prototype.visitDate = function(e, t) {
+            return e.type.unit === Ht.DAY ? Rs(e, t) : Vs(e, t)
+        }, Ms.prototype.visitDateDay = Rs, Ms.prototype.visitDateMillisecond = Vs, Ms.prototype.visitTimestamp = function(e, t) {
             switch (e.type.unit) {
-                case qt.SECOND:
+                case $t.SECOND:
+                    return Hs(e, t);
+                case $t.MILLISECOND:
+                    return $s(e, t);
+                case $t.MICROSECOND:
                     return Ks(e, t);
-                case qt.MILLISECOND:
-                    return Qs(e, t);
-                case qt.MICROSECOND:
-                    return qs(e, t);
-                case qt.NANOSECOND:
-                    return Gs(e, t)
+                case $t.NANOSECOND:
+                    return Qs(e, t)
             }
-        }, Us.prototype.visitTimestampSecond = Ks, Us.prototype.visitTimestampMillisecond = Qs, Us.prototype.visitTimestampMicrosecond = qs, Us.prototype.visitTimestampNanosecond = Gs, Us.prototype.visitTime = function(e, t) {
+        }, Ms.prototype.visitTimestampSecond = Hs, Ms.prototype.visitTimestampMillisecond = $s, Ms.prototype.visitTimestampMicrosecond = Ks, Ms.prototype.visitTimestampNanosecond = Qs, Ms.prototype.visitTime = function(e, t) {
             switch (e.type.unit) {
-                case qt.SECOND:
+                case $t.SECOND:
+                    return qs(e, t);
+                case $t.MILLISECOND:
+                    return Gs(e, t);
+                case $t.MICROSECOND:
                     return Js(e, t);
-                case qt.MILLISECOND:
-                    return Zs(e, t);
-                case qt.MICROSECOND:
-                    return Xs(e, t);
-                case qt.NANOSECOND:
-                    return ec(e, t)
+                case $t.NANOSECOND:
+                    return Zs(e, t)
             }
-        }, Us.prototype.visitTimeSecond = Js, Us.prototype.visitTimeMillisecond = Zs, Us.prototype.visitTimeMicrosecond = Xs, Us.prototype.visitTimeNanosecond = ec, Us.prototype.visitDecimal = function(e, t) {
+        }, Ms.prototype.visitTimeSecond = qs, Ms.prototype.visitTimeMillisecond = Gs, Ms.prototype.visitTimeMicrosecond = Js, Ms.prototype.visitTimeNanosecond = Zs, Ms.prototype.visitDecimal = function(e, t) {
             var n = e.values;
-            return Gr.decimal(n.subarray(4 * t, 4 * (t + 1)))
-        }, Us.prototype.visitList = function(e, t) {
+            return Kr.decimal(n.subarray(4 * t, 4 * (t + 1)))
+        }, Ms.prototype.visitList = function(e, t) {
             var n = e.getChildAt(0),
                 r = e.valueOffsets,
                 i = e.stride;
             return n.slice(r[t * i], r[t * i + 1])
-        }, Us.prototype.visitStruct = function(e, t) {
+        }, Ms.prototype.visitStruct = function(e, t) {
             return e.bind(t)
-        }, Us.prototype.visitUnion = function(e, t) {
-            return e.type.mode === Jt.Dense ? tc(e, t) : nc(e, t)
-        }, Us.prototype.visitDenseUnion = tc, Us.prototype.visitSparseUnion = nc, Us.prototype.visitDictionary = function(e, t) {
+        }, Ms.prototype.visitUnion = function(e, t) {
+            return e.type.mode === Qt.Dense ? Xs(e, t) : ec(e, t)
+        }, Ms.prototype.visitDenseUnion = Xs, Ms.prototype.visitSparseUnion = ec, Ms.prototype.visitDictionary = function(e, t) {
             return e.getValue(e.getKey(t))
-        }, Us.prototype.visitInterval = function(e, t) {
-            return e.type.unit === Zt.DAY_TIME ? rc(e, t) : ic(e, t)
-        }, Us.prototype.visitIntervalDayTime = rc, Us.prototype.visitIntervalYearMonth = ic, Us.prototype.visitFixedSizeList = function(e, t) {
+        }, Ms.prototype.visitInterval = function(e, t) {
+            return e.type.unit === qt.DAY_TIME ? tc(e, t) : nc(e, t)
+        }, Ms.prototype.visitIntervalDayTime = tc, Ms.prototype.visitIntervalYearMonth = nc, Ms.prototype.visitFixedSizeList = function(e, t) {
             var n = e.getChildAt(0),
                 r = e.stride;
             return n.slice(t * r, (t + 1) * r)
-        }, Us.prototype.visitMap = function(e, t) {
+        }, Ms.prototype.visitMap = function(e, t) {
             return e.bind(t)
         };
-        var ac = new Us,
-            oc = function(e) {
+        var rc = new Ms,
+            ic = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(dn);
+            }(ln);
 
-        function uc(e, t, n) {
+        function ac(e, t, n) {
             if (void 0 === t) return -1;
             if (null === t) return function(e, t) {
                 var n = e.nullBitmap;
                 if (!n || e.nullCount <= 0) return -1;
                 var r, i = 0,
-                    a = D(sn(n, e.data.offset + (t || 0), e.length, n, nn));
+                    a = D(an(n, e.data.offset + (t || 0), e.length, n, Xt));
                 try {
                     for (a.s(); !(r = a.n()).done;) {
                         if (!r.value) return i;
                         ++i
                     }
                 } catch (o) {
                     a.e(o)
                 } finally {
                     a.f()
                 }
                 return -1
             }(e, n);
-            for (var r = Ri(t), i = (n || 0) - 1, a = e.length; ++i < a;)
+            for (var r = Ui(t), i = (n || 0) - 1, a = e.length; ++i < a;)
                 if (r(e.get(i))) return i;
             return -1
         }
 
-        function sc(e, t, n) {
-            for (var r = Ri(t), i = (n || 0) - 1, a = e.length; ++i < a;)
+        function oc(e, t, n) {
+            for (var r = Ui(t), i = (n || 0) - 1, a = e.length; ++i < a;)
                 if (r(e.get(i))) return i;
             return -1
         }
-        oc.prototype.visitNull = function(e, t) {
+        ic.prototype.visitNull = function(e, t) {
             return null === t && e.length > 0 ? 0 : -1
-        }, oc.prototype.visitBool = uc, oc.prototype.visitInt = uc, oc.prototype.visitInt8 = uc, oc.prototype.visitInt16 = uc, oc.prototype.visitInt32 = uc, oc.prototype.visitInt64 = uc, oc.prototype.visitUint8 = uc, oc.prototype.visitUint16 = uc, oc.prototype.visitUint32 = uc, oc.prototype.visitUint64 = uc, oc.prototype.visitFloat = uc, oc.prototype.visitFloat16 = uc, oc.prototype.visitFloat32 = uc, oc.prototype.visitFloat64 = uc, oc.prototype.visitUtf8 = uc, oc.prototype.visitBinary = uc, oc.prototype.visitFixedSizeBinary = uc, oc.prototype.visitDate = uc, oc.prototype.visitDateDay = uc, oc.prototype.visitDateMillisecond = uc, oc.prototype.visitTimestamp = uc, oc.prototype.visitTimestampSecond = uc, oc.prototype.visitTimestampMillisecond = uc, oc.prototype.visitTimestampMicrosecond = uc, oc.prototype.visitTimestampNanosecond = uc, oc.prototype.visitTime = uc, oc.prototype.visitTimeSecond = uc, oc.prototype.visitTimeMillisecond = uc, oc.prototype.visitTimeMicrosecond = uc, oc.prototype.visitTimeNanosecond = uc, oc.prototype.visitDecimal = uc, oc.prototype.visitList = uc, oc.prototype.visitStruct = uc, oc.prototype.visitUnion = uc, oc.prototype.visitDenseUnion = sc, oc.prototype.visitSparseUnion = sc, oc.prototype.visitDictionary = uc, oc.prototype.visitInterval = uc, oc.prototype.visitIntervalDayTime = uc, oc.prototype.visitIntervalYearMonth = uc, oc.prototype.visitFixedSizeList = uc, oc.prototype.visitMap = uc;
-        var cc = new oc,
-            lc = function(e) {
+        }, ic.prototype.visitBool = ac, ic.prototype.visitInt = ac, ic.prototype.visitInt8 = ac, ic.prototype.visitInt16 = ac, ic.prototype.visitInt32 = ac, ic.prototype.visitInt64 = ac, ic.prototype.visitUint8 = ac, ic.prototype.visitUint16 = ac, ic.prototype.visitUint32 = ac, ic.prototype.visitUint64 = ac, ic.prototype.visitFloat = ac, ic.prototype.visitFloat16 = ac, ic.prototype.visitFloat32 = ac, ic.prototype.visitFloat64 = ac, ic.prototype.visitUtf8 = ac, ic.prototype.visitBinary = ac, ic.prototype.visitFixedSizeBinary = ac, ic.prototype.visitDate = ac, ic.prototype.visitDateDay = ac, ic.prototype.visitDateMillisecond = ac, ic.prototype.visitTimestamp = ac, ic.prototype.visitTimestampSecond = ac, ic.prototype.visitTimestampMillisecond = ac, ic.prototype.visitTimestampMicrosecond = ac, ic.prototype.visitTimestampNanosecond = ac, ic.prototype.visitTime = ac, ic.prototype.visitTimeSecond = ac, ic.prototype.visitTimeMillisecond = ac, ic.prototype.visitTimeMicrosecond = ac, ic.prototype.visitTimeNanosecond = ac, ic.prototype.visitDecimal = ac, ic.prototype.visitList = ac, ic.prototype.visitStruct = ac, ic.prototype.visitUnion = ac, ic.prototype.visitDenseUnion = oc, ic.prototype.visitSparseUnion = oc, ic.prototype.visitDictionary = ac, ic.prototype.visitInterval = ac, ic.prototype.visitIntervalDayTime = ac, ic.prototype.visitIntervalYearMonth = ac, ic.prototype.visitFixedSizeList = ac, ic.prototype.visitMap = ac;
+        var uc = new ic,
+            sc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(dn);
+            }(ln);
 
-        function fc(e) {
+        function cc(e) {
             if (e.nullCount > 0) return function(e) {
-                var t = ac.getVisitFn(e);
-                return sn(e.nullBitmap, e.offset, e.length, e, (function(e, n, r, i) {
+                var t = rc.getVisitFn(e);
+                return an(e.nullBitmap, e.offset, e.length, e, (function(e, n, r, i) {
                     return 0 !== (r & 1 << i) ? t(e, n) : null
                 }))
             }(e);
             var t = e.type,
                 n = e.typeId,
                 r = e.length;
-            return 1 === e.stride && (n === $t.Timestamp || n === $t.Int && 64 !== t.bitWidth || n === $t.Time && 64 !== t.bitWidth || n === $t.Float && t.precision > 0) ? e.values.subarray(0, r)[Symbol.iterator]() : U().mark((function t(n) {
+            return 1 === e.stride && (n === Wt.Timestamp || n === Wt.Int && 64 !== t.bitWidth || n === Wt.Time && 64 !== t.bitWidth || n === Wt.Float && t.precision > 0) ? e.values.subarray(0, r)[Symbol.iterator]() : U().mark((function t(n) {
                 var i;
                 return U().wrap((function(t) {
                     for (;;) switch (t.prev = t.next) {
                         case 0:
                             i = -1;
                         case 1:
                             if (!(++i < r)) {
@@ -13251,51 +13264,51 @@
                             t.next = 1;
                             break;
                         case 6:
                         case "end":
                             return t.stop()
                     }
                 }), t)
-            }))(ac.getVisitFn(e))
+            }))(rc.getVisitFn(e))
         }
-        lc.prototype.visitNull = fc, lc.prototype.visitBool = fc, lc.prototype.visitInt = fc, lc.prototype.visitInt8 = fc, lc.prototype.visitInt16 = fc, lc.prototype.visitInt32 = fc, lc.prototype.visitInt64 = fc, lc.prototype.visitUint8 = fc, lc.prototype.visitUint16 = fc, lc.prototype.visitUint32 = fc, lc.prototype.visitUint64 = fc, lc.prototype.visitFloat = fc, lc.prototype.visitFloat16 = fc, lc.prototype.visitFloat32 = fc, lc.prototype.visitFloat64 = fc, lc.prototype.visitUtf8 = fc, lc.prototype.visitBinary = fc, lc.prototype.visitFixedSizeBinary = fc, lc.prototype.visitDate = fc, lc.prototype.visitDateDay = fc, lc.prototype.visitDateMillisecond = fc, lc.prototype.visitTimestamp = fc, lc.prototype.visitTimestampSecond = fc, lc.prototype.visitTimestampMillisecond = fc, lc.prototype.visitTimestampMicrosecond = fc, lc.prototype.visitTimestampNanosecond = fc, lc.prototype.visitTime = fc, lc.prototype.visitTimeSecond = fc, lc.prototype.visitTimeMillisecond = fc, lc.prototype.visitTimeMicrosecond = fc, lc.prototype.visitTimeNanosecond = fc, lc.prototype.visitDecimal = fc, lc.prototype.visitList = fc, lc.prototype.visitStruct = fc, lc.prototype.visitUnion = fc, lc.prototype.visitDenseUnion = fc, lc.prototype.visitSparseUnion = fc, lc.prototype.visitDictionary = fc, lc.prototype.visitInterval = fc, lc.prototype.visitIntervalDayTime = fc, lc.prototype.visitIntervalYearMonth = fc, lc.prototype.visitFixedSizeList = fc, lc.prototype.visitMap = fc;
-        var hc = new lc,
-            dc = function(e) {
+        sc.prototype.visitNull = cc, sc.prototype.visitBool = cc, sc.prototype.visitInt = cc, sc.prototype.visitInt8 = cc, sc.prototype.visitInt16 = cc, sc.prototype.visitInt32 = cc, sc.prototype.visitInt64 = cc, sc.prototype.visitUint8 = cc, sc.prototype.visitUint16 = cc, sc.prototype.visitUint32 = cc, sc.prototype.visitUint64 = cc, sc.prototype.visitFloat = cc, sc.prototype.visitFloat16 = cc, sc.prototype.visitFloat32 = cc, sc.prototype.visitFloat64 = cc, sc.prototype.visitUtf8 = cc, sc.prototype.visitBinary = cc, sc.prototype.visitFixedSizeBinary = cc, sc.prototype.visitDate = cc, sc.prototype.visitDateDay = cc, sc.prototype.visitDateMillisecond = cc, sc.prototype.visitTimestamp = cc, sc.prototype.visitTimestampSecond = cc, sc.prototype.visitTimestampMillisecond = cc, sc.prototype.visitTimestampMicrosecond = cc, sc.prototype.visitTimestampNanosecond = cc, sc.prototype.visitTime = cc, sc.prototype.visitTimeSecond = cc, sc.prototype.visitTimeMillisecond = cc, sc.prototype.visitTimeMicrosecond = cc, sc.prototype.visitTimeNanosecond = cc, sc.prototype.visitDecimal = cc, sc.prototype.visitList = cc, sc.prototype.visitStruct = cc, sc.prototype.visitUnion = cc, sc.prototype.visitDenseUnion = cc, sc.prototype.visitSparseUnion = cc, sc.prototype.visitDictionary = cc, sc.prototype.visitInterval = cc, sc.prototype.visitIntervalDayTime = cc, sc.prototype.visitIntervalYearMonth = cc, sc.prototype.visitFixedSizeList = cc, sc.prototype.visitMap = cc;
+        var lc = new sc,
+            fc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n)
-            }(dn);
+            }(ln);
 
-        function pc(e) {
+        function hc(e) {
             var t = e.type,
                 n = e.length,
                 r = e.stride;
             switch (t.typeId) {
-                case $t.Int:
-                case $t.Float:
-                case $t.Decimal:
-                case $t.Time:
-                case $t.Timestamp:
+                case Wt.Int:
+                case Wt.Float:
+                case Wt.Decimal:
+                case Wt.Time:
+                case Wt.Timestamp:
                     return e.values.subarray(0, n * r)
             }
-            return hn(hc.visit(e))
+            return cn(lc.visit(e))
         }
-        dc.prototype.visitNull = pc, dc.prototype.visitBool = pc, dc.prototype.visitInt = pc, dc.prototype.visitInt8 = pc, dc.prototype.visitInt16 = pc, dc.prototype.visitInt32 = pc, dc.prototype.visitInt64 = pc, dc.prototype.visitUint8 = pc, dc.prototype.visitUint16 = pc, dc.prototype.visitUint32 = pc, dc.prototype.visitUint64 = pc, dc.prototype.visitFloat = pc, dc.prototype.visitFloat16 = pc, dc.prototype.visitFloat32 = pc, dc.prototype.visitFloat64 = pc, dc.prototype.visitUtf8 = pc, dc.prototype.visitBinary = pc, dc.prototype.visitFixedSizeBinary = pc, dc.prototype.visitDate = pc, dc.prototype.visitDateDay = pc, dc.prototype.visitDateMillisecond = pc, dc.prototype.visitTimestamp = pc, dc.prototype.visitTimestampSecond = pc, dc.prototype.visitTimestampMillisecond = pc, dc.prototype.visitTimestampMicrosecond = pc, dc.prototype.visitTimestampNanosecond = pc, dc.prototype.visitTime = pc, dc.prototype.visitTimeSecond = pc, dc.prototype.visitTimeMillisecond = pc, dc.prototype.visitTimeMicrosecond = pc, dc.prototype.visitTimeNanosecond = pc, dc.prototype.visitDecimal = pc, dc.prototype.visitList = pc, dc.prototype.visitStruct = pc, dc.prototype.visitUnion = pc, dc.prototype.visitDenseUnion = pc, dc.prototype.visitSparseUnion = pc, dc.prototype.visitDictionary = pc, dc.prototype.visitInterval = pc, dc.prototype.visitIntervalDayTime = pc, dc.prototype.visitIntervalYearMonth = pc, dc.prototype.visitFixedSizeList = pc, dc.prototype.visitMap = pc;
-        var yc = new dc,
-            vc = function(e, t) {
+        fc.prototype.visitNull = hc, fc.prototype.visitBool = hc, fc.prototype.visitInt = hc, fc.prototype.visitInt8 = hc, fc.prototype.visitInt16 = hc, fc.prototype.visitInt32 = hc, fc.prototype.visitInt64 = hc, fc.prototype.visitUint8 = hc, fc.prototype.visitUint16 = hc, fc.prototype.visitUint32 = hc, fc.prototype.visitUint64 = hc, fc.prototype.visitFloat = hc, fc.prototype.visitFloat16 = hc, fc.prototype.visitFloat32 = hc, fc.prototype.visitFloat64 = hc, fc.prototype.visitUtf8 = hc, fc.prototype.visitBinary = hc, fc.prototype.visitFixedSizeBinary = hc, fc.prototype.visitDate = hc, fc.prototype.visitDateDay = hc, fc.prototype.visitDateMillisecond = hc, fc.prototype.visitTimestamp = hc, fc.prototype.visitTimestampSecond = hc, fc.prototype.visitTimestampMillisecond = hc, fc.prototype.visitTimestampMicrosecond = hc, fc.prototype.visitTimestampNanosecond = hc, fc.prototype.visitTime = hc, fc.prototype.visitTimeSecond = hc, fc.prototype.visitTimeMillisecond = hc, fc.prototype.visitTimeMicrosecond = hc, fc.prototype.visitTimeNanosecond = hc, fc.prototype.visitDecimal = hc, fc.prototype.visitList = hc, fc.prototype.visitStruct = hc, fc.prototype.visitUnion = hc, fc.prototype.visitDenseUnion = hc, fc.prototype.visitSparseUnion = hc, fc.prototype.visitDictionary = hc, fc.prototype.visitInterval = hc, fc.prototype.visitIntervalDayTime = hc, fc.prototype.visitIntervalYearMonth = hc, fc.prototype.visitFixedSizeList = hc, fc.prototype.visitMap = hc;
+        var dc = new fc,
+            pc = function(e, t) {
                 return e + t
             },
-            bc = function(e) {
+            yc = function(e) {
                 return "Cannot compute the byte width of variable-width column ".concat(e)
             },
-            mc = function(e) {
+            vc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -13312,20 +13325,20 @@
                     key: "visitFloat",
                     value: function(e) {
                         return e.ArrayType.BYTES_PER_ELEMENT
                     }
                 }, {
                     key: "visitBinary",
                     value: function(e) {
-                        throw new Error(bc(e))
+                        throw new Error(yc(e))
                     }
                 }, {
                     key: "visitUtf8",
                     value: function(e) {
-                        throw new Error(bc(e))
+                        throw new Error(yc(e))
                     }
                 }, {
                     key: "visitBool",
                     value: function(e) {
                         return 1 / 8
                     }
                 }, {
@@ -13342,50 +13355,50 @@
                     key: "visitTime",
                     value: function(e) {
                         return e.bitWidth / 8
                     }
                 }, {
                     key: "visitTimestamp",
                     value: function(e) {
-                        return e.unit === qt.SECOND ? 4 : 8
+                        return e.unit === $t.SECOND ? 4 : 8
                     }
                 }, {
                     key: "visitInterval",
                     value: function(e) {
                         return 4 * (e.unit + 1)
                     }
                 }, {
                     key: "visitList",
                     value: function(e) {
-                        throw new Error(bc(e))
+                        throw new Error(yc(e))
                     }
                 }, {
                     key: "visitStruct",
                     value: function(e) {
-                        return this.visitFields(e.children).reduce(vc, 0)
+                        return this.visitFields(e.children).reduce(pc, 0)
                     }
                 }, {
                     key: "visitUnion",
                     value: function(e) {
-                        return this.visitFields(e.children).reduce(vc, 0)
+                        return this.visitFields(e.children).reduce(pc, 0)
                     }
                 }, {
                     key: "visitFixedSizeBinary",
                     value: function(e) {
                         return e.byteWidth
                     }
                 }, {
                     key: "visitFixedSizeList",
                     value: function(e) {
-                        return e.listSize * this.visitFields(e.children).reduce(vc, 0)
+                        return e.listSize * this.visitFields(e.children).reduce(pc, 0)
                     }
                 }, {
                     key: "visitMap",
                     value: function(e) {
-                        return this.visitFields(e.children).reduce(vc, 0)
+                        return this.visitFields(e.children).reduce(pc, 0)
                     }
                 }, {
                     key: "visitDictionary",
                     value: function(e) {
                         return this.visit(e.indices)
                     }
                 }, {
@@ -13395,291 +13408,291 @@
                         return (e || []).map((function(e) {
                             return t.visit(e.type)
                         }))
                     }
                 }, {
                     key: "visitSchema",
                     value: function(e) {
-                        return this.visitFields(e.fields).reduce(vc, 0)
+                        return this.visitFields(e.fields).reduce(pc, 0)
                     }
                 }]), n
-            }(dn),
-            gc = new mc,
-            kc = function(e) {
+            }(ln),
+            bc = new vc,
+            mc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "visitNull",
                     value: function() {
-                        return gs
+                        return bs
                     }
                 }, {
                     key: "visitBool",
                     value: function() {
-                        return Vu
+                        return Pu
                     }
                 }, {
                     key: "visitInt",
                     value: function() {
-                        return as
+                        return rs
                     }
                 }, {
                     key: "visitInt8",
                     value: function() {
-                        return os
+                        return is
                     }
                 }, {
                     key: "visitInt16",
                     value: function() {
-                        return us
+                        return as
                     }
                 }, {
                     key: "visitInt32",
                     value: function() {
-                        return ss
+                        return os
                     }
                 }, {
                     key: "visitInt64",
                     value: function() {
-                        return cs
+                        return us
                     }
                 }, {
                     key: "visitUint8",
                     value: function() {
-                        return ls
+                        return ss
                     }
                 }, {
                     key: "visitUint16",
                     value: function() {
-                        return fs
+                        return cs
                     }
                 }, {
                     key: "visitUint32",
                     value: function() {
-                        return hs
+                        return ls
                     }
                 }, {
                     key: "visitUint64",
                     value: function() {
-                        return ds
+                        return fs
                     }
                 }, {
                     key: "visitFloat",
                     value: function() {
-                        return qu
+                        return Ku
                     }
                 }, {
                     key: "visitFloat16",
                     value: function() {
-                        return Gu
+                        return Qu
                     }
                 }, {
                     key: "visitFloat32",
                     value: function() {
-                        return Ju
+                        return qu
                     }
                 }, {
                     key: "visitFloat64",
                     value: function() {
-                        return Zu
+                        return Gu
                     }
                 }, {
                     key: "visitUtf8",
                     value: function() {
-                        return Cs
+                        return Ls
                     }
                 }, {
                     key: "visitBinary",
                     value: function() {
-                        return Ru
+                        return Uu
                     }
                 }, {
                     key: "visitFixedSizeBinary",
                     value: function() {
-                        return Ku
+                        return Hu
                     }
                 }, {
                     key: "visitDate",
                     value: function() {
-                        return zu
+                        return Ru
                     }
                 }, {
                     key: "visitDateDay",
                     value: function() {
-                        return Wu
+                        return Vu
                     }
                 }, {
                     key: "visitDateMillisecond",
                     value: function() {
-                        return Yu
+                        return zu
                     }
                 }, {
                     key: "visitTimestamp",
                     value: function() {
-                        return _s
+                        return ks
                     }
                 }, {
                     key: "visitTimestampSecond",
                     value: function() {
-                        return Os
+                        return ws
                     }
                 }, {
                     key: "visitTimestampMillisecond",
                     value: function() {
-                        return xs
+                        return _s
                     }
                 }, {
                     key: "visitTimestampMicrosecond",
                     value: function() {
-                        return js
+                        return Os
                     }
                 }, {
                     key: "visitTimestampNanosecond",
                     value: function() {
-                        return Ss
+                        return js
                     }
                 }, {
                     key: "visitTime",
                     value: function() {
-                        return Ts
+                        return xs
                     }
                 }, {
                     key: "visitTimeSecond",
                     value: function() {
-                        return Is
+                        return Ss
                     }
                 }, {
                     key: "visitTimeMillisecond",
                     value: function() {
-                        return Es
+                        return Ts
                     }
                 }, {
                     key: "visitTimeMicrosecond",
                     value: function() {
-                        return As
+                        return Is
                     }
                 }, {
                     key: "visitTimeNanosecond",
                     value: function() {
-                        return Bs
+                        return Es
                     }
                 }, {
                     key: "visitDecimal",
                     value: function() {
-                        return Hu
+                        return Wu
                     }
                 }, {
                     key: "visitList",
                     value: function() {
-                        return bs
+                        return ys
                     }
                 }, {
                     key: "visitStruct",
                     value: function() {
-                        return ws
+                        return gs
                     }
                 }, {
                     key: "visitUnion",
                     value: function() {
-                        return Ds
+                        return As
                     }
                 }, {
                     key: "visitDenseUnion",
                     value: function() {
-                        return Ls
+                        return Bs
                     }
                 }, {
                     key: "visitSparseUnion",
                     value: function() {
-                        return Fs
+                        return Ds
                     }
                 }, {
                     key: "visitDictionary",
                     value: function() {
-                        return $u
+                        return Yu
                     }
                 }, {
                     key: "visitInterval",
                     value: function() {
-                        return ns
+                        return es
                     }
                 }, {
                     key: "visitIntervalDayTime",
                     value: function() {
-                        return rs
+                        return ts
                     }
                 }, {
                     key: "visitIntervalYearMonth",
                     value: function() {
-                        return is
+                        return ns
                     }
                 }, {
                     key: "visitFixedSizeList",
                     value: function() {
-                        return Qu
+                        return $u
                     }
                 }, {
                     key: "visitMap",
                     value: function() {
-                        return ms
+                        return vs
                     }
                 }]), n
-            }(dn),
-            wc = new kc,
-            _c = ["values"];
+            }(ln),
+            gc = new mc,
+            kc = ["values"];
 
-        function Oc(e, t) {
-            if (Te(t)) return Ht.from({
+        function wc(e, t) {
+            if (Te(t)) return zt.from({
                 nullValues: [null, void 0],
                 type: e(),
                 values: t
             });
-            if (Ie(t)) return Ht.from({
+            if (Ie(t)) return zt.from({
                 nullValues: [null, void 0],
                 type: e(),
                 values: t
             });
-            var n = Mt({}, t),
+            var n = Object(Lt.a)({}, t),
                 r = n.values,
                 i = void 0 === r ? [] : r,
                 a = n.type,
                 o = void 0 === a ? e() : a,
                 u = n.nullValues,
                 s = void 0 === u ? [null, void 0] : u;
-            return Te(i), Ht.from(Mt(Mt({
+            return Te(i), zt.from(Object(Lt.a)(Object(Lt.a)({
                 nullValues: s
             }, t), {}, {
                 type: o
             }))
         }
-        Ht.new = function(e) {
+        zt.new = function(e) {
             for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
-            return Pr(wc.getVisitFn(e)(), [e].concat(n))
-        }, Ht.from = function(e) {
-            var t = Mt({
+            return Mr(gc.getVisitFn(e)(), [e].concat(n))
+        }, zt.from = function(e) {
+            var t = Object(Lt.a)({
                     nullValues: [null, void 0]
                 }, e),
                 n = t.values,
                 r = void 0 === n ? [] : n,
-                i = Uu(t, _c);
+                i = Mu(t, kc);
             if (Te(r)) {
-                var a = hn(mr.throughIterable(i)(r));
-                return 1 === a.length ? a[0] : Wi.concat(a)
+                var a = cn(yr.throughIterable(i)(r));
+                return 1 === a.length ? a[0] : Vi.concat(a)
             }
             return function() {
                 var e = F(U().mark((function e(t) {
                     var n, a, o, u, s, c, l;
                     return U().wrap((function(e) {
                         for (;;) switch (e.prev = e.next) {
                             case 0:
-                                n = mr.throughAsyncIterable(i), a = !1, o = !1, e.prev = 3, s = H(n(r));
+                                n = yr.throughAsyncIterable(i), a = !1, o = !1, e.prev = 3, s = H(n(r));
                             case 5:
                                 return e.next = 7, s.next();
                             case 7:
                                 if (!(a = !(c = e.sent).done)) {
                                     e.next = 13;
                                     break
                                 }
@@ -13705,78 +13718,78 @@
                                 }
                                 throw u;
                             case 27:
                                 return e.finish(24);
                             case 28:
                                 return e.finish(19);
                             case 29:
-                                return e.abrupt("return", 1 === t.length ? t[0] : Wi.concat(t));
+                                return e.abrupt("return", 1 === t.length ? t[0] : Vi.concat(t));
                             case 30:
                             case "end":
                                 return e.stop()
                         }
                     }), e, null, [
                         [3, 15, 19, 29],
                         [20, , 24, 28]
                     ])
                 })));
                 return function(t) {
                     return e.apply(this, arguments)
                 }
             }()([])
-        }, Pu.prototype.get = function(e) {
-            return ac.visit(this, e)
-        }, Pu.prototype.set = function(e, t) {
-            return Ma.visit(this, e, t)
-        }, Pu.prototype.indexOf = function(e, t) {
-            return cc.visit(this, e, t)
-        }, Pu.prototype.toArray = function() {
-            return yc.visit(this)
-        }, Pu.prototype.getByteWidth = function() {
-            return gc.visit(this.type)
-        }, Pu.prototype[Symbol.iterator] = function() {
-            return hc.visit(this)
-        }, Pu.prototype._bindDataAccessors = function() {
+        }, Nu.prototype.get = function(e) {
+            return rc.visit(this, e)
+        }, Nu.prototype.set = function(e, t) {
+            return Fa.visit(this, e, t)
+        }, Nu.prototype.indexOf = function(e, t) {
+            return uc.visit(this, e, t)
+        }, Nu.prototype.toArray = function() {
+            return dc.visit(this)
+        }, Nu.prototype.getByteWidth = function() {
+            return bc.visit(this.type)
+        }, Nu.prototype[Symbol.iterator] = function() {
+            return lc.visit(this)
+        }, Nu.prototype._bindDataAccessors = function() {
             var e = this.nullBitmap;
             e && e.byteLength > 0 && (this.get = (t = this.get, function(e) {
                 return this.isValid(e) ? t.call(this, e) : null
             }), this.set = function(e) {
                 return function(t, n) {
-                    an(this.nullBitmap, this.offset + t, !(null === n || void 0 === n)) && e.call(this, t, n)
+                    tn(this.nullBitmap, this.offset + t, !(null === n || void 0 === n)) && e.call(this, t, n)
                 }
             }(this.set));
             var t
-        }, Object.keys($t).map((function(e) {
-            return $t[e]
+        }, Object.keys(Wt).map((function(e) {
+            return Wt[e]
         })).filter((function(e) {
             return "number" === typeof e
         })).filter((function(e) {
-            return e !== $t.NONE
+            return e !== Wt.NONE
         })).forEach((function(e) {
-            var t, n = wc.visit(e);
-            n.prototype.get = (t = ac.getVisitFn(e), function(e) {
+            var t, n = gc.visit(e);
+            n.prototype.get = (t = rc.getVisitFn(e), function(e) {
                 return t(this, e)
-            }), n.prototype.set = Ns(Ma.getVisitFn(e)), n.prototype.indexOf = Ns(cc.getVisitFn(e)), n.prototype.toArray = Ms(yc.getVisitFn(e)), n.prototype.getByteWidth = function(e) {
+            }), n.prototype.set = Cs(Fa.getVisitFn(e)), n.prototype.indexOf = Cs(uc.getVisitFn(e)), n.prototype.toArray = Fs(dc.getVisitFn(e)), n.prototype.getByteWidth = function(e) {
                 return function() {
                     return e(this.type)
                 }
-            }(gc.getVisitFn(e)), n.prototype[Symbol.iterator] = Ms(hc.getVisitFn(e))
+            }(bc.getVisitFn(e)), n.prototype[Symbol.iterator] = Fs(lc.getVisitFn(e))
         }));
-        var xc = function(e) {
+        var _c = function(e) {
             Object(ce.a)(n, e);
             var t = Object(le.a)(n);
 
             function n() {
                 var e;
                 Object(C.a)(this, n);
                 for (var r = null, i = arguments.length, a = new Array(i), o = 0; o < i; o++) a[o] = arguments[o];
-                a[0] instanceof ia && (r = a.shift());
-                var u = qi(jc, a);
+                a[0] instanceof na && (r = a.shift());
+                var u = Ki(Oc, a);
                 if (!r && !(r = u[0] && u[0].schema)) throw new TypeError("Table must be initialized with a Schema or at least one RecordBatch");
-                return u[0] || (u[0] = new Sc(r)), (e = t.call(this, new Xn(r.fields), u))._schema = r, e._chunks = u, e
+                return u[0] || (u[0] = new jc(r)), (e = t.call(this, new Gn(r.fields), u))._schema = r, e._chunks = u, e
             }
             return Object(M.a)(n, [{
                 key: "schema",
                 get: function() {
                     return this._schema
                 }
             }, {
@@ -13826,49 +13839,49 @@
                     if (n = i[e]) return n;
                     if (t = r[e]) {
                         var a = this._chunks.map((function(t) {
                             return t.getChildAt(e)
                         })).filter((function(e) {
                             return null != e
                         }));
-                        if (a.length > 0) return i[e] = new $i(t, a)
+                        if (a.length > 0) return i[e] = new Yi(t, a)
                     }
                     return null
                 }
             }, {
                 key: "serialize",
                 value: function() {
-                    return (!(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1] ? Eu : Au).writeAll(this).toUint8Array(!0)
+                    return (!(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1] ? Tu : Iu).writeAll(this).toUint8Array(!0)
                 }
             }, {
                 key: "count",
                 value: function() {
                     return this._length
                 }
             }, {
                 key: "select",
                 value: function() {
                     for (var e = this._schema.fields.reduce((function(e, t, n) {
                             return e.set(t.name, n)
                         }), new Map), t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
-                    return this.selectAt.apply(this, hn(n.map((function(t) {
+                    return this.selectAt.apply(this, cn(n.map((function(t) {
                         return e.get(t)
                     })).filter((function(e) {
                         return e > -1
                     }))))
                 }
             }, {
                 key: "selectAt",
                 value: function() {
                     for (var e, t = arguments.length, r = new Array(t), i = 0; i < t; i++) r[i] = arguments[i];
                     var a = (e = this._schema).selectAt.apply(e, r);
                     return new n(a, this._chunks.map((function(e) {
                         var t = e.length,
                             n = e.data.childData;
-                        return new jc(a, t, r.map((function(e) {
+                        return new Oc(a, t, r.map((function(e) {
                             return n[e]
                         })).filter(Boolean))
                     })))
                 }
             }, {
                 key: "assign",
                 value: function(e) {
@@ -13886,61 +13899,61 @@
                             [],
                             []
                         ]),
                         a = P(i, 2),
                         o = a[0],
                         u = a[1],
                         s = this._schema.assign(e.schema),
-                        c = [].concat(hn(r.map((function(n, r, i) {
+                        c = [].concat(cn(r.map((function(n, r, i) {
                             var a = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : u[r];
                             return void 0 === a ? t.getColumnAt(r) : e.getColumnAt(a)
-                        }))), hn(o.map((function(t) {
+                        }))), cn(o.map((function(t) {
                             return e.getColumnAt(t)
                         })))).filter(Boolean);
-                    return Pr(n, hn(Mu(s, c)))
+                    return Mr(n, cn(Fu(s, c)))
                 }
             }], [{
                 key: "empty",
                 value: function() {
-                    return new n(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : new ia([]), [])
+                    return new n(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : new na([]), [])
                 }
             }, {
                 key: "from",
                 value: function(e) {
                     if (!e) return n.empty();
                     if ("object" === typeof e) {
                         var t = Te(e.values) ? function(e) {
                             var t = e.type;
-                            if (t instanceof Xn) return xc.fromStruct(ws.from(e));
+                            if (t instanceof Gn) return _c.fromStruct(gs.from(e));
                             return null
                         }(e) : Ie(e.values) ? function(e) {
                             var t = e.type;
-                            if (t instanceof Xn) return ws.from(e).then((function(e) {
-                                return xc.fromStruct(e)
+                            if (t instanceof Gn) return gs.from(e).then((function(e) {
+                                return _c.fromStruct(e)
                             }));
                             return null
                         }(e) : null;
                         if (null !== t) return t
                     }
-                    var r = Ec.from(e);
+                    var r = Tc.from(e);
                     return Se(r) ? F(U().mark((function e() {
                         return U().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
                                     return e.t0 = n, e.next = 3, r;
                                 case 3:
                                     return e.t1 = e.sent, e.next = 6, e.t0.from.call(e.t0, e.t1);
                                 case 6:
                                     return e.abrupt("return", e.sent);
                                 case 7:
                                 case "end":
                                     return e.stop()
                             }
                         }), e)
-                    })))() : r.isSync() && (r = r.open()) ? r.schema ? new n(r.schema, hn(r)) : n.empty() : function() {
+                    })))() : r.isSync() && (r = r.open()) ? r.schema ? new n(r.schema, cn(r)) : n.empty() : function() {
                         var e = F(U().mark((function e(t) {
                             var r, i, a, o, u, s, c, l, f;
                             return U().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.next = 2, t;
                                     case 2:
@@ -14024,61 +14037,61 @@
                 value: function(e) {
                     return n.new(e.data.childData, e.type.children)
                 }
             }, {
                 key: "new",
                 value: function() {
                     for (var e = arguments.length, t = new Array(e), r = 0; r < e; r++) t[r] = arguments[r];
-                    return Pr(n, hn((i = function(e) {
-                        var t = P(ra(e, [
+                    return Mr(n, cn((i = function(e) {
+                        var t = P(ta(e, [
                                 [],
                                 []
                             ]), 2),
                             n = t[0];
                         return t[1].map((function(e, t) {
-                            return e instanceof $i ? $i.new(e.field.clone(n[t]), e) : e instanceof Ht ? $i.new(n[t], e) : $i.new(n[t], [])
+                            return e instanceof Yi ? Yi.new(e.field.clone(n[t]), e) : e instanceof zt ? Yi.new(n[t], e) : Yi.new(n[t], [])
                         }))
-                    }(t), Mu(new ia(i.map((function(e) {
+                    }(t), Fu(new na(i.map((function(e) {
                         return e.field
                     }))), i))));
                     var i
                 }
             }]), n
-        }(Wi);
-        var jc = function(e) {
+        }(Vi);
+        var Oc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e, r;
                     Object(C.a)(this, n);
                     for (var i = arguments.length, a = new Array(i), o = 0; o < i; o++) a[o] = arguments[o];
                     var u, s = a[0];
-                    if (a[1] instanceof sr) r = a[1], u = a[2];
+                    if (a[1] instanceof ar) r = a[1], u = a[2];
                     else {
                         var c = s.fields,
                             l = a[1],
                             f = a[2];
-                        r = sr.Struct(new Xn(c), 0, l, 0, null, f)
+                        r = ar.Struct(new Gn(c), 0, l, 0, null, f)
                     }
                     return (e = t.call(this, r, u))._schema = s, e
                 }
                 return Object(M.a)(n, [{
                     key: "clone",
                     value: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this._children;
                         return new n(this._schema, e, t)
                     }
                 }, {
                     key: "concat",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), r = 0; r < e; r++) t[r] = arguments[r];
                         var i = this._schema,
-                            a = Wi.flatten.apply(Wi, [this].concat(t));
-                        return new xc(i, a.map((function(e) {
+                            a = Vi.flatten.apply(Vi, [this].concat(t));
+                        return new _c(i, a.map((function(e) {
                             var t = e.data;
                             return new n(i, t)
                         })))
                     }
                 }, {
                     key: "schema",
                     get: function() {
@@ -14088,23 +14101,23 @@
                     key: "numCols",
                     get: function() {
                         return this._schema.fields.length
                     }
                 }, {
                     key: "dictionaries",
                     get: function() {
-                        return this._dictionaries || (this._dictionaries = Tc.collect(this))
+                        return this._dictionaries || (this._dictionaries = xc.collect(this))
                     }
                 }, {
                     key: "select",
                     value: function() {
                         for (var e = this._schema.fields.reduce((function(e, t, n) {
                                 return e.set(t.name, n)
                             }), new Map), t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
-                        return this.selectAt.apply(this, hn(n.map((function(t) {
+                        return this.selectAt.apply(this, cn(n.map((function(t) {
                             return e.get(t)
                         })).filter((function(e) {
                             return e > -1
                         }))))
                     }
                 }, {
                     key: "selectAt",
@@ -14115,80 +14128,80 @@
                                 return t.data.childData[e]
                             })).filter(Boolean);
                         return new n(o, this.length, u)
                     }
                 }], [{
                     key: "from",
                     value: function(e) {
-                        return Te(e.values), xc.from(e)
+                        return Te(e.values), _c.from(e)
                     }
                 }, {
                     key: "new",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), r = 0; r < e; r++) t[r] = arguments[r];
-                        var i = P(Gi(t), 2),
+                        var i = P(Qi(t), 2),
                             a = i[0],
                             o = i[1].filter((function(e) {
-                                return e instanceof Ht
+                                return e instanceof zt
                             }));
-                        return Pr(n, hn(function(e, t) {
+                        return Mr(n, cn(function(e, t) {
                             for (var n, r, i = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : t.reduce((function(e, t) {
                                     return Math.max(e, t.length)
-                                }), 0), a = -1, o = t.length, u = hn(e.fields), s = [], c = (i + 63 & -64) >> 3; ++a < o;)(n = t[a]) && n.length === i ? s[a] = n : ((r = u[a]).nullable || (u[a] = u[a].clone({
+                                }), 0), a = -1, o = t.length, u = cn(e.fields), s = [], c = (i + 63 & -64) >> 3; ++a < o;)(n = t[a]) && n.length === i ? s[a] = n : ((r = u[a]).nullable || (u[a] = u[a].clone({
                                 nullable: !0
-                            })), s[a] = n ? n._changeLengthAndBackfillNullBitmap(i) : sr.new(r.type, 0, i, i, Cu(c)));
-                            return [new ia(u), i, s]
-                        }(new ia(a), o.map((function(e) {
+                            })), s[a] = n ? n._changeLengthAndBackfillNullBitmap(i) : ar.new(r.type, 0, i, i, Lu(c)));
+                            return [new na(u), i, s]
+                        }(new na(a), o.map((function(e) {
                             return e.data
                         })))))
                     }
                 }]), n
-            }(ws),
-            Sc = function(e) {
+            }(gs),
+            jc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     return Object(C.a)(this, n), t.call(this, e, 0, e.fields.map((function(e) {
-                        return sr.new(e.type, 0, 0, 0)
+                        return ar.new(e.type, 0, 0, 0)
                     })))
                 }
                 return Object(M.a)(n)
-            }(jc),
-            Tc = function(e) {
+            }(Oc),
+            xc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e;
                     return Object(C.a)(this, n), (e = t.apply(this, arguments)).dictionaries = new Map, e
                 }
                 return Object(M.a)(n, [{
                     key: "visit",
                     value: function(e, t) {
                         var n = this;
-                        return Tn.isDictionary(t) ? this.visitDictionary(e, t) : (e.childData.forEach((function(e, r) {
+                        return jn.isDictionary(t) ? this.visitDictionary(e, t) : (e.childData.forEach((function(e, r) {
                             return n.visit(e, t.children[r].type)
                         })), this)
                     }
                 }, {
                     key: "visitDictionary",
                     value: function(e, t) {
                         var n = e.dictionary;
                         return n && n.length > 0 && this.dictionaries.set(t.id, n), this
                     }
                 }], [{
                     key: "collect",
                     value: function(e) {
-                        return (new n).visit(e.data, new Xn(e.schema.fields)).dictionaries
+                        return (new n).visit(e.data, new Gn(e.schema.fields)).dictionaries
                     }
                 }]), n
-            }(dn),
-            Ic = U().mark(Vc),
-            Ec = function(e, t, n) {
+            }(ln),
+            Sc = U().mark(Pc),
+            Tc = function(e, t, n) {
                 Object(ce.a)(i, e);
                 var r = Object(le.a)(i);
 
                 function i(e) {
                     var t;
                     return Object(C.a)(this, i), (t = r.call(this))._impl = e, t
                 }
@@ -14296,27 +14309,27 @@
                     value: function() {
                         return this._impl[Symbol.asyncIterator]()
                     }
                 }, {
                     key: "toDOMStream",
                     value: function() {
                         var e = this;
-                        return Ot.toDOMStream(this.isSync() ? Ft({}, Symbol.iterator, (function() {
+                        return Ot.toDOMStream(this.isSync() ? Object(_i.a)({}, Symbol.iterator, (function() {
                             return e
-                        })) : Ft({}, Symbol.asyncIterator, (function() {
+                        })) : Object(_i.a)({}, Symbol.asyncIterator, (function() {
                             return e
                         })))
                     }
                 }, {
                     key: "toNodeStream",
                     value: function() {
                         var e = this;
-                        return Ot.toNodeStream(this.isSync() ? Ft({}, Symbol.iterator, (function() {
+                        return Ot.toNodeStream(this.isSync() ? Object(_i.a)({}, Symbol.iterator, (function() {
                             return e
-                        })) : Ft({}, Symbol.asyncIterator, (function() {
+                        })) : Object(_i.a)({}, Symbol.asyncIterator, (function() {
                             return e
                         })), {
                             objectMode: !0
                         })
                     }
                 }], [{
                     key: "throughNode",
@@ -14328,17 +14341,17 @@
                     value: function(e, t) {
                         throw new Error('"throughDOM" not available in this environment')
                     }
                 }, {
                     key: "from",
                     value: function(e) {
                         return e instanceof i ? e : Ee(e) ? function(e) {
-                            return new Ac(new Pc(e))
+                            return new Ic(new Nc(e))
                         }(e) : Be(e) ? function(e) {
-                            return Hc.apply(this, arguments)
+                            return Wc.apply(this, arguments)
                         }(e) : Se(e) ? F(U().mark((function t() {
                             return U().wrap((function(t) {
                                 for (;;) switch (t.prev = t.next) {
                                     case 0:
                                         return t.t0 = i, t.next = 3, e;
                                     case 3:
                                         return t.t1 = t.sent, t.next = 6, t.t0.from.call(t.t0, t.t1);
@@ -14346,36 +14359,36 @@
                                         return t.abrupt("return", t.sent);
                                     case 7:
                                     case "end":
                                         return t.stop()
                                 }
                             }), t)
                         })))() : De(e) || Le(e) || Fe(e) || Ie(e) ? function(e) {
-                            return Yc.apply(this, arguments)
-                        }(new qa(e)) : function(e) {
-                            var t = e.peek(gu + 7 & -8);
-                            return t && t.byteLength >= 4 ? mu(t) ? new Dc(new Nc(e.read())) : new Ac(new Cc(e)) : new Ac(new Cc(U().mark((function e() {
+                            return zc.apply(this, arguments)
+                        }(new Ka(e)) : function(e) {
+                            var t = e.peek(bu + 7 & -8);
+                            return t && t.byteLength >= 4 ? vu(t) ? new Ac(new Cc(e.read())) : new Ic(new Lc(e)) : new Ic(new Lc(U().mark((function e() {
                                 return U().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
                                         case "end":
                                             return e.stop()
                                     }
                                 }), e)
                             }))()))
-                        }(new Qa(e))
+                        }(new $a(e))
                     }
                 }, {
                     key: "readAll",
                     value: function(e) {
-                        return e instanceof i ? e.isSync() ? Vc(e) : zc(e) : Ee(e) || ArrayBuffer.isView(e) || Te(e) || Ae(e) ? Vc(e) : zc(e)
+                        return e instanceof i ? e.isSync() ? Pc(e) : Rc(e) : Ee(e) || ArrayBuffer.isView(e) || Te(e) || Ae(e) ? Pc(e) : Rc(e)
                     }
                 }]), i
             }(de, Symbol.iterator, Symbol.asyncIterator),
-            Ac = function(e, t, n) {
+            Ic = function(e, t, n) {
                 Object(ce.a)(i, e);
                 var r = Object(le.a)(i);
 
                 function i(e) {
                     var t;
                     return Object(C.a)(this, i), (t = r.call(this, e))._impl = e, t
                 }
@@ -14397,16 +14410,16 @@
                                     case "end":
                                         return t.stop()
                                 }
                             }), t)
                         })))()
                     }
                 }]), i
-            }(Ec, Symbol.iterator, Symbol.asyncIterator),
-            Bc = function(e, t, n) {
+            }(Tc, Symbol.iterator, Symbol.asyncIterator),
+            Ec = function(e, t, n) {
                 Object(ce.a)(i, e);
                 var r = Object(le.a)(i);
 
                 function i(e) {
                     var t;
                     return Object(C.a)(this, i), (t = r.call(this, e))._impl = e, t
                 }
@@ -14417,36 +14430,36 @@
                     }
                 }, {
                     key: n,
                     value: function() {
                         return this._impl[Symbol.asyncIterator]()
                     }
                 }]), i
-            }(Ec, Symbol.iterator, Symbol.asyncIterator),
-            Dc = function(e) {
+            }(Tc, Symbol.iterator, Symbol.asyncIterator),
+            Ac = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
                     return Object(C.a)(this, n), (r = t.call(this, e))._impl = e, r
                 }
                 return Object(M.a)(n)
-            }(Ac),
-            Lc = function(e) {
+            }(Ic),
+            Bc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
                     return Object(C.a)(this, n), (r = t.call(this, e))._impl = e, r
                 }
                 return Object(M.a)(n)
-            }(Bc),
-            Fc = function() {
+            }(Ec),
+            Dc = function() {
                 function e() {
                     var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : new Map;
                     Object(C.a)(this, e), this.closed = !1, this.autoDestroy = !0, this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.dictionaries = t
                 }
                 return Object(M.a)(e, [{
                     key: "numDictionaries",
                     get: function() {
@@ -14481,45 +14494,45 @@
                     key: "reset",
                     value: function(e) {
                         return this._dictionaryIndex = 0, this._recordBatchIndex = 0, this.schema = e, this.dictionaries = new Map, this
                     }
                 }, {
                     key: "_loadRecordBatch",
                     value: function(e, t) {
-                        return new jc(this.schema, e.length, this._loadVectors(e, t, this.schema.fields))
+                        return new Oc(this.schema, e.length, this._loadVectors(e, t, this.schema.fields))
                     }
                 }, {
                     key: "_loadDictionaryBatch",
                     value: function(e, t) {
                         var n = e.id,
                             r = e.isDelta,
                             i = e.data,
                             a = this.dictionaries,
                             o = this.schema,
                             u = a.get(n);
                         if (r || !u) {
                             var s = o.dictionaries.get(n);
-                            return u && r ? u.concat(Ht.new(this._loadVectors(i, t, [s])[0])) : Ht.new(this._loadVectors(i, t, [s])[0])
+                            return u && r ? u.concat(zt.new(this._loadVectors(i, t, [s])[0])) : zt.new(this._loadVectors(i, t, [s])[0])
                         }
                         return u
                     }
                 }, {
                     key: "_loadVectors",
                     value: function(e, t, n) {
-                        return new oo(t, e.nodes, e.buffers, this.dictionaries).visitMany(n)
+                        return new io(t, e.nodes, e.buffers, this.dictionaries).visitMany(n)
                     }
                 }]), e
             }(),
-            Cc = function(e, t) {
+            Lc = function(e, t) {
                 Object(ce.a)(r, e);
                 var n = Object(le.a)(r);
 
                 function r(e, t) {
                     var i;
-                    return Object(C.a)(this, r), (i = n.call(this, t))._reader = Ee(e) ? new du(i._handle = e) : new fu(i._handle = e), i
+                    return Object(C.a)(this, r), (i = n.call(this, t))._reader = Ee(e) ? new fu(i._handle = e) : new cu(i._handle = e), i
                 }
                 return Object(M.a)(r, [{
                     key: "isSync",
                     value: function() {
                         return !0
                     }
                 }, {
@@ -14536,15 +14549,15 @@
                     key: "cancel",
                     value: function() {
                         !this.closed && (this.closed = !0) && (this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
                     }
                 }, {
                     key: "open",
                     value: function(e) {
-                        return this.closed || (this.autoDestroy = Rc(this, e), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
+                        return this.closed || (this.autoDestroy = Uc(this, e), this.schema || (this.schema = this._reader.readSchema()) || this.cancel()), this
                     }
                 }, {
                     key: "throw",
                     value: function(e) {
                         return !this.closed && this.autoDestroy && (this.closed = !0) ? this.reset()._reader.throw(e) : fe
                     }
                 }, {
@@ -14573,31 +14586,31 @@
                                     var i = e.header(),
                                         a = t.readMessageBody(e.bodyLength),
                                         o = this._loadDictionaryBatch(i, a);
                                     this.dictionaries.set(i.id, o)
                                 }
                             } return this.schema && 0 === this._recordBatchIndex ? (this._recordBatchIndex++, {
                             done: !1,
-                            value: new Sc(this.schema)
+                            value: new jc(this.schema)
                         }) : this.return()
                     }
                 }, {
                     key: "_readNextMessageAndValidate",
                     value: function(e) {
                         return this._reader.readMessage(e)
                     }
                 }]), r
-            }(Fc, Symbol.iterator),
-            Mc = function(e, t) {
+            }(Dc, Symbol.iterator),
+            Fc = function(e, t) {
                 Object(ce.a)(r, e);
                 var n = Object(le.a)(r);
 
                 function r(e, t) {
                     var i;
-                    return Object(C.a)(this, r), (i = n.call(this, t))._reader = new hu(i._handle = e), i
+                    return Object(C.a)(this, r), (i = n.call(this, t))._reader = new lu(i._handle = e), i
                 }
                 return Object(M.a)(r, [{
                     key: "isAsync",
                     value: function() {
                         return !0
                     }
                 }, {
@@ -14641,15 +14654,15 @@
                             return U().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         if (this.closed) {
                                             e.next = 10;
                                             break
                                         }
-                                        if (this.autoDestroy = Rc(this, t), e.t0 = this.schema, e.t0) {
+                                        if (this.autoDestroy = Uc(this, t), e.t0 = this.schema, e.t0) {
                                             e.next = 7;
                                             break
                                         }
                                         return e.next = 6, this._reader.readSchema();
                                     case 6:
                                         e.t0 = this.schema = e.sent;
                                     case 7:
@@ -14777,15 +14790,15 @@
                                     case 31:
                                         if (!this.schema || 0 !== this._recordBatchIndex) {
                                             e.next = 34;
                                             break
                                         }
                                         return this._recordBatchIndex++, e.abrupt("return", {
                                             done: !1,
-                                            value: new Sc(this.schema)
+                                            value: new jc(this.schema)
                                         });
                                     case 34:
                                         return e.next = 36, this.return();
                                     case 36:
                                         return e.abrupt("return", e.sent);
                                     case 37:
                                     case "end":
@@ -14814,21 +14827,21 @@
                             }), e, this)
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 }]), r
-            }(Fc, Symbol.asyncIterator),
-            Nc = function(e) {
+            }(Dc, Symbol.asyncIterator),
+            Cc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
-                    return Object(C.a)(this, n), t.call(this, e instanceof Za ? e : new Za(e), r)
+                    return Object(C.a)(this, n), t.call(this, e instanceof Ga ? e : new Ga(e), r)
                 }
                 return Object(M.a)(n, [{
                     key: "footer",
                     get: function() {
                         return this._footer
                     }
                 }, {
@@ -14863,76 +14876,76 @@
                                 }
                             } catch (i) {
                                 r.e(i)
                             } finally {
                                 r.f()
                             }
                         }
-                        return Ut(Object(Nt.a)(n.prototype), "open", this).call(this, e)
+                        return Ct(Object(Ft.a)(n.prototype), "open", this).call(this, e)
                     }
                 }, {
                     key: "readRecordBatch",
                     value: function(e) {
                         if (this.closed) return null;
                         this._footer || this.open();
                         var t = this._footer && this._footer.getRecordBatch(e);
                         if (t && this._handle.seek(t.offset)) {
-                            var n = this._reader.readMessage(Xt.RecordBatch);
+                            var n = this._reader.readMessage(Gt.RecordBatch);
                             if (n && n.isRecordBatch()) {
                                 var r = n.header(),
                                     i = this._reader.readMessageBody(n.bodyLength);
                                 return this._loadRecordBatch(r, i)
                             }
                         }
                         return null
                     }
                 }, {
                     key: "_readDictionaryBatch",
                     value: function(e) {
                         var t = this._footer && this._footer.getDictionaryBatch(e);
                         if (t && this._handle.seek(t.offset)) {
-                            var n = this._reader.readMessage(Xt.DictionaryBatch);
+                            var n = this._reader.readMessage(Gt.DictionaryBatch);
                             if (n && n.isDictionaryBatch()) {
                                 var r = n.header(),
                                     i = this._reader.readMessageBody(n.bodyLength),
                                     a = this._loadDictionaryBatch(r, i);
                                 this.dictionaries.set(r.id, a)
                             }
                         }
                     }
                 }, {
                     key: "_readFooter",
                     value: function() {
                         var e = this._handle,
-                            t = e.size - ku,
+                            t = e.size - mu,
                             n = e.readInt32(t),
                             r = e.readAt(t - n, n);
-                        return Ya.decode(r)
+                        return za.decode(r)
                     }
                 }, {
                     key: "_readNextMessageAndValidate",
                     value: function(e) {
                         if (this._footer || this.open(), this._footer && this._recordBatchIndex < this.numRecordBatches) {
                             var t = this._footer && this._footer.getRecordBatch(this._recordBatchIndex);
                             if (t && this._handle.seek(t.offset)) return this._reader.readMessage(e)
                         }
                         return null
                     }
                 }]), n
-            }(Cc),
-            Uc = function(e) {
+            }(Lc),
+            Mc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     Object(C.a)(this, n);
                     for (var r = arguments.length, i = new Array(r > 1 ? r - 1 : 0), a = 1; a < r; a++) i[a - 1] = arguments[a];
                     var o = "number" !== typeof i[0] ? i.shift() : void 0,
                         u = i[0] instanceof Map ? i.shift() : void 0;
-                    return t.call(this, e instanceof Xa ? e : new Xa(e, o), u)
+                    return t.call(this, e instanceof Ja ? e : new Ja(e, o), u)
                 }
                 return Object(M.a)(n, [{
                     key: "footer",
                     get: function() {
                         return this._footer
                     }
                 }, {
@@ -14987,15 +15000,15 @@
                                         e.next = 20;
                                         break;
                                     case 17:
                                         e.prev = 17, e.t1 = e.catch(5), r.e(e.t1);
                                     case 20:
                                         return e.prev = 20, r.f(), e.finish(20);
                                     case 23:
-                                        return e.next = 25, Ut(Object(Nt.a)(n.prototype), "open", this).call(this, t);
+                                        return e.next = 25, Ct(Object(Ft.a)(n.prototype), "open", this).call(this, t);
                                     case 25:
                                         return e.abrupt("return", e.sent);
                                     case 26:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, this, [
@@ -15034,15 +15047,15 @@
                                     case 10:
                                         e.t0 = e.sent;
                                     case 11:
                                         if (!e.t0) {
                                             e.next = 22;
                                             break
                                         }
-                                        return e.next = 14, this._reader.readMessage(Xt.RecordBatch);
+                                        return e.next = 14, this._reader.readMessage(Gt.RecordBatch);
                                     case 14:
                                         if (!(r = e.sent) || !r.isRecordBatch()) {
                                             e.next = 22;
                                             break
                                         }
                                         return i = r.header(), e.next = 19, this._reader.readMessageBody(r.bodyLength);
                                     case 19:
@@ -15075,15 +15088,15 @@
                                     case 5:
                                         e.t0 = e.sent;
                                     case 6:
                                         if (!e.t0) {
                                             e.next = 17;
                                             break
                                         }
-                                        return e.next = 9, this._reader.readMessage(Xt.DictionaryBatch);
+                                        return e.next = 9, this._reader.readMessage(Gt.DictionaryBatch);
                                     case 9:
                                         if (!(r = e.sent) || !r.isDictionaryBatch()) {
                                             e.next = 17;
                                             break
                                         }
                                         return i = r.header(), e.next = 14, this._reader.readMessageBody(r.bodyLength);
                                     case 14:
@@ -15108,19 +15121,19 @@
                                     case 0:
                                         if (t = this._handle, e.t0 = t._pending, !e.t0) {
                                             e.next = 5;
                                             break
                                         }
                                         return e.next = 5, t._pending;
                                     case 5:
-                                        return n = t.size - ku, e.next = 8, t.readInt32(n);
+                                        return n = t.size - mu, e.next = 8, t.readInt32(n);
                                     case 8:
                                         return r = e.sent, e.next = 11, t.readAt(n - r, r);
                                     case 11:
-                                        return i = e.sent, e.abrupt("return", Ya.decode(i));
+                                        return i = e.sent, e.abrupt("return", za.decode(i));
                                     case 13:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, this)
                         })));
                         return function() {
@@ -15169,40 +15182,40 @@
                             }), e, this)
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 }]), n
-            }(Mc),
-            Pc = function(e) {
+            }(Fc),
+            Nc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     return Object(C.a)(this, n), t.call(this, e, r)
                 }
                 return Object(M.a)(n, [{
                     key: "_loadVectors",
                     value: function(e, t, n) {
-                        return new uo(t, e.nodes, e.buffers, this.dictionaries).visitMany(n)
+                        return new ao(t, e.nodes, e.buffers, this.dictionaries).visitMany(n)
                     }
                 }]), n
-            }(Cc);
+            }(Lc);
 
-        function Rc(e, t) {
+        function Uc(e, t) {
             return t && "boolean" === typeof t.autoDestroy ? t.autoDestroy : e.autoDestroy
         }
 
-        function Vc(e) {
+        function Pc(e) {
             var t;
             return U().wrap((function(n) {
                 for (;;) switch (n.prev = n.next) {
                     case 0:
-                        if (t = Ec.from(e), n.prev = 1, t.open({
+                        if (t = Tc.from(e), n.prev = 1, t.open({
                                 autoDestroy: !1
                             }).closed) {
                             n.next = 6;
                             break
                         }
                     case 3:
                         return n.next = 5, t;
@@ -15213,30 +15226,30 @@
                         }
                     case 6:
                         return n.prev = 6, t.cancel(), n.finish(6);
                     case 9:
                     case "end":
                         return n.stop()
                 }
-            }), Ic, null, [
+            }), Sc, null, [
                 [1, , 6, 9]
             ])
         }
 
-        function zc(e) {
-            return Wc.apply(this, arguments)
+        function Rc(e) {
+            return Vc.apply(this, arguments)
         }
 
-        function Wc() {
-            return (Wc = W(U().mark((function e(t) {
+        function Vc() {
+            return (Vc = W(U().mark((function e(t) {
                 var n;
                 return U().wrap((function(e) {
                     for (;;) switch (e.prev = e.next) {
                         case 0:
-                            return e.next = 2, V(Ec.from(t));
+                            return e.next = 2, V(Tc.from(t));
                         case 2:
                             return n = e.sent, e.prev = 3, e.next = 6, V(n.open({
                                 autoDestroy: !1
                             }));
                         case 6:
                             if (e.sent.closed) {
                                 e.next = 12;
@@ -15261,41 +15274,41 @@
                     }
                 }), e, null, [
                     [3, , 12, 16]
                 ])
             })))).apply(this, arguments)
         }
 
-        function Yc() {
-            return (Yc = F(U().mark((function e(t) {
+        function zc() {
+            return (zc = F(U().mark((function e(t) {
                 var n;
                 return U().wrap((function(e) {
                     for (;;) switch (e.prev = e.next) {
                         case 0:
-                            return e.next = 2, t.peek(gu + 7 & -8);
+                            return e.next = 2, t.peek(bu + 7 & -8);
                         case 2:
                             if (!((n = e.sent) && n.byteLength >= 4)) {
                                 e.next = 18;
                                 break
                             }
-                            if (mu(n)) {
+                            if (vu(n)) {
                                 e.next = 8;
                                 break
                             }
-                            e.t1 = new Bc(new Mc(t)), e.next = 15;
+                            e.t1 = new Ec(new Fc(t)), e.next = 15;
                             break;
                         case 8:
-                            return e.t2 = Dc, e.t3 = Nc, e.next = 12, t.read();
+                            return e.t2 = Ac, e.t3 = Cc, e.next = 12, t.read();
                         case 12:
                             e.t4 = e.sent, e.t5 = new e.t3(e.t4), e.t1 = new e.t2(e.t5);
                         case 15:
                             e.t0 = e.t1, e.next = 19;
                             break;
                         case 18:
-                            e.t0 = new Bc(new Mc(W(U().mark((function e() {
+                            e.t0 = new Ec(new Fc(W(U().mark((function e() {
                                 return U().wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
                                         case "end":
                                             return e.stop()
                                     }
                                 }), e)
@@ -15306,71 +15319,71 @@
                         case "end":
                             return e.stop()
                     }
                 }), e)
             })))).apply(this, arguments)
         }
 
-        function Hc() {
-            return (Hc = F(U().mark((function e(t) {
+        function Wc() {
+            return (Wc = F(U().mark((function e(t) {
                 var n, r, i;
                 return U().wrap((function(e) {
                     for (;;) switch (e.prev = e.next) {
                         case 0:
                             return e.next = 2, t.stat();
                         case 2:
-                            if (n = e.sent, r = n.size, i = new Xa(t, r), !(r >= wu)) {
+                            if (n = e.sent, r = n.size, i = new Ja(t, r), !(r >= gu)) {
                                 e.next = 12;
                                 break
                             }
-                            return e.t0 = mu, e.next = 9, i.readAt(0, gu + 7 & -8);
+                            return e.t0 = vu, e.next = 9, i.readAt(0, bu + 7 & -8);
                         case 9:
                             if (e.t1 = e.sent, !(0, e.t0)(e.t1)) {
                                 e.next = 12;
                                 break
                             }
-                            return e.abrupt("return", new Lc(new Uc(i)));
-                        case 12:
                             return e.abrupt("return", new Bc(new Mc(i)));
+                        case 12:
+                            return e.abrupt("return", new Ec(new Fc(i)));
                         case 13:
                         case "end":
                             return e.stop()
                     }
                 }), e)
             })))).apply(this, arguments)
         }
-        var $c = ["readableStrategy", "writableStrategy", "queueingStrategy"];
-        var Kc = function() {
+        var Yc = ["readableStrategy", "writableStrategy", "queueingStrategy"];
+        var Hc = function() {
                 function e(t) {
                     var n, r, i = this;
                     Object(C.a)(this, e), this._numChunks = 0, this._finished = !1, this._bufferedSize = 0;
                     var a = t.readableStrategy,
                         o = t.writableStrategy,
                         u = t.queueingStrategy,
                         s = void 0 === u ? "count" : u,
-                        c = Uu(t, $c);
-                    this._controller = null, this._builder = mr.new(c), this._getSize = "bytes" !== s ? Qc : qc;
-                    var l = Mt({}, a).highWaterMark,
+                        c = Mu(t, Yc);
+                    this._controller = null, this._builder = yr.new(c), this._getSize = "bytes" !== s ? $c : Kc;
+                    var l = Object(Lt.a)({}, a).highWaterMark,
                         f = void 0 === l ? "bytes" === s ? Math.pow(2, 14) : 1e3 : l,
-                        h = Mt({}, o).highWaterMark,
+                        h = Object(Lt.a)({}, o).highWaterMark,
                         d = void 0 === h ? "bytes" === s ? Math.pow(2, 14) : 1e3 : h;
-                    this.readable = new ReadableStream((Ft(n = {}, "cancel", (function() {
+                    this.readable = new ReadableStream((n = {}, Object(_i.a)(n, "cancel", (function() {
                         i._builder.clear()
-                    })), Ft(n, "pull", (function(e) {
+                    })), Object(_i.a)(n, "pull", (function(e) {
                         i._maybeFlush(i._builder, i._controller = e)
-                    })), Ft(n, "start", (function(e) {
+                    })), Object(_i.a)(n, "start", (function(e) {
                         i._maybeFlush(i._builder, i._controller = e)
                     })), n), {
                         highWaterMark: f,
-                        size: "bytes" !== s ? Qc : qc
-                    }), this.writable = new WritableStream((Ft(r = {}, "abort", (function() {
+                        size: "bytes" !== s ? $c : Kc
+                    }), this.writable = new WritableStream((r = {}, Object(_i.a)(r, "abort", (function() {
                         i._builder.clear()
-                    })), Ft(r, "write", (function() {
+                    })), Object(_i.a)(r, "write", (function() {
                         i._maybeFlush(i._builder, i._controller)
-                    })), Ft(r, "close", (function() {
+                    })), Object(_i.a)(r, "close", (function() {
                         i._maybeFlush(i._builder.finish(), i._controller)
                     })), r), {
                         highWaterMark: d,
                         size: function(e) {
                             return i._writeValueAndReturnChunkSize(e)
                         }
                     })
@@ -15389,67 +15402,67 @@
                 }, {
                     key: "_enqueue",
                     value: function(e, t) {
                         this._bufferedSize = 0, this._controller = null, null === t ? e.close() : e.enqueue(t)
                     }
                 }]), e
             }(),
-            Qc = function(e) {
+            $c = function(e) {
                 return e.length
             },
-            qc = function(e) {
+            Kc = function(e) {
                 return e.byteLength
             };
-        var Gc = function() {
+        var Qc = function() {
                 function e() {
                     Object(C.a)(this, e)
                 }
                 return Object(M.a)(e, [{
                     key: "eq",
                     value: function(t) {
-                        return t instanceof e || (t = new Jc(t)), new il(this, t)
+                        return t instanceof e || (t = new qc(t)), new nl(this, t)
                     }
                 }, {
                     key: "le",
                     value: function(t) {
-                        return t instanceof e || (t = new Jc(t)), new al(this, t)
+                        return t instanceof e || (t = new qc(t)), new rl(this, t)
                     }
                 }, {
                     key: "ge",
                     value: function(t) {
-                        return t instanceof e || (t = new Jc(t)), new ol(this, t)
+                        return t instanceof e || (t = new qc(t)), new il(this, t)
                     }
                 }, {
                     key: "lt",
                     value: function(e) {
-                        return new ul(this.ge(e))
+                        return new al(this.ge(e))
                     }
                 }, {
                     key: "gt",
                     value: function(e) {
-                        return new ul(this.le(e))
+                        return new al(this.le(e))
                     }
                 }, {
                     key: "ne",
                     value: function(e) {
-                        return new ul(this.eq(e))
+                        return new al(this.eq(e))
                     }
                 }]), e
             }(),
-            Jc = function(e) {
+            qc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
                     return Object(C.a)(this, n), (r = t.call(this)).v = e, r
                 }
                 return Object(M.a)(n)
-            }(Gc),
-            Zc = function(e) {
+            }(Qc),
+            Gc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
                     return Object(C.a)(this, n), (r = t.call(this)).name = e, r
                 }
@@ -15466,115 +15479,115 @@
                         }
                         var r = this.vector = e.getChildAt(this.colidx);
                         return function(e) {
                             return r.get(e)
                         }
                     }
                 }]), n
-            }(Gc),
-            Xc = function() {
+            }(Qc),
+            Jc = function() {
                 function e() {
                     Object(C.a)(this, e)
                 }
                 return Object(M.a)(e, [{
                     key: "and",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                        return Pr(nl, [this].concat(t))
+                        return Mr(el, [this].concat(t))
                     }
                 }, {
                     key: "or",
                     value: function() {
                         for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                        return Pr(rl, [this].concat(t))
+                        return Mr(tl, [this].concat(t))
                     }
                 }, {
                     key: "not",
                     value: function() {
-                        return new ul(this)
+                        return new al(this)
                     }
                 }]), e
             }(),
-            el = function(e) {
+            Zc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     var i;
                     return Object(C.a)(this, n), (i = t.call(this)).left = e, i.right = r, i
                 }
                 return Object(M.a)(n, [{
                     key: "bind",
                     value: function(e) {
-                        return this.left instanceof Jc ? this.right instanceof Jc ? this._bindLitLit(e, this.left, this.right) : this._bindLitCol(e, this.left, this.right) : this.right instanceof Jc ? this._bindColLit(e, this.left, this.right) : this._bindColCol(e, this.left, this.right)
+                        return this.left instanceof qc ? this.right instanceof qc ? this._bindLitLit(e, this.left, this.right) : this._bindLitCol(e, this.left, this.right) : this.right instanceof qc ? this._bindColLit(e, this.left, this.right) : this._bindColCol(e, this.left, this.right)
                     }
                 }]), n
-            }(Xc),
-            tl = function(e) {
+            }(Jc),
+            Xc = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     var e;
                     Object(C.a)(this, n), e = t.call(this);
                     for (var r = arguments.length, i = new Array(r), a = 0; a < r; a++) i[a] = arguments[a];
                     return e.children = i, e
                 }
                 return Object(M.a)(n)
-            }(Xc);
-        tl.prototype.children = Object.freeze([]);
-        var nl = function(e) {
+            }(Jc);
+        Xc.prototype.children = Object.freeze([]);
+        var el = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     for (var e = arguments.length, r = new Array(e), i = 0; i < e; i++) r[i] = arguments[i];
                     return Object(C.a)(this, n), r = r.reduce((function(e, t) {
                         return e.concat(t instanceof n ? t.children : t)
-                    }), []), t.call.apply(t, [this].concat(hn(r)))
+                    }), []), t.call.apply(t, [this].concat(cn(r)))
                 }
                 return Object(M.a)(n, [{
                     key: "bind",
                     value: function(e) {
                         var t = this.children.map((function(t) {
                             return t.bind(e)
                         }));
                         return function(e, n) {
                             return t.every((function(t) {
                                 return t(e, n)
                             }))
                         }
                     }
                 }]), n
-            }(tl),
-            rl = function(e) {
+            }(Xc),
+            tl = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     for (var e = arguments.length, r = new Array(e), i = 0; i < e; i++) r[i] = arguments[i];
                     return Object(C.a)(this, n), r = r.reduce((function(e, t) {
                         return e.concat(t instanceof n ? t.children : t)
-                    }), []), t.call.apply(t, [this].concat(hn(r)))
+                    }), []), t.call.apply(t, [this].concat(cn(r)))
                 }
                 return Object(M.a)(n, [{
                     key: "bind",
                     value: function(e) {
                         var t = this.children.map((function(t) {
                             return t.bind(e)
                         }));
                         return function(e, n) {
                             return t.some((function(t) {
                                 return t(e, n)
                             }))
                         }
                     }
                 }]), n
-            }(tl),
-            il = function(e) {
+            }(Xc),
+            nl = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -15594,15 +15607,15 @@
                             return r(e, t) == i(e, t)
                         }
                     }
                 }, {
                     key: "_bindColLit",
                     value: function(e, t, n) {
                         var r = t.bind(e);
-                        if (t.vector instanceof $u) {
+                        if (t.vector instanceof Yu) {
                             var i, a = t.vector;
                             return a.dictionary !== this.lastDictionary ? (i = a.reverseLookup(n.v), this.lastDictionary = a.dictionary, this.lastKey = i) : i = this.lastKey, -1 === i ? function() {
                                 return !1
                             } : function(e) {
                                 return a.getKey(e) === i
                             }
                         }
@@ -15612,16 +15625,16 @@
                     }
                 }, {
                     key: "_bindLitCol",
                     value: function(e, t, n) {
                         return this._bindColLit(e, n, t)
                     }
                 }]), n
-            }(el),
-            al = function(e) {
+            }(Zc),
+            rl = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -15654,16 +15667,16 @@
                     value: function(e, t, n) {
                         var r = n.bind(e);
                         return function(e, n) {
                             return t.v <= r(e, n)
                         }
                     }
                 }]), n
-            }(el),
-            ol = function(e) {
+            }(Zc),
+            il = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
@@ -15696,16 +15709,16 @@
                     value: function(e, t, n) {
                         var r = n.bind(e);
                         return function(e, n) {
                             return t.v >= r(e, n)
                         }
                     }
                 }]), n
-            }(el),
-            ul = function(e) {
+            }(Zc),
+            al = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e) {
                     var r;
                     return Object(C.a)(this, n), (r = t.call(this)).child = e, r
                 }
@@ -15714,35 +15727,35 @@
                     value: function(e) {
                         var t = this.child.bind(e);
                         return function(e, n) {
                             return !t(e, n)
                         }
                     }
                 }]), n
-            }(Xc);
-        xc.prototype.countBy = function(e) {
-            return new sl(this.chunks).countBy(e)
-        }, xc.prototype.scan = function(e, t) {
-            return new sl(this.chunks).scan(e, t)
-        }, xc.prototype.scanReverse = function(e, t) {
-            return new sl(this.chunks).scanReverse(e, t)
-        }, xc.prototype.filter = function(e) {
-            return new sl(this.chunks).filter(e)
+            }(Jc);
+        _c.prototype.countBy = function(e) {
+            return new ol(this.chunks).countBy(e)
+        }, _c.prototype.scan = function(e, t) {
+            return new ol(this.chunks).scan(e, t)
+        }, _c.prototype.scanReverse = function(e, t) {
+            return new ol(this.chunks).scanReverse(e, t)
+        }, _c.prototype.filter = function(e) {
+            return new ol(this.chunks).filter(e)
         };
-        var sl = function(e) {
+        var ol = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n() {
                     return Object(C.a)(this, n), t.apply(this, arguments)
                 }
                 return Object(M.a)(n, [{
                     key: "filter",
                     value: function(e) {
-                        return new ll(this.chunks, e)
+                        return new sl(this.chunks, e)
                     }
                 }, {
                     key: "scan",
                     value: function(e, t) {
                         for (var n = this.chunks, r = n.length, i = -1; ++i < r;) {
                             var a = n[i];
                             t && t(a);
@@ -15759,48 +15772,48 @@
                         }
                     }
                 }, {
                     key: "countBy",
                     value: function(e) {
                         var t = this.chunks,
                             n = t.length,
-                            r = "string" === typeof e ? new Zc(e) : e;
+                            r = "string" === typeof e ? new Gc(e) : e;
                         r.bind(t[n - 1]);
                         var i = r.vector;
-                        if (!Tn.isDictionary(i.type)) throw new Error("countBy currently only supports dictionary-encoded columns");
+                        if (!jn.isDictionary(i.type)) throw new Error("countBy currently only supports dictionary-encoded columns");
                         for (var a = Math.ceil(Math.log(i.length) / Math.log(256)), o = new(4 == a ? Uint32Array : a >= 2 ? Uint16Array : Uint8Array)(i.dictionary.length), u = -1; ++u < n;) {
                             var s = t[u];
                             r.bind(s);
                             for (var c = r.vector.indices, l = -1, f = s.length; ++l < f;) {
                                 var h = c.get(l);
                                 null !== h && o[h]++
                             }
                         }
-                        return new cl(i.dictionary, as.from(o))
+                        return new ul(i.dictionary, rs.from(o))
                     }
                 }]), n
-            }(xc),
-            cl = function(e) {
+            }(_c),
+            ul = function(e) {
                 Object(ce.a)(n, e);
                 var t = Object(le.a)(n);
 
                 function n(e, r) {
                     Object(C.a)(this, n);
-                    var i = new ia([new aa("values", e.type), new aa("counts", r.type)]);
-                    return t.call(this, new jc(i, r.length, [e, r]))
+                    var i = new na([new ra("values", e.type), new ra("counts", r.type)]);
+                    return t.call(this, new Oc(i, r.length, [e, r]))
                 }
                 return Object(M.a)(n, [{
                     key: "toJSON",
                     value: function() {
                         for (var e = this.getColumnAt(0), t = this.getColumnAt(1), n = {}, r = -1; ++r < this.length;) n[e.get(r)] = t.get(r);
                         return n
                     }
                 }]), n
-            }(xc),
-            ll = function(e, t) {
+            }(_c),
+            sl = function(e, t) {
                 Object(ce.a)(r, e);
                 var n = Object(le.a)(r);
 
                 function r(e, t) {
                     var i;
                     return Object(C.a)(this, r), (i = n.call(this, e))._predicate = t, i
                 }
@@ -15865,38 +15878,38 @@
                         return new r(this._chunks, this._predicate.and(e))
                     }
                 }, {
                     key: "countBy",
                     value: function(e) {
                         var t = this._chunks,
                             n = t.length,
-                            r = "string" === typeof e ? new Zc(e) : e;
+                            r = "string" === typeof e ? new Gc(e) : e;
                         r.bind(t[n - 1]);
                         var i = r.vector;
-                        if (!Tn.isDictionary(i.type)) throw new Error("countBy currently only supports dictionary-encoded columns");
+                        if (!jn.isDictionary(i.type)) throw new Error("countBy currently only supports dictionary-encoded columns");
                         for (var a = Math.ceil(Math.log(i.length) / Math.log(256)), o = new(4 == a ? Uint32Array : a >= 2 ? Uint16Array : Uint8Array)(i.dictionary.length), u = -1; ++u < n;) {
                             var s = t[u],
                                 c = this._predicate.bind(s);
                             r.bind(s);
                             for (var l = r.vector.indices, f = -1, h = s.length; ++f < h;) {
                                 var d = l.get(f);
                                 null !== d && c(f, s) && o[d]++
                             }
                         }
-                        return new cl(i.dictionary, as.from(o))
+                        return new ul(i.dictionary, rs.from(o))
                     }
                 }]), r
-            }(sl, Symbol.iterator);
-        Mt(Mt(Mt(Mt(Mt(Mt({}, o), s), i), a), r), u);
+            }(ol, Symbol.iterator);
+        Object(Lt.a)(Object(Lt.a)(Object(Lt.a)(Object(Lt.a)(Object(Lt.a)(Object(Lt.a)({}, o), s), i), a), r), u);
         Ot.toDOMStream = function(e, t) {
             if (Ie(e)) return function(e, t) {
                 var n = null,
                     r = t && "bytes" === t.type || !1,
                     i = t && t.highWaterMark || Math.pow(2, 24);
-                return new ReadableStream(Mt(Mt({}, t), {}, {
+                return new ReadableStream(Object(Lt.a)(Object(Lt.a)({}, t), {}, {
                     start: function(t) {
                         return F(U().mark((function r() {
                             return U().wrap((function(r) {
                                 for (;;) switch (r.prev = r.next) {
                                     case 0:
                                         return r.next = 2, a(t, n || (n = e[Symbol.asyncIterator]()));
                                     case 2:
@@ -15961,15 +15974,15 @@
                                     case 14:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e)
                         })))()
                     }
-                }), Mt({
+                }), Object(Lt.a)({
                     highWaterMark: r ? i : void 0
                 }, t));
 
                 function a(e, t) {
                     return o.apply(this, arguments)
                 }
 
@@ -16005,39 +16018,39 @@
                     }))), o.apply(this, arguments)
                 }
             }(e, t);
             if (Te(e)) return function(e, t) {
                 var n = null,
                     r = t && "bytes" === t.type || !1,
                     i = t && t.highWaterMark || Math.pow(2, 24);
-                return new ReadableStream(Mt(Mt({}, t), {}, {
+                return new ReadableStream(Object(Lt.a)(Object(Lt.a)({}, t), {}, {
                     start: function(t) {
                         a(t, n || (n = e[Symbol.iterator]()))
                     },
                     pull: function(e) {
                         n ? a(e, n) : e.close()
                     },
                     cancel: function() {
                         n && n.return && n.return(), n = null
                     }
-                }), Mt({
+                }), Object(Lt.a)({
                     highWaterMark: r ? i : void 0
                 }, t));
 
                 function a(e, t) {
                     for (var n, i = null, a = e.desiredSize || null; !(i = t.next(r ? a : null)).done;)
                         if (ArrayBuffer.isView(i.value) && (n = He(i.value)) && (null != a && r && (a = a - n.byteLength + 1), i.value = n), e.enqueue(i.value), null != a && --a <= 0) return;
                     e.close()
                 }
             }(e, t);
             throw new Error("toDOMStream() must be called with an Iterable or AsyncIterable")
-        }, mr.throughDOM = function(e) {
-            return new Kc(e)
-        }, Ec.throughDOM = function(e, t) {
-            var n = new Ka,
+        }, yr.throughDOM = function(e) {
+            return new Hc(e)
+        }, Tc.throughDOM = function(e, t) {
+            var n = new Ha,
                 r = null,
                 i = new ReadableStream({
                     cancel: function() {
                         return F(U().mark((function e() {
                             return U().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
@@ -16090,30 +16103,30 @@
                                         return t.stop()
                                 }
                             }), t)
                         })))()
                     }
                 });
             return {
-                writable: new WritableStream(n, Mt({
+                writable: new WritableStream(n, Object(Lt.a)({
                     highWaterMark: Math.pow(2, 14)
                 }, e)),
                 readable: i
             };
 
             function a() {
                 return o.apply(this, arguments)
             }
 
             function o() {
                 return (o = F(U().mark((function e() {
                     return U().wrap((function(e) {
                         for (;;) switch (e.prev = e.next) {
                             case 0:
-                                return e.next = 2, Ec.from(n);
+                                return e.next = 2, Tc.from(n);
                             case 2:
                                 return e.next = 4, e.sent.open(t);
                             case 4:
                                 return e.abrupt("return", e.sent);
                             case 5:
                             case "end":
                                 return e.stop()
@@ -16153,17 +16166,17 @@
                             case 11:
                             case "end":
                                 return e.stop()
                         }
                     }), e)
                 }))), s.apply(this, arguments)
             }
-        }, Iu.throughDOM = function(e, t) {
+        }, Su.throughDOM = function(e, t) {
             var n = new this(e),
-                r = new qa(n),
+                r = new Ka(n),
                 i = new ReadableStream({
                     type: "bytes",
                     cancel: function() {
                         return F(U().mark((function e() {
                             return U().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
@@ -16197,15 +16210,15 @@
                                     case 2:
                                     case "end":
                                         return t.stop()
                                 }
                             }), t)
                         })))()
                     }
-                }, Mt({
+                }, Object(Lt.a)({
                     highWaterMark: Math.pow(2, 14)
                 }, t));
             return {
                 writable: new WritableStream(n, e),
                 readable: i
             };
 
@@ -16241,15 +16254,15 @@
                             case "end":
                                 return e.stop()
                         }
                     }), e)
                 })))).apply(this, arguments)
             }
         };
-        var fl, hl = function() {
+        var cl, ll = function() {
                 function e(e, t, n, r) {
                     var i = this;
                     this.getCell = function(e, t) {
                         var n = e < i.headerRows && t < i.headerColumns,
                             r = e >= i.headerRows && t < i.headerColumns,
                             a = e < i.headerRows && t >= i.headerColumns;
                         if (n) {
@@ -16280,18 +16293,18 @@
                             type: "data",
                             id: "T_" + i.uuid + "row" + u + "_col" + s,
                             classNames: o.join(" "),
                             content: c
                         }
                     }, this.getContent = function(e, t, n) {
                         var r = e.getColumnAt(n);
-                        return null === r ? "" : i.getColumnTypeId(e, n) === $t.Timestamp ? i.nanosToDate(r.get(t)) : r.get(t)
-                    }, this.dataTable = xc.from(e), this.indexTable = xc.from(t), this.columnsTable = xc.from(n), this.styler = r ? {
+                        return null === r ? "" : i.getColumnTypeId(e, n) === Wt.Timestamp ? i.nanosToDate(r.get(t)) : r.get(t)
+                    }, this.dataTable = _c.from(e), this.indexTable = _c.from(t), this.columnsTable = _c.from(n), this.styler = r ? {
                         caption: r.caption,
-                        displayValuesTable: xc.from(r.displayValues),
+                        displayValuesTable: _c.from(r.displayValues),
                         styles: r.styles,
                         uuid: r.uuid
                     } : void 0
                 }
                 return Object.defineProperty(e.prototype, "rows", {
                     get: function() {
                         return this.indexTable.length + this.columnsTable.numCols
@@ -16372,56 +16385,56 @@
                     }
                 }, e.prototype.getColumnTypeId = function(e, t) {
                     return e.schema.fields[t].type.typeId
                 }, e.prototype.nanosToDate = function(e) {
                     return new Date(e / 1e6)
                 }, e
             }(),
-            dl = function() {
-                return dl = Object.assign || function(e) {
+            fl = function() {
+                return fl = Object.assign || function(e) {
                     for (var t, n = 1, r = arguments.length; n < r; n++)
                         for (var i in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, i) && (e[i] = t[i]);
                     return e
-                }, dl.apply(this, arguments)
+                }, fl.apply(this, arguments)
             };
         ! function(e) {
             e.COMPONENT_READY = "streamlit:componentReady", e.SET_COMPONENT_VALUE = "streamlit:setComponentValue", e.SET_FRAME_HEIGHT = "streamlit:setFrameHeight"
-        }(fl || (fl = {}));
-        var pl = function() {
+        }(cl || (cl = {}));
+        var hl = function() {
                 function e() {}
                 return e.API_VERSION = 1, e.RENDER_EVENT = "streamlit:render", e.events = new E, e.registeredMessageListener = !1, e.setComponentReady = function() {
-                    e.registeredMessageListener || (window.addEventListener("message", e.onMessageEvent), e.registeredMessageListener = !0), e.sendBackMsg(fl.COMPONENT_READY, {
+                    e.registeredMessageListener || (window.addEventListener("message", e.onMessageEvent), e.registeredMessageListener = !0), e.sendBackMsg(cl.COMPONENT_READY, {
                         apiVersion: e.API_VERSION
                     })
                 }, e.setFrameHeight = function(t) {
-                    void 0 === t && (t = document.body.scrollHeight), t !== e.lastFrameHeight && (e.lastFrameHeight = t, e.sendBackMsg(fl.SET_FRAME_HEIGHT, {
+                    void 0 === t && (t = document.body.scrollHeight), t !== e.lastFrameHeight && (e.lastFrameHeight = t, e.sendBackMsg(cl.SET_FRAME_HEIGHT, {
                         height: t
                     }))
                 }, e.setComponentValue = function(t) {
                     var n;
-                    t instanceof hl ? (n = "dataframe", t = t.serialize()) : ! function(e) {
+                    t instanceof ll ? (n = "dataframe", t = t.serialize()) : ! function(e) {
                         var t = !1;
                         try {
                             t = e instanceof BigInt64Array || e instanceof BigUint64Array
                         } catch (n) {}
                         return e instanceof Int8Array || e instanceof Uint8Array || e instanceof Uint8ClampedArray || e instanceof Int16Array || e instanceof Uint16Array || e instanceof Int32Array || e instanceof Uint32Array || e instanceof Float32Array || e instanceof Float64Array || t
-                    }(t) ? t instanceof ArrayBuffer ? (n = "bytes", t = new Uint8Array(t)) : n = "json" : (n = "bytes", t = new Uint8Array(t.buffer)), e.sendBackMsg(fl.SET_COMPONENT_VALUE, {
+                    }(t) ? t instanceof ArrayBuffer ? (n = "bytes", t = new Uint8Array(t)) : n = "json" : (n = "bytes", t = new Uint8Array(t.buffer)), e.sendBackMsg(cl.SET_COMPONENT_VALUE, {
                         value: t,
                         dataType: n
                     })
                 }, e.onMessageEvent = function(t) {
                     if (t.data.type === e.RENDER_EVENT) e.onRenderMessage(t.data)
                 }, e.onRenderMessage = function(t) {
                     var n = t.args;
                     null == n && (console.error("Got null args in onRenderMessage. This should never happen"), n = {});
                     var r = t.dfs && t.dfs.length > 0 ? e.argsDataframeToObject(t.dfs) : {};
-                    n = dl(dl({}, n), r);
+                    n = fl(fl({}, n), r);
                     var i = Boolean(t.disabled),
                         a = t.theme;
-                    a && yl(a);
+                    a && dl(a);
                     var o = {
                             disabled: i,
                             args: n,
                             theme: a
                         },
                         u = new CustomEvent(e.RENDER_EVENT, {
                             detail: o
@@ -16436,27 +16449,27 @@
                     return Object.fromEntries(n)
                 }, e.toArrowTable = function(e) {
                     var t = e.data,
                         n = t.data,
                         r = t.index,
                         i = t.columns,
                         a = t.styler;
-                    return new hl(n, r, i, a)
+                    return new ll(n, r, i, a)
                 }, e.sendBackMsg = function(e, t) {
-                    window.parent.postMessage(dl({
+                    window.parent.postMessage(fl({
                         isStreamlitMessage: !0,
                         type: e
                     }, t), "*")
                 }, e
             }(),
-            yl = function(e) {
+            dl = function(e) {
                 var t = document.createElement("style");
                 document.head.appendChild(t), t.innerHTML = "\n    :root {\n      --primary-color: " + e.primaryColor + ";\n      --background-color: " + e.backgroundColor + ";\n      --secondary-background-color: " + e.secondaryBackgroundColor + ";\n      --text-color: " + e.textColor + ";\n      --font: " + e.font + ";\n    }\n\n    body {\n      background-color: var(--background-color);\n      color: var(--text-color);\n    }\n  "
             };
-        var vl = function() {
+        var pl = function() {
                 var e = function(t, n) {
                     return e = Object.setPrototypeOf || {
                         __proto__: []
                     }
                     instanceof Array && function(e, t) {
                         e.__proto__ = t
                     } || function(e, t) {
@@ -16466,35 +16479,35 @@
                 return function(t, n) {
                     function r() {
                         this.constructor = t
                     }
                     e(t, n), t.prototype = null === n ? Object.create(n) : (r.prototype = n.prototype, new r)
                 }
             }(),
-            bl = function(e) {
+            yl = function(e) {
                 function t() {
                     return null !== e && e.apply(this, arguments) || this
                 }
-                return vl(t, e), t.prototype.componentDidMount = function() {
-                    pl.setFrameHeight()
+                return pl(t, e), t.prototype.componentDidMount = function() {
+                    hl.setFrameHeight()
                 }, t.prototype.componentDidUpdate = function() {
-                    pl.setFrameHeight()
+                    hl.setFrameHeight()
                 }, t
             }(h.a.PureComponent);
 
-        function ml(e) {
+        function vl(e) {
             var t = function(t) {
                 function n(n) {
                     var r = t.call(this, n) || this;
                     return r.componentDidMount = function() {
-                        pl.events.addEventListener(pl.RENDER_EVENT, r.onRenderEvent), pl.setComponentReady()
+                        hl.events.addEventListener(hl.RENDER_EVENT, r.onRenderEvent), hl.setComponentReady()
                     }, r.componentDidUpdate = function() {
-                        null != r.state.componentError && pl.setFrameHeight()
+                        null != r.state.componentError && hl.setFrameHeight()
                     }, r.componentWillUnmount = function() {
-                        pl.events.removeEventListener(pl.RENDER_EVENT, r.onRenderEvent)
+                        hl.events.removeEventListener(hl.RENDER_EVENT, r.onRenderEvent)
                     }, r.onRenderEvent = function(e) {
                         var t = e;
                         r.setState({
                             renderData: t.detail
                         })
                     }, r.render = function() {
                         return null != r.state.componentError ? h.a.createElement("div", null, h.a.createElement("h1", null, "Component Error"), h.a.createElement("span", null, r.state.componentError.message)) : null == r.state.renderData ? null : h.a.createElement(e, {
@@ -16504,15 +16517,15 @@
                             theme: r.state.renderData.theme
                         })
                     }, r.state = {
                         renderData: void 0,
                         componentError: void 0
                     }, r
                 }
-                return vl(n, t), n.getDerivedStateFromError = function(e) {
+                return pl(n, t), n.getDerivedStateFromError = function(e) {
                     return {
                         componentError: e
                     }
                 }, n
             }(h.a.PureComponent);
             return l()(t, e)
         }
@@ -16554,18 +16567,18 @@
         "use strict";
         ! function e() {
             if ("undefined" !== typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ && "function" === typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE) try {
                 __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(e)
             } catch (t) {
                 console.error(t)
             }
-        }(), e.exports = n(18)
+        }(), e.exports = n(20)
     }, function(e, t, n) {
         "use strict";
-        var r = n(21),
+        var r = n(23),
             i = {
                 childContextTypes: !0,
                 contextType: !0,
                 contextTypes: !0,
                 defaultProps: !0,
                 displayName: !0,
                 getDefaultProps: !0,
@@ -16628,15 +16641,15 @@
                     }
                 }
             }
             return t
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(14),
+        var r = n(16),
             i = "function" === typeof Symbol && Symbol.for,
             a = i ? Symbol.for("react.element") : 60103,
             o = i ? Symbol.for("react.portal") : 60106,
             u = i ? Symbol.for("react.fragment") : 60107,
             s = i ? Symbol.for("react.strict_mode") : 60108,
             c = i ? Symbol.for("react.profiler") : 60114,
             l = i ? Symbol.for("react.provider") : 60109,
@@ -16674,46 +16687,46 @@
             if ("object" !== typeof e && "function" !== typeof e && null != e) throw Error(b(85));
             this.updater.enqueueSetState(this, e, t, "setState")
         }, k.prototype.forceUpdate = function(e) {
             this.updater.enqueueForceUpdate(this, e, "forceUpdate")
         }, w.prototype = k.prototype;
         var O = _.prototype = new w;
         O.constructor = _, r(O, k.prototype), O.isPureReactComponent = !0;
-        var x = {
+        var j = {
                 current: null
             },
-            j = Object.prototype.hasOwnProperty,
+            x = Object.prototype.hasOwnProperty,
             S = {
                 key: !0,
                 ref: !0,
                 __self: !0,
                 __source: !0
             };
 
         function T(e, t, n) {
             var r, i = {},
                 o = null,
                 u = null;
             if (null != t)
-                for (r in void 0 !== t.ref && (u = t.ref), void 0 !== t.key && (o = "" + t.key), t) j.call(t, r) && !S.hasOwnProperty(r) && (i[r] = t[r]);
+                for (r in void 0 !== t.ref && (u = t.ref), void 0 !== t.key && (o = "" + t.key), t) x.call(t, r) && !S.hasOwnProperty(r) && (i[r] = t[r]);
             var s = arguments.length - 2;
             if (1 === s) i.children = n;
             else if (1 < s) {
                 for (var c = Array(s), l = 0; l < s; l++) c[l] = arguments[l + 2];
                 i.children = c
             }
             if (e && e.defaultProps)
                 for (r in s = e.defaultProps) void 0 === i[r] && (i[r] = s[r]);
             return {
                 $$typeof: a,
                 type: e,
                 key: o,
                 ref: u,
                 props: i,
-                _owner: x.current
+                _owner: j.current
             }
         }
 
         function I(e) {
             return "object" === typeof e && null !== e && e.$$typeof === a
         }
         var E = /\/+/g,
@@ -16816,15 +16829,15 @@
             return e
         }
         var V = {
             ReactCurrentDispatcher: P,
             ReactCurrentBatchConfig: {
                 suspense: null
             },
-            ReactCurrentOwner: x,
+            ReactCurrentOwner: j,
             IsSomeRendererActing: {
                 current: !1
             },
             assign: r
         };
         t.Children = {
             map: function(e, t, n) {
@@ -16854,16 +16867,16 @@
         }, t.Component = k, t.Fragment = u, t.Profiler = c, t.PureComponent = _, t.StrictMode = s, t.Suspense = d, t.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = V, t.cloneElement = function(e, t, n) {
             if (null === e || void 0 === e) throw Error(b(267, e));
             var i = r({}, e.props),
                 o = e.key,
                 u = e.ref,
                 s = e._owner;
             if (null != t) {
-                if (void 0 !== t.ref && (u = t.ref, s = x.current), void 0 !== t.key && (o = "" + t.key), e.type && e.type.defaultProps) var c = e.type.defaultProps;
-                for (l in t) j.call(t, l) && !S.hasOwnProperty(l) && (i[l] = void 0 === t[l] && void 0 !== c ? c[l] : t[l])
+                if (void 0 !== t.ref && (u = t.ref, s = j.current), void 0 !== t.key && (o = "" + t.key), e.type && e.type.defaultProps) var c = e.type.defaultProps;
+                for (l in t) x.call(t, l) && !S.hasOwnProperty(l) && (i[l] = void 0 === t[l] && void 0 !== c ? c[l] : t[l])
             }
             var l = arguments.length - 2;
             if (1 === l) i.children = n;
             else if (1 < l) {
                 c = Array(l);
                 for (var f = 0; f < l; f++) c[f] = arguments[f + 2];
                 i.children = c
@@ -16931,17 +16944,17 @@
         }, t.useRef = function(e) {
             return R().useRef(e)
         }, t.useState = function(e) {
             return R().useState(e)
         }, t.version = "16.14.0"
     }, function(e, t, n) {
         "use strict";
-        var r = n(6),
-            i = n(14),
-            a = n(19);
+        var r = n(8),
+            i = n(16),
+            a = n(21);
 
         function o(e) {
             for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, n = 1; n < arguments.length; n++) t += "&args[]=" + encodeURIComponent(arguments[n]);
             return "Minified React error #" + e + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
         }
         if (!r) throw Error(o(227));
 
@@ -17007,21 +17020,21 @@
                             if (!i) throw Error(o(98, r, e))
                         }
                     }
                 }
         }
 
         function w(e, t, n) {
-            if (x[e]) throw Error(o(100, e));
-            x[e] = t, j[e] = t.eventTypes[n].dependencies
+            if (j[e]) throw Error(o(100, e));
+            j[e] = t, x[e] = t.eventTypes[n].dependencies
         }
         var _ = [],
             O = {},
-            x = {},
-            j = {};
+            j = {},
+            x = {};
 
         function S(e) {
             var t, n = !1;
             for (t in e)
                 if (e.hasOwnProperty(t)) {
                     var r = e[t];
                     if (!g.hasOwnProperty(t) || g[t] !== r) {
@@ -17331,20 +17344,20 @@
             n = me(null != t.value ? t.value : n), e._wrapperState = {
                 initialChecked: r,
                 initialValue: n,
                 controlled: "checkbox" === t.type || "radio" === t.type ? null != t.checked : null != t.value
             }
         }
 
-        function xe(e, t) {
+        function je(e, t) {
             null != (t = t.checked) && J(e, "checked", t, !1)
         }
 
-        function je(e, t) {
-            xe(e, t);
+        function xe(e, t) {
+            je(e, t);
             var n = me(t.value),
                 r = t.type;
             if (null != n) "number" === r ? (0 === n && "" === e.value || e.value != n) && (e.value = "" + n) : e.value !== "" + n && (e.value = "" + n);
             else if ("submit" === r || "reset" === r) return void e.removeAttribute("value");
             t.hasOwnProperty("value") ? Te(e, t.type, n) : t.hasOwnProperty("defaultValue") && Te(e, t.type, me(t.defaultValue)), null == t.checked && null != t.defaultChecked && (e.defaultChecked = !!t.defaultChecked)
         }
 
@@ -17708,16 +17721,16 @@
             }
         }
         var vt, bt, mt, gt = !1,
             kt = [],
             wt = null,
             _t = null,
             Ot = null,
-            xt = new Map,
             jt = new Map,
+            xt = new Map,
             St = [],
             Tt = "mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput close cancel copy cut paste click change contextmenu reset submit".split(" "),
             It = "focus blur dragenter dragleave mouseover mouseout pointerover pointerout gotpointercapture lostpointercapture".split(" ");
 
         function Et(e, t, n, r, i) {
             return {
                 blockedOn: e,
@@ -17740,19 +17753,19 @@
                     break;
                 case "mouseover":
                 case "mouseout":
                     Ot = null;
                     break;
                 case "pointerover":
                 case "pointerout":
-                    xt.delete(t.pointerId);
+                    jt.delete(t.pointerId);
                     break;
                 case "gotpointercapture":
                 case "lostpointercapture":
-                    jt.delete(t.pointerId)
+                    xt.delete(t.pointerId)
             }
         }
 
         function Bt(e, t, n, r, i, a) {
             return null === e || e.nativeEvent !== a ? (e = Et(t, n, r, i, a), null !== t && (null !== (t = Fn(t)) && bt(t)), e) : (e.eventSystemFlags |= r, e)
         }
 
@@ -17790,15 +17803,15 @@
                 if (null !== e.blockedOn) {
                     null !== (e = Fn(e.blockedOn)) && vt(e);
                     break
                 }
                 var t = Xt(e.topLevelType, e.eventSystemFlags, e.container, e.nativeEvent);
                 null !== t ? e.blockedOn = t : kt.shift()
             }
-            null !== wt && Lt(wt) && (wt = null), null !== _t && Lt(_t) && (_t = null), null !== Ot && Lt(Ot) && (Ot = null), xt.forEach(Ft), jt.forEach(Ft)
+            null !== wt && Lt(wt) && (wt = null), null !== _t && Lt(_t) && (_t = null), null !== Ot && Lt(Ot) && (Ot = null), jt.forEach(Ft), xt.forEach(Ft)
         }
 
         function Mt(e, t) {
             e.blockedOn === t && (e.blockedOn = null, gt || (gt = !0, a.unstable_scheduleCallback(a.unstable_NormalPriority, Ct)))
         }
 
         function Nt(e) {
@@ -17808,15 +17821,15 @@
             if (0 < kt.length) {
                 Mt(kt[0], e);
                 for (var n = 1; n < kt.length; n++) {
                     var r = kt[n];
                     r.blockedOn === e && (r.blockedOn = null)
                 }
             }
-            for (null !== wt && Mt(wt, e), null !== _t && Mt(_t, e), null !== Ot && Mt(Ot, e), xt.forEach(t), jt.forEach(t), n = 0; n < St.length; n++)(r = St[n]).blockedOn === e && (r.blockedOn = null);
+            for (null !== wt && Mt(wt, e), null !== _t && Mt(_t, e), null !== Ot && Mt(Ot, e), jt.forEach(t), xt.forEach(t), n = 0; n < St.length; n++)(r = St[n]).blockedOn === e && (r.blockedOn = null);
             for (; 0 < St.length && null === (n = St[0]).blockedOn;) Dt(n), null === n.blockedOn && St.shift()
         }
         var Ut = {},
             Pt = new Map,
             Rt = new Map,
             Vt = ["abort", "abort", Ke, "animationEnd", Qe, "animationIteration", qe, "animationStart", "canplay", "canPlay", "canplaythrough", "canPlayThrough", "durationchange", "durationChange", "emptied", "emptied", "encrypted", "encrypted", "ended", "ended", "error", "error", "gotpointercapture", "gotPointerCapture", "load", "load", "loadeddata", "loadedData", "loadedmetadata", "loadedMetadata", "loadstart", "loadStart", "lostpointercapture", "lostPointerCapture", "playing", "playing", "progress", "progress", "seeking", "seeking", "stalled", "stalled", "suspend", "suspend", "timeupdate", "timeUpdate", Ge, "transitionEnd", "waiting", "waiting"];
 
@@ -17889,17 +17902,17 @@
                                     return wt = Bt(wt, e, t, n, r, i), !0;
                                 case "dragenter":
                                     return _t = Bt(_t, e, t, n, r, i), !0;
                                 case "mouseover":
                                     return Ot = Bt(Ot, e, t, n, r, i), !0;
                                 case "pointerover":
                                     var a = i.pointerId;
-                                    return xt.set(a, Bt(xt.get(a) || null, e, t, n, r, i)), !0;
+                                    return jt.set(a, Bt(jt.get(a) || null, e, t, n, r, i)), !0;
                                 case "gotpointercapture":
-                                    return a = i.pointerId, jt.set(a, Bt(jt.get(a) || null, e, t, n, r, i)), !0
+                                    return a = i.pointerId, xt.set(a, Bt(xt.get(a) || null, e, t, n, r, i)), !0
                             }
                             return !1
                         }(i, e, t, n, r)) {
                         At(e, r), e = dt(e, r, null, t);
                         try {
                             V(pt, e)
                         } finally {
@@ -18042,15 +18055,15 @@
                     return !0
             }
         }
         var sn = Fe;
 
         function cn(e, t) {
             var n = Xe(e = 9 === e.nodeType || 11 === e.nodeType ? e : e.ownerDocument);
-            t = j[t];
+            t = x[t];
             for (var r = 0; r < t.length; r++) yt(t[r], e, n)
         }
 
         function ln() {}
 
         function fn(e) {
             if ("undefined" === typeof(e = e || ("undefined" !== typeof document ? document : void 0))) return null;
@@ -18125,18 +18138,18 @@
                 case "select":
                 case "textarea":
                     return !!t.autoFocus
             }
             return !1
         }
 
-        function xn(e, t) {
+        function jn(e, t) {
             return "textarea" === e || "option" === e || "noscript" === e || "string" === typeof t.children || "number" === typeof t.children || "object" === typeof t.dangerouslySetInnerHTML && null !== t.dangerouslySetInnerHTML && null != t.dangerouslySetInnerHTML.__html
         }
-        var jn = "function" === typeof setTimeout ? setTimeout : void 0,
+        var xn = "function" === typeof setTimeout ? setTimeout : void 0,
             Sn = "function" === typeof clearTimeout ? clearTimeout : void 0;
 
         function Tn(e) {
             for (; null != e; e = e.nextSibling) {
                 var t = e.nodeType;
                 if (1 === t || 3 === t) break
             }
@@ -18498,33 +18511,33 @@
         }
 
         function _r(e, t) {
             if ("change" === e) return t
         }
         var Or = !1;
 
-        function xr() {
-            mr && (mr.detachEvent("onpropertychange", jr), gr = mr = null)
+        function jr() {
+            mr && (mr.detachEvent("onpropertychange", xr), gr = mr = null)
         }
 
-        function jr(e) {
+        function xr(e) {
             if ("value" === e.propertyName && wr(gr))
                 if (e = br(gr, e, ct(e)), U) st(e);
                 else {
                     U = !0;
                     try {
                         F(kr, e)
                     } finally {
                         U = !1, R()
                     }
                 }
         }
 
         function Sr(e, t, n) {
-            "focus" === e ? (xr(), gr = n, (mr = t).attachEvent("onpropertychange", jr)) : "blur" === e && xr()
+            "focus" === e ? (jr(), gr = n, (mr = t).attachEvent("onpropertychange", xr)) : "blur" === e && jr()
         }
 
         function Tr(e) {
             if ("selectionchange" === e || "keyup" === e || "keydown" === e) return wr(gr)
         }
 
         function Ir(e, t) {
@@ -18712,15 +18725,15 @@
         }
         var Xr = {
                 eventTypes: Kr,
                 extractEvents: function(e, t, n, r, i, a) {
                     if (!(a = !(i = a || (r.window === r ? r.document : 9 === r.nodeType ? r : r.ownerDocument)))) {
                         e: {
                             i = Xe(i),
-                            a = j.onSelect;
+                            a = x.onSelect;
                             for (var o = 0; o < a.length; o++)
                                 if (!i.has(a[o])) {
                                     i = !1;
                                     break e
                                 } i = !0
                         }
                         a = !i
@@ -18998,30 +19011,30 @@
         }
 
         function Oi(e, t, n) {
             if (bi.current !== vi) throw Error(o(168));
             yi(bi, t), yi(mi, n)
         }
 
-        function xi(e, t, n) {
+        function ji(e, t, n) {
             var r = e.stateNode;
             if (e = t.childContextTypes, "function" !== typeof r.getChildContext) return n;
             for (var a in r = r.getChildContext())
                 if (!(a in e)) throw Error(o(108, ve(t) || "Unknown", a));
             return i({}, n, {}, r)
         }
 
-        function ji(e) {
+        function xi(e) {
             return e = (e = e.stateNode) && e.__reactInternalMemoizedMergedChildContext || vi, gi = bi.current, yi(bi, e), yi(mi, mi.current), !0
         }
 
         function Si(e, t, n) {
             var r = e.stateNode;
             if (!r) throw Error(o(169));
-            n ? (e = xi(e, t, gi), r.__reactInternalMemoizedMergedChildContext = e, pi(mi), pi(bi), yi(bi, e)) : pi(mi), yi(mi, n)
+            n ? (e = ji(e, t, gi), r.__reactInternalMemoizedMergedChildContext = e, pi(mi), pi(bi), yi(bi, e)) : pi(mi), yi(mi, n)
         }
         var Ti = a.unstable_runWithPriority,
             Ii = a.unstable_scheduleCallback,
             Ei = a.unstable_cancelCallback,
             Ai = a.unstable_requestPaint,
             Bi = a.unstable_now,
             Di = a.unstable_getCurrentPriorityLevel,
@@ -19339,19 +19352,19 @@
         function Oa(e, t, n) {
             var r = !1,
                 i = vi,
                 a = t.contextType;
             return "object" === typeof a && null !== a ? a = ca(a) : (i = wi(t) ? gi : bi.current, a = (r = null !== (r = t.contextTypes) && void 0 !== r) ? ki(e, i) : vi), t = new t(n, a), e.memoizedState = null !== t.state && void 0 !== t.state ? t.state : null, t.updater = wa, e.stateNode = t, t._reactInternalFiber = e, r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = i, e.__reactInternalMemoizedMaskedChildContext = a), t
         }
 
-        function xa(e, t, n, r) {
+        function ja(e, t, n, r) {
             e = t.state, "function" === typeof t.componentWillReceiveProps && t.componentWillReceiveProps(n, r), "function" === typeof t.UNSAFE_componentWillReceiveProps && t.UNSAFE_componentWillReceiveProps(n, r), t.state !== e && wa.enqueueReplaceState(t, t.state, null)
         }
 
-        function ja(e, t, n, r) {
+        function xa(e, t, n, r) {
             var i = e.stateNode;
             i.props = n, i.state = e.memoizedState, i.refs = ga, fa(e);
             var a = t.contextType;
             "object" === typeof a && null !== a ? i.context = ca(a) : (a = wi(t) ? gi : bi.current, i.context = ki(e, a)), va(e, n, i, r), i.state = e.memoizedState, "function" === typeof(a = t.getDerivedStateFromProps) && (ka(e, t, a, n), i.state = e.memoizedState), "function" === typeof t.getDerivedStateFromProps || "function" === typeof i.getSnapshotBeforeUpdate || "function" !== typeof i.UNSAFE_componentWillMount && "function" !== typeof i.componentWillMount || (t = i.state, "function" === typeof i.componentWillMount && i.componentWillMount(), "function" === typeof i.UNSAFE_componentWillMount && i.UNSAFE_componentWillMount(), t !== i.state && wa.enqueueReplaceState(i, i.state, null), va(e, n, i, r), i.state = e.memoizedState), "function" === typeof i.componentDidMount && (e.effectTag |= 4)
         }
         var Sa = Array.isArray;
 
@@ -19661,19 +19674,19 @@
             if (null === t) return !1;
             for (var n = 0; n < t.length && n < e.length; n++)
                 if (!Wr(e[n], t[n])) return !1;
             return !0
         }
 
         function Xa(e, t, n, r, i, a) {
-            if ($a = a, Ka = t, t.memoizedState = null, t.updateQueue = null, t.expirationTime = 0, Ya.current = null === e || null === e.memoizedState ? Oo : xo, e = n(r, i), t.expirationTime === $a) {
+            if ($a = a, Ka = t, t.memoizedState = null, t.updateQueue = null, t.expirationTime = 0, Ya.current = null === e || null === e.memoizedState ? Oo : jo, e = n(r, i), t.expirationTime === $a) {
                 a = 0;
                 do {
                     if (t.expirationTime = 0, !(25 > a)) throw Error(o(301));
-                    a += 1, qa = Qa = null, t.updateQueue = null, Ya.current = jo, e = n(r, i)
+                    a += 1, qa = Qa = null, t.updateQueue = null, Ya.current = xo, e = n(r, i)
                 } while (t.expirationTime === $a)
             }
             if (Ya.current = _o, t = null !== Qa && null !== Qa.next, $a = 0, qa = Qa = Ka = null, Ga = !1, t) throw Error(o(300));
             return e
         }
 
         function eo() {
@@ -19963,15 +19976,15 @@
                 },
                 useTransition: function(e) {
                     var t = ao(!1),
                         n = t[0];
                     return t = t[1], [bo(ko.bind(null, t, e), [t, e]), n]
                 }
             },
-            xo = {
+            jo = {
                 readContext: ca,
                 useCallback: mo,
                 useContext: ca,
                 useEffect: fo,
                 useImperativeHandle: yo,
                 useLayoutEffect: ho,
                 useMemo: go,
@@ -19998,15 +20011,15 @@
                 },
                 useTransition: function(e) {
                     var t = ro(no),
                         n = t[0];
                     return t = t[1], [mo(ko.bind(null, t, e), [t, e]), n]
                 }
             },
-            jo = {
+            xo = {
                 readContext: ca,
                 useCallback: mo,
                 useContext: ca,
                 useEffect: fo,
                 useImperativeHandle: yo,
                 useLayoutEffect: ho,
                 useMemo: go,
@@ -20077,15 +20090,15 @@
             So = e
         }
 
         function Lo(e) {
             if (e !== So) return !1;
             if (!Io) return Do(e), Io = !0, !1;
             var t = e.type;
-            if (5 !== e.tag || "head" !== t && "body" !== t && !xn(t, e.memoizedProps))
+            if (5 !== e.tag || "head" !== t && "body" !== t && !jn(t, e.memoizedProps))
                 for (t = To; t;) Eo(e, t), t = Tn(t.nextSibling);
             if (Do(e), 13 === e.tag) {
                 if (!(e = null !== (e = e.memoizedState) ? e.dehydrated : null)) throw Error(o(317));
                 e: {
                     for (e = e.nextSibling, t = 0; e;) {
                         if (8 === e.nodeType) {
                             var n = e.data;
@@ -20142,30 +20155,30 @@
             var a = wi(n) ? gi : bi.current;
             return a = ki(t, a), sa(t, i), n = Xa(e, t, n, r, a, i), null === e || Mo ? (t.effectTag |= 1, No(e, t, n, i), t.child) : (t.updateQueue = e.updateQueue, t.effectTag &= -517, e.expirationTime <= i && (e.expirationTime = 0), tu(e, t, i))
         }
 
         function Wo(e, t, n, r, i) {
             if (wi(n)) {
                 var a = !0;
-                ji(t)
+                xi(t)
             } else a = !1;
-            if (sa(t, i), null === t.stateNode) null !== e && (e.alternate = null, t.alternate = null, t.effectTag |= 2), Oa(t, n, r), ja(t, n, r, i), r = !0;
+            if (sa(t, i), null === t.stateNode) null !== e && (e.alternate = null, t.alternate = null, t.effectTag |= 2), Oa(t, n, r), xa(t, n, r, i), r = !0;
             else if (null === e) {
                 var o = t.stateNode,
                     u = t.memoizedProps;
                 o.props = u;
                 var s = o.context,
                     c = n.contextType;
                 "object" === typeof c && null !== c ? c = ca(c) : c = ki(t, c = wi(n) ? gi : bi.current);
                 var l = n.getDerivedStateFromProps,
                     f = "function" === typeof l || "function" === typeof o.getSnapshotBeforeUpdate;
-                f || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== r || s !== c) && xa(t, o, r, c), la = !1;
+                f || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== r || s !== c) && ja(t, o, r, c), la = !1;
                 var h = t.memoizedState;
                 o.state = h, va(t, r, o, i), s = t.memoizedState, u !== r || h !== s || mi.current || la ? ("function" === typeof l && (ka(t, n, l, r), s = t.memoizedState), (u = la || _a(t, n, u, r, h, s, c)) ? (f || "function" !== typeof o.UNSAFE_componentWillMount && "function" !== typeof o.componentWillMount || ("function" === typeof o.componentWillMount && o.componentWillMount(), "function" === typeof o.UNSAFE_componentWillMount && o.UNSAFE_componentWillMount()), "function" === typeof o.componentDidMount && (t.effectTag |= 4)) : ("function" === typeof o.componentDidMount && (t.effectTag |= 4), t.memoizedProps = r, t.memoizedState = s), o.props = r, o.state = s, o.context = c, r = u) : ("function" === typeof o.componentDidMount && (t.effectTag |= 4), r = !1)
-            } else o = t.stateNode, ha(e, t), u = t.memoizedProps, o.props = t.type === t.elementType ? u : ea(t.type, u), s = o.context, "object" === typeof(c = n.contextType) && null !== c ? c = ca(c) : c = ki(t, c = wi(n) ? gi : bi.current), (f = "function" === typeof(l = n.getDerivedStateFromProps) || "function" === typeof o.getSnapshotBeforeUpdate) || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== r || s !== c) && xa(t, o, r, c), la = !1, s = t.memoizedState, o.state = s, va(t, r, o, i), h = t.memoizedState, u !== r || s !== h || mi.current || la ? ("function" === typeof l && (ka(t, n, l, r), h = t.memoizedState), (l = la || _a(t, n, u, r, s, h, c)) ? (f || "function" !== typeof o.UNSAFE_componentWillUpdate && "function" !== typeof o.componentWillUpdate || ("function" === typeof o.componentWillUpdate && o.componentWillUpdate(r, h, c), "function" === typeof o.UNSAFE_componentWillUpdate && o.UNSAFE_componentWillUpdate(r, h, c)), "function" === typeof o.componentDidUpdate && (t.effectTag |= 4), "function" === typeof o.getSnapshotBeforeUpdate && (t.effectTag |= 256)) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 256), t.memoizedProps = r, t.memoizedState = h), o.props = r, o.state = h, o.context = c, r = l) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 256), r = !1);
+            } else o = t.stateNode, ha(e, t), u = t.memoizedProps, o.props = t.type === t.elementType ? u : ea(t.type, u), s = o.context, "object" === typeof(c = n.contextType) && null !== c ? c = ca(c) : c = ki(t, c = wi(n) ? gi : bi.current), (f = "function" === typeof(l = n.getDerivedStateFromProps) || "function" === typeof o.getSnapshotBeforeUpdate) || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== r || s !== c) && ja(t, o, r, c), la = !1, s = t.memoizedState, o.state = s, va(t, r, o, i), h = t.memoizedState, u !== r || s !== h || mi.current || la ? ("function" === typeof l && (ka(t, n, l, r), h = t.memoizedState), (l = la || _a(t, n, u, r, s, h, c)) ? (f || "function" !== typeof o.UNSAFE_componentWillUpdate && "function" !== typeof o.componentWillUpdate || ("function" === typeof o.componentWillUpdate && o.componentWillUpdate(r, h, c), "function" === typeof o.UNSAFE_componentWillUpdate && o.UNSAFE_componentWillUpdate(r, h, c)), "function" === typeof o.componentDidUpdate && (t.effectTag |= 4), "function" === typeof o.getSnapshotBeforeUpdate && (t.effectTag |= 256)) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 256), t.memoizedProps = r, t.memoizedState = h), o.props = r, o.state = h, o.context = c, r = l) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && s === e.memoizedState || (t.effectTag |= 256), r = !1);
             return Yo(e, t, n, r, a, i)
         }
 
         function Yo(e, t, n, r, i, a) {
             Vo(e, t);
             var o = 0 !== (64 & t.effectTag);
             if (!r && !o) return i && Si(t, n, !1), tu(e, t, a);
@@ -20370,15 +20383,15 @@
                                     break;
                                 case "textarea":
                                     Be(r, u), Qt("invalid", r), cn(n, "onChange")
                             }
                             for (var s in on(a, u), e = null, u)
                                 if (u.hasOwnProperty(s)) {
                                     var c = u[s];
-                                    "children" === s ? "string" === typeof c ? r.textContent !== c && (e = ["children", c]) : "number" === typeof c && r.textContent !== "" + c && (e = ["children", "" + c]) : x.hasOwnProperty(s) && null != c && cn(n, s)
+                                    "children" === s ? "string" === typeof c ? r.textContent !== c && (e = ["children", c]) : "number" === typeof c && r.textContent !== "" + c && (e = ["children", "" + c]) : j.hasOwnProperty(s) && null != c && cn(n, s)
                                 } switch (a) {
                                 case "input":
                                     ke(r), Se(r, u, !0);
                                     break;
                                 case "textarea":
                                     ke(r), Le(r);
                                     break;
@@ -20437,15 +20450,15 @@
                                     c = r
                             }
                             on(a, c);
                             var l = c;
                             for (u in l)
                                 if (l.hasOwnProperty(u)) {
                                     var f = l[u];
-                                    "style" === u ? rn(e, f) : "dangerouslySetInnerHTML" === u ? null != (f = f ? f.__html : void 0) && Re(e, f) : "children" === u ? "string" === typeof f ? ("textarea" !== a || "" !== f) && Ve(e, f) : "number" === typeof f && Ve(e, "" + f) : "suppressContentEditableWarning" !== u && "suppressHydrationWarning" !== u && "autoFocus" !== u && (x.hasOwnProperty(u) ? null != f && cn(n, u) : null != f && J(e, u, f, s))
+                                    "style" === u ? rn(e, f) : "dangerouslySetInnerHTML" === u ? null != (f = f ? f.__html : void 0) && Re(e, f) : "children" === u ? "string" === typeof f ? ("textarea" !== a || "" !== f) && Ve(e, f) : "number" === typeof f && Ve(e, "" + f) : "suppressContentEditableWarning" !== u && "suppressHydrationWarning" !== u && "autoFocus" !== u && (j.hasOwnProperty(u) ? null != f && cn(n, u) : null != f && J(e, u, f, s))
                                 } switch (a) {
                                 case "input":
                                     ke(e), Se(e, r, !1);
                                     break;
                                 case "textarea":
                                     ke(e), Le(e);
                                     break;
@@ -20573,24 +20586,24 @@
                     default:
                         "function" !== typeof o.onClick && "function" === typeof r.onClick && (c.onclick = ln)
                 }
                 for (u in on(n, r), n = null, o)
                     if (!r.hasOwnProperty(u) && o.hasOwnProperty(u) && null != o[u])
                         if ("style" === u)
                             for (s in c = o[u]) c.hasOwnProperty(s) && (n || (n = {}), n[s] = "");
-                        else "dangerouslySetInnerHTML" !== u && "children" !== u && "suppressContentEditableWarning" !== u && "suppressHydrationWarning" !== u && "autoFocus" !== u && (x.hasOwnProperty(u) ? e || (e = []) : (e = e || []).push(u, null));
+                        else "dangerouslySetInnerHTML" !== u && "children" !== u && "suppressContentEditableWarning" !== u && "suppressHydrationWarning" !== u && "autoFocus" !== u && (j.hasOwnProperty(u) ? e || (e = []) : (e = e || []).push(u, null));
                 for (u in r) {
                     var l = r[u];
                     if (c = null != o ? o[u] : void 0, r.hasOwnProperty(u) && l !== c && (null != l || null != c))
                         if ("style" === u)
                             if (c) {
                                 for (s in c) !c.hasOwnProperty(s) || l && l.hasOwnProperty(s) || (n || (n = {}), n[s] = "");
                                 for (s in l) l.hasOwnProperty(s) && c[s] !== l[s] && (n || (n = {}), n[s] = l[s])
                             } else n || (e || (e = []), e.push(u, n)), n = l;
-                    else "dangerouslySetInnerHTML" === u ? (l = l ? l.__html : void 0, c = c ? c.__html : void 0, null != l && c !== l && (e = e || []).push(u, l)) : "children" === u ? c === l || "string" !== typeof l && "number" !== typeof l || (e = e || []).push(u, "" + l) : "suppressContentEditableWarning" !== u && "suppressHydrationWarning" !== u && (x.hasOwnProperty(u) ? (null != l && cn(a, u), e || c === l || (e = [])) : (e = e || []).push(u, l))
+                    else "dangerouslySetInnerHTML" === u ? (l = l ? l.__html : void 0, c = c ? c.__html : void 0, null != l && c !== l && (e = e || []).push(u, l)) : "children" === u ? c === l || "string" !== typeof l && "number" !== typeof l || (e = e || []).push(u, "" + l) : "suppressContentEditableWarning" !== u && "suppressHydrationWarning" !== u && (j.hasOwnProperty(u) ? (null != l && cn(a, u), e || c === l || (e = [])) : (e = e || []).push(u, l))
                 }
                 n && (e = e || []).push("style", n), a = e, (t.updateQueue = a) && (t.effectTag |= 4)
             }
         }, qo = function(e, t, n, r) {
             n !== r && (t.effectTag |= 4)
         };
         var ou = "function" === typeof WeakSet ? WeakSet : Set;
@@ -20883,22 +20896,22 @@
                     var n = t.stateNode;
                     if (null != n) {
                         var r = t.memoizedProps,
                             i = null !== e ? e.memoizedProps : r;
                         e = t.type;
                         var a = t.updateQueue;
                         if (t.updateQueue = null, null !== a) {
-                            for (n[Bn] = r, "input" === e && "radio" === r.type && null != r.name && xe(n, r), un(e, i), t = un(e, r), i = 0; i < a.length; i += 2) {
+                            for (n[Bn] = r, "input" === e && "radio" === r.type && null != r.name && je(n, r), un(e, i), t = un(e, r), i = 0; i < a.length; i += 2) {
                                 var u = a[i],
                                     s = a[i + 1];
                                 "style" === u ? rn(n, s) : "dangerouslySetInnerHTML" === u ? Re(n, s) : "children" === u ? Ve(n, s) : J(n, u, s, t)
                             }
                             switch (e) {
                                 case "input":
-                                    je(n, r);
+                                    xe(n, r);
                                     break;
                                 case "textarea":
                                     De(n, r);
                                     break;
                                 case "select":
                                     t = n._wrapperState.wasMultiple, n._wrapperState.wasMultiple = !!r.multiple, null != (e = r.value) ? Ee(n, !!r.multiple, e, !1) : t !== !!r.multiple && (null != r.defaultValue ? Ee(n, !!r.multiple, r.defaultValue, !0) : Ee(n, !!r.multiple, r.multiple ? [] : "", !1))
                             }
@@ -20957,15 +20970,15 @@
             };
             var r = t.value;
             return n.callback = function() {
                 Xu || (Xu = !0, es = r), uu(e, t)
             }, n
         }
 
-        function xu(e, t, n) {
+        function ju(e, t, n) {
             (n = da(n, null)).tag = 3;
             var r = e.type.getDerivedStateFromError;
             if ("function" === typeof r) {
                 var i = t.value;
                 n.payload = function() {
                     return uu(e, t), r(i)
                 }
@@ -20975,15 +20988,15 @@
                 "function" !== typeof r && (null === ts ? ts = new Set([this]) : ts.add(this), uu(e, t));
                 var n = t.stack;
                 this.componentDidCatch(t.value, {
                     componentStack: null !== n ? n : ""
                 })
             }), n
         }
-        var ju, Su = Math.ceil,
+        var xu, Su = Math.ceil,
             Tu = G.ReactCurrentDispatcher,
             Iu = G.ReactCurrentOwner,
             Eu = 0,
             Au = 8,
             Bu = 16,
             Du = 32,
             Lu = 0,
@@ -21108,15 +21121,15 @@
             var n = ds(e);
             if (0 !== n) {
                 if (t = e.callbackNode, (Pu & (Bu | Du)) !== Eu) throw Error(o(327));
                 if (Ds(), e === Ru && n === zu || gs(e, n), null !== Vu) {
                     var r = Pu;
                     Pu |= Bu;
                     for (var i = ws();;) try {
-                        js();
+                        xs();
                         break
                     } catch (s) {
                         ks(e, s)
                     }
                     if (aa(), Pu = r, Tu.current = i, Wu === Fu) throw t = Yu, gs(e, n), Gs(e, n), ps(e), t;
                     if (null === Vu) switch (i = e.finishedWork = e.current.alternate, e.finishedExpirationTime = n, r = Wu, Ru = null, r) {
                         case Lu:
@@ -21135,15 +21148,15 @@
                                     }
                                 }
                                 if (0 !== (a = ds(e)) && a !== n) break;
                                 if (0 !== r && r !== n) {
                                     e.lastPingedTime = r;
                                     break
                                 }
-                                e.timeoutHandle = jn(Es.bind(null, e), i);
+                                e.timeoutHandle = xn(Es.bind(null, e), i);
                                 break
                             }
                             Es(e);
                             break;
                         case Nu:
                             if (Gs(e, n), n === (r = e.lastSuspendedTime) && (e.nextKnownPendingLevel = Is(i)), qu && (0 === (i = e.lastPingedTime) || i >= n)) {
                                 e.lastPingedTime = n, gs(e, n);
@@ -21151,25 +21164,25 @@
                             }
                             if (0 !== (i = ds(e)) && i !== n) break;
                             if (0 !== r && r !== n) {
                                 e.lastPingedTime = r;
                                 break
                             }
                             if (1073741823 !== $u ? r = 10 * (1073741821 - $u) - Hi() : 1073741823 === Hu ? r = 0 : (r = 10 * (1073741821 - Hu) - 5e3, 0 > (r = (i = Hi()) - r) && (r = 0), (n = 10 * (1073741821 - n) - i) < (r = (120 > r ? 120 : 480 > r ? 480 : 1080 > r ? 1080 : 1920 > r ? 1920 : 3e3 > r ? 3e3 : 4320 > r ? 4320 : 1960 * Su(r / 1960)) - r) && (r = n)), 10 < r) {
-                                e.timeoutHandle = jn(Es.bind(null, e), r);
+                                e.timeoutHandle = xn(Es.bind(null, e), r);
                                 break
                             }
                             Es(e);
                             break;
                         case Uu:
                             if (1073741823 !== Hu && null !== Ku) {
                                 a = Hu;
                                 var u = Ku;
                                 if (0 >= (r = 0 | u.busyMinDurationMs) ? r = 0 : (i = 0 | u.busyDelayMs, r = (a = Hi() - (10 * (1073741821 - a) - (0 | u.timeoutMs || 5e3))) <= i ? 0 : i + r - a), 10 < r) {
-                                    Gs(e, n), e.timeoutHandle = jn(Es.bind(null, e), r);
+                                    Gs(e, n), e.timeoutHandle = xn(Es.bind(null, e), r);
                                     break
                                 }
                             }
                             Es(e);
                             break;
                         default:
                             throw Error(o(329))
@@ -21183,15 +21196,15 @@
         function vs(e) {
             var t = e.lastExpiredTime;
             if (t = 0 !== t ? t : 1073741823, (Pu & (Bu | Du)) !== Eu) throw Error(o(327));
             if (Ds(), e === Ru && t === zu || gs(e, t), null !== Vu) {
                 var n = Pu;
                 Pu |= Bu;
                 for (var r = ws();;) try {
-                    xs();
+                    js();
                     break
                 } catch (i) {
                     ks(e, i)
                 }
                 if (aa(), Pu = n, Tu.current = r, Wu === Fu) throw n = Yu, gs(e, t), Gs(e, t), ps(e), n;
                 if (null !== Vu) throw Error(o(261));
                 e.finishedWork = e.current.alternate, e.finishedExpirationTime = t, Ru = null, Es(e), ps(e)
@@ -21319,15 +21332,15 @@
                                     s = u, f.effectTag |= 4096, f.expirationTime = t, ya(f, Ou(f, s, t));
                                     break e;
                                 case 1:
                                     s = u;
                                     var k = f.type,
                                         w = f.stateNode;
                                     if (0 === (64 & f.effectTag) && ("function" === typeof k.getDerivedStateFromError || null !== w && "function" === typeof w.componentDidCatch && (null === ts || !ts.has(w)))) {
-                                        f.effectTag |= 4096, f.expirationTime = t, ya(f, xu(f, s, t));
+                                        f.effectTag |= 4096, f.expirationTime = t, ya(f, ju(f, s, t));
                                         break e
                                     }
                             }
                             f = f.return
                         } while (null !== f)
                     }
                     Vu = Ts(Vu)
@@ -21348,24 +21361,24 @@
             e < Hu && 2 < e && (Hu = e), null !== t && e < $u && 2 < e && ($u = e, Ku = t)
         }
 
         function Os(e) {
             e > Qu && (Qu = e)
         }
 
-        function xs() {
+        function js() {
             for (; null !== Vu;) Vu = Ss(Vu)
         }
 
-        function js() {
+        function xs() {
             for (; null !== Vu && !Pi();) Vu = Ss(Vu)
         }
 
         function Ss(e) {
-            var t = ju(e.alternate, e, zu);
+            var t = xu(e.alternate, e, zu);
             return e.memoizedProps = e.pendingProps, null === t && (t = Ts(e)), Iu.current = null, t
         }
 
         function Ts(e) {
             Vu = e;
             do {
                 var t = Vu.alternate;
@@ -21523,18 +21536,18 @@
                 Kt = !!wn, _n = wn = null, e.current = n, Zu = i;
                 do {
                     try {
                         for (k = e; null !== Zu;) {
                             var O = Zu.effectTag;
                             if (36 & O && hu(k, Zu.alternate, Zu), 128 & O) {
                                 w = void 0;
-                                var x = Zu.ref;
-                                if (null !== x) {
-                                    var j = Zu.stateNode;
-                                    Zu.tag, w = j, "function" === typeof x ? x(w) : x.current = w
+                                var j = Zu.ref;
+                                if (null !== j) {
+                                    var x = Zu.stateNode;
+                                    Zu.tag, w = x, "function" === typeof j ? j(w) : j.current = w
                                 }
                             }
                             Zu = Zu.nextEffect
                         }
                     } catch (S) {
                         if (null === Zu) throw Error(o(330));
                         Cs(Zu, S), Zu = Zu.nextEffect
@@ -21600,15 +21613,15 @@
                     if (3 === n.tag) {
                         Fs(n, e, t);
                         break
                     }
                     if (1 === n.tag) {
                         var r = n.stateNode;
                         if ("function" === typeof n.type.getDerivedStateFromError || "function" === typeof r.componentDidCatch && (null === ts || !ts.has(r))) {
-                            pa(n, e = xu(n, e = au(t, e), 1073741823)), null !== (n = hs(n, 1073741823)) && ps(n);
+                            pa(n, e = ju(n, e = au(t, e), 1073741823)), null !== (n = hs(n, 1073741823)) && ps(n);
                             break
                         }
                     }
                     n = n.return
                 }
         }
 
@@ -21617,30 +21630,30 @@
             null !== r && r.delete(t), Ru === e && zu === n ? Wu === Nu || Wu === Mu && 1073741823 === Hu && Hi() - Gu < Ju ? gs(e, zu) : qu = !0 : qs(e, n) && (0 !== (t = e.lastPingedTime) && t < n || (e.lastPingedTime = n, ps(e)))
         }
 
         function Ns(e, t) {
             var n = e.stateNode;
             null !== n && n.delete(t), 0 === (t = 0) && (t = ls(t = cs(), e, null)), null !== (e = hs(e, t)) && ps(e)
         }
-        ju = function(e, t, n) {
+        xu = function(e, t, n) {
             var r = t.expirationTime;
             if (null !== e) {
                 var i = t.pendingProps;
                 if (e.memoizedProps !== i || mi.current) Mo = !0;
                 else {
                     if (r < n) {
                         switch (Mo = !1, t.tag) {
                             case 3:
                                 Ho(t), Fo();
                                 break;
                             case 5:
                                 if (Pa(t), 4 & t.mode && 1 !== n && i.hidden) return t.expirationTime = t.childExpirationTime = 1, null;
                                 break;
                             case 1:
-                                wi(t.type) && ji(t);
+                                wi(t.type) && xi(t);
                                 break;
                             case 4:
                                 Na(t, t.stateNode.containerInfo);
                                 break;
                             case 10:
                                 r = t.memoizedProps.value, i = t.type._context, yi(ta, i._currentValue), i._currentValue = r;
                                 break;
@@ -21661,19 +21674,19 @@
                 }
             } else Mo = !1;
             switch (t.expirationTime = 0, t.tag) {
                 case 2:
                     if (r = t.type, null !== e && (e.alternate = null, t.alternate = null, t.effectTag |= 2), e = t.pendingProps, i = ki(t, bi.current), sa(t, n), i = Xa(null, t, r, e, i, n), t.effectTag |= 1, "object" === typeof i && null !== i && "function" === typeof i.render && void 0 === i.$$typeof) {
                         if (t.tag = 1, t.memoizedState = null, t.updateQueue = null, wi(r)) {
                             var a = !0;
-                            ji(t)
+                            xi(t)
                         } else a = !1;
                         t.memoizedState = null !== i.state && void 0 !== i.state ? i.state : null, fa(t);
                         var u = r.getDerivedStateFromProps;
-                        "function" === typeof u && ka(t, r, u, e), i.updater = wa, t.stateNode = i, i._reactInternalFiber = t, ja(t, r, e, n), t = Yo(null, t, r, !0, a, n)
+                        "function" === typeof u && ka(t, r, u, e), i.updater = wa, t.stateNode = i, i._reactInternalFiber = t, xa(t, r, e, n), t = Yo(null, t, r, !0, a, n)
                     } else t.tag = 0, No(null, t, i, n), t = t.child;
                     return t;
                 case 16:
                     e: {
                         if (i = t.elementType, null !== e && (e.alternate = null, t.alternate = null, t.effectTag |= 2), e = t.pendingProps, function(e) {
                                 if (-1 === e._status) {
                                     e._status = 0;
@@ -21720,15 +21733,15 @@
                         if ((i = t.stateNode.hydrate) && (To = Tn(t.stateNode.containerInfo.firstChild), So = t, i = Io = !0), i)
                             for (n = Ba(t, null, r, n), t.child = n; n;) n.effectTag = -3 & n.effectTag | 1024, n = n.sibling;
                         else No(e, t, r, n), Fo();
                         t = t.child
                     }
                     return t;
                 case 5:
-                    return Pa(t), null === e && Bo(t), r = t.type, i = t.pendingProps, a = null !== e ? e.memoizedProps : null, u = i.children, xn(r, i) ? u = null : null !== a && xn(r, a) && (t.effectTag |= 16), Vo(e, t), 4 & t.mode && 1 !== n && i.hidden ? (t.expirationTime = t.childExpirationTime = 1, t = null) : (No(e, t, u, n), t = t.child), t;
+                    return Pa(t), null === e && Bo(t), r = t.type, i = t.pendingProps, a = null !== e ? e.memoizedProps : null, u = i.children, jn(r, i) ? u = null : null !== a && jn(r, a) && (t.effectTag |= 16), Vo(e, t), 4 & t.mode && 1 !== n && i.hidden ? (t.expirationTime = t.childExpirationTime = 1, t = null) : (No(e, t, u, n), t = t.child), t;
                 case 6:
                     return null === e && Bo(t), null;
                 case 13:
                     return Jo(e, t, n);
                 case 4:
                     return Na(t, t.stateNode.containerInfo), r = t.pendingProps, null === e ? t.child = Aa(t, null, r, n) : No(e, t, r, n), t.child;
                 case 11:
@@ -21786,15 +21799,15 @@
                 case 9:
                     return i = t.type, r = (a = t.pendingProps).children, sa(t, n), r = r(i = ca(i, a.unstable_observedBits)), t.effectTag |= 1, No(e, t, r, n), t.child;
                 case 14:
                     return a = ea(i = t.type, t.pendingProps), Po(e, t, i, a = ea(i.type, a), r, n);
                 case 15:
                     return Ro(e, t, t.type, t.pendingProps, r, n);
                 case 17:
-                    return r = t.type, i = t.pendingProps, i = t.elementType === r ? i : ea(r, i), null !== e && (e.alternate = null, t.alternate = null, t.effectTag |= 2), t.tag = 1, wi(r) ? (e = !0, ji(t)) : e = !1, sa(t, n), Oa(t, r, i), ja(t, r, i, n), Yo(null, t, r, !0, e, n);
+                    return r = t.type, i = t.pendingProps, i = t.elementType === r ? i : ea(r, i), null !== e && (e.alternate = null, t.alternate = null, t.effectTag |= 2), t.tag = 1, wi(r) ? (e = !0, xi(t)) : e = !1, sa(t, n), Oa(t, r, i), xa(t, r, i, n), Yo(null, t, r, !0, e, n);
                 case 19:
                     return eu(e, t, n)
             }
             throw Error(o(156, t.tag))
         };
         var Us = null,
             Ps = null;
@@ -21929,15 +21942,15 @@
                         s = s.return
                     } while (null !== s);
                     throw Error(o(171))
                 }
                 if (1 === n.tag) {
                     var c = n.type;
                     if (wi(c)) {
-                        n = xi(n, c, s);
+                        n = ji(n, c, s);
                         break e
                     }
                 }
                 n = s
             }
             else n = vi;
             return null === t.context ? t.context = n : t.pendingContext = n, (t = da(a, u)).payload = {
@@ -22040,22 +22053,22 @@
             if (13 === e.tag) {
                 var t = cs();
                 fs(e, t = ls(t, e, null)), nc(e, t)
             }
         }, I = function(e, t, n) {
             switch (t) {
                 case "input":
-                    if (je(e, n), t = n.name, "radio" === n.type && null != t) {
+                    if (xe(e, n), t = n.name, "radio" === n.type && null != t) {
                         for (n = e; n.parentNode;) n = n.parentNode;
                         for (n = n.querySelectorAll("input[name=" + JSON.stringify("" + t) + '][type="radio"]'), t = 0; t < n.length; t++) {
                             var r = n[t];
                             if (r !== e && r.form === e.form) {
                                 var i = Mn(r);
                                 if (!i) throw Error(o(90));
-                                we(r), je(r, i)
+                                we(r), xe(r, i)
                             }
                         }
                     }
                     break;
                 case "textarea":
                     De(e, n);
                     break;
@@ -22172,15 +22185,15 @@
         }, t.unstable_renderSubtreeIntoContainer = function(e, t, n, r) {
             if (!ic(n)) throw Error(o(200));
             if (null == e || void 0 === e._reactInternalFiber) throw Error(o(38));
             return ac(e, t, n, !1, r)
         }, t.version = "16.14.0"
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(20)
+        e.exports = n(22)
     }, function(e, t, n) {
         "use strict";
         var r, i, a, o, u;
         if ("undefined" === typeof window || "function" !== typeof MessageChannel) {
             var s = null,
                 c = null,
                 l = function e() {
@@ -22228,37 +22241,37 @@
                 _ = 0;
             o = function() {
                 return t.unstable_now() >= _
             }, u = function() {}, t.unstable_forceFrameRate = function(e) {
                 0 > e || 125 < e ? console.error("forceFrameRate takes a positive int between 0 and 125, forcing framerates higher than 125 fps is not unsupported") : w = 0 < e ? Math.floor(1e3 / e) : 5
             };
             var O = new MessageChannel,
-                x = O.port2;
+                j = O.port2;
             O.port1.onmessage = function() {
                 if (null !== g) {
                     var e = t.unstable_now();
                     _ = e + w;
                     try {
-                        g(!0, e) ? x.postMessage(null) : (m = !1, g = null)
+                        g(!0, e) ? j.postMessage(null) : (m = !1, g = null)
                     } catch (n) {
-                        throw x.postMessage(null), n
+                        throw j.postMessage(null), n
                     }
                 } else m = !1
             }, r = function(e) {
-                g = e, m || (m = !0, x.postMessage(null))
+                g = e, m || (m = !0, j.postMessage(null))
             }, i = function(e, n) {
                 k = p((function() {
                     e(t.unstable_now())
                 }), n)
             }, a = function() {
                 y(k), k = -1
             }
         }
 
-        function j(e, t) {
+        function x(e, t) {
             var n = e.length;
             e.push(t);
             e: for (;;) {
                 var r = n - 1 >>> 1,
                     i = e[r];
                 if (!(void 0 !== i && 0 < I(i, t))) break e;
                 e[r] = t, e[n] = i, n = r
@@ -22306,15 +22319,15 @@
             M = !1;
 
         function N(e) {
             for (var t = S(A); null !== t;) {
                 if (null === t.callback) T(A);
                 else {
                     if (!(t.startTime <= e)) break;
-                    T(A), t.sortIndex = t.expirationTime, j(E, t)
+                    T(A), t.sortIndex = t.expirationTime, x(E, t)
                 }
                 t = S(A)
             }
         }
 
         function U(e) {
             if (M = !1, N(e), !C)
@@ -22416,15 +22429,15 @@
             return e = {
                 id: B++,
                 callback: n,
                 priorityLevel: e,
                 startTime: s,
                 expirationTime: o = s + o,
                 sortIndex: -1
-            }, s > u ? (e.sortIndex = s, j(A, e), null === S(E) && e === S(A) && (M ? a() : M = !0, i(U, s - u))) : (e.sortIndex = o, j(E, e), C || F || (C = !0, r(P))), e
+            }, s > u ? (e.sortIndex = s, x(A, e), null === S(E) && e === S(A) && (M ? a() : M = !0, i(U, s - u))) : (e.sortIndex = o, x(E, e), C || F || (C = !0, r(P))), e
         }, t.unstable_shouldYield = function() {
             var e = t.unstable_now();
             N(e);
             var n = S(E);
             return n !== D && null !== D && null !== n && null !== n.callback && n.startTime <= e && n.expirationTime < D.expirationTime || o()
         }, t.unstable_wrapCallback = function(e) {
             var t = L;
@@ -22436,15 +22449,15 @@
                 } finally {
                     L = n
                 }
             }
         }
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(22)
+        e.exports = n(24)
     }, function(e, t, n) {
         "use strict";
         var r = "function" === typeof Symbol && Symbol.for,
             i = r ? Symbol.for("react.element") : 60103,
             a = r ? Symbol.for("react.portal") : 60106,
             o = r ? Symbol.for("react.fragment") : 60107,
             u = r ? Symbol.for("react.strict_mode") : 60108,
@@ -22522,15 +22535,15 @@
         }, t.isSuspense = function(e) {
             return _(e) === p
         }, t.isValidElementType = function(e) {
             return "string" === typeof e || "function" === typeof e || e === o || e === h || e === s || e === u || e === p || e === y || "object" === typeof e && null !== e && (e.$$typeof === b || e.$$typeof === v || e.$$typeof === c || e.$$typeof === l || e.$$typeof === d || e.$$typeof === g || e.$$typeof === k || e.$$typeof === w || e.$$typeof === m)
         }, t.typeOf = _
     }, function(e, t, n) {
         "use strict";
-        var r = n(6),
+        var r = n(8),
             i = 60103;
         if (t.Fragment = 60107, "function" === typeof Symbol && Symbol.for) {
             var a = Symbol.for;
             i = a("react.element"), t.Fragment = a("react.fragment")
         }
         var o = r.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
             u = Object.prototype.hasOwnProperty,
@@ -22556,8 +22569,8 @@
                 props: a,
                 _owner: o.current
             }
         }
         t.jsx = c, t.jsxs = c
     }]
 ]);
-//# sourceMappingURL=2.cfa3d2aa.chunk.js.map
+//# sourceMappingURL=2.38865783.chunk.js.map
```

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js.LICENSE.txt` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js.map` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8528292593658736%*

 * *Differences: {"'file'": "'static/js/2.38865783.chunk.js'",*

 * * "'mappings'": "';sHAAA,8CACA,SAASA,EAAkBC,EAAQC,GACjC,IAAK,IAAIC,EAAI,EAAGA,EAAID,EAAME,OAAQD,IAAK,CACrC,IAAIE,EAAaH,EAAMC,GACvBE,EAAWC,WAAaD,EAAWC,aAAc,EACjDD,EAAWE,cAAe,EACtB,UAAWF,IAAYA,EAAWG,UAAW,GACjDC,OAAOC,eAAeT,EAAQ,YAAcI,EAAWM,KAAMN,EAC/D,CACF,CACe,SAASO,EAAaC,EAAaC,EAAYC,GAM5D,OALID,GAAYd,EAAkBa,EAAYG,UAAWF,GACrDC,GAAaf,EAAkBa,EAAaE,GAChDN,OAAOC,eAAeG,EAAa,YAAa,CAC9CL,UAAU,IAELK,CACT,C,+BCjBe,SAASI,EAAgBC,EAAUL,GAChD,KAAMK,aAAoBL,GACxB,MAAM,IAAIM,UAAU […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.cfa3d2aa.chunk.js",
+    "file": "static/js/2.38865783.chunk.js",
     "names": [
         "_defineProperties",
         "target",
         "props",
         "i",
         "length",
         "descriptor",
@@ -41,19 +41,35 @@
         "apply",
         "_getPrototypeOf",
         "o",
         "setPrototypeOf",
         "getPrototypeOf",
         "bind",
         "__proto__",
+        "ownKeys",
+        "object",
+        "enumerableOnly",
+        "keys",
+        "getOwnPropertySymbols",
+        "symbols",
+        "filter",
+        "sym",
+        "getOwnPropertyDescriptor",
+        "push",
+        "_objectSpread2",
+        "source",
+        "forEach",
+        "getOwnPropertyDescriptors",
+        "defineProperties",
+        "_defineProperty",
+        "obj",
         "module",
         "exports",
         "require",
         "_typeof",
-        "obj",
         "Symbol",
         "iterator",
         "_possibleConstructorReturn",
         "self",
         "call",
         "_assertThisInitialized",
         "ReferenceError",
@@ -97,24 +113,22 @@
         "eventPhase",
         "currentTarget",
         "stopped",
         "immediateStopped",
         "timeStamp",
         "Date",
         "now",
-        "keys",
         "defineRedirectDescriptor",
         "defineCallDescriptor",
         "getWrapper",
         "proto",
         "wrapper",
         "BaseEvent",
         "CustomEvent",
         "isFunc",
-        "getOwnPropertyDescriptor",
         "defineWrapper",
         "isStopped",
         "setPassiveListener",
         "type",
         "composedPath",
         "NONE",
         "CAPTURING_PHASE",
@@ -234,15 +248,14 @@
         "GeneratorFunctionPrototype",
         "IteratorPrototype",
         "getProto",
         "NativeIteratorPrototype",
         "values",
         "Gp",
         "defineIteratorMethods",
-        "forEach",
         "method",
         "_invoke",
         "AsyncIterator",
         "PromiseImpl",
         "invoke",
         "record",
         "__await",
@@ -266,15 +279,14 @@
         "locs",
         "entry",
         "tryLoc",
         "catchLoc",
         "finallyLoc",
         "afterLoc",
         "tryEntries",
-        "push",
         "resetTryEntry",
         "completion",
         "reset",
         "iterable",
         "iteratorMethod",
         "isNaN",
         "displayName",
@@ -282,15 +294,14 @@
         "genFun",
         "ctor",
         "mark",
         "awrap",
         "async",
         "iter",
         "val",
-        "object",
         "reverse",
         "pop",
         "skipTempReset",
         "charAt",
         "stop",
         "rootRecord",
         "rval",
@@ -638,15 +649,14 @@
         "isFetchResponse",
         "isReadableDOMStream",
         "isReadableNodeStream",
         "toArrayBufferViewIterator",
         "SharedArrayBuf",
         "SharedArrayBuffer",
         "memcpy",
-        "source",
         "targetByteOffset",
         "sourceByteLength",
         "targetByteLength",
         "dst",
         "src",
         "Math",
         "joinUint8Arrays",
@@ -780,24 +790,14 @@
         "destroy",
         "_x11",
         "_x12",
         "_joinUint8Arrays8",
         "race",
         "map",
         "isFinite",
-        "_defineProperty",
-        "toPropertyKey",
-        "enumerableOnly",
-        "getOwnPropertySymbols",
-        "symbols",
-        "filter",
-        "sym",
-        "_objectSpread2",
-        "getOwnPropertyDescriptors",
-        "defineProperties",
         "property",
         "receiver",
         "base",
         "org",
         "flatbuf",
         "arrow",
         "apache",
@@ -1465,15 +1465,14 @@
         "setter",
         "_iterator3",
         "getKey",
         "RowProxyHandler",
         "isExtensible",
         "deleteProperty",
         "preventExtensions",
-        "ownKeys",
         "clampIndex",
         "adjust",
         "clampRange",
         "end",
         "_source$length",
         "big0",
         "isNaNFast",
@@ -3576,14 +3575,16 @@
     "sourceRoot": "",
     "sources": [
         "../node_modules/@babel/runtime/helpers/esm/createClass.js",
         "../node_modules/@babel/runtime/helpers/esm/classCallCheck.js",
         "../node_modules/@babel/runtime/helpers/esm/inherits.js",
         "../node_modules/@babel/runtime/helpers/esm/createSuper.js",
         "../node_modules/@babel/runtime/helpers/esm/getPrototypeOf.js",
+        "../node_modules/@babel/runtime/helpers/esm/objectSpread2.js",
+        "../node_modules/@babel/runtime/helpers/esm/defineProperty.js",
         "../node_modules/react/jsx-runtime.js",
         "../node_modules/react/index.js",
         "../node_modules/@babel/runtime/helpers/esm/typeof.js",
         "../node_modules/@babel/runtime/helpers/esm/possibleConstructorReturn.js",
         "../node_modules/@babel/runtime/helpers/esm/assertThisInitialized.js",
         "../node_modules/@babel/runtime/helpers/esm/setPrototypeOf.js",
         "../node_modules/@babel/runtime/helpers/esm/isNativeReflectConstruct.js",
@@ -3609,16 +3610,14 @@
         "../node_modules/flatbuffers/js/flatbuffers.mjs",
         "../node_modules/text-encoding-utf-8/lib/encoding.lib.mjs",
         "../util/utf8.ts",
         "../io/interfaces.ts",
         "../util/compat.ts",
         "../util/buffer.ts",
         "../io/adapters.ts",
-        "../node_modules/@babel/runtime/helpers/esm/defineProperty.js",
-        "../node_modules/@babel/runtime/helpers/esm/objectSpread2.js",
         "../node_modules/@babel/runtime/helpers/esm/get.js",
         "../node_modules/@babel/runtime/helpers/esm/superPropBase.js",
         "../vector.ts",
         "../fb/Schema.ts",
         "../fb/Message.ts",
         "../enum.ts",
         "../util/bit.ts",
@@ -3734,14 +3733,16 @@
     ],
     "sourcesContent": [
         "import toPropertyKey from \"./toPropertyKey.js\";\nfunction _defineProperties(target, props) {\n  for (var i = 0; i < props.length; i++) {\n    var descriptor = props[i];\n    descriptor.enumerable = descriptor.enumerable || false;\n    descriptor.configurable = true;\n    if (\"value\" in descriptor) descriptor.writable = true;\n    Object.defineProperty(target, toPropertyKey(descriptor.key), descriptor);\n  }\n}\nexport default function _createClass(Constructor, protoProps, staticProps) {\n  if (protoProps) _defineProperties(Constructor.prototype, protoProps);\n  if (staticProps) _defineProperties(Constructor, staticProps);\n  Object.defineProperty(Constructor, \"prototype\", {\n    writable: false\n  });\n  return Constructor;\n}",
         "export default function _classCallCheck(instance, Constructor) {\n  if (!(instance instanceof Constructor)) {\n    throw new TypeError(\"Cannot call a class as a function\");\n  }\n}",
         "import setPrototypeOf from \"./setPrototypeOf.js\";\nexport default function _inherits(subClass, superClass) {\n  if (typeof superClass !== \"function\" && superClass !== null) {\n    throw new TypeError(\"Super expression must either be null or a function\");\n  }\n  subClass.prototype = Object.create(superClass && superClass.prototype, {\n    constructor: {\n      value: subClass,\n      writable: true,\n      configurable: true\n    }\n  });\n  Object.defineProperty(subClass, \"prototype\", {\n    writable: false\n  });\n  if (superClass) setPrototypeOf(subClass, superClass);\n}",
         "import getPrototypeOf from \"./getPrototypeOf.js\";\nimport isNativeReflectConstruct from \"./isNativeReflectConstruct.js\";\nimport possibleConstructorReturn from \"./possibleConstructorReturn.js\";\nexport default function _createSuper(Derived) {\n  var hasNativeReflectConstruct = isNativeReflectConstruct();\n  return function _createSuperInternal() {\n    var Super = getPrototypeOf(Derived),\n      result;\n    if (hasNativeReflectConstruct) {\n      var NewTarget = getPrototypeOf(this).constructor;\n      result = Reflect.construct(Super, arguments, NewTarget);\n    } else {\n      result = Super.apply(this, arguments);\n    }\n    return possibleConstructorReturn(this, result);\n  };\n}",
         "export default function _getPrototypeOf(o) {\n  _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function _getPrototypeOf(o) {\n    return o.__proto__ || Object.getPrototypeOf(o);\n  };\n  return _getPrototypeOf(o);\n}",
+        "import defineProperty from \"./defineProperty.js\";\nfunction ownKeys(object, enumerableOnly) {\n  var keys = Object.keys(object);\n  if (Object.getOwnPropertySymbols) {\n    var symbols = Object.getOwnPropertySymbols(object);\n    enumerableOnly && (symbols = symbols.filter(function (sym) {\n      return Object.getOwnPropertyDescriptor(object, sym).enumerable;\n    })), keys.push.apply(keys, symbols);\n  }\n  return keys;\n}\nexport default function _objectSpread2(target) {\n  for (var i = 1; i < arguments.length; i++) {\n    var source = null != arguments[i] ? arguments[i] : {};\n    i % 2 ? ownKeys(Object(source), !0).forEach(function (key) {\n      defineProperty(target, key, source[key]);\n    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)) : ownKeys(Object(source)).forEach(function (key) {\n      Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));\n    });\n  }\n  return target;\n}",
+        "import toPropertyKey from \"./toPropertyKey.js\";\nexport default function _defineProperty(obj, key, value) {\n  key = toPropertyKey(key);\n  if (key in obj) {\n    Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: true,\n      configurable: true,\n      writable: true\n    });\n  } else {\n    obj[key] = value;\n  }\n  return obj;\n}",
         "'use strict';\n\nif (process.env.NODE_ENV === 'production') {\n  module.exports = require('./cjs/react-jsx-runtime.production.min.js');\n} else {\n  module.exports = require('./cjs/react-jsx-runtime.development.js');\n}\n",
         "'use strict';\n\nif (process.env.NODE_ENV === 'production') {\n  module.exports = require('./cjs/react.production.min.js');\n} else {\n  module.exports = require('./cjs/react.development.js');\n}\n",
         "export default function _typeof(obj) {\n  \"@babel/helpers - typeof\";\n\n  return _typeof = \"function\" == typeof Symbol && \"symbol\" == typeof Symbol.iterator ? function (obj) {\n    return typeof obj;\n  } : function (obj) {\n    return obj && \"function\" == typeof Symbol && obj.constructor === Symbol && obj !== Symbol.prototype ? \"symbol\" : typeof obj;\n  }, _typeof(obj);\n}",
         "import _typeof from \"./typeof.js\";\nimport assertThisInitialized from \"./assertThisInitialized.js\";\nexport default function _possibleConstructorReturn(self, call) {\n  if (call && (_typeof(call) === \"object\" || typeof call === \"function\")) {\n    return call;\n  } else if (call !== void 0) {\n    throw new TypeError(\"Derived constructors may only return object or undefined\");\n  }\n  return assertThisInitialized(self);\n}",
         "export default function _assertThisInitialized(self) {\n  if (self === void 0) {\n    throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\");\n  }\n  return self;\n}",
         "export default function _setPrototypeOf(o, p) {\n  _setPrototypeOf = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function _setPrototypeOf(o, p) {\n    o.__proto__ = p;\n    return o;\n  };\n  return _setPrototypeOf(o, p);\n}",
         "export default function _isNativeReflectConstruct() {\n  if (typeof Reflect === \"undefined\" || !Reflect.construct) return false;\n  if (Reflect.construct.sham) return false;\n  if (typeof Proxy === \"function\") return true;\n  try {\n    Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function () {}));\n    return true;\n  } catch (e) {\n    return false;\n  }\n}",
@@ -3767,16 +3768,14 @@
         "/// @file\n/// @addtogroup flatbuffers_javascript_api\n/// @{\n/// @cond FLATBUFFERS_INTERNAL\n\n/**\n * @fileoverview\n *\n * Need to suppress 'global this' error so the Node.js export line doesn't cause\n * closure compile to error out.\n * @suppress {globalThis}\n */\n\n/**\n * @const\n * @namespace\n */\nvar flatbuffers = {};\n\n/**\n * @typedef {number}\n */\nflatbuffers.Offset;\n\n/**\n * @typedef {{\n *   bb: flatbuffers.ByteBuffer,\n *   bb_pos: number\n * }}\n */\nflatbuffers.Table;\n\n/**\n * @type {number}\n * @const\n */\nflatbuffers.SIZEOF_SHORT = 2;\n\n/**\n * @type {number}\n * @const\n */\nflatbuffers.SIZEOF_INT = 4;\n\n/**\n * @type {number}\n * @const\n */\nflatbuffers.FILE_IDENTIFIER_LENGTH = 4;\n\n/**\n * @enum {number}\n */\nflatbuffers.Encoding = {\n  UTF8_BYTES: 1,\n  UTF16_STRING: 2\n};\n\n/**\n * @type {Int32Array}\n * @const\n */\nflatbuffers.int32 = new Int32Array(2);\n\n/**\n * @type {Float32Array}\n * @const\n */\nflatbuffers.float32 = new Float32Array(flatbuffers.int32.buffer);\n\n/**\n * @type {Float64Array}\n * @const\n */\nflatbuffers.float64 = new Float64Array(flatbuffers.int32.buffer);\n\n/**\n * @type {boolean}\n * @const\n */\nflatbuffers.isLittleEndian = new Uint16Array(new Uint8Array([1, 0]).buffer)[0] === 1;\n\n////////////////////////////////////////////////////////////////////////////////\n\n/**\n * @constructor\n * @param {number} low\n * @param {number} high\n */\nflatbuffers.Long = function(low, high) {\n  /**\n   * @type {number}\n   * @const\n   */\n  this.low = low | 0;\n\n  /**\n   * @type {number}\n   * @const\n   */\n  this.high = high | 0;\n};\n\n/**\n * @param {number} low\n * @param {number} high\n * @returns {flatbuffers.Long}\n */\nflatbuffers.Long.create = function(low, high) {\n  // Special-case zero to avoid GC overhead for default values\n  return low == 0 && high == 0 ? flatbuffers.Long.ZERO : new flatbuffers.Long(low, high);\n};\n\n/**\n * @returns {number}\n */\nflatbuffers.Long.prototype.toFloat64 = function() {\n  return (this.low >>> 0) + this.high * 0x100000000;\n};\n\n/**\n * @param {flatbuffers.Long} other\n * @returns {boolean}\n */\nflatbuffers.Long.prototype.equals = function(other) {\n  return this.low == other.low && this.high == other.high;\n};\n\n/**\n * @type {flatbuffers.Long}\n * @const\n */\nflatbuffers.Long.ZERO = new flatbuffers.Long(0, 0);\n\n/// @endcond\n////////////////////////////////////////////////////////////////////////////////\n/**\n * Create a FlatBufferBuilder.\n *\n * @constructor\n * @param {number=} opt_initial_size\n */\nflatbuffers.Builder = function(opt_initial_size) {\n  if (!opt_initial_size) {\n    var initial_size = 1024;\n  } else {\n    var initial_size = opt_initial_size;\n  }\n\n  /**\n   * @type {flatbuffers.ByteBuffer}\n   * @private\n   */\n  this.bb = flatbuffers.ByteBuffer.allocate(initial_size);\n\n  /**\n   * Remaining space in the ByteBuffer.\n   *\n   * @type {number}\n   * @private\n   */\n  this.space = initial_size;\n\n  /**\n   * Minimum alignment encountered so far.\n   *\n   * @type {number}\n   * @private\n   */\n  this.minalign = 1;\n\n  /**\n   * The vtable for the current table.\n   *\n   * @type {Array.<number>}\n   * @private\n   */\n  this.vtable = null;\n\n  /**\n   * The amount of fields we're actually using.\n   *\n   * @type {number}\n   * @private\n   */\n  this.vtable_in_use = 0;\n\n  /**\n   * Whether we are currently serializing a table.\n   *\n   * @type {boolean}\n   * @private\n   */\n  this.isNested = false;\n\n  /**\n   * Starting offset of the current struct/table.\n   *\n   * @type {number}\n   * @private\n   */\n  this.object_start = 0;\n\n  /**\n   * List of offsets of all vtables.\n   *\n   * @type {Array.<number>}\n   * @private\n   */\n  this.vtables = [];\n\n  /**\n   * For the current vector being built.\n   *\n   * @type {number}\n   * @private\n   */\n  this.vector_num_elems = 0;\n\n  /**\n   * False omits default values from the serialized data\n   *\n   * @type {boolean}\n   * @private\n   */\n  this.force_defaults = false;\n};\n\nflatbuffers.Builder.prototype.clear = function() {\n  this.bb.clear();\n  this.space = this.bb.capacity();\n  this.minalign = 1;\n  this.vtable = null;\n  this.vtable_in_use = 0;\n  this.isNested = false;\n  this.object_start = 0;\n  this.vtables = [];\n  this.vector_num_elems = 0;\n  this.force_defaults = false;\n};\n\n/**\n * In order to save space, fields that are set to their default value\n * don't get serialized into the buffer. Forcing defaults provides a\n * way to manually disable this optimization.\n *\n * @param {boolean} forceDefaults true always serializes default values\n */\nflatbuffers.Builder.prototype.forceDefaults = function(forceDefaults) {\n  this.force_defaults = forceDefaults;\n};\n\n/**\n * Get the ByteBuffer representing the FlatBuffer. Only call this after you've\n * called finish(). The actual data starts at the ByteBuffer's current position,\n * not necessarily at 0.\n *\n * @returns {flatbuffers.ByteBuffer}\n */\nflatbuffers.Builder.prototype.dataBuffer = function() {\n  return this.bb;\n};\n\n/**\n * Get the bytes representing the FlatBuffer. Only call this after you've\n * called finish().\n *\n * @returns {Uint8Array}\n */\nflatbuffers.Builder.prototype.asUint8Array = function() {\n  return this.bb.bytes().subarray(this.bb.position(), this.bb.position() + this.offset());\n};\n\n/// @cond FLATBUFFERS_INTERNAL\n/**\n * Prepare to write an element of `size` after `additional_bytes` have been\n * written, e.g. if you write a string, you need to align such the int length\n * field is aligned to 4 bytes, and the string data follows it directly. If all\n * you need to do is alignment, `additional_bytes` will be 0.\n *\n * @param {number} size This is the of the new element to write\n * @param {number} additional_bytes The padding size\n */\nflatbuffers.Builder.prototype.prep = function(size, additional_bytes) {\n  // Track the biggest thing we've ever aligned to.\n  if (size > this.minalign) {\n    this.minalign = size;\n  }\n\n  // Find the amount of alignment needed such that `size` is properly\n  // aligned after `additional_bytes`\n  var align_size = ((~(this.bb.capacity() - this.space + additional_bytes)) + 1) & (size - 1);\n\n  // Reallocate the buffer if needed.\n  while (this.space < align_size + size + additional_bytes) {\n    var old_buf_size = this.bb.capacity();\n    this.bb = flatbuffers.Builder.growByteBuffer(this.bb);\n    this.space += this.bb.capacity() - old_buf_size;\n  }\n\n  this.pad(align_size);\n};\n\n/**\n * @param {number} byte_size\n */\nflatbuffers.Builder.prototype.pad = function(byte_size) {\n  for (var i = 0; i < byte_size; i++) {\n    this.bb.writeInt8(--this.space, 0);\n  }\n};\n\n/**\n * @param {number} value\n */\nflatbuffers.Builder.prototype.writeInt8 = function(value) {\n  this.bb.writeInt8(this.space -= 1, value);\n};\n\n/**\n * @param {number} value\n */\nflatbuffers.Builder.prototype.writeInt16 = function(value) {\n  this.bb.writeInt16(this.space -= 2, value);\n};\n\n/**\n * @param {number} value\n */\nflatbuffers.Builder.prototype.writeInt32 = function(value) {\n  this.bb.writeInt32(this.space -= 4, value);\n};\n\n/**\n * @param {flatbuffers.Long} value\n */\nflatbuffers.Builder.prototype.writeInt64 = function(value) {\n  this.bb.writeInt64(this.space -= 8, value);\n};\n\n/**\n * @param {number} value\n */\nflatbuffers.Builder.prototype.writeFloat32 = function(value) {\n  this.bb.writeFloat32(this.space -= 4, value);\n};\n\n/**\n * @param {number} value\n */\nflatbuffers.Builder.prototype.writeFloat64 = function(value) {\n  this.bb.writeFloat64(this.space -= 8, value);\n};\n/// @endcond\n\n/**\n * Add an `int8` to the buffer, properly aligned, and grows the buffer (if necessary).\n * @param {number} value The `int8` to add the the buffer.\n */\nflatbuffers.Builder.prototype.addInt8 = function(value) {\n  this.prep(1, 0);\n  this.writeInt8(value);\n};\n\n/**\n * Add an `int16` to the buffer, properly aligned, and grows the buffer (if necessary).\n * @param {number} value The `int16` to add the the buffer.\n */\nflatbuffers.Builder.prototype.addInt16 = function(value) {\n  this.prep(2, 0);\n  this.writeInt16(value);\n};\n\n/**\n * Add an `int32` to the buffer, properly aligned, and grows the buffer (if necessary).\n * @param {number} value The `int32` to add the the buffer.\n */\nflatbuffers.Builder.prototype.addInt32 = function(value) {\n  this.prep(4, 0);\n  this.writeInt32(value);\n};\n\n/**\n * Add an `int64` to the buffer, properly aligned, and grows the buffer (if necessary).\n * @param {flatbuffers.Long} value The `int64` to add the the buffer.\n */\nflatbuffers.Builder.prototype.addInt64 = function(value) {\n  this.prep(8, 0);\n  this.writeInt64(value);\n};\n\n/**\n * Add a `float32` to the buffer, properly aligned, and grows the buffer (if necessary).\n * @param {number} value The `float32` to add the the buffer.\n */\nflatbuffers.Builder.prototype.addFloat32 = function(value) {\n  this.prep(4, 0);\n  this.writeFloat32(value);\n};\n\n/**\n * Add a `float64` to the buffer, properly aligned, and grows the buffer (if necessary).\n * @param {number} value The `float64` to add the the buffer.\n */\nflatbuffers.Builder.prototype.addFloat64 = function(value) {\n  this.prep(8, 0);\n  this.writeFloat64(value);\n};\n\n/// @cond FLATBUFFERS_INTERNAL\n/**\n * @param {number} voffset\n * @param {number} value\n * @param {number} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldInt8 = function(voffset, value, defaultValue) {\n  if (this.force_defaults || value != defaultValue) {\n    this.addInt8(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * @param {number} voffset\n * @param {number} value\n * @param {number} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldInt16 = function(voffset, value, defaultValue) {\n  if (this.force_defaults || value != defaultValue) {\n    this.addInt16(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * @param {number} voffset\n * @param {number} value\n * @param {number} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldInt32 = function(voffset, value, defaultValue) {\n  if (this.force_defaults || value != defaultValue) {\n    this.addInt32(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * @param {number} voffset\n * @param {flatbuffers.Long} value\n * @param {flatbuffers.Long} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldInt64 = function(voffset, value, defaultValue) {\n  if (this.force_defaults || !value.equals(defaultValue)) {\n    this.addInt64(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * @param {number} voffset\n * @param {number} value\n * @param {number} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldFloat32 = function(voffset, value, defaultValue) {\n  if (this.force_defaults || value != defaultValue) {\n    this.addFloat32(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * @param {number} voffset\n * @param {number} value\n * @param {number} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldFloat64 = function(voffset, value, defaultValue) {\n  if (this.force_defaults || value != defaultValue) {\n    this.addFloat64(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * @param {number} voffset\n * @param {flatbuffers.Offset} value\n * @param {flatbuffers.Offset} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldOffset = function(voffset, value, defaultValue) {\n  if (this.force_defaults || value != defaultValue) {\n    this.addOffset(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * Structs are stored inline, so nothing additional is being added. `d` is always 0.\n *\n * @param {number} voffset\n * @param {flatbuffers.Offset} value\n * @param {flatbuffers.Offset} defaultValue\n */\nflatbuffers.Builder.prototype.addFieldStruct = function(voffset, value, defaultValue) {\n  if (value != defaultValue) {\n    this.nested(value);\n    this.slot(voffset);\n  }\n};\n\n/**\n * Structures are always stored inline, they need to be created right\n * where they're used.  You'll get this assertion failure if you\n * created it elsewhere.\n *\n * @param {flatbuffers.Offset} obj The offset of the created object\n */\nflatbuffers.Builder.prototype.nested = function(obj) {\n  if (obj != this.offset()) {\n    throw new Error('FlatBuffers: struct must be serialized inline.');\n  }\n};\n\n/**\n * Should not be creating any other object, string or vector\n * while an object is being constructed\n */\nflatbuffers.Builder.prototype.notNested = function() {\n  if (this.isNested) {\n    throw new Error('FlatBuffers: object serialization must not be nested.');\n  }\n};\n\n/**\n * Set the current vtable at `voffset` to the current location in the buffer.\n *\n * @param {number} voffset\n */\nflatbuffers.Builder.prototype.slot = function(voffset) {\n  this.vtable[voffset] = this.offset();\n};\n\n/**\n * @returns {flatbuffers.Offset} Offset relative to the end of the buffer.\n */\nflatbuffers.Builder.prototype.offset = function() {\n  return this.bb.capacity() - this.space;\n};\n\n/**\n * Doubles the size of the backing ByteBuffer and copies the old data towards\n * the end of the new buffer (since we build the buffer backwards).\n *\n * @param {flatbuffers.ByteBuffer} bb The current buffer with the existing data\n * @returns {flatbuffers.ByteBuffer} A new byte buffer with the old data copied\n * to it. The data is located at the end of the buffer.\n *\n * uint8Array.set() formally takes {Array<number>|ArrayBufferView}, so to pass\n * it a uint8Array we need to suppress the type check:\n * @suppress {checkTypes}\n */\nflatbuffers.Builder.growByteBuffer = function(bb) {\n  var old_buf_size = bb.capacity();\n\n  // Ensure we don't grow beyond what fits in an int.\n  if (old_buf_size & 0xC0000000) {\n    throw new Error('FlatBuffers: cannot grow buffer beyond 2 gigabytes.');\n  }\n\n  var new_buf_size = old_buf_size << 1;\n  var nbb = flatbuffers.ByteBuffer.allocate(new_buf_size);\n  nbb.setPosition(new_buf_size - old_buf_size);\n  nbb.bytes().set(bb.bytes(), new_buf_size - old_buf_size);\n  return nbb;\n};\n/// @endcond\n\n/**\n * Adds on offset, relative to where it will be written.\n *\n * @param {flatbuffers.Offset} offset The offset to add.\n */\nflatbuffers.Builder.prototype.addOffset = function(offset) {\n  this.prep(flatbuffers.SIZEOF_INT, 0); // Ensure alignment is already done.\n  this.writeInt32(this.offset() - offset + flatbuffers.SIZEOF_INT);\n};\n\n/// @cond FLATBUFFERS_INTERNAL\n/**\n * Start encoding a new object in the buffer.  Users will not usually need to\n * call this directly. The FlatBuffers compiler will generate helper methods\n * that call this method internally.\n *\n * @param {number} numfields\n */\nflatbuffers.Builder.prototype.startObject = function(numfields) {\n  this.notNested();\n  if (this.vtable == null) {\n    this.vtable = [];\n  }\n  this.vtable_in_use = numfields;\n  for (var i = 0; i < numfields; i++) {\n    this.vtable[i] = 0; // This will push additional elements as needed\n  }\n  this.isNested = true;\n  this.object_start = this.offset();\n};\n\n/**\n * Finish off writing the object that is under construction.\n *\n * @returns {flatbuffers.Offset} The offset to the object inside `dataBuffer`\n */\nflatbuffers.Builder.prototype.endObject = function() {\n  if (this.vtable == null || !this.isNested) {\n    throw new Error('FlatBuffers: endObject called without startObject');\n  }\n\n  this.addInt32(0);\n  var vtableloc = this.offset();\n\n  // Trim trailing zeroes.\n  var i = this.vtable_in_use - 1;\n  for (; i >= 0 && this.vtable[i] == 0; i--) {}\n  var trimmed_size = i + 1;\n\n  // Write out the current vtable.\n  for (; i >= 0; i--) {\n    // Offset relative to the start of the table.\n    this.addInt16(this.vtable[i] != 0 ? vtableloc - this.vtable[i] : 0);\n  }\n\n  var standard_fields = 2; // The fields below:\n  this.addInt16(vtableloc - this.object_start);\n  var len = (trimmed_size + standard_fields) * flatbuffers.SIZEOF_SHORT;\n  this.addInt16(len);\n\n  // Search for an existing vtable that matches the current one.\n  var existing_vtable = 0;\n  var vt1 = this.space;\nouter_loop:\n  for (i = 0; i < this.vtables.length; i++) {\n    var vt2 = this.bb.capacity() - this.vtables[i];\n    if (len == this.bb.readInt16(vt2)) {\n      for (var j = flatbuffers.SIZEOF_SHORT; j < len; j += flatbuffers.SIZEOF_SHORT) {\n        if (this.bb.readInt16(vt1 + j) != this.bb.readInt16(vt2 + j)) {\n          continue outer_loop;\n        }\n      }\n      existing_vtable = this.vtables[i];\n      break;\n    }\n  }\n\n  if (existing_vtable) {\n    // Found a match:\n    // Remove the current vtable.\n    this.space = this.bb.capacity() - vtableloc;\n\n    // Point table to existing vtable.\n    this.bb.writeInt32(this.space, existing_vtable - vtableloc);\n  } else {\n    // No match:\n    // Add the location of the current vtable to the list of vtables.\n    this.vtables.push(this.offset());\n\n    // Point table to current vtable.\n    this.bb.writeInt32(this.bb.capacity() - vtableloc, this.offset() - vtableloc);\n  }\n\n  this.isNested = false;\n  return vtableloc;\n};\n/// @endcond\n\n/**\n * Finalize a buffer, poiting to the given `root_table`.\n *\n * @param {flatbuffers.Offset} root_table\n * @param {string=} opt_file_identifier\n */\nflatbuffers.Builder.prototype.finish = function(root_table, opt_file_identifier) {\n  if (opt_file_identifier) {\n    var file_identifier = opt_file_identifier;\n    this.prep(this.minalign, flatbuffers.SIZEOF_INT +\n      flatbuffers.FILE_IDENTIFIER_LENGTH);\n    if (file_identifier.length != flatbuffers.FILE_IDENTIFIER_LENGTH) {\n      throw new Error('FlatBuffers: file identifier must be length ' +\n        flatbuffers.FILE_IDENTIFIER_LENGTH);\n    }\n    for (var i = flatbuffers.FILE_IDENTIFIER_LENGTH - 1; i >= 0; i--) {\n      this.writeInt8(file_identifier.charCodeAt(i));\n    }\n  }\n  this.prep(this.minalign, flatbuffers.SIZEOF_INT);\n  this.addOffset(root_table);\n  this.bb.setPosition(this.space);\n};\n\n/// @cond FLATBUFFERS_INTERNAL\n/**\n * This checks a required field has been set in a given table that has\n * just been constructed.\n *\n * @param {flatbuffers.Offset} table\n * @param {number} field\n */\nflatbuffers.Builder.prototype.requiredField = function(table, field) {\n  var table_start = this.bb.capacity() - table;\n  var vtable_start = table_start - this.bb.readInt32(table_start);\n  var ok = this.bb.readInt16(vtable_start + field) != 0;\n\n  // If this fails, the caller will show what field needs to be set.\n  if (!ok) {\n    throw new Error('FlatBuffers: field ' + field + ' must be set');\n  }\n};\n\n/**\n * Start a new array/vector of objects.  Users usually will not call\n * this directly. The FlatBuffers compiler will create a start/end\n * method for vector types in generated code.\n *\n * @param {number} elem_size The size of each element in the array\n * @param {number} num_elems The number of elements in the array\n * @param {number} alignment The alignment of the array\n */\nflatbuffers.Builder.prototype.startVector = function(elem_size, num_elems, alignment) {\n  this.notNested();\n  this.vector_num_elems = num_elems;\n  this.prep(flatbuffers.SIZEOF_INT, elem_size * num_elems);\n  this.prep(alignment, elem_size * num_elems); // Just in case alignment > int.\n};\n\n/**\n * Finish off the creation of an array and all its elements. The array must be\n * created with `startVector`.\n *\n * @returns {flatbuffers.Offset} The offset at which the newly created array\n * starts.\n */\nflatbuffers.Builder.prototype.endVector = function() {\n  this.writeInt32(this.vector_num_elems);\n  return this.offset();\n};\n/// @endcond\n\n/**\n * Encode the string `s` in the buffer using UTF-8. If a Uint8Array is passed\n * instead of a string, it is assumed to contain valid UTF-8 encoded data.\n *\n * @param {string|Uint8Array} s The string to encode\n * @return {flatbuffers.Offset} The offset in the buffer where the encoded string starts\n */\nflatbuffers.Builder.prototype.createString = function(s) {\n  if (s instanceof Uint8Array) {\n    var utf8 = s;\n  } else {\n    var utf8 = [];\n    var i = 0;\n\n    while (i < s.length) {\n      var codePoint;\n\n      // Decode UTF-16\n      var a = s.charCodeAt(i++);\n      if (a < 0xD800 || a >= 0xDC00) {\n        codePoint = a;\n      } else {\n        var b = s.charCodeAt(i++);\n        codePoint = (a << 10) + b + (0x10000 - (0xD800 << 10) - 0xDC00);\n      }\n\n      // Encode UTF-8\n      if (codePoint < 0x80) {\n        utf8.push(codePoint);\n      } else {\n        if (codePoint < 0x800) {\n          utf8.push(((codePoint >> 6) & 0x1F) | 0xC0);\n        } else {\n          if (codePoint < 0x10000) {\n            utf8.push(((codePoint >> 12) & 0x0F) | 0xE0);\n          } else {\n            utf8.push(\n              ((codePoint >> 18) & 0x07) | 0xF0,\n              ((codePoint >> 12) & 0x3F) | 0x80);\n          }\n          utf8.push(((codePoint >> 6) & 0x3F) | 0x80);\n        }\n        utf8.push((codePoint & 0x3F) | 0x80);\n      }\n    }\n  }\n\n  this.addInt8(0);\n  this.startVector(1, utf8.length, 1);\n  this.bb.setPosition(this.space -= utf8.length);\n  for (var i = 0, offset = this.space, bytes = this.bb.bytes(); i < utf8.length; i++) {\n    bytes[offset++] = utf8[i];\n  }\n  return this.endVector();\n};\n\n/**\n * A helper function to avoid generated code depending on this file directly.\n *\n * @param {number} low\n * @param {number} high\n * @returns {flatbuffers.Long}\n */\nflatbuffers.Builder.prototype.createLong = function(low, high) {\n  return flatbuffers.Long.create(low, high);\n};\n////////////////////////////////////////////////////////////////////////////////\n/// @cond FLATBUFFERS_INTERNAL\n/**\n * Create a new ByteBuffer with a given array of bytes (`Uint8Array`).\n *\n * @constructor\n * @param {Uint8Array} bytes\n */\nflatbuffers.ByteBuffer = function(bytes) {\n  /**\n   * @type {Uint8Array}\n   * @private\n   */\n  this.bytes_ = bytes;\n\n  /**\n   * @type {number}\n   * @private\n   */\n  this.position_ = 0;\n};\n\n/**\n * Create and allocate a new ByteBuffer with a given size.\n *\n * @param {number} byte_size\n * @returns {flatbuffers.ByteBuffer}\n */\nflatbuffers.ByteBuffer.allocate = function(byte_size) {\n  return new flatbuffers.ByteBuffer(new Uint8Array(byte_size));\n};\n\nflatbuffers.ByteBuffer.prototype.clear = function() {\n  this.position_ = 0;\n};\n\n/**\n * Get the underlying `Uint8Array`.\n *\n * @returns {Uint8Array}\n */\nflatbuffers.ByteBuffer.prototype.bytes = function() {\n  return this.bytes_;\n};\n\n/**\n * Get the buffer's position.\n *\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.position = function() {\n  return this.position_;\n};\n\n/**\n * Set the buffer's position.\n *\n * @param {number} position\n */\nflatbuffers.ByteBuffer.prototype.setPosition = function(position) {\n  this.position_ = position;\n};\n\n/**\n * Get the buffer's capacity.\n *\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.capacity = function() {\n  return this.bytes_.length;\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readInt8 = function(offset) {\n  return this.readUint8(offset) << 24 >> 24;\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readUint8 = function(offset) {\n  return this.bytes_[offset];\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readInt16 = function(offset) {\n  return this.readUint16(offset) << 16 >> 16;\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readUint16 = function(offset) {\n  return this.bytes_[offset] | this.bytes_[offset + 1] << 8;\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readInt32 = function(offset) {\n  return this.bytes_[offset] | this.bytes_[offset + 1] << 8 | this.bytes_[offset + 2] << 16 | this.bytes_[offset + 3] << 24;\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readUint32 = function(offset) {\n  return this.readInt32(offset) >>> 0;\n};\n\n/**\n * @param {number} offset\n * @returns {flatbuffers.Long}\n */\nflatbuffers.ByteBuffer.prototype.readInt64 = function(offset) {\n  return new flatbuffers.Long(this.readInt32(offset), this.readInt32(offset + 4));\n};\n\n/**\n * @param {number} offset\n * @returns {flatbuffers.Long}\n */\nflatbuffers.ByteBuffer.prototype.readUint64 = function(offset) {\n  return new flatbuffers.Long(this.readUint32(offset), this.readUint32(offset + 4));\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readFloat32 = function(offset) {\n  flatbuffers.int32[0] = this.readInt32(offset);\n  return flatbuffers.float32[0];\n};\n\n/**\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.readFloat64 = function(offset) {\n  flatbuffers.int32[flatbuffers.isLittleEndian ? 0 : 1] = this.readInt32(offset);\n  flatbuffers.int32[flatbuffers.isLittleEndian ? 1 : 0] = this.readInt32(offset + 4);\n  return flatbuffers.float64[0];\n};\n\n/**\n * @param {number} offset\n * @param {number|boolean} value\n */\nflatbuffers.ByteBuffer.prototype.writeInt8 = function(offset, value) {\n  this.bytes_[offset] = /** @type {number} */(value);\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeUint8 = function(offset, value) {\n  this.bytes_[offset] = value;\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeInt16 = function(offset, value) {\n  this.bytes_[offset] = value;\n  this.bytes_[offset + 1] = value >> 8;\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeUint16 = function(offset, value) {\n    this.bytes_[offset] = value;\n    this.bytes_[offset + 1] = value >> 8;\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeInt32 = function(offset, value) {\n  this.bytes_[offset] = value;\n  this.bytes_[offset + 1] = value >> 8;\n  this.bytes_[offset + 2] = value >> 16;\n  this.bytes_[offset + 3] = value >> 24;\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeUint32 = function(offset, value) {\n    this.bytes_[offset] = value;\n    this.bytes_[offset + 1] = value >> 8;\n    this.bytes_[offset + 2] = value >> 16;\n    this.bytes_[offset + 3] = value >> 24;\n};\n\n/**\n * @param {number} offset\n * @param {flatbuffers.Long} value\n */\nflatbuffers.ByteBuffer.prototype.writeInt64 = function(offset, value) {\n  this.writeInt32(offset, value.low);\n  this.writeInt32(offset + 4, value.high);\n};\n\n/**\n * @param {number} offset\n * @param {flatbuffers.Long} value\n */\nflatbuffers.ByteBuffer.prototype.writeUint64 = function(offset, value) {\n    this.writeUint32(offset, value.low);\n    this.writeUint32(offset + 4, value.high);\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeFloat32 = function(offset, value) {\n  flatbuffers.float32[0] = value;\n  this.writeInt32(offset, flatbuffers.int32[0]);\n};\n\n/**\n * @param {number} offset\n * @param {number} value\n */\nflatbuffers.ByteBuffer.prototype.writeFloat64 = function(offset, value) {\n  flatbuffers.float64[0] = value;\n  this.writeInt32(offset, flatbuffers.int32[flatbuffers.isLittleEndian ? 0 : 1]);\n  this.writeInt32(offset + 4, flatbuffers.int32[flatbuffers.isLittleEndian ? 1 : 0]);\n};\n\n/**\n * Return the file identifier.   Behavior is undefined for FlatBuffers whose\n * schema does not include a file_identifier (likely points at padding or the\n * start of a the root vtable).\n * @returns {string}\n */\nflatbuffers.ByteBuffer.prototype.getBufferIdentifier = function() {\n  if (this.bytes_.length < this.position_ + flatbuffers.SIZEOF_INT +\n      flatbuffers.FILE_IDENTIFIER_LENGTH) {\n    throw new Error(\n        'FlatBuffers: ByteBuffer is too short to contain an identifier.');\n  }\n  var result = \"\";\n  for (var i = 0; i < flatbuffers.FILE_IDENTIFIER_LENGTH; i++) {\n    result += String.fromCharCode(\n        this.readInt8(this.position_ + flatbuffers.SIZEOF_INT + i));\n  }\n  return result;\n};\n\n/**\n * Look up a field in the vtable, return an offset into the object, or 0 if the\n * field is not present.\n *\n * @param {number} bb_pos\n * @param {number} vtable_offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.__offset = function(bb_pos, vtable_offset) {\n  var vtable = bb_pos - this.readInt32(bb_pos);\n  return vtable_offset < this.readInt16(vtable) ? this.readInt16(vtable + vtable_offset) : 0;\n};\n\n/**\n * Initialize any Table-derived type to point to the union at the given offset.\n *\n * @param {flatbuffers.Table} t\n * @param {number} offset\n * @returns {flatbuffers.Table}\n */\nflatbuffers.ByteBuffer.prototype.__union = function(t, offset) {\n  t.bb_pos = offset + this.readInt32(offset);\n  t.bb = this;\n  return t;\n};\n\n/**\n * Create a JavaScript string from UTF-8 data stored inside the FlatBuffer.\n * This allocates a new string and converts to wide chars upon each access.\n *\n * To avoid the conversion to UTF-16, pass flatbuffers.Encoding.UTF8_BYTES as\n * the \"optionalEncoding\" argument. This is useful for avoiding conversion to\n * and from UTF-16 when the data will just be packaged back up in another\n * FlatBuffer later on.\n *\n * @param {number} offset\n * @param {flatbuffers.Encoding=} opt_encoding Defaults to UTF16_STRING\n * @returns {string|Uint8Array}\n */\nflatbuffers.ByteBuffer.prototype.__string = function(offset, opt_encoding) {\n  offset += this.readInt32(offset);\n\n  var length = this.readInt32(offset);\n  var result = '';\n  var i = 0;\n\n  offset += flatbuffers.SIZEOF_INT;\n\n  if (opt_encoding === flatbuffers.Encoding.UTF8_BYTES) {\n    return this.bytes_.subarray(offset, offset + length);\n  }\n\n  while (i < length) {\n    var codePoint;\n\n    // Decode UTF-8\n    var a = this.readUint8(offset + i++);\n    if (a < 0xC0) {\n      codePoint = a;\n    } else {\n      var b = this.readUint8(offset + i++);\n      if (a < 0xE0) {\n        codePoint =\n          ((a & 0x1F) << 6) |\n          (b & 0x3F);\n      } else {\n        var c = this.readUint8(offset + i++);\n        if (a < 0xF0) {\n          codePoint =\n            ((a & 0x0F) << 12) |\n            ((b & 0x3F) << 6) |\n            (c & 0x3F);\n        } else {\n          var d = this.readUint8(offset + i++);\n          codePoint =\n            ((a & 0x07) << 18) |\n            ((b & 0x3F) << 12) |\n            ((c & 0x3F) << 6) |\n            (d & 0x3F);\n        }\n      }\n    }\n\n    // Encode UTF-16\n    if (codePoint < 0x10000) {\n      result += String.fromCharCode(codePoint);\n    } else {\n      codePoint -= 0x10000;\n      result += String.fromCharCode(\n        (codePoint >> 10) + 0xD800,\n        (codePoint & ((1 << 10) - 1)) + 0xDC00);\n    }\n  }\n\n  return result;\n};\n\n/**\n * Retrieve the relative offset stored at \"offset\"\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.__indirect = function(offset) {\n  return offset + this.readInt32(offset);\n};\n\n/**\n * Get the start of data of a vector whose offset is stored at \"offset\" in this object.\n *\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.__vector = function(offset) {\n  return offset + this.readInt32(offset) + flatbuffers.SIZEOF_INT; // data starts after the length\n};\n\n/**\n * Get the length of a vector whose offset is stored at \"offset\" in this object.\n *\n * @param {number} offset\n * @returns {number}\n */\nflatbuffers.ByteBuffer.prototype.__vector_len = function(offset) {\n  return this.readInt32(offset + this.readInt32(offset));\n};\n\n/**\n * @param {string} ident\n * @returns {boolean}\n */\nflatbuffers.ByteBuffer.prototype.__has_identifier = function(ident) {\n  if (ident.length != flatbuffers.FILE_IDENTIFIER_LENGTH) {\n    throw new Error('FlatBuffers: file identifier must be length ' +\n                    flatbuffers.FILE_IDENTIFIER_LENGTH);\n  }\n  for (var i = 0; i < flatbuffers.FILE_IDENTIFIER_LENGTH; i++) {\n    if (ident.charCodeAt(i) != this.readInt8(this.position_ + flatbuffers.SIZEOF_INT + i)) {\n      return false;\n    }\n  }\n  return true;\n};\n\n/**\n * A helper function to avoid generated code depending on this file directly.\n *\n * @param {number} low\n * @param {number} high\n * @returns {flatbuffers.Long}\n */\nflatbuffers.ByteBuffer.prototype.createLong = function(low, high) {\n  return flatbuffers.Long.create(low, high);\n};\n\n// Exports for Node.js and RequireJS\nexport { flatbuffers };\n\n/// @endcond\n/// @}\n",
         "'use strict';\n\n// This is free and unencumbered software released into the public domain.\n// See LICENSE.md for more information.\n\n//\n// Utilities\n//\n\n/**\n * @param {number} a The number to test.\n * @param {number} min The minimum value in the range, inclusive.\n * @param {number} max The maximum value in the range, inclusive.\n * @return {boolean} True if a >= min and a <= max.\n */\nfunction inRange(a, min, max) {\n  return min <= a && a <= max;\n}\n\n/**\n * @param {*} o\n * @return {Object}\n */\nfunction ToDictionary(o) {\n  if (o === undefined) return {};\n  if (o === Object(o)) return o;\n  throw TypeError('Could not convert argument to dictionary');\n}\n\n/**\n * @param {string} string Input string of UTF-16 code units.\n * @return {!Array.<number>} Code points.\n */\nfunction stringToCodePoints(string) {\n  // https://heycam.github.io/webidl/#dfn-obtain-unicode\n\n  // 1. Let S be the DOMString value.\n  var s = String(string);\n\n  // 2. Let n be the length of S.\n  var n = s.length;\n\n  // 3. Initialize i to 0.\n  var i = 0;\n\n  // 4. Initialize U to be an empty sequence of Unicode characters.\n  var u = [];\n\n  // 5. While i < n:\n  while (i < n) {\n\n    // 1. Let c be the code unit in S at index i.\n    var c = s.charCodeAt(i);\n\n    // 2. Depending on the value of c:\n\n    // c < 0xD800 or c > 0xDFFF\n    if (c < 0xD800 || c > 0xDFFF) {\n      // Append to U the Unicode character with code point c.\n      u.push(c);\n    }\n\n    // 0xDC00 \u2264 c \u2264 0xDFFF\n    else if (0xDC00 <= c && c <= 0xDFFF) {\n      // Append to U a U+FFFD REPLACEMENT CHARACTER.\n      u.push(0xFFFD);\n    }\n\n    // 0xD800 \u2264 c \u2264 0xDBFF\n    else if (0xD800 <= c && c <= 0xDBFF) {\n      // 1. If i = n\u22121, then append to U a U+FFFD REPLACEMENT\n      // CHARACTER.\n      if (i === n - 1) {\n        u.push(0xFFFD);\n      }\n      // 2. Otherwise, i < n\u22121:\n      else {\n        // 1. Let d be the code unit in S at index i+1.\n        var d = string.charCodeAt(i + 1);\n\n        // 2. If 0xDC00 \u2264 d \u2264 0xDFFF, then:\n        if (0xDC00 <= d && d <= 0xDFFF) {\n          // 1. Let a be c & 0x3FF.\n          var a = c & 0x3FF;\n\n          // 2. Let b be d & 0x3FF.\n          var b = d & 0x3FF;\n\n          // 3. Append to U the Unicode character with code point\n          // 2^16+2^10*a+b.\n          u.push(0x10000 + (a << 10) + b);\n\n          // 4. Set i to i+1.\n          i += 1;\n        }\n\n        // 3. Otherwise, d < 0xDC00 or d > 0xDFFF. Append to U a\n        // U+FFFD REPLACEMENT CHARACTER.\n        else  {\n          u.push(0xFFFD);\n        }\n      }\n    }\n\n    // 3. Set i to i+1.\n    i += 1;\n  }\n\n  // 6. Return U.\n  return u;\n}\n\n/**\n * @param {!Array.<number>} code_points Array of code points.\n * @return {string} string String of UTF-16 code units.\n */\nfunction codePointsToString(code_points) {\n  var s = '';\n  for (var i = 0; i < code_points.length; ++i) {\n    var cp = code_points[i];\n    if (cp <= 0xFFFF) {\n      s += String.fromCharCode(cp);\n    } else {\n      cp -= 0x10000;\n      s += String.fromCharCode((cp >> 10) + 0xD800,\n                               (cp & 0x3FF) + 0xDC00);\n    }\n  }\n  return s;\n}\n\n\n//\n// Implementation of Encoding specification\n// https://encoding.spec.whatwg.org/\n//\n\n//\n// 3. Terminology\n//\n\n/**\n * End-of-stream is a special token that signifies no more tokens\n * are in the stream.\n * @const\n */ var end_of_stream = -1;\n\n/**\n * A stream represents an ordered sequence of tokens.\n *\n * @constructor\n * @param {!(Array.<number>|Uint8Array)} tokens Array of tokens that provide the\n * stream.\n */\nfunction Stream(tokens) {\n  /** @type {!Array.<number>} */\n  this.tokens = [].slice.call(tokens);\n}\n\nStream.prototype = {\n  /**\n   * @return {boolean} True if end-of-stream has been hit.\n   */\n  endOfStream: function() {\n    return !this.tokens.length;\n  },\n\n  /**\n   * When a token is read from a stream, the first token in the\n   * stream must be returned and subsequently removed, and\n   * end-of-stream must be returned otherwise.\n   *\n   * @return {number} Get the next token from the stream, or\n   * end_of_stream.\n   */\n   read: function() {\n    if (!this.tokens.length)\n      return end_of_stream;\n     return this.tokens.shift();\n   },\n\n  /**\n   * When one or more tokens are prepended to a stream, those tokens\n   * must be inserted, in given order, before the first token in the\n   * stream.\n   *\n   * @param {(number|!Array.<number>)} token The token(s) to prepend to the stream.\n   */\n  prepend: function(token) {\n    if (Array.isArray(token)) {\n      var tokens = /**@type {!Array.<number>}*/(token);\n      while (tokens.length)\n        this.tokens.unshift(tokens.pop());\n    } else {\n      this.tokens.unshift(token);\n    }\n  },\n\n  /**\n   * When one or more tokens are pushed to a stream, those tokens\n   * must be inserted, in given order, after the last token in the\n   * stream.\n   *\n   * @param {(number|!Array.<number>)} token The tokens(s) to prepend to the stream.\n   */\n  push: function(token) {\n    if (Array.isArray(token)) {\n      var tokens = /**@type {!Array.<number>}*/(token);\n      while (tokens.length)\n        this.tokens.push(tokens.shift());\n    } else {\n      this.tokens.push(token);\n    }\n  }\n};\n\n//\n// 4. Encodings\n//\n\n// 4.1 Encoders and decoders\n\n/** @const */\nvar finished = -1;\n\n/**\n * @param {boolean} fatal If true, decoding errors raise an exception.\n * @param {number=} opt_code_point Override the standard fallback code point.\n * @return {number} The code point to insert on a decoding error.\n */\nfunction decoderError(fatal, opt_code_point) {\n  if (fatal)\n    throw TypeError('Decoder error');\n  return opt_code_point || 0xFFFD;\n}\n\n/** @interface */\nfunction Decoder() {}\nDecoder.prototype = {\n  /**\n   * @param {Stream} stream The stream of bytes being decoded.\n   * @param {number} bite The next byte read from the stream.\n   * @return {?(number|!Array.<number>)} The next code point(s)\n   *     decoded, or null if not enough data exists in the input\n   *     stream to decode a complete code point, or |finished|.\n   */\n  handler: function(stream, bite) {}\n};\n\n/** @interface */\nfunction Encoder() {}\nEncoder.prototype = {\n  /**\n   * @param {Stream} stream The stream of code points being encoded.\n   * @param {number} code_point Next code point read from the stream.\n   * @return {(number|!Array.<number>)} Byte(s) to emit, or |finished|.\n   */\n  handler: function(stream, code_point) {}\n};\n\n//\n// 7. API\n//\n\n/** @const */ var DEFAULT_ENCODING = 'utf-8';\n\n// 7.1 Interface TextDecoder\n\n/**\n * @constructor\n * @param {string=} encoding The label of the encoding;\n *     defaults to 'utf-8'.\n * @param {Object=} options\n */\nfunction TextDecoder(encoding, options) {\n  if (!(this instanceof TextDecoder)) {\n    return new TextDecoder(encoding, options);\n  }\n  encoding = encoding !== undefined ? String(encoding).toLowerCase() : DEFAULT_ENCODING;\n  if (encoding !== DEFAULT_ENCODING) {\n    throw new Error('Encoding not supported. Only utf-8 is supported');\n  }\n  options = ToDictionary(options);\n\n  /** @private @type {boolean} */\n  this._streaming = false;\n  /** @private @type {boolean} */\n  this._BOMseen = false;\n  /** @private @type {?Decoder} */\n  this._decoder = null;\n  /** @private @type {boolean} */\n  this._fatal = Boolean(options['fatal']);\n  /** @private @type {boolean} */\n  this._ignoreBOM = Boolean(options['ignoreBOM']);\n\n  Object.defineProperty(this, 'encoding', {value: 'utf-8'});\n  Object.defineProperty(this, 'fatal', {value: this._fatal});\n  Object.defineProperty(this, 'ignoreBOM', {value: this._ignoreBOM});\n}\n\nTextDecoder.prototype = {\n  /**\n   * @param {ArrayBufferView=} input The buffer of bytes to decode.\n   * @param {Object=} options\n   * @return {string} The decoded string.\n   */\n  decode: function decode(input, options) {\n    var bytes;\n    if (typeof input === 'object' && input instanceof ArrayBuffer) {\n      bytes = new Uint8Array(input);\n    } else if (typeof input === 'object' && 'buffer' in input &&\n               input.buffer instanceof ArrayBuffer) {\n      bytes = new Uint8Array(input.buffer,\n                             input.byteOffset,\n                             input.byteLength);\n    } else {\n      bytes = new Uint8Array(0);\n    }\n\n    options = ToDictionary(options);\n\n    if (!this._streaming) {\n      this._decoder = new UTF8Decoder({fatal: this._fatal});\n      this._BOMseen = false;\n    }\n    this._streaming = Boolean(options['stream']);\n\n    var input_stream = new Stream(bytes);\n\n    var code_points = [];\n\n    /** @type {?(number|!Array.<number>)} */\n    var result;\n\n    while (!input_stream.endOfStream()) {\n      result = this._decoder.handler(input_stream, input_stream.read());\n      if (result === finished)\n        break;\n      if (result === null)\n        continue;\n      if (Array.isArray(result))\n        code_points.push.apply(code_points, /**@type {!Array.<number>}*/(result));\n      else\n        code_points.push(result);\n    }\n    if (!this._streaming) {\n      do {\n        result = this._decoder.handler(input_stream, input_stream.read());\n        if (result === finished)\n          break;\n        if (result === null)\n          continue;\n        if (Array.isArray(result))\n          code_points.push.apply(code_points, /**@type {!Array.<number>}*/(result));\n        else\n          code_points.push(result);\n      } while (!input_stream.endOfStream());\n      this._decoder = null;\n    }\n\n    if (code_points.length) {\n      // If encoding is one of utf-8, utf-16be, and utf-16le, and\n      // ignore BOM flag and BOM seen flag are unset, run these\n      // subsubsteps:\n      if (['utf-8'].indexOf(this.encoding) !== -1 &&\n          !this._ignoreBOM && !this._BOMseen) {\n        // If token is U+FEFF, set BOM seen flag.\n        if (code_points[0] === 0xFEFF) {\n          this._BOMseen = true;\n          code_points.shift();\n        } else {\n          // Otherwise, if token is not end-of-stream, set BOM seen\n          // flag and append token to output.\n          this._BOMseen = true;\n        }\n      }\n    }\n\n    return codePointsToString(code_points);\n  }\n};\n\n// 7.2 Interface TextEncoder\n\n/**\n * @constructor\n * @param {string=} encoding The label of the encoding;\n *     defaults to 'utf-8'.\n * @param {Object=} options\n */\nfunction TextEncoder(encoding, options) {\n  if (!(this instanceof TextEncoder))\n    return new TextEncoder(encoding, options);\n  encoding = encoding !== undefined ? String(encoding).toLowerCase() : DEFAULT_ENCODING;\n  if (encoding !== DEFAULT_ENCODING) {\n    throw new Error('Encoding not supported. Only utf-8 is supported');\n  }\n  options = ToDictionary(options);\n\n  /** @private @type {boolean} */\n  this._streaming = false;\n  /** @private @type {?Encoder} */\n  this._encoder = null;\n  /** @private @type {{fatal: boolean}} */\n  this._options = {fatal: Boolean(options['fatal'])};\n\n  Object.defineProperty(this, 'encoding', {value: 'utf-8'});\n}\n\nTextEncoder.prototype = {\n  /**\n   * @param {string=} opt_string The string to encode.\n   * @param {Object=} options\n   * @return {Uint8Array} Encoded bytes, as a Uint8Array.\n   */\n  encode: function encode(opt_string, options) {\n    opt_string = opt_string ? String(opt_string) : '';\n    options = ToDictionary(options);\n\n    // NOTE: This option is nonstandard. None of the encodings\n    // permitted for encoding (i.e. UTF-8, UTF-16) are stateful,\n    // so streaming is not necessary.\n    if (!this._streaming)\n      this._encoder = new UTF8Encoder(this._options);\n    this._streaming = Boolean(options['stream']);\n\n    var bytes = [];\n    var input_stream = new Stream(stringToCodePoints(opt_string));\n    /** @type {?(number|!Array.<number>)} */\n    var result;\n    while (!input_stream.endOfStream()) {\n      result = this._encoder.handler(input_stream, input_stream.read());\n      if (result === finished)\n        break;\n      if (Array.isArray(result))\n        bytes.push.apply(bytes, /**@type {!Array.<number>}*/(result));\n      else\n        bytes.push(result);\n    }\n    if (!this._streaming) {\n      while (true) {\n        result = this._encoder.handler(input_stream, input_stream.read());\n        if (result === finished)\n          break;\n        if (Array.isArray(result))\n          bytes.push.apply(bytes, /**@type {!Array.<number>}*/(result));\n        else\n          bytes.push(result);\n      }\n      this._encoder = null;\n    }\n    return new Uint8Array(bytes);\n  }\n};\n\n//\n// 8. The encoding\n//\n\n// 8.1 utf-8\n\n/**\n * @constructor\n * @implements {Decoder}\n * @param {{fatal: boolean}} options\n */\nfunction UTF8Decoder(options) {\n  var fatal = options.fatal;\n\n  // utf-8's decoder's has an associated utf-8 code point, utf-8\n  // bytes seen, and utf-8 bytes needed (all initially 0), a utf-8\n  // lower boundary (initially 0x80), and a utf-8 upper boundary\n  // (initially 0xBF).\n  var /** @type {number} */ utf8_code_point = 0,\n      /** @type {number} */ utf8_bytes_seen = 0,\n      /** @type {number} */ utf8_bytes_needed = 0,\n      /** @type {number} */ utf8_lower_boundary = 0x80,\n      /** @type {number} */ utf8_upper_boundary = 0xBF;\n\n  /**\n   * @param {Stream} stream The stream of bytes being decoded.\n   * @param {number} bite The next byte read from the stream.\n   * @return {?(number|!Array.<number>)} The next code point(s)\n   *     decoded, or null if not enough data exists in the input\n   *     stream to decode a complete code point.\n   */\n  this.handler = function(stream, bite) {\n    // 1. If byte is end-of-stream and utf-8 bytes needed is not 0,\n    // set utf-8 bytes needed to 0 and return error.\n    if (bite === end_of_stream && utf8_bytes_needed !== 0) {\n      utf8_bytes_needed = 0;\n      return decoderError(fatal);\n    }\n\n    // 2. If byte is end-of-stream, return finished.\n    if (bite === end_of_stream)\n      return finished;\n\n    // 3. If utf-8 bytes needed is 0, based on byte:\n    if (utf8_bytes_needed === 0) {\n\n      // 0x00 to 0x7F\n      if (inRange(bite, 0x00, 0x7F)) {\n        // Return a code point whose value is byte.\n        return bite;\n      }\n\n      // 0xC2 to 0xDF\n      if (inRange(bite, 0xC2, 0xDF)) {\n        // Set utf-8 bytes needed to 1 and utf-8 code point to byte\n        // \u2212 0xC0.\n        utf8_bytes_needed = 1;\n        utf8_code_point = bite - 0xC0;\n      }\n\n      // 0xE0 to 0xEF\n      else if (inRange(bite, 0xE0, 0xEF)) {\n        // 1. If byte is 0xE0, set utf-8 lower boundary to 0xA0.\n        if (bite === 0xE0)\n          utf8_lower_boundary = 0xA0;\n        // 2. If byte is 0xED, set utf-8 upper boundary to 0x9F.\n        if (bite === 0xED)\n          utf8_upper_boundary = 0x9F;\n        // 3. Set utf-8 bytes needed to 2 and utf-8 code point to\n        // byte \u2212 0xE0.\n        utf8_bytes_needed = 2;\n        utf8_code_point = bite - 0xE0;\n      }\n\n      // 0xF0 to 0xF4\n      else if (inRange(bite, 0xF0, 0xF4)) {\n        // 1. If byte is 0xF0, set utf-8 lower boundary to 0x90.\n        if (bite === 0xF0)\n          utf8_lower_boundary = 0x90;\n        // 2. If byte is 0xF4, set utf-8 upper boundary to 0x8F.\n        if (bite === 0xF4)\n          utf8_upper_boundary = 0x8F;\n        // 3. Set utf-8 bytes needed to 3 and utf-8 code point to\n        // byte \u2212 0xF0.\n        utf8_bytes_needed = 3;\n        utf8_code_point = bite - 0xF0;\n      }\n\n      // Otherwise\n      else {\n        // Return error.\n        return decoderError(fatal);\n      }\n\n      // Then (byte is in the range 0xC2 to 0xF4) set utf-8 code\n      // point to utf-8 code point << (6 \u00d7 utf-8 bytes needed) and\n      // return continue.\n      utf8_code_point = utf8_code_point << (6 * utf8_bytes_needed);\n      return null;\n    }\n\n    // 4. If byte is not in the range utf-8 lower boundary to utf-8\n    // upper boundary, run these substeps:\n    if (!inRange(bite, utf8_lower_boundary, utf8_upper_boundary)) {\n\n      // 1. Set utf-8 code point, utf-8 bytes needed, and utf-8\n      // bytes seen to 0, set utf-8 lower boundary to 0x80, and set\n      // utf-8 upper boundary to 0xBF.\n      utf8_code_point = utf8_bytes_needed = utf8_bytes_seen = 0;\n      utf8_lower_boundary = 0x80;\n      utf8_upper_boundary = 0xBF;\n\n      // 2. Prepend byte to stream.\n      stream.prepend(bite);\n\n      // 3. Return error.\n      return decoderError(fatal);\n    }\n\n    // 5. Set utf-8 lower boundary to 0x80 and utf-8 upper boundary\n    // to 0xBF.\n    utf8_lower_boundary = 0x80;\n    utf8_upper_boundary = 0xBF;\n\n    // 6. Increase utf-8 bytes seen by one and set utf-8 code point\n    // to utf-8 code point + (byte \u2212 0x80) << (6 \u00d7 (utf-8 bytes\n    // needed \u2212 utf-8 bytes seen)).\n    utf8_bytes_seen += 1;\n    utf8_code_point += (bite - 0x80) << (6 * (utf8_bytes_needed - utf8_bytes_seen));\n\n    // 7. If utf-8 bytes seen is not equal to utf-8 bytes needed,\n    // continue.\n    if (utf8_bytes_seen !== utf8_bytes_needed)\n      return null;\n\n    // 8. Let code point be utf-8 code point.\n    var code_point = utf8_code_point;\n\n    // 9. Set utf-8 code point, utf-8 bytes needed, and utf-8 bytes\n    // seen to 0.\n    utf8_code_point = utf8_bytes_needed = utf8_bytes_seen = 0;\n\n    // 10. Return a code point whose value is code point.\n    return code_point;\n  };\n}\n\n/**\n * @constructor\n * @implements {Encoder}\n * @param {{fatal: boolean}} options\n */\nfunction UTF8Encoder(options) {\n  var fatal = options.fatal;\n  /**\n   * @param {Stream} stream Input stream.\n   * @param {number} code_point Next code point read from the stream.\n   * @return {(number|!Array.<number>)} Byte(s) to emit.\n   */\n  this.handler = function(stream, code_point) {\n    // 1. If code point is end-of-stream, return finished.\n    if (code_point === end_of_stream)\n      return finished;\n\n    // 2. If code point is in the range U+0000 to U+007F, return a\n    // byte whose value is code point.\n    if (inRange(code_point, 0x0000, 0x007f))\n      return code_point;\n\n    // 3. Set count and offset based on the range code point is in:\n    var count, offset;\n    // U+0080 to U+07FF:    1 and 0xC0\n    if (inRange(code_point, 0x0080, 0x07FF)) {\n      count = 1;\n      offset = 0xC0;\n    }\n    // U+0800 to U+FFFF:    2 and 0xE0\n    else if (inRange(code_point, 0x0800, 0xFFFF)) {\n      count = 2;\n      offset = 0xE0;\n    }\n    // U+10000 to U+10FFFF: 3 and 0xF0\n    else if (inRange(code_point, 0x10000, 0x10FFFF)) {\n      count = 3;\n      offset = 0xF0;\n    }\n\n    // 4.Let bytes be a byte sequence whose first byte is (code\n    // point >> (6 \u00d7 count)) + offset.\n    var bytes = [(code_point >> (6 * count)) + offset];\n\n    // 5. Run these substeps while count is greater than 0:\n    while (count > 0) {\n\n      // 1. Set temp to code point >> (6 \u00d7 (count \u2212 1)).\n      var temp = code_point >> (6 * (count - 1));\n\n      // 2. Append to bytes 0x80 | (temp & 0x3F).\n      bytes.push(0x80 | (temp & 0x3F));\n\n      // 3. Decrease count by one.\n      count -= 1;\n    }\n\n    // 6. Return bytes bytes, in order.\n    return bytes;\n  };\n}\n\nexport {TextEncoder, TextDecoder};\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { toUint8Array } from './buffer';\nimport {\n    TextDecoder as TextDecoderPolyfill,\n    TextEncoder as TextEncoderPolyfill,\n} from 'text-encoding-utf-8';\n\n/** @ignore @suppress {missingRequire} */\nconst _Buffer = typeof Buffer === 'function' ? Buffer : null;\n/** @ignore */\nconst useNativeEncoders = typeof TextDecoder === 'function' && typeof TextEncoder === 'function';\n\n/** @ignore */\nexport const decodeUtf8 = ((TextDecoder) => {\n    if (useNativeEncoders || !_Buffer) {\n        const decoder = new TextDecoder('utf-8');\n        return (buffer?: ArrayBuffer | ArrayBufferView) => decoder.decode(buffer);\n    }\n    return (input: ArrayBufferLike | ArrayBufferView) => {\n        const { buffer, byteOffset, length } = toUint8Array(input);\n        return _Buffer.from(buffer, byteOffset, length).toString();\n    };\n})(typeof TextDecoder !== 'undefined' ? TextDecoder : TextDecoderPolyfill);\n\n/** @ignore */\nexport const encodeUtf8 = ((TextEncoder) => {\n    if (useNativeEncoders || !_Buffer) {\n        const encoder = new TextEncoder();\n        return (value?: string) => encoder.encode(value);\n    }\n    return (input = '') => toUint8Array(_Buffer.from(input, 'utf8'));\n})(typeof TextEncoder !== 'undefined' ? TextEncoder : TextEncoderPolyfill);\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport streamAdapters from './adapters';\n\n/** @ignore */\nexport const ITERATOR_DONE: any = Object.freeze({ done: true, value: void (0) });\n\n/** @ignore */\nexport type FileHandle = import('fs').promises.FileHandle;\n/** @ignore */\nexport type ArrowJSONLike = { schema: any; batches?: any[]; dictionaries?: any[]; };\n/** @ignore */\nexport type ReadableDOMStreamOptions = { type: 'bytes' | undefined, autoAllocateChunkSize?: number, highWaterMark?: number };\n\n/** @ignore */\nexport class ArrowJSON {\n    // @ts-ignore\n    constructor(private _json: ArrowJSONLike) {}\n    public get schema(): any { return this._json['schema']; }\n    public get batches(): any[] { return (this._json['batches'] || []) as any[]; }\n    public get dictionaries(): any[] { return (this._json['dictionaries'] || []) as any[]; }\n}\n\n/** @ignore */\nexport interface Readable<T> {\n\n    readonly closed: Promise<void>;\n    cancel(reason?: any): Promise<void>;\n\n    read(size?: number | null): Promise<T | null>;\n    peek(size?: number | null): Promise<T | null>;\n    throw(value?: any): Promise<IteratorResult<any>>;\n    return(value?: any): Promise<IteratorResult<any>>;\n    next(size?: number | null): Promise<IteratorResult<T>>;\n}\n\n/** @ignore */\nexport interface Writable<T> {\n    readonly closed: Promise<void>;\n    close(): void;\n    write(chunk: T): void;\n    abort(reason?: any): void;\n}\n\n/** @ignore */\nexport interface ReadableWritable<TReadable, TWritable> extends Readable<TReadable>, Writable<TWritable> {\n    [Symbol.asyncIterator](): AsyncIterableIterator<TReadable>;\n    toDOMStream(options?: ReadableDOMStreamOptions): ReadableStream<TReadable>;\n    toNodeStream(options?: import('stream').ReadableOptions): import('stream').Readable;\n}\n\n/** @ignore */\nexport abstract class ReadableInterop<T> {\n\n    public abstract toDOMStream(options?: ReadableDOMStreamOptions): ReadableStream<T>;\n    public abstract toNodeStream(options?: import('stream').ReadableOptions): import('stream').Readable;\n\n    public tee(): [ReadableStream<T>, ReadableStream<T>] {\n        return this._getDOMStream().tee();\n    }\n    public pipe<R extends NodeJS.WritableStream>(writable: R, options?: { end?: boolean; }) {\n        return this._getNodeStream().pipe(writable, options);\n    }\n    public pipeTo(writable: WritableStream<T>, options?: PipeOptions) { return this._getDOMStream().pipeTo(writable, options); }\n    public pipeThrough<R extends ReadableStream<any>>(duplex: { writable: WritableStream<T>, readable: R }, options?: PipeOptions) {\n        return this._getDOMStream().pipeThrough(duplex, options);\n    }\n\n    protected _DOMStream?: ReadableStream<T>;\n    private _getDOMStream() {\n        return this._DOMStream || (this._DOMStream = this.toDOMStream());\n    }\n\n    protected _nodeStream?: import('stream').Readable;\n    private _getNodeStream() {\n        return this._nodeStream || (this._nodeStream = this.toNodeStream());\n    }\n}\n\n/** @ignore */\ntype Resolution<T> = { resolve: (value?: T | PromiseLike<T>) => void; reject: (reason?: any) => void; };\n\n/** @ignore */\nexport class AsyncQueue<TReadable = Uint8Array, TWritable = TReadable> extends ReadableInterop<TReadable>\n    implements AsyncIterableIterator<TReadable>, ReadableWritable<TReadable, TWritable> {\n\n    protected _values: TWritable[] = [];\n    protected _error?: { error: any; };\n    protected _closedPromise: Promise<void>;\n    protected _closedPromiseResolve?: (value?: any) => void;\n    protected resolvers: Resolution<IteratorResult<TReadable>>[] = [];\n\n    constructor() {\n        super();\n        this._closedPromise = new Promise((r) => this._closedPromiseResolve = r);\n    }\n\n    public get closed(): Promise<void> { return this._closedPromise; }\n    public async cancel(reason?: any) { await this.return(reason); }\n    public write(value: TWritable) {\n        if (this._ensureOpen()) {\n            this.resolvers.length <= 0\n                ? (this._values.push(value))\n                : (this.resolvers.shift()!.resolve({ done: false, value } as any));\n        }\n    }\n    public abort(value?: any) {\n        if (this._closedPromiseResolve) {\n            this.resolvers.length <= 0\n                ? (this._error = { error: value })\n                : (this.resolvers.shift()!.reject({ done: true, value }));\n        }\n    }\n    public close() {\n        if (this._closedPromiseResolve) {\n            const { resolvers } = this;\n            while (resolvers.length > 0) {\n                resolvers.shift()!.resolve(ITERATOR_DONE);\n            }\n            this._closedPromiseResolve();\n            this._closedPromiseResolve = undefined;\n        }\n    }\n\n    public [Symbol.asyncIterator]() { return this; }\n    public toDOMStream(options?: ReadableDOMStreamOptions) {\n        return streamAdapters.toDOMStream(\n            (this._closedPromiseResolve || this._error)\n                ? (this as AsyncIterable<TReadable>)\n                : (this._values as any) as Iterable<TReadable>,\n            options);\n    }\n    public toNodeStream(options?: import('stream').ReadableOptions) {\n        return streamAdapters.toNodeStream(\n            (this._closedPromiseResolve || this._error)\n                ? (this as AsyncIterable<TReadable>)\n                : (this._values as any) as Iterable<TReadable>,\n            options);\n    }\n    public async throw(_?: any) { await this.abort(_); return ITERATOR_DONE; }\n    public async return(_?: any) { await this.close(); return ITERATOR_DONE; }\n\n    public async read(size?: number | null): Promise<TReadable | null> { return (await this.next(size, 'read')).value; }\n    public async peek(size?: number | null): Promise<TReadable | null> { return (await this.next(size, 'peek')).value; }\n    public next(..._args: any[]): Promise<IteratorResult<TReadable>> {\n        if (this._values.length > 0) {\n            return Promise.resolve({ done: false, value: this._values.shift()! } as any);\n        } else if (this._error) {\n            return Promise.reject({ done: true, value: this._error.error });\n        } else if (!this._closedPromiseResolve) {\n            return Promise.resolve(ITERATOR_DONE);\n        } else {\n            return new Promise<IteratorResult<TReadable>>((resolve, reject) => {\n                this.resolvers.push({ resolve, reject });\n            });\n        }\n    }\n\n    protected _ensureOpen() {\n        if (this._closedPromiseResolve) {\n            return true;\n        }\n        throw new Error(`${this} is closed`);\n    }\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { ReadableInterop, ArrowJSONLike } from '../io/interfaces';\n\n/** @ignore */\ntype FSReadStream = import('fs').ReadStream;\n/** @ignore */\ntype FileHandle = import('fs').promises.FileHandle;\n\n/** @ignore */\nexport interface Subscription {\n    unsubscribe: () => void;\n}\n\n/** @ignore */\nexport interface Observer<T> {\n    closed?: boolean;\n    next: (value: T) => void;\n    error: (err: any) => void;\n    complete: () => void;\n}\n\n/** @ignore */\nexport interface Observable<T> {\n    subscribe: (observer: Observer<T>) => Subscription;\n}\n\n/** @ignore */\nconst [BigIntCtor, BigIntAvailable] = (() => {\n    const BigIntUnavailableError = () => { throw new Error('BigInt is not available in this environment'); };\n    function BigIntUnavailable() { throw BigIntUnavailableError(); }\n    BigIntUnavailable.asIntN = () => { throw BigIntUnavailableError(); };\n    BigIntUnavailable.asUintN = () => { throw BigIntUnavailableError(); };\n    return typeof BigInt !== 'undefined' ? [BigInt, true] : [<any> BigIntUnavailable, false];\n})() as [BigIntConstructor, boolean];\n\n/** @ignore */\nconst [BigInt64ArrayCtor, BigInt64ArrayAvailable] = (() => {\n    const BigInt64ArrayUnavailableError = () => { throw new Error('BigInt64Array is not available in this environment'); };\n    class BigInt64ArrayUnavailable {\n        static get BYTES_PER_ELEMENT() { return 8; }\n        static of() { throw BigInt64ArrayUnavailableError(); }\n        static from() { throw BigInt64ArrayUnavailableError(); }\n        constructor() { throw BigInt64ArrayUnavailableError(); }\n    }\n    return typeof BigInt64Array !== 'undefined' ? [BigInt64Array, true] : [<any> BigInt64ArrayUnavailable, false];\n})() as [BigInt64ArrayConstructor, boolean];\n\n/** @ignore */\nconst [BigUint64ArrayCtor, BigUint64ArrayAvailable] = (() => {\n    const BigUint64ArrayUnavailableError = () => { throw new Error('BigUint64Array is not available in this environment'); };\n    class BigUint64ArrayUnavailable {\n        static get BYTES_PER_ELEMENT() { return 8; }\n        static of() { throw BigUint64ArrayUnavailableError(); }\n        static from() { throw BigUint64ArrayUnavailableError(); }\n        constructor() { throw BigUint64ArrayUnavailableError(); }\n    }\n    return typeof BigUint64Array !== 'undefined' ? [BigUint64Array, true] : [<any> BigUint64ArrayUnavailable, false];\n})() as [BigUint64ArrayConstructor, boolean];\n\nexport { BigIntCtor as BigInt, BigIntAvailable };\nexport { BigInt64ArrayCtor as BigInt64Array, BigInt64ArrayAvailable };\nexport { BigUint64ArrayCtor as BigUint64Array, BigUint64ArrayAvailable };\n\n/** @ignore */ const isNumber = (x: any) => typeof x === 'number';\n/** @ignore */ const isBoolean = (x: any) => typeof x === 'boolean';\n/** @ignore */ const isFunction = (x: any) => typeof x === 'function';\n/** @ignore */\nexport const isObject = (x: any): x is Object => x != null && Object(x) === x;\n\n/** @ignore */\nexport const isPromise = <T = any>(x: any): x is PromiseLike<T> => {\n    return isObject(x) && isFunction(x.then);\n};\n\n/** @ignore */\nexport const isObservable = <T = any>(x: any): x is Observable<T> => {\n    return isObject(x) && isFunction(x.subscribe);\n};\n\n/** @ignore */\nexport const isIterable = <T = any>(x: any): x is Iterable<T> => {\n    return isObject(x) && isFunction(x[Symbol.iterator]);\n};\n\n/** @ignore */\nexport const isAsyncIterable = <T = any>(x: any): x is AsyncIterable<T> => {\n    return isObject(x) && isFunction(x[Symbol.asyncIterator]);\n};\n\n/** @ignore */\nexport const isArrowJSON = (x: any): x is ArrowJSONLike  => {\n    return isObject(x) && isObject(x['schema']);\n};\n\n/** @ignore */\nexport const isArrayLike = <T = any>(x: any): x is ArrayLike<T> => {\n    return isObject(x) && isNumber(x['length']);\n};\n\n/** @ignore */\nexport const isIteratorResult = <T = any>(x: any): x is IteratorResult<T> => {\n    return isObject(x) && ('done' in x) && ('value' in x);\n};\n\n/** @ignore */\nexport const isUnderlyingSink = <T = any>(x: any): x is UnderlyingSink<T> => {\n    return isObject(x) &&\n        isFunction(x['abort']) &&\n        isFunction(x['close']) &&\n        isFunction(x['start']) &&\n        isFunction(x['write']);\n};\n\n/** @ignore */\nexport const isFileHandle = (x: any): x is FileHandle => {\n    return isObject(x) && isFunction(x['stat']) && isNumber(x['fd']);\n};\n\n/** @ignore */\nexport const isFSReadStream = (x: any): x is FSReadStream => {\n    return isReadableNodeStream(x) && isNumber((<any> x)['bytesRead']);\n};\n\n/** @ignore */\nexport const isFetchResponse = (x: any): x is Response => {\n    return isObject(x) && isReadableDOMStream(x['body']);\n};\n\n/** @ignore */\nexport const isWritableDOMStream = <T = any>(x: any): x is WritableStream<T> => {\n    return isObject(x) &&\n        isFunction(x['abort']) &&\n        isFunction(x['getWriter']) &&\n        !(x instanceof ReadableInterop);\n};\n\n/** @ignore */\nexport const isReadableDOMStream = <T = any>(x: any): x is ReadableStream<T> => {\n    return isObject(x) &&\n        isFunction(x['cancel']) &&\n        isFunction(x['getReader']) &&\n        !(x instanceof ReadableInterop);\n};\n\n/** @ignore */\nexport const isWritableNodeStream = (x: any): x is NodeJS.WritableStream => {\n    return isObject(x) &&\n        isFunction(x['end']) &&\n        isFunction(x['write']) &&\n        isBoolean(x['writable']) &&\n        !(x instanceof ReadableInterop);\n};\n\n/** @ignore */\nexport const isReadableNodeStream = (x: any): x is NodeJS.ReadableStream => {\n    return isObject(x) &&\n        isFunction(x['read']) &&\n        isFunction(x['pipe']) &&\n        isBoolean(x['readable']) &&\n        !(x instanceof ReadableInterop);\n};\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { flatbuffers } from 'flatbuffers';\nimport { encodeUtf8 } from '../util/utf8';\nimport ByteBuffer = flatbuffers.ByteBuffer;\nimport { TypedArray, TypedArrayConstructor } from '../interfaces';\nimport { BigIntArray, BigIntArrayConstructor } from '../interfaces';\nimport { isPromise, isIterable, isAsyncIterable, isIteratorResult, BigInt64Array, BigUint64Array } from './compat';\n\n/** @ignore */\nconst SharedArrayBuf = (typeof SharedArrayBuffer !== 'undefined' ? SharedArrayBuffer : ArrayBuffer);\n\n/** @ignore */\nfunction collapseContiguousByteRanges(chunks: Uint8Array[]) {\n    let result = chunks[0] ? [chunks[0]] : [];\n    let xOffset: number, yOffset: number, xLen: number, yLen: number;\n    for (let x, y, i = 0, j = 0, n = chunks.length; ++i < n;) {\n        x = result[j];\n        y = chunks[i];\n        // continue if x and y don't share the same underlying ArrayBuffer, or if x isn't before y\n        if (!x || !y || x.buffer !== y.buffer || y.byteOffset < x.byteOffset) {\n            y && (result[++j] = y);\n            continue;\n        }\n        ({ byteOffset: xOffset, byteLength: xLen } = x);\n        ({ byteOffset: yOffset, byteLength: yLen } = y);\n        // continue if the byte ranges of x and y aren't contiguous\n        if ((xOffset + xLen) < yOffset || (yOffset + yLen) < xOffset) {\n            y && (result[++j] = y);\n            continue;\n        }\n        result[j] = new Uint8Array(x.buffer, xOffset, yOffset - xOffset + yLen);\n    }\n    return result;\n}\n\n/** @ignore */\nexport function memcpy<TTarget extends ArrayBufferView, TSource extends ArrayBufferView>(target: TTarget, source: TSource, targetByteOffset = 0, sourceByteLength = source.byteLength) {\n    const targetByteLength = target.byteLength;\n    const dst = new Uint8Array(target.buffer, target.byteOffset, targetByteLength);\n    const src = new Uint8Array(source.buffer, source.byteOffset, Math.min(sourceByteLength, targetByteLength));\n    dst.set(src, targetByteOffset);\n    return target;\n}\n\n/** @ignore */\nexport function joinUint8Arrays(chunks: Uint8Array[], size?: number | null): [Uint8Array, Uint8Array[], number] {\n    // collapse chunks that share the same underlying ArrayBuffer and whose byte ranges overlap,\n    // to avoid unnecessarily copying the bytes to do this buffer join. This is a common case during\n    // streaming, where we may be reading partial byte ranges out of the same underlying ArrayBuffer\n    let result = collapseContiguousByteRanges(chunks);\n    let byteLength = result.reduce((x, b) => x + b.byteLength, 0);\n    let source: Uint8Array, sliced: Uint8Array, buffer: Uint8Array | void;\n    let offset = 0, index = -1, length = Math.min(size || Infinity, byteLength);\n    for (let n = result.length; ++index < n;) {\n        source = result[index];\n        sliced = source.subarray(0, Math.min(source.length, length - offset));\n        if (length <= (offset + sliced.length)) {\n            if (sliced.length < source.length) {\n                result[index] = source.subarray(sliced.length);\n            } else if (sliced.length === source.length) { index++; }\n            buffer ? memcpy(buffer, sliced, offset) : (buffer = sliced);\n            break;\n        }\n        memcpy(buffer || (buffer = new Uint8Array(length)), sliced, offset);\n        offset += sliced.length;\n    }\n    return [buffer || new Uint8Array(0), result.slice(index), byteLength - (buffer ? buffer.byteLength : 0)];\n}\n\n/** @ignore */\nexport type ArrayBufferViewInput = ArrayBufferView | ArrayBufferLike | ArrayBufferView | Iterable<number> | ArrayLike<number> | ByteBuffer | string | null | undefined  |\n                    IteratorResult<ArrayBufferView | ArrayBufferLike | ArrayBufferView | Iterable<number> | ArrayLike<number> | ByteBuffer | string | null | undefined> |\n          ReadableStreamReadResult<ArrayBufferView | ArrayBufferLike | ArrayBufferView | Iterable<number> | ArrayLike<number> | ByteBuffer | string | null | undefined> ;\n\n/** @ignore */\nexport function toArrayBufferView<T extends TypedArray>(ArrayBufferViewCtor: TypedArrayConstructor<T>, input: ArrayBufferViewInput): T;\nexport function toArrayBufferView<T extends BigIntArray>(ArrayBufferViewCtor: BigIntArrayConstructor<T>, input: ArrayBufferViewInput): T;\nexport function toArrayBufferView(ArrayBufferViewCtor: any, input: ArrayBufferViewInput) {\n\n    let value: any = isIteratorResult(input) ? input.value : input;\n\n    if (value instanceof ArrayBufferViewCtor) {\n        if (ArrayBufferViewCtor === Uint8Array) {\n            // Node's `Buffer` class passes the `instanceof Uint8Array` check, but we need\n            // a real Uint8Array, since Buffer#slice isn't the same as Uint8Array#slice :/\n            return new ArrayBufferViewCtor(value.buffer, value.byteOffset, value.byteLength);\n        }\n        return value;\n    }\n    if (!value) { return new ArrayBufferViewCtor(0); }\n    if (typeof value === 'string') { value = encodeUtf8(value); }\n    if (value instanceof ArrayBuffer) { return new ArrayBufferViewCtor(value); }\n    if (value instanceof SharedArrayBuf) { return new ArrayBufferViewCtor(value); }\n    if (value instanceof ByteBuffer) { return toArrayBufferView(ArrayBufferViewCtor, value.bytes()); }\n    return !ArrayBuffer.isView(value) ? ArrayBufferViewCtor.from(value) : value.byteLength <= 0 ? new ArrayBufferViewCtor(0)\n        : new ArrayBufferViewCtor(value.buffer, value.byteOffset, value.byteLength / ArrayBufferViewCtor.BYTES_PER_ELEMENT);\n}\n\n/** @ignore */ export const toInt8Array = (input: ArrayBufferViewInput) => toArrayBufferView(Int8Array, input);\n/** @ignore */ export const toInt16Array = (input: ArrayBufferViewInput) => toArrayBufferView(Int16Array, input);\n/** @ignore */ export const toInt32Array = (input: ArrayBufferViewInput) => toArrayBufferView(Int32Array, input);\n/** @ignore */ export const toBigInt64Array = (input: ArrayBufferViewInput) => toArrayBufferView(BigInt64Array, input);\n/** @ignore */ export const toUint8Array = (input: ArrayBufferViewInput) => toArrayBufferView(Uint8Array, input);\n/** @ignore */ export const toUint16Array = (input: ArrayBufferViewInput) => toArrayBufferView(Uint16Array, input);\n/** @ignore */ export const toUint32Array = (input: ArrayBufferViewInput) => toArrayBufferView(Uint32Array, input);\n/** @ignore */ export const toBigUint64Array = (input: ArrayBufferViewInput) => toArrayBufferView(BigUint64Array, input);\n/** @ignore */ export const toFloat32Array = (input: ArrayBufferViewInput) => toArrayBufferView(Float32Array, input);\n/** @ignore */ export const toFloat64Array = (input: ArrayBufferViewInput) => toArrayBufferView(Float64Array, input);\n/** @ignore */ export const toUint8ClampedArray = (input: ArrayBufferViewInput) => toArrayBufferView(Uint8ClampedArray, input);\n\n/** @ignore */\ntype ArrayBufferViewIteratorInput = Iterable<ArrayBufferViewInput> | ArrayBufferViewInput;\n\n/** @ignore */\nconst pump = <T extends Iterator<any> | AsyncIterator<any>>(iterator: T) => { iterator.next(); return iterator; };\n\n/** @ignore */\nexport function* toArrayBufferViewIterator<T extends TypedArray>(ArrayCtor: TypedArrayConstructor<T>, source: ArrayBufferViewIteratorInput) {\n\n    const wrap = function*<T>(x: T) { yield x; };\n    const buffers: Iterable<ArrayBufferViewInput> =\n                   (typeof source === 'string') ? wrap(source)\n                 : (ArrayBuffer.isView(source)) ? wrap(source)\n              : (source instanceof ArrayBuffer) ? wrap(source)\n           : (source instanceof SharedArrayBuf) ? wrap(source)\n    : !isIterable<ArrayBufferViewInput>(source) ? wrap(source) : source;\n\n    yield* pump((function* (it) {\n        let r: IteratorResult<any> = <any> null;\n        do {\n            r = it.next(yield toArrayBufferView(ArrayCtor, r));\n        } while (!r.done);\n    })(buffers[Symbol.iterator]()));\n}\n\n/** @ignore */ export const toInt8ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Int8Array, input);\n/** @ignore */ export const toInt16ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Int16Array, input);\n/** @ignore */ export const toInt32ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Int32Array, input);\n/** @ignore */ export const toUint8ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Uint8Array, input);\n/** @ignore */ export const toUint16ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Uint16Array, input);\n/** @ignore */ export const toUint32ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Uint32Array, input);\n/** @ignore */ export const toFloat32ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Float32Array, input);\n/** @ignore */ export const toFloat64ArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Float64Array, input);\n/** @ignore */ export const toUint8ClampedArrayIterator = (input: ArrayBufferViewIteratorInput) => toArrayBufferViewIterator(Uint8ClampedArray, input);\n\n/** @ignore */\ntype ArrayBufferViewAsyncIteratorInput = AsyncIterable<ArrayBufferViewInput> | Iterable<ArrayBufferViewInput> | PromiseLike<ArrayBufferViewInput> | ArrayBufferViewInput;\n\n/** @ignore */\nexport async function* toArrayBufferViewAsyncIterator<T extends TypedArray>(ArrayCtor: TypedArrayConstructor<T>, source: ArrayBufferViewAsyncIteratorInput): AsyncIterableIterator<T> {\n\n    // if a Promise, unwrap the Promise and iterate the resolved value\n    if (isPromise<ArrayBufferViewInput>(source)) {\n        return yield* toArrayBufferViewAsyncIterator(ArrayCtor, await source);\n    }\n\n    const wrap = async function*<T>(x: T) { yield await x; };\n    const emit = async function* <T extends Iterable<any>>(source: T) {\n        yield* pump((function*(it: Iterator<any>) {\n            let r: IteratorResult<any> = <any> null;\n            do {\n                r = it.next(yield r && r.value);\n            } while (!r.done);\n        })(source[Symbol.iterator]()));\n    };\n\n    const buffers: AsyncIterable<ArrayBufferViewInput> =\n                        (typeof source === 'string') ? wrap(source) // if string, wrap in an AsyncIterableIterator\n                      : (ArrayBuffer.isView(source)) ? wrap(source) // if TypedArray, wrap in an AsyncIterableIterator\n                   : (source instanceof ArrayBuffer) ? wrap(source) // if ArrayBuffer, wrap in an AsyncIterableIterator\n                : (source instanceof SharedArrayBuf) ? wrap(source) // if SharedArrayBuffer, wrap in an AsyncIterableIterator\n          : isIterable<ArrayBufferViewInput>(source) ? emit(source) // If Iterable, wrap in an AsyncIterableIterator and compose the `next` values\n    : !isAsyncIterable<ArrayBufferViewInput>(source) ? wrap(source) // If not an AsyncIterable, treat as a sentinel and wrap in an AsyncIterableIterator\n                                                     : source; // otherwise if AsyncIterable, use it\n\n    yield* pump((async function* (it) {\n        let r: IteratorResult<any> = <any> null;\n        do {\n            r = await it.next(yield toArrayBufferView(ArrayCtor, r));\n        } while (!r.done);\n    })(buffers[Symbol.asyncIterator]()));\n}\n\n/** @ignore */ export const toInt8ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Int8Array, input);\n/** @ignore */ export const toInt16ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Int16Array, input);\n/** @ignore */ export const toInt32ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Int32Array, input);\n/** @ignore */ export const toUint8ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Uint8Array, input);\n/** @ignore */ export const toUint16ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Uint16Array, input);\n/** @ignore */ export const toUint32ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Uint32Array, input);\n/** @ignore */ export const toFloat32ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Float32Array, input);\n/** @ignore */ export const toFloat64ArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Float64Array, input);\n/** @ignore */ export const toUint8ClampedArrayAsyncIterator = (input: ArrayBufferViewAsyncIteratorInput) => toArrayBufferViewAsyncIterator(Uint8ClampedArray, input);\n\n/** @ignore */\nexport function rebaseValueOffsets(offset: number, length: number, valueOffsets: Int32Array) {\n    // If we have a non-zero offset, create a new offsets array with the values\n    // shifted by the start offset, such that the new start offset is 0\n    if (offset !== 0) {\n        valueOffsets = valueOffsets.slice(0, length + 1);\n        for (let i = -1; ++i <= length;) {\n            valueOffsets[i] += offset;\n        }\n    }\n    return valueOffsets;\n}\n\n/** @ignore */\nexport function compareArrayLike<T extends ArrayLike<any>>(a: T, b: T) {\n    let i = 0, n = a.length;\n    if (n !== b.length) { return false; }\n    if (n > 0) {\n        do { if (a[i] !== b[i]) { return false; } } while (++i < n);\n    }\n    return true;\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport {\n    toUint8Array,\n    joinUint8Arrays,\n    ArrayBufferViewInput,\n    toUint8ArrayIterator,\n    toUint8ArrayAsyncIterator\n} from '../util/buffer';\n\nimport { ReadableDOMStreamOptions } from './interfaces';\n\n/** @ignore */\nexport default {\n    fromIterable<T extends ArrayBufferViewInput>(source: Iterable<T> | T): IterableIterator<Uint8Array> {\n        return pump(fromIterable<T>(source));\n    },\n    fromAsyncIterable<T extends ArrayBufferViewInput>(source: AsyncIterable<T> | PromiseLike<T>): AsyncIterableIterator<Uint8Array> {\n        return pump(fromAsyncIterable<T>(source));\n    },\n    fromDOMStream<T extends ArrayBufferViewInput>(source: ReadableStream<T>): AsyncIterableIterator<Uint8Array> {\n        return pump(fromDOMStream<T>(source));\n    },\n    fromNodeStream(stream: NodeJS.ReadableStream): AsyncIterableIterator<Uint8Array> {\n        return pump(fromNodeStream(stream));\n    },\n    // @ts-ignore\n    toDOMStream<T>(source: Iterable<T> | AsyncIterable<T>, options?: ReadableDOMStreamOptions): ReadableStream<T> {\n        throw new Error(`\"toDOMStream\" not available in this environment`);\n    },\n    // @ts-ignore\n    toNodeStream<T>(source: Iterable<T> | AsyncIterable<T>, options?: import('stream').ReadableOptions): import('stream').Readable {\n        throw new Error(`\"toNodeStream\" not available in this environment`);\n    },\n};\n\n/** @ignore */\nconst pump = <T extends Iterator<any> | AsyncIterator<any>>(iterator: T) => { iterator.next(); return iterator; };\n\n/** @ignore */\nfunction* fromIterable<T extends ArrayBufferViewInput>(source: Iterable<T> | T): IterableIterator<Uint8Array> {\n\n    let done: boolean, threw = false;\n    let buffers: Uint8Array[] = [], buffer: Uint8Array;\n    let cmd: 'peek' | 'read', size: number, bufferLength = 0;\n\n    function byteRange() {\n        if (cmd === 'peek') {\n            return joinUint8Arrays(buffers, size)[0];\n        }\n        [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);\n        return buffer;\n    }\n\n    // Yield so the caller can inject the read command before creating the source Iterator\n    ({ cmd, size } = yield <any> null);\n\n    // initialize the iterator\n    let it = toUint8ArrayIterator(source)[Symbol.iterator]();\n\n    try {\n        do {\n            // read the next value\n            ({ done, value: buffer } = isNaN(size - bufferLength) ?\n                it.next(undefined) : it.next(size - bufferLength));\n            // if chunk is not null or empty, push it onto the queue\n            if (!done && buffer.byteLength > 0) {\n                buffers.push(buffer);\n                bufferLength += buffer.byteLength;\n            }\n            // If we have enough bytes in our buffer, yield chunks until we don't\n            if (done || size <= bufferLength) {\n                do {\n                    ({ cmd, size } = yield byteRange());\n                } while (size < bufferLength);\n            }\n        } while (!done);\n    } catch (e) {\n        (threw = true) && (typeof it.throw === 'function') && (it.throw(e));\n    } finally {\n        (threw === false) && (typeof it.return === 'function') && (it.return());\n    }\n}\n\n/** @ignore */\nasync function* fromAsyncIterable<T extends ArrayBufferViewInput>(source: AsyncIterable<T> | PromiseLike<T>): AsyncIterableIterator<Uint8Array> {\n\n    let done: boolean, threw = false;\n    let buffers: Uint8Array[] = [], buffer: Uint8Array;\n    let cmd: 'peek' | 'read', size: number, bufferLength = 0;\n\n    function byteRange() {\n        if (cmd === 'peek') {\n            return joinUint8Arrays(buffers, size)[0];\n        }\n        [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);\n        return buffer;\n    }\n\n    // Yield so the caller can inject the read command before creating the source AsyncIterator\n    ({ cmd, size } = yield <any> null);\n\n    // initialize the iterator\n    let it = toUint8ArrayAsyncIterator(source)[Symbol.asyncIterator]();\n\n    try {\n        do {\n            // read the next value\n            ({ done, value: buffer } = isNaN(size - bufferLength)\n                ? await it.next(undefined)\n                : await it.next(size - bufferLength));\n            // if chunk is not null or empty, push it onto the queue\n            if (!done && buffer.byteLength > 0) {\n                buffers.push(buffer);\n                bufferLength += buffer.byteLength;\n            }\n            // If we have enough bytes in our buffer, yield chunks until we don't\n            if (done || size <= bufferLength) {\n                do {\n                    ({ cmd, size } = yield byteRange());\n                } while (size < bufferLength);\n            }\n        } while (!done);\n    } catch (e) {\n        (threw = true) && (typeof it.throw === 'function') && (await it.throw(e));\n    } finally {\n        (threw === false) && (typeof it.return === 'function') && (await it.return());\n    }\n}\n\n// All this manual Uint8Array chunk management can be avoided if/when engines\n// add support for ArrayBuffer.transfer() or ArrayBuffer.prototype.realloc():\n// https://github.com/domenic/proposal-arraybuffer-transfer\n/** @ignore */\nasync function* fromDOMStream<T extends ArrayBufferViewInput>(source: ReadableStream<T>): AsyncIterableIterator<Uint8Array> {\n\n    let done = false, threw = false;\n    let buffers: Uint8Array[] = [], buffer: Uint8Array;\n    let cmd: 'peek' | 'read', size: number, bufferLength = 0;\n\n    function byteRange() {\n        if (cmd === 'peek') {\n            return joinUint8Arrays(buffers, size)[0];\n        }\n        [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);\n        return buffer;\n    }\n\n    // Yield so the caller can inject the read command before we establish the ReadableStream lock\n    ({ cmd, size } = yield <any> null);\n\n    // initialize the reader and lock the stream\n    let it = new AdaptiveByteReader(source);\n\n    try {\n        do {\n            // read the next value\n            ({ done, value: buffer } = isNaN(size - bufferLength)\n                ? await it['read'](undefined)\n                : await it['read'](size - bufferLength));\n            // if chunk is not null or empty, push it onto the queue\n            if (!done && buffer.byteLength > 0) {\n                buffers.push(toUint8Array(buffer));\n                bufferLength += buffer.byteLength;\n            }\n            // If we have enough bytes in our buffer, yield chunks until we don't\n            if (done || size <= bufferLength) {\n                do {\n                    ({ cmd, size } = yield byteRange());\n                } while (size < bufferLength);\n            }\n        } while (!done);\n    } catch (e) {\n        (threw = true) && (await it['cancel'](e));\n    } finally {\n        (threw === false) ? (await it['cancel']())\n            : source['locked'] && it.releaseLock();\n    }\n}\n\n/** @ignore */\nclass AdaptiveByteReader<T extends ArrayBufferViewInput> {\n\n    private supportsBYOB: boolean;\n    private byobReader: ReadableStreamBYOBReader | null = null;\n    private defaultReader: ReadableStreamDefaultReader<T> | null = null;\n    private reader: ReadableStreamBYOBReader | ReadableStreamDefaultReader<T> | null;\n\n    constructor(private source: ReadableStream<T>) {\n        try {\n            this.supportsBYOB = !!(this.reader = this.getBYOBReader());\n        } catch (e) {\n            this.supportsBYOB = !!!(this.reader = this.getDefaultReader());\n        }\n    }\n\n    get closed(): Promise<void> {\n        return this.reader ? this.reader['closed'].catch(() => {}) : Promise.resolve();\n    }\n\n    releaseLock(): void {\n        if (this.reader) {\n            this.reader.releaseLock();\n        }\n        this.reader = this.byobReader = this.defaultReader = null;\n    }\n\n    async cancel(reason?: any): Promise<void> {\n        const { reader, source } = this;\n        reader && (await reader['cancel'](reason).catch(() => {}));\n        source && (source['locked'] && this.releaseLock());\n    }\n\n    async read(size?: number): Promise<ReadableStreamReadResult<Uint8Array>> {\n        if (size === 0) {\n            return { done: this.reader == null, value: new Uint8Array(0) };\n        }\n        const result = !this.supportsBYOB || typeof size !== 'number'\n            ? await this.getDefaultReader().read()\n            : await this.readFromBYOBReader(size);\n        !result.done && (result.value = toUint8Array(result as ReadableStreamReadResult<Uint8Array>));\n        return result as ReadableStreamReadResult<Uint8Array>;\n    }\n\n    private getDefaultReader() {\n        if (this.byobReader) { this.releaseLock(); }\n        if (!this.defaultReader) {\n            this.defaultReader = this.source['getReader']();\n            // We have to catch and swallow errors here to avoid uncaught promise rejection exceptions\n            // that seem to be raised when we call `releaseLock()` on this reader. I'm still mystified\n            // about why these errors are raised, but I'm sure there's some important spec reason that\n            // I haven't considered. I hate to employ such an anti-pattern here, but it seems like the\n            // only solution in this case :/\n            this.defaultReader['closed'].catch(() => {});\n        }\n        return (this.reader = this.defaultReader);\n    }\n\n    private getBYOBReader() {\n        if (this.defaultReader) { this.releaseLock(); }\n        if (!this.byobReader) {\n            this.byobReader = this.source['getReader']({ mode: 'byob' });\n            // We have to catch and swallow errors here to avoid uncaught promise rejection exceptions\n            // that seem to be raised when we call `releaseLock()` on this reader. I'm still mystified\n            // about why these errors are raised, but I'm sure there's some important spec reason that\n            // I haven't considered. I hate to employ such an anti-pattern here, but it seems like the\n            // only solution in this case :/\n            this.byobReader['closed'].catch(() => {});\n        }\n        return (this.reader = this.byobReader);\n    }\n\n    // This strategy plucked from the example in the streams spec:\n    // https://streams.spec.whatwg.org/#example-manual-read-bytes\n    private async readFromBYOBReader(size: number) {\n        return await readInto(this.getBYOBReader(), new ArrayBuffer(size), 0, size);\n    }\n}\n\n/** @ignore */\nasync function readInto(reader: ReadableStreamBYOBReader, buffer: ArrayBufferLike, offset: number, size: number): Promise<ReadableStreamReadResult<Uint8Array>> {\n    if (offset >= size) {\n        return { done: false, value: new Uint8Array(buffer, 0, size) };\n    }\n    const { done, value } = await reader.read(new Uint8Array(buffer, offset, size - offset));\n    if (((offset += value.byteLength) < size) && !done) {\n        return await readInto(reader, value.buffer, offset, size);\n    }\n    return { done, value: new Uint8Array(value.buffer, 0, offset) };\n}\n\n/** @ignore */\ntype EventName = 'end' | 'error' | 'readable';\n/** @ignore */\ntype Event = [EventName, (_: any) => void, Promise<[EventName, Error | null]>];\n/** @ignore */\nconst onEvent = <T extends string>(stream: NodeJS.ReadableStream, event: T) => {\n    let handler = (_: any) => resolve([event, _]);\n    let resolve: (value?: [T, any] | PromiseLike<[T, any]>) => void;\n    return [event, handler, new Promise<[T, any]>(\n        (r) => (resolve = r) && stream['once'](event, handler)\n    )] as Event;\n};\n\n/** @ignore */\nasync function* fromNodeStream(stream: NodeJS.ReadableStream): AsyncIterableIterator<Uint8Array> {\n\n    let events: Event[] = [];\n    let event: EventName = 'error';\n    let done = false, err: Error | null = null;\n    let cmd: 'peek' | 'read', size: number, bufferLength = 0;\n    let buffers: Uint8Array[] = [], buffer: Uint8Array | Buffer | string;\n\n    function byteRange() {\n        if (cmd === 'peek') {\n            return joinUint8Arrays(buffers, size)[0];\n        }\n        [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);\n        return buffer;\n    }\n\n    // Yield so the caller can inject the read command before we\n    // add the listener for the source stream's 'readable' event.\n    ({ cmd, size } = yield <any> null);\n\n    // ignore stdin if it's a TTY\n    if ((stream as any)['isTTY']) { return yield new Uint8Array(0); }\n\n    try {\n        // initialize the stream event handlers\n        events[0] = onEvent(stream, 'end');\n        events[1] = onEvent(stream, 'error');\n\n        do {\n            events[2] = onEvent(stream, 'readable');\n\n            // wait on the first message event from the stream\n            [event, err] = await Promise.race(events.map((x) => x[2]));\n\n            // if the stream emitted an Error, rethrow it\n            if (event === 'error') { break; }\n            if (!(done = event === 'end')) {\n                // If the size is NaN, request to read everything in the stream's internal buffer\n                if (!isFinite(size - bufferLength)) {\n                    buffer = toUint8Array(stream['read'](undefined));\n                } else {\n                    buffer = toUint8Array(stream['read'](size - bufferLength));\n                    // If the byteLength is 0, then the requested amount is more than the stream has\n                    // in its internal buffer. In this case the stream needs a \"kick\" to tell it to\n                    // continue emitting readable events, so request to read everything the stream\n                    // has in its internal buffer right now.\n                    if (buffer.byteLength < (size - bufferLength)) {\n                        buffer = toUint8Array(stream['read'](undefined));\n                    }\n                }\n                // if chunk is not null or empty, push it onto the queue\n                if (buffer.byteLength > 0) {\n                    buffers.push(buffer);\n                    bufferLength += buffer.byteLength;\n                }\n            }\n            // If we have enough bytes in our buffer, yield chunks until we don't\n            if (done || size <= bufferLength) {\n                do {\n                    ({ cmd, size } = yield byteRange());\n                } while (size < bufferLength);\n            }\n        } while (!done);\n    } finally {\n        await cleanup(events, event === 'error' ? err : null);\n    }\n\n    function cleanup<T extends Error | null | void>(events: Event[], err?: T) {\n        buffer = buffers = <any> null;\n        return new Promise<T>(async (resolve, reject) => {\n            for (const [evt, fn] of events) {\n                stream['off'](evt, fn);\n            }\n            try {\n                // Some stream implementations don't call the destroy callback,\n                // because it's really a node-internal API. Just calling `destroy`\n                // here should be enough to conform to the ReadableStream contract\n                const destroy = (stream as any)['destroy'];\n                destroy && destroy.call(stream, err);\n                err = undefined;\n            } catch (e) { err = e || err; } finally {\n                err != null ? reject(err) : resolve();\n            }\n        });\n    }\n}\n",
-        "import toPropertyKey from \"./toPropertyKey.js\";\nexport default function _defineProperty(obj, key, value) {\n  key = toPropertyKey(key);\n  if (key in obj) {\n    Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: true,\n      configurable: true,\n      writable: true\n    });\n  } else {\n    obj[key] = value;\n  }\n  return obj;\n}",
-        "import defineProperty from \"./defineProperty.js\";\nfunction ownKeys(object, enumerableOnly) {\n  var keys = Object.keys(object);\n  if (Object.getOwnPropertySymbols) {\n    var symbols = Object.getOwnPropertySymbols(object);\n    enumerableOnly && (symbols = symbols.filter(function (sym) {\n      return Object.getOwnPropertyDescriptor(object, sym).enumerable;\n    })), keys.push.apply(keys, symbols);\n  }\n  return keys;\n}\nexport default function _objectSpread2(target) {\n  for (var i = 1; i < arguments.length; i++) {\n    var source = null != arguments[i] ? arguments[i] : {};\n    i % 2 ? ownKeys(Object(source), !0).forEach(function (key) {\n      defineProperty(target, key, source[key]);\n    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)) : ownKeys(Object(source)).forEach(function (key) {\n      Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));\n    });\n  }\n  return target;\n}",
         "import superPropBase from \"./superPropBase.js\";\nexport default function _get() {\n  if (typeof Reflect !== \"undefined\" && Reflect.get) {\n    _get = Reflect.get.bind();\n  } else {\n    _get = function _get(target, property, receiver) {\n      var base = superPropBase(target, property);\n      if (!base) return;\n      var desc = Object.getOwnPropertyDescriptor(base, property);\n      if (desc.get) {\n        return desc.get.call(arguments.length < 3 ? target : receiver);\n      }\n      return desc.value;\n    };\n  }\n  return _get.apply(this, arguments);\n}",
         "import getPrototypeOf from \"./getPrototypeOf.js\";\nexport default function _superPropBase(object, property) {\n  while (!Object.prototype.hasOwnProperty.call(object, property)) {\n    object = getPrototypeOf(object);\n    if (object === null) break;\n  }\n  return object;\n}",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport { Data } from './data';\nimport { DataType } from './type';\nimport { Chunked } from './vector/chunked';\n\n/** @ignore */\nexport interface Clonable<R extends AbstractVector> {\n    clone(...args: any[]): R;\n}\n\n/** @ignore */\nexport interface Sliceable<R extends AbstractVector> {\n    slice(begin?: number, end?: number): R;\n}\n\n/** @ignore */\nexport interface Applicative<T extends DataType, R extends Chunked> {\n    concat(...others: Vector<T>[]): R;\n    readonly [Symbol.isConcatSpreadable]: boolean;\n}\n\nexport interface AbstractVector<T extends DataType = any>\n    extends Clonable<Vector<T>>,\n            Sliceable<Vector<T>>,\n            Applicative<T, Chunked<T>> {\n\n    readonly TType: T['TType'];\n    readonly TArray: T['TArray'];\n    readonly TValue: T['TValue'];\n}\n\nexport abstract class AbstractVector<T extends DataType = any> implements Iterable<T['TValue'] | null> {\n\n    public abstract readonly data: Data<T>;\n    public abstract readonly type: T;\n    public abstract readonly typeId: T['TType'];\n    public abstract readonly length: number;\n    public abstract readonly stride: number;\n    public abstract readonly nullCount: number;\n    public abstract readonly byteLength: number;\n    public abstract readonly numChildren: number;\n\n    public abstract readonly ArrayType: T['ArrayType'];\n\n    public abstract isValid(index: number): boolean;\n    public abstract get(index: number): T['TValue'] | null;\n    public abstract set(index: number, value: T['TValue'] | null): void;\n    public abstract indexOf(value: T['TValue'] | null, fromIndex?: number): number;\n    public abstract [Symbol.iterator](): IterableIterator<T['TValue'] | null>;\n\n    public abstract toArray(): T['TArray'];\n    public abstract getChildAt<R extends DataType = any>(index: number): Vector<R> | null;\n}\n\nexport { AbstractVector as Vector };\n",
         "/* tslint:disable:class-name */\n\n// automatically generated by the FlatBuffers compiler, do not modify\n\nimport { flatbuffers } from 'flatbuffers';\n/**\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum MetadataVersion {\n        /**\n         * 0.1.0\n         */\n        V1 = 0,\n\n        /**\n         * 0.2.0\n         */\n        V2 = 1,\n\n        /**\n         * 0.3.0 -> 0.7.1\n         */\n        V3 = 2,\n\n        /**\n         * >= 0.8.0\n         */\n        V4 = 3\n    }\n}\n\n/**\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum UnionMode {\n        Sparse = 0,\n        Dense = 1\n    }\n}\n\n/**\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum Precision {\n        HALF = 0,\n        SINGLE = 1,\n        DOUBLE = 2\n    }\n}\n\n/**\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum DateUnit {\n        DAY = 0,\n        MILLISECOND = 1\n    }\n}\n\n/**\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum TimeUnit {\n        SECOND = 0,\n        MILLISECOND = 1,\n        MICROSECOND = 2,\n        NANOSECOND = 3\n    }\n}\n\n/**\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum IntervalUnit {\n        YEAR_MONTH = 0,\n        DAY_TIME = 1\n    }\n}\n\n/**\n * ----------------------------------------------------------------------\n * Top-level Type value, enabling extensible type-specific metadata. We can\n * add new logical types to Type without breaking backwards compatibility\n *\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum Type {\n        NONE = 0,\n        Null = 1,\n        Int = 2,\n        FloatingPoint = 3,\n        Binary = 4,\n        Utf8 = 5,\n        Bool = 6,\n        Decimal = 7,\n        Date = 8,\n        Time = 9,\n        Timestamp = 10,\n        Interval = 11,\n        List = 12,\n        Struct_ = 13,\n        Union = 14,\n        FixedSizeBinary = 15,\n        FixedSizeList = 16,\n        Map = 17,\n        Duration = 18,\n        LargeBinary = 19,\n        LargeUtf8 = 20,\n        LargeList = 21\n    }\n}\n\n/**\n * ----------------------------------------------------------------------\n * Endianness of the platform producing the data\n *\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum Endianness {\n        Little = 0,\n        Big = 1\n    }\n}\n\n/**\n * These are stored in the flatbuffer in the Type union below\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Null {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Null\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Null {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Null= obj\n         * @returns Null\n         */\n        static getRootAsNull(bb: flatbuffers.ByteBuffer, obj?: Null): Null {\n            return (obj || new Null).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startNull(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endNull(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createNull(builder: flatbuffers.Builder): flatbuffers.Offset {\n            Null.startNull(builder);\n            return Null.endNull(builder);\n        }\n    }\n}\n/**\n * A Struct_ in the flatbuffer metadata is the same as an Arrow Struct\n * (according to the physical memory layout). We used Struct_ here as\n * Struct is a reserved word in Flatbuffers\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Struct_ {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Struct_\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Struct_ {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Struct_= obj\n         * @returns Struct_\n         */\n        static getRootAsStruct_(bb: flatbuffers.ByteBuffer, obj?: Struct_): Struct_ {\n            return (obj || new Struct_).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startStruct_(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endStruct_(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createStruct_(builder: flatbuffers.Builder): flatbuffers.Offset {\n            Struct_.startStruct_(builder);\n            return Struct_.endStruct_(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class List {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns List\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): List {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param List= obj\n         * @returns List\n         */\n        static getRootAsList(bb: flatbuffers.ByteBuffer, obj?: List): List {\n            return (obj || new List).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startList(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endList(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createList(builder: flatbuffers.Builder): flatbuffers.Offset {\n            List.startList(builder);\n            return List.endList(builder);\n        }\n    }\n}\n/**\n * Same as List, but with 64-bit offsets, allowing to represent\n * extremely large data values.\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class LargeList {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns LargeList\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): LargeList {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param LargeList= obj\n         * @returns LargeList\n         */\n        static getRootAsLargeList(bb: flatbuffers.ByteBuffer, obj?: LargeList): LargeList {\n            return (obj || new LargeList).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startLargeList(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endLargeList(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createLargeList(builder: flatbuffers.Builder): flatbuffers.Offset {\n            LargeList.startLargeList(builder);\n            return LargeList.endLargeList(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class FixedSizeList {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns FixedSizeList\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): FixedSizeList {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param FixedSizeList= obj\n         * @returns FixedSizeList\n         */\n        static getRootAsFixedSizeList(bb: flatbuffers.ByteBuffer, obj?: FixedSizeList): FixedSizeList {\n            return (obj || new FixedSizeList).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * Number of list items per value\n         *\n         * @returns number\n         */\n        listSize(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt32(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startFixedSizeList(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number listSize\n         */\n        static addListSize(builder: flatbuffers.Builder, listSize: number) {\n            builder.addFieldInt32(0, listSize, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endFixedSizeList(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createFixedSizeList(builder: flatbuffers.Builder, listSize: number): flatbuffers.Offset {\n            FixedSizeList.startFixedSizeList(builder);\n            FixedSizeList.addListSize(builder, listSize);\n            return FixedSizeList.endFixedSizeList(builder);\n        }\n    }\n}\n/**\n * A Map is a logical nested type that is represented as\n *\n * List<entry: Struct<key: K, value: V>>\n *\n * In this layout, the keys and values are each respectively contiguous. We do\n * not constrain the key and value types, so the application is responsible\n * for ensuring that the keys are hashable and unique. Whether the keys are sorted\n * may be set in the metadata for this field\n *\n * In a Field with Map type, the Field has a child Struct field, which then\n * has two children: key type and the second the value type. The names of the\n * child fields may be respectively \"entry\", \"key\", and \"value\", but this is\n * not enforced\n *\n * Map\n *   - child[0] entry: Struct\n *     - child[0] key: K\n *     - child[1] value: V\n *\n * Neither the \"entry\" field nor the \"key\" field may be nullable.\n *\n * The metadata is structured so that Arrow systems without special handling\n * for Map can make Map an alias for List. The \"layout\" attribute for the Map\n * field must have the same contents as a List.\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Map {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Map\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Map {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Map= obj\n         * @returns Map\n         */\n        static getRootAsMap(bb: flatbuffers.ByteBuffer, obj?: Map): Map {\n            return (obj || new Map).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * Set to true if the keys within each value are sorted\n         *\n         * @returns boolean\n         */\n        keysSorted(): boolean {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? !!this.bb!.readInt8(this.bb_pos + offset) : false;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startMap(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param boolean keysSorted\n         */\n        static addKeysSorted(builder: flatbuffers.Builder, keysSorted: boolean) {\n            builder.addFieldInt8(0, +keysSorted, +false);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endMap(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createMap(builder: flatbuffers.Builder, keysSorted: boolean): flatbuffers.Offset {\n            Map.startMap(builder);\n            Map.addKeysSorted(builder, keysSorted);\n            return Map.endMap(builder);\n        }\n    }\n}\n/**\n * A union is a complex type with children in Field\n * By default ids in the type vector refer to the offsets in the children\n * optionally typeIds provides an indirection between the child offset and the type id\n * for each child typeIds[offset] is the id used in the type vector\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Union {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Union\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Union {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Union= obj\n         * @returns Union\n         */\n        static getRootAsUnion(bb: flatbuffers.ByteBuffer, obj?: Union): Union {\n            return (obj || new Union).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.UnionMode\n         */\n        mode(): org.apache.arrow.flatbuf.UnionMode {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.UnionMode.Sparse;\n        }\n\n        /**\n         * @param number index\n         * @returns number\n         */\n        typeIds(index: number): number | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.readInt32(this.bb!.__vector(this.bb_pos + offset) + index * 4) : 0;\n        }\n\n        /**\n         * @returns number\n         */\n        typeIdsLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @returns Int32Array\n         */\n        typeIdsArray(): Int32Array | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? new Int32Array(this.bb!.bytes().buffer, this.bb!.bytes().byteOffset + this.bb!.__vector(this.bb_pos + offset), this.bb!.__vector_len(this.bb_pos + offset)) : null;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startUnion(builder: flatbuffers.Builder) {\n            builder.startObject(2);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.UnionMode mode\n         */\n        static addMode(builder: flatbuffers.Builder, mode: org.apache.arrow.flatbuf.UnionMode) {\n            builder.addFieldInt16(0, mode, org.apache.arrow.flatbuf.UnionMode.Sparse);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset typeIdsOffset\n         */\n        static addTypeIds(builder: flatbuffers.Builder, typeIdsOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, typeIdsOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param Array.<number> data\n         * @returns flatbuffers.Offset\n         */\n        static createTypeIdsVector(builder: flatbuffers.Builder, data: number[] | Int32Array): flatbuffers.Offset {\n            builder.startVector(4, data.length, 4);\n            for (let i = data.length - 1; i >= 0; i--) {\n                builder.addInt32(data[i]);\n            }\n            return builder.endVector();\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startTypeIdsVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(4, numElems, 4);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endUnion(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createUnion(builder: flatbuffers.Builder, mode: org.apache.arrow.flatbuf.UnionMode, typeIdsOffset: flatbuffers.Offset): flatbuffers.Offset {\n            Union.startUnion(builder);\n            Union.addMode(builder, mode);\n            Union.addTypeIds(builder, typeIdsOffset);\n            return Union.endUnion(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Int {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Int\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Int {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Int= obj\n         * @returns Int\n         */\n        static getRootAsInt(bb: flatbuffers.ByteBuffer, obj?: Int): Int {\n            return (obj || new Int).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns number\n         */\n        bitWidth(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt32(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @returns boolean\n         */\n        isSigned(): boolean {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? !!this.bb!.readInt8(this.bb_pos + offset) : false;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startInt(builder: flatbuffers.Builder) {\n            builder.startObject(2);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number bitWidth\n         */\n        static addBitWidth(builder: flatbuffers.Builder, bitWidth: number) {\n            builder.addFieldInt32(0, bitWidth, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param boolean isSigned\n         */\n        static addIsSigned(builder: flatbuffers.Builder, isSigned: boolean) {\n            builder.addFieldInt8(1, +isSigned, +false);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endInt(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createInt(builder: flatbuffers.Builder, bitWidth: number, isSigned: boolean): flatbuffers.Offset {\n            Int.startInt(builder);\n            Int.addBitWidth(builder, bitWidth);\n            Int.addIsSigned(builder, isSigned);\n            return Int.endInt(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class FloatingPoint {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns FloatingPoint\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): FloatingPoint {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param FloatingPoint= obj\n         * @returns FloatingPoint\n         */\n        static getRootAsFloatingPoint(bb: flatbuffers.ByteBuffer, obj?: FloatingPoint): FloatingPoint {\n            return (obj || new FloatingPoint).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.Precision\n         */\n        precision(): org.apache.arrow.flatbuf.Precision {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.Precision.HALF;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startFloatingPoint(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.Precision precision\n         */\n        static addPrecision(builder: flatbuffers.Builder, precision: org.apache.arrow.flatbuf.Precision) {\n            builder.addFieldInt16(0, precision, org.apache.arrow.flatbuf.Precision.HALF);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endFloatingPoint(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createFloatingPoint(builder: flatbuffers.Builder, precision: org.apache.arrow.flatbuf.Precision): flatbuffers.Offset {\n            FloatingPoint.startFloatingPoint(builder);\n            FloatingPoint.addPrecision(builder, precision);\n            return FloatingPoint.endFloatingPoint(builder);\n        }\n    }\n}\n/**\n * Unicode with UTF-8 encoding\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Utf8 {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Utf8\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Utf8 {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Utf8= obj\n         * @returns Utf8\n         */\n        static getRootAsUtf8(bb: flatbuffers.ByteBuffer, obj?: Utf8): Utf8 {\n            return (obj || new Utf8).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startUtf8(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endUtf8(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createUtf8(builder: flatbuffers.Builder): flatbuffers.Offset {\n            Utf8.startUtf8(builder);\n            return Utf8.endUtf8(builder);\n        }\n    }\n}\n/**\n * Opaque binary data\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Binary {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Binary\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Binary {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Binary= obj\n         * @returns Binary\n         */\n        static getRootAsBinary(bb: flatbuffers.ByteBuffer, obj?: Binary): Binary {\n            return (obj || new Binary).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startBinary(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endBinary(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createBinary(builder: flatbuffers.Builder): flatbuffers.Offset {\n            Binary.startBinary(builder);\n            return Binary.endBinary(builder);\n        }\n    }\n}\n/**\n * Same as Utf8, but with 64-bit offsets, allowing to represent\n * extremely large data values.\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class LargeUtf8 {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns LargeUtf8\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): LargeUtf8 {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param LargeUtf8= obj\n         * @returns LargeUtf8\n         */\n        static getRootAsLargeUtf8(bb: flatbuffers.ByteBuffer, obj?: LargeUtf8): LargeUtf8 {\n            return (obj || new LargeUtf8).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startLargeUtf8(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endLargeUtf8(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createLargeUtf8(builder: flatbuffers.Builder): flatbuffers.Offset {\n            LargeUtf8.startLargeUtf8(builder);\n            return LargeUtf8.endLargeUtf8(builder);\n        }\n    }\n}\n/**\n * Same as Binary, but with 64-bit offsets, allowing to represent\n * extremely large data values.\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class LargeBinary {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns LargeBinary\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): LargeBinary {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param LargeBinary= obj\n         * @returns LargeBinary\n         */\n        static getRootAsLargeBinary(bb: flatbuffers.ByteBuffer, obj?: LargeBinary): LargeBinary {\n            return (obj || new LargeBinary).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startLargeBinary(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endLargeBinary(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createLargeBinary(builder: flatbuffers.Builder): flatbuffers.Offset {\n            LargeBinary.startLargeBinary(builder);\n            return LargeBinary.endLargeBinary(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class FixedSizeBinary {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns FixedSizeBinary\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): FixedSizeBinary {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param FixedSizeBinary= obj\n         * @returns FixedSizeBinary\n         */\n        static getRootAsFixedSizeBinary(bb: flatbuffers.ByteBuffer, obj?: FixedSizeBinary): FixedSizeBinary {\n            return (obj || new FixedSizeBinary).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * Number of bytes per value\n         *\n         * @returns number\n         */\n        byteWidth(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt32(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startFixedSizeBinary(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number byteWidth\n         */\n        static addByteWidth(builder: flatbuffers.Builder, byteWidth: number) {\n            builder.addFieldInt32(0, byteWidth, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endFixedSizeBinary(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createFixedSizeBinary(builder: flatbuffers.Builder, byteWidth: number): flatbuffers.Offset {\n            FixedSizeBinary.startFixedSizeBinary(builder);\n            FixedSizeBinary.addByteWidth(builder, byteWidth);\n            return FixedSizeBinary.endFixedSizeBinary(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Bool {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Bool\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Bool {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Bool= obj\n         * @returns Bool\n         */\n        static getRootAsBool(bb: flatbuffers.ByteBuffer, obj?: Bool): Bool {\n            return (obj || new Bool).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startBool(builder: flatbuffers.Builder) {\n            builder.startObject(0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endBool(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createBool(builder: flatbuffers.Builder): flatbuffers.Offset {\n            Bool.startBool(builder);\n            return Bool.endBool(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Decimal {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Decimal\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Decimal {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Decimal= obj\n         * @returns Decimal\n         */\n        static getRootAsDecimal(bb: flatbuffers.ByteBuffer, obj?: Decimal): Decimal {\n            return (obj || new Decimal).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * Total number of decimal digits\n         *\n         * @returns number\n         */\n        precision(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt32(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * Number of digits after the decimal point \".\"\n         *\n         * @returns number\n         */\n        scale(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.readInt32(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startDecimal(builder: flatbuffers.Builder) {\n            builder.startObject(2);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number precision\n         */\n        static addPrecision(builder: flatbuffers.Builder, precision: number) {\n            builder.addFieldInt32(0, precision, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number scale\n         */\n        static addScale(builder: flatbuffers.Builder, scale: number) {\n            builder.addFieldInt32(1, scale, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endDecimal(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createDecimal(builder: flatbuffers.Builder, precision: number, scale: number): flatbuffers.Offset {\n            Decimal.startDecimal(builder);\n            Decimal.addPrecision(builder, precision);\n            Decimal.addScale(builder, scale);\n            return Decimal.endDecimal(builder);\n        }\n    }\n}\n/**\n * Date is either a 32-bit or 64-bit type representing elapsed time since UNIX\n * epoch (1970-01-01), stored in either of two units:\n *\n * * Milliseconds (64 bits) indicating UNIX time elapsed since the epoch (no\n *   leap seconds), where the values are evenly divisible by 86400000\n * * Days (32 bits) since the UNIX epoch\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Date {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Date\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Date {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Date= obj\n         * @returns Date\n         */\n        static getRootAsDate(bb: flatbuffers.ByteBuffer, obj?: Date): Date {\n            return (obj || new Date).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.DateUnit\n         */\n        unit(): org.apache.arrow.flatbuf.DateUnit {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.DateUnit.MILLISECOND;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startDate(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.DateUnit unit\n         */\n        static addUnit(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.DateUnit) {\n            builder.addFieldInt16(0, unit, org.apache.arrow.flatbuf.DateUnit.MILLISECOND);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endDate(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createDate(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.DateUnit): flatbuffers.Offset {\n            Date.startDate(builder);\n            Date.addUnit(builder, unit);\n            return Date.endDate(builder);\n        }\n    }\n}\n/**\n * Time type. The physical storage type depends on the unit\n * - SECOND and MILLISECOND: 32 bits\n * - MICROSECOND and NANOSECOND: 64 bits\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Time {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Time\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Time {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Time= obj\n         * @returns Time\n         */\n        static getRootAsTime(bb: flatbuffers.ByteBuffer, obj?: Time): Time {\n            return (obj || new Time).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.TimeUnit\n         */\n        unit(): org.apache.arrow.flatbuf.TimeUnit {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.TimeUnit.MILLISECOND;\n        }\n\n        /**\n         * @returns number\n         */\n        bitWidth(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.readInt32(this.bb_pos + offset) : 32;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startTime(builder: flatbuffers.Builder) {\n            builder.startObject(2);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.TimeUnit unit\n         */\n        static addUnit(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.TimeUnit) {\n            builder.addFieldInt16(0, unit, org.apache.arrow.flatbuf.TimeUnit.MILLISECOND);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number bitWidth\n         */\n        static addBitWidth(builder: flatbuffers.Builder, bitWidth: number) {\n            builder.addFieldInt32(1, bitWidth, 32);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endTime(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createTime(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.TimeUnit, bitWidth: number): flatbuffers.Offset {\n            Time.startTime(builder);\n            Time.addUnit(builder, unit);\n            Time.addBitWidth(builder, bitWidth);\n            return Time.endTime(builder);\n        }\n    }\n}\n/**\n * Time elapsed from the Unix epoch, 00:00:00.000 on 1 January 1970, excluding\n * leap seconds, as a 64-bit integer. Note that UNIX time does not include\n * leap seconds.\n *\n * The Timestamp metadata supports both \"time zone naive\" and \"time zone\n * aware\" timestamps. Read about the timezone attribute for more detail\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Timestamp {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Timestamp\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Timestamp {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Timestamp= obj\n         * @returns Timestamp\n         */\n        static getRootAsTimestamp(bb: flatbuffers.ByteBuffer, obj?: Timestamp): Timestamp {\n            return (obj || new Timestamp).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.TimeUnit\n         */\n        unit(): org.apache.arrow.flatbuf.TimeUnit {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.TimeUnit.SECOND;\n        }\n\n        /**\n         * The time zone is a string indicating the name of a time zone, one of:\n         *\n         * * As used in the Olson time zone database (the \"tz database\" or\n         *   \"tzdata\"), such as \"America/New_York\"\n         * * An absolute time zone offset of the form +XX:XX or -XX:XX, such as +07:30\n         *\n         * Whether a timezone string is present indicates different semantics about\n         * the data:\n         *\n         * * If the time zone is null or equal to an empty string, the data is \"time\n         *   zone naive\" and shall be displayed *as is* to the user, not localized\n         *   to the locale of the user. This data can be though of as UTC but\n         *   without having \"UTC\" as the time zone, it is not considered to be\n         *   localized to any time zone\n         *\n         * * If the time zone is set to a valid value, values can be displayed as\n         *   \"localized\" to that time zone, even though the underlying 64-bit\n         *   integers are identical to the same data stored in UTC. Converting\n         *   between time zones is a metadata-only operation and does not change the\n         *   underlying values\n         *\n         * @param flatbuffers.Encoding= optionalEncoding\n         * @returns string|Uint8Array|null\n         */\n        timezone(): string | null;\n        timezone(optionalEncoding: flatbuffers.Encoding): string | Uint8Array | null;\n        timezone(optionalEncoding?: any): string | Uint8Array | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.__string(this.bb_pos + offset, optionalEncoding) : null;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startTimestamp(builder: flatbuffers.Builder) {\n            builder.startObject(2);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.TimeUnit unit\n         */\n        static addUnit(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.TimeUnit) {\n            builder.addFieldInt16(0, unit, org.apache.arrow.flatbuf.TimeUnit.SECOND);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset timezoneOffset\n         */\n        static addTimezone(builder: flatbuffers.Builder, timezoneOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, timezoneOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endTimestamp(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createTimestamp(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.TimeUnit, timezoneOffset: flatbuffers.Offset): flatbuffers.Offset {\n            Timestamp.startTimestamp(builder);\n            Timestamp.addUnit(builder, unit);\n            Timestamp.addTimezone(builder, timezoneOffset);\n            return Timestamp.endTimestamp(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Interval {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Interval\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Interval {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Interval= obj\n         * @returns Interval\n         */\n        static getRootAsInterval(bb: flatbuffers.ByteBuffer, obj?: Interval): Interval {\n            return (obj || new Interval).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.IntervalUnit\n         */\n        unit(): org.apache.arrow.flatbuf.IntervalUnit {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.IntervalUnit.YEAR_MONTH;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startInterval(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.IntervalUnit unit\n         */\n        static addUnit(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.IntervalUnit) {\n            builder.addFieldInt16(0, unit, org.apache.arrow.flatbuf.IntervalUnit.YEAR_MONTH);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endInterval(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createInterval(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.IntervalUnit): flatbuffers.Offset {\n            Interval.startInterval(builder);\n            Interval.addUnit(builder, unit);\n            return Interval.endInterval(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Duration {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Duration\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Duration {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Duration= obj\n         * @returns Duration\n         */\n        static getRootAsDuration(bb: flatbuffers.ByteBuffer, obj?: Duration): Duration {\n            return (obj || new Duration).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.TimeUnit\n         */\n        unit(): org.apache.arrow.flatbuf.TimeUnit {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.TimeUnit.MILLISECOND;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startDuration(builder: flatbuffers.Builder) {\n            builder.startObject(1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.TimeUnit unit\n         */\n        static addUnit(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.TimeUnit) {\n            builder.addFieldInt16(0, unit, org.apache.arrow.flatbuf.TimeUnit.MILLISECOND);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endDuration(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createDuration(builder: flatbuffers.Builder, unit: org.apache.arrow.flatbuf.TimeUnit): flatbuffers.Offset {\n            Duration.startDuration(builder);\n            Duration.addUnit(builder, unit);\n            return Duration.endDuration(builder);\n        }\n    }\n}\n/**\n * ----------------------------------------------------------------------\n * user defined key value pairs to add custom metadata to arrow\n * key namespacing is the responsibility of the user\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class KeyValue {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns KeyValue\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): KeyValue {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param KeyValue= obj\n         * @returns KeyValue\n         */\n        static getRootAsKeyValue(bb: flatbuffers.ByteBuffer, obj?: KeyValue): KeyValue {\n            return (obj || new KeyValue).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @param flatbuffers.Encoding= optionalEncoding\n         * @returns string|Uint8Array|null\n         */\n        key(): string | null;\n        key(optionalEncoding: flatbuffers.Encoding): string | Uint8Array | null;\n        key(optionalEncoding?: any): string | Uint8Array | null {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.__string(this.bb_pos + offset, optionalEncoding) : null;\n        }\n\n        /**\n         * @param flatbuffers.Encoding= optionalEncoding\n         * @returns string|Uint8Array|null\n         */\n        value(): string | null;\n        value(optionalEncoding: flatbuffers.Encoding): string | Uint8Array | null;\n        value(optionalEncoding?: any): string | Uint8Array | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.__string(this.bb_pos + offset, optionalEncoding) : null;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startKeyValue(builder: flatbuffers.Builder) {\n            builder.startObject(2);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset keyOffset\n         */\n        static addKey(builder: flatbuffers.Builder, keyOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(0, keyOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset valueOffset\n         */\n        static addValue(builder: flatbuffers.Builder, valueOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, valueOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endKeyValue(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createKeyValue(builder: flatbuffers.Builder, keyOffset: flatbuffers.Offset, valueOffset: flatbuffers.Offset): flatbuffers.Offset {\n            KeyValue.startKeyValue(builder);\n            KeyValue.addKey(builder, keyOffset);\n            KeyValue.addValue(builder, valueOffset);\n            return KeyValue.endKeyValue(builder);\n        }\n    }\n}\n/**\n * ----------------------------------------------------------------------\n * Dictionary encoding metadata\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class DictionaryEncoding {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns DictionaryEncoding\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): DictionaryEncoding {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param DictionaryEncoding= obj\n         * @returns DictionaryEncoding\n         */\n        static getRootAsDictionaryEncoding(bb: flatbuffers.ByteBuffer, obj?: DictionaryEncoding): DictionaryEncoding {\n            return (obj || new DictionaryEncoding).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * The known dictionary id in the application where this data is used. In\n         * the file or streaming formats, the dictionary ids are found in the\n         * DictionaryBatch messages\n         *\n         * @returns flatbuffers.Long\n         */\n        id(): flatbuffers.Long {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt64(this.bb_pos + offset) : this.bb!.createLong(0, 0);\n        }\n\n        /**\n         * The dictionary indices are constrained to be positive integers. If this\n         * field is null, the indices must be signed int32\n         *\n         * @param org.apache.arrow.flatbuf.Int= obj\n         * @returns org.apache.arrow.flatbuf.Int|null\n         */\n        indexType(obj?: org.apache.arrow.flatbuf.Int): org.apache.arrow.flatbuf.Int | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? (obj || new org.apache.arrow.flatbuf.Int).__init(this.bb!.__indirect(this.bb_pos + offset), this.bb!) : null;\n        }\n\n        /**\n         * By default, dictionaries are not ordered, or the order does not have\n         * semantic meaning. In some statistical, applications, dictionary-encoding\n         * is used to represent ordered categorical data, and we provide a way to\n         * preserve that metadata here\n         *\n         * @returns boolean\n         */\n        isOrdered(): boolean {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? !!this.bb!.readInt8(this.bb_pos + offset) : false;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startDictionaryEncoding(builder: flatbuffers.Builder) {\n            builder.startObject(3);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Long id\n         */\n        static addId(builder: flatbuffers.Builder, id: flatbuffers.Long) {\n            builder.addFieldInt64(0, id, builder.createLong(0, 0));\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset indexTypeOffset\n         */\n        static addIndexType(builder: flatbuffers.Builder, indexTypeOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, indexTypeOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param boolean isOrdered\n         */\n        static addIsOrdered(builder: flatbuffers.Builder, isOrdered: boolean) {\n            builder.addFieldInt8(2, +isOrdered, +false);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endDictionaryEncoding(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createDictionaryEncoding(builder: flatbuffers.Builder, id: flatbuffers.Long, indexTypeOffset: flatbuffers.Offset, isOrdered: boolean): flatbuffers.Offset {\n            DictionaryEncoding.startDictionaryEncoding(builder);\n            DictionaryEncoding.addId(builder, id);\n            DictionaryEncoding.addIndexType(builder, indexTypeOffset);\n            DictionaryEncoding.addIsOrdered(builder, isOrdered);\n            return DictionaryEncoding.endDictionaryEncoding(builder);\n        }\n    }\n}\n/**\n * ----------------------------------------------------------------------\n * A field represents a named column in a record / row batch or child of a\n * nested type.\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Field {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Field\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Field {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Field= obj\n         * @returns Field\n         */\n        static getRootAsField(bb: flatbuffers.ByteBuffer, obj?: Field): Field {\n            return (obj || new Field).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * Name is not required, in i.e. a List\n         *\n         * @param flatbuffers.Encoding= optionalEncoding\n         * @returns string|Uint8Array|null\n         */\n        name(): string | null;\n        name(optionalEncoding: flatbuffers.Encoding): string | Uint8Array | null;\n        name(optionalEncoding?: any): string | Uint8Array | null {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.__string(this.bb_pos + offset, optionalEncoding) : null;\n        }\n\n        /**\n         * Whether or not this field can contain nulls. Should be true in general.\n         *\n         * @returns boolean\n         */\n        nullable(): boolean {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? !!this.bb!.readInt8(this.bb_pos + offset) : false;\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.Type\n         */\n        typeType(): org.apache.arrow.flatbuf.Type {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? /**  */ (this.bb!.readUint8(this.bb_pos + offset)) : org.apache.arrow.flatbuf.Type.NONE;\n        }\n\n        /**\n         * This is the type of the decoded value if the field is dictionary encoded.\n         *\n         * @param flatbuffers.Table obj\n         * @returns ?flatbuffers.Table\n         */\n        type<T extends flatbuffers.Table>(obj: T): T | null {\n            let offset = this.bb!.__offset(this.bb_pos, 10);\n            return offset ? this.bb!.__union(obj, this.bb_pos + offset) : null;\n        }\n\n        /**\n         * Present only if the field is dictionary encoded.\n         *\n         * @param org.apache.arrow.flatbuf.DictionaryEncoding= obj\n         * @returns org.apache.arrow.flatbuf.DictionaryEncoding|null\n         */\n        dictionary(obj?: org.apache.arrow.flatbuf.DictionaryEncoding): org.apache.arrow.flatbuf.DictionaryEncoding | null {\n            let offset = this.bb!.__offset(this.bb_pos, 12);\n            return offset ? (obj || new org.apache.arrow.flatbuf.DictionaryEncoding).__init(this.bb!.__indirect(this.bb_pos + offset), this.bb!) : null;\n        }\n\n        /**\n         * children apply only to nested data types like Struct, List and Union. For\n         * primitive types children will have length 0.\n         *\n         * @param number index\n         * @param org.apache.arrow.flatbuf.Field= obj\n         * @returns org.apache.arrow.flatbuf.Field\n         */\n        children(index: number, obj?: org.apache.arrow.flatbuf.Field): org.apache.arrow.flatbuf.Field | null {\n            let offset = this.bb!.__offset(this.bb_pos, 14);\n            return offset ? (obj || new org.apache.arrow.flatbuf.Field).__init(this.bb!.__indirect(this.bb!.__vector(this.bb_pos + offset) + index * 4), this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        childrenLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 14);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * User-defined metadata\n         *\n         * @param number index\n         * @param org.apache.arrow.flatbuf.KeyValue= obj\n         * @returns org.apache.arrow.flatbuf.KeyValue\n         */\n        customMetadata(index: number, obj?: org.apache.arrow.flatbuf.KeyValue): org.apache.arrow.flatbuf.KeyValue | null {\n            let offset = this.bb!.__offset(this.bb_pos, 16);\n            return offset ? (obj || new org.apache.arrow.flatbuf.KeyValue).__init(this.bb!.__indirect(this.bb!.__vector(this.bb_pos + offset) + index * 4), this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        customMetadataLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 16);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startField(builder: flatbuffers.Builder) {\n            builder.startObject(7);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset nameOffset\n         */\n        static addName(builder: flatbuffers.Builder, nameOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(0, nameOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param boolean nullable\n         */\n        static addNullable(builder: flatbuffers.Builder, nullable: boolean) {\n            builder.addFieldInt8(1, +nullable, +false);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.Type typeType\n         */\n        static addTypeType(builder: flatbuffers.Builder, typeType: org.apache.arrow.flatbuf.Type) {\n            builder.addFieldInt8(2, typeType, org.apache.arrow.flatbuf.Type.NONE);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset typeOffset\n         */\n        static addType(builder: flatbuffers.Builder, typeOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(3, typeOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset dictionaryOffset\n         */\n        static addDictionary(builder: flatbuffers.Builder, dictionaryOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(4, dictionaryOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset childrenOffset\n         */\n        static addChildren(builder: flatbuffers.Builder, childrenOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(5, childrenOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param Array.<flatbuffers.Offset> data\n         * @returns flatbuffers.Offset\n         */\n        static createChildrenVector(builder: flatbuffers.Builder, data: flatbuffers.Offset[]): flatbuffers.Offset {\n            builder.startVector(4, data.length, 4);\n            for (let i = data.length - 1; i >= 0; i--) {\n                builder.addOffset(data[i]);\n            }\n            return builder.endVector();\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startChildrenVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(4, numElems, 4);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset customMetadataOffset\n         */\n        static addCustomMetadata(builder: flatbuffers.Builder, customMetadataOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(6, customMetadataOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param Array.<flatbuffers.Offset> data\n         * @returns flatbuffers.Offset\n         */\n        static createCustomMetadataVector(builder: flatbuffers.Builder, data: flatbuffers.Offset[]): flatbuffers.Offset {\n            builder.startVector(4, data.length, 4);\n            for (let i = data.length - 1; i >= 0; i--) {\n                builder.addOffset(data[i]);\n            }\n            return builder.endVector();\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startCustomMetadataVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(4, numElems, 4);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endField(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createField(builder: flatbuffers.Builder, nameOffset: flatbuffers.Offset, nullable: boolean, typeType: org.apache.arrow.flatbuf.Type, typeOffset: flatbuffers.Offset, dictionaryOffset: flatbuffers.Offset, childrenOffset: flatbuffers.Offset, customMetadataOffset: flatbuffers.Offset): flatbuffers.Offset {\n            Field.startField(builder);\n            Field.addName(builder, nameOffset);\n            Field.addNullable(builder, nullable);\n            Field.addTypeType(builder, typeType);\n            Field.addType(builder, typeOffset);\n            Field.addDictionary(builder, dictionaryOffset);\n            Field.addChildren(builder, childrenOffset);\n            Field.addCustomMetadata(builder, customMetadataOffset);\n            return Field.endField(builder);\n        }\n    }\n}\n/**\n * ----------------------------------------------------------------------\n * A Buffer represents a single contiguous memory segment\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Buffer {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Buffer\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Buffer {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * The relative offset into the shared memory page where the bytes for this\n         * buffer starts\n         *\n         * @returns flatbuffers.Long\n         */\n        offset(): flatbuffers.Long {\n            return this.bb!.readInt64(this.bb_pos);\n        }\n\n        /**\n         * The absolute length (in bytes) of the memory buffer. The memory is found\n         * from offset (inclusive) to offset + length (non-inclusive).\n         *\n         * @returns flatbuffers.Long\n         */\n        length(): flatbuffers.Long {\n            return this.bb!.readInt64(this.bb_pos + 8);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Long offset\n         * @param flatbuffers.Long length\n         * @returns flatbuffers.Offset\n         */\n        static createBuffer(builder: flatbuffers.Builder, offset: flatbuffers.Long, length: flatbuffers.Long): flatbuffers.Offset {\n            builder.prep(8, 16);\n            builder.writeInt64(length);\n            builder.writeInt64(offset);\n            return builder.offset();\n        }\n\n    }\n}\n/**\n * ----------------------------------------------------------------------\n * A Schema describes the columns in a row batch\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Schema {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Schema\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Schema {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Schema= obj\n         * @returns Schema\n         */\n        static getRootAsSchema(bb: flatbuffers.ByteBuffer, obj?: Schema): Schema {\n            return (obj || new Schema).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * endianness of the buffer\n         * it is Little Endian by default\n         * if endianness doesn't match the underlying system then the vectors need to be converted\n         *\n         * @returns org.apache.arrow.flatbuf.Endianness\n         */\n        endianness(): org.apache.arrow.flatbuf.Endianness {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : org.apache.arrow.flatbuf.Endianness.Little;\n        }\n\n        /**\n         * @param number index\n         * @param org.apache.arrow.flatbuf.Field= obj\n         * @returns org.apache.arrow.flatbuf.Field\n         */\n        fields(index: number, obj?: org.apache.arrow.flatbuf.Field): org.apache.arrow.flatbuf.Field | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? (obj || new org.apache.arrow.flatbuf.Field).__init(this.bb!.__indirect(this.bb!.__vector(this.bb_pos + offset) + index * 4), this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        fieldsLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param number index\n         * @param org.apache.arrow.flatbuf.KeyValue= obj\n         * @returns org.apache.arrow.flatbuf.KeyValue\n         */\n        customMetadata(index: number, obj?: org.apache.arrow.flatbuf.KeyValue): org.apache.arrow.flatbuf.KeyValue | null {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? (obj || new org.apache.arrow.flatbuf.KeyValue).__init(this.bb!.__indirect(this.bb!.__vector(this.bb_pos + offset) + index * 4), this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        customMetadataLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startSchema(builder: flatbuffers.Builder) {\n            builder.startObject(3);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.Endianness endianness\n         */\n        static addEndianness(builder: flatbuffers.Builder, endianness: org.apache.arrow.flatbuf.Endianness) {\n            builder.addFieldInt16(0, endianness, org.apache.arrow.flatbuf.Endianness.Little);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset fieldsOffset\n         */\n        static addFields(builder: flatbuffers.Builder, fieldsOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, fieldsOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param Array.<flatbuffers.Offset> data\n         * @returns flatbuffers.Offset\n         */\n        static createFieldsVector(builder: flatbuffers.Builder, data: flatbuffers.Offset[]): flatbuffers.Offset {\n            builder.startVector(4, data.length, 4);\n            for (let i = data.length - 1; i >= 0; i--) {\n                builder.addOffset(data[i]);\n            }\n            return builder.endVector();\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startFieldsVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(4, numElems, 4);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset customMetadataOffset\n         */\n        static addCustomMetadata(builder: flatbuffers.Builder, customMetadataOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(2, customMetadataOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param Array.<flatbuffers.Offset> data\n         * @returns flatbuffers.Offset\n         */\n        static createCustomMetadataVector(builder: flatbuffers.Builder, data: flatbuffers.Offset[]): flatbuffers.Offset {\n            builder.startVector(4, data.length, 4);\n            for (let i = data.length - 1; i >= 0; i--) {\n                builder.addOffset(data[i]);\n            }\n            return builder.endVector();\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startCustomMetadataVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(4, numElems, 4);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endSchema(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset offset\n         */\n        static finishSchemaBuffer(builder: flatbuffers.Builder, offset: flatbuffers.Offset) {\n            builder.finish(offset);\n        }\n\n        static createSchema(builder: flatbuffers.Builder, endianness: org.apache.arrow.flatbuf.Endianness, fieldsOffset: flatbuffers.Offset, customMetadataOffset: flatbuffers.Offset): flatbuffers.Offset {\n            Schema.startSchema(builder);\n            Schema.addEndianness(builder, endianness);\n            Schema.addFields(builder, fieldsOffset);\n            Schema.addCustomMetadata(builder, customMetadataOffset);\n            return Schema.endSchema(builder);\n        }\n    }\n}\n",
         "// automatically generated by the FlatBuffers compiler, do not modify\n\nimport { flatbuffers } from 'flatbuffers';\nimport * as NS7624605610262437867 from './Schema';\nexport namespace org.apache.arrow.flatbuf {\n    export import Schema = NS7624605610262437867.org.apache.arrow.flatbuf.Schema;\n}\n/**\n * ----------------------------------------------------------------------\n * The root Message type\n * This union enables us to easily send different message types without\n * redundant storage, and in the future we can easily add new message types.\n *\n * Arrow implementations do not need to implement all of the message types,\n * which may include experimental metadata types. For maximum compatibility,\n * it is best to send data using RecordBatch\n *\n * @enum {number}\n */\nexport namespace org.apache.arrow.flatbuf {\n    export enum MessageHeader {\n        NONE = 0,\n        Schema = 1,\n        DictionaryBatch = 2,\n        RecordBatch = 3,\n        Tensor = 4,\n        SparseTensor = 5\n    }\n}\n\n/**\n * ----------------------------------------------------------------------\n * Data structures for describing a table row batch (a collection of\n * equal-length Arrow arrays)\n * Metadata about a field at some level of a nested type tree (but not\n * its children).\n *\n * For example, a List<Int16> with values [[1, 2, 3], null, [4], [5, 6], null]\n * would have {length: 5, null_count: 2} for its List node, and {length: 6,\n * null_count: 0} for its Int16 node, as separate FieldNode structs\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class FieldNode {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns FieldNode\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): FieldNode {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * The number of value slots in the Arrow array at this level of a nested\n         * tree\n         *\n         * @returns flatbuffers.Long\n         */\n        length(): flatbuffers.Long {\n            return this.bb!.readInt64(this.bb_pos);\n        }\n\n        /**\n         * The number of observed nulls. Fields with null_count == 0 may choose not\n         * to write their physical validity bitmap out as a materialized buffer,\n         * instead setting the length of the bitmap buffer to 0.\n         *\n         * @returns flatbuffers.Long\n         */\n        nullCount(): flatbuffers.Long {\n            return this.bb!.readInt64(this.bb_pos + 8);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Long length\n         * @param flatbuffers.Long null_count\n         * @returns flatbuffers.Offset\n         */\n        static createFieldNode(builder: flatbuffers.Builder, length: flatbuffers.Long, null_count: flatbuffers.Long): flatbuffers.Offset {\n            builder.prep(8, 16);\n            builder.writeInt64(null_count);\n            builder.writeInt64(length);\n            return builder.offset();\n        }\n\n    }\n}\n/**\n * A data header describing the shared memory layout of a \"record\" or \"row\"\n * batch. Some systems call this a \"row batch\" internally and others a \"record\n * batch\".\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class RecordBatch {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns RecordBatch\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): RecordBatch {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param RecordBatch= obj\n         * @returns RecordBatch\n         */\n        static getRootAsRecordBatch(bb: flatbuffers.ByteBuffer, obj?: RecordBatch): RecordBatch {\n            return (obj || new RecordBatch).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * number of records / rows. The arrays in the batch should all have this\n         * length\n         *\n         * @returns flatbuffers.Long\n         */\n        length(): flatbuffers.Long {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt64(this.bb_pos + offset) : this.bb!.createLong(0, 0);\n        }\n\n        /**\n         * Nodes correspond to the pre-ordered flattened logical schema\n         *\n         * @param number index\n         * @param org.apache.arrow.flatbuf.FieldNode= obj\n         * @returns org.apache.arrow.flatbuf.FieldNode\n         */\n        nodes(index: number, obj?: org.apache.arrow.flatbuf.FieldNode): org.apache.arrow.flatbuf.FieldNode | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? (obj || new org.apache.arrow.flatbuf.FieldNode).__init(this.bb!.__vector(this.bb_pos + offset) + index * 16, this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        nodesLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * Buffers correspond to the pre-ordered flattened buffer tree\n         *\n         * The number of buffers appended to this list depends on the schema. For\n         * example, most primitive arrays will have 2 buffers, 1 for the validity\n         * bitmap and 1 for the values. For struct arrays, there will only be a\n         * single buffer for the validity (nulls) bitmap\n         *\n         * @param number index\n         * @param org.apache.arrow.flatbuf.Buffer= obj\n         * @returns org.apache.arrow.flatbuf.Buffer\n         */\n        buffers(index: number, obj?: NS7624605610262437867.org.apache.arrow.flatbuf.Buffer): NS7624605610262437867.org.apache.arrow.flatbuf.Buffer | null {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? (obj || new NS7624605610262437867.org.apache.arrow.flatbuf.Buffer).__init(this.bb!.__vector(this.bb_pos + offset) + index * 16, this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        buffersLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startRecordBatch(builder: flatbuffers.Builder) {\n            builder.startObject(3);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Long length\n         */\n        static addLength(builder: flatbuffers.Builder, length: flatbuffers.Long) {\n            builder.addFieldInt64(0, length, builder.createLong(0, 0));\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset nodesOffset\n         */\n        static addNodes(builder: flatbuffers.Builder, nodesOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, nodesOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startNodesVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(16, numElems, 8);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset buffersOffset\n         */\n        static addBuffers(builder: flatbuffers.Builder, buffersOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(2, buffersOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startBuffersVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(16, numElems, 8);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endRecordBatch(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createRecordBatch(builder: flatbuffers.Builder, length: flatbuffers.Long, nodesOffset: flatbuffers.Offset, buffersOffset: flatbuffers.Offset): flatbuffers.Offset {\n            RecordBatch.startRecordBatch(builder);\n            RecordBatch.addLength(builder, length);\n            RecordBatch.addNodes(builder, nodesOffset);\n            RecordBatch.addBuffers(builder, buffersOffset);\n            return RecordBatch.endRecordBatch(builder);\n        }\n    }\n}\n/**\n * For sending dictionary encoding information. Any Field can be\n * dictionary-encoded, but in this case none of its children may be\n * dictionary-encoded.\n * There is one vector / column per dictionary, but that vector / column\n * may be spread across multiple dictionary batches by using the isDelta\n * flag\n *\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class DictionaryBatch {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns DictionaryBatch\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): DictionaryBatch {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param DictionaryBatch= obj\n         * @returns DictionaryBatch\n         */\n        static getRootAsDictionaryBatch(bb: flatbuffers.ByteBuffer, obj?: DictionaryBatch): DictionaryBatch {\n            return (obj || new DictionaryBatch).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns flatbuffers.Long\n         */\n        id(): flatbuffers.Long {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? this.bb!.readInt64(this.bb_pos + offset) : this.bb!.createLong(0, 0);\n        }\n\n        /**\n         * @param org.apache.arrow.flatbuf.RecordBatch= obj\n         * @returns org.apache.arrow.flatbuf.RecordBatch|null\n         */\n        data(obj?: org.apache.arrow.flatbuf.RecordBatch): org.apache.arrow.flatbuf.RecordBatch | null {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? (obj || new org.apache.arrow.flatbuf.RecordBatch).__init(this.bb!.__indirect(this.bb_pos + offset), this.bb!) : null;\n        }\n\n        /**\n         * If isDelta is true the values in the dictionary are to be appended to a\n         * dictionary with the indicated id\n         *\n         * @returns boolean\n         */\n        isDelta(): boolean {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? !!this.bb!.readInt8(this.bb_pos + offset) : false;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startDictionaryBatch(builder: flatbuffers.Builder) {\n            builder.startObject(3);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Long id\n         */\n        static addId(builder: flatbuffers.Builder, id: flatbuffers.Long) {\n            builder.addFieldInt64(0, id, builder.createLong(0, 0));\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset dataOffset\n         */\n        static addData(builder: flatbuffers.Builder, dataOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(1, dataOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param boolean isDelta\n         */\n        static addIsDelta(builder: flatbuffers.Builder, isDelta: boolean) {\n            builder.addFieldInt8(2, +isDelta, +false);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endDictionaryBatch(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        static createDictionaryBatch(builder: flatbuffers.Builder, id: flatbuffers.Long, dataOffset: flatbuffers.Offset, isDelta: boolean): flatbuffers.Offset {\n            DictionaryBatch.startDictionaryBatch(builder);\n            DictionaryBatch.addId(builder, id);\n            DictionaryBatch.addData(builder, dataOffset);\n            DictionaryBatch.addIsDelta(builder, isDelta);\n            return DictionaryBatch.endDictionaryBatch(builder);\n        }\n    }\n}\n/**\n * @constructor\n */\nexport namespace org.apache.arrow.flatbuf {\n    export class Message {\n        bb: flatbuffers.ByteBuffer | null = null;\n\n        bb_pos: number = 0;\n        /**\n         * @param number i\n         * @param flatbuffers.ByteBuffer bb\n         * @returns Message\n         */\n        __init(i: number, bb: flatbuffers.ByteBuffer): Message {\n            this.bb_pos = i;\n            this.bb = bb;\n            return this;\n        }\n\n        /**\n         * @param flatbuffers.ByteBuffer bb\n         * @param Message= obj\n         * @returns Message\n         */\n        static getRootAsMessage(bb: flatbuffers.ByteBuffer, obj?: Message): Message {\n            return (obj || new Message).__init(bb.readInt32(bb.position()) + bb.position(), bb);\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.MetadataVersion\n         */\n        version(): NS7624605610262437867.org.apache.arrow.flatbuf.MetadataVersion {\n            let offset = this.bb!.__offset(this.bb_pos, 4);\n            return offset ? /**  */ (this.bb!.readInt16(this.bb_pos + offset)) : NS7624605610262437867.org.apache.arrow.flatbuf.MetadataVersion.V1;\n        }\n\n        /**\n         * @returns org.apache.arrow.flatbuf.MessageHeader\n         */\n        headerType(): org.apache.arrow.flatbuf.MessageHeader {\n            let offset = this.bb!.__offset(this.bb_pos, 6);\n            return offset ? /**  */ (this.bb!.readUint8(this.bb_pos + offset)) : org.apache.arrow.flatbuf.MessageHeader.NONE;\n        }\n\n        /**\n         * @param flatbuffers.Table obj\n         * @returns ?flatbuffers.Table\n         */\n        header<T extends flatbuffers.Table>(obj: T): T | null {\n            let offset = this.bb!.__offset(this.bb_pos, 8);\n            return offset ? this.bb!.__union(obj, this.bb_pos + offset) : null;\n        }\n\n        /**\n         * @returns flatbuffers.Long\n         */\n        bodyLength(): flatbuffers.Long {\n            let offset = this.bb!.__offset(this.bb_pos, 10);\n            return offset ? this.bb!.readInt64(this.bb_pos + offset) : this.bb!.createLong(0, 0);\n        }\n\n        /**\n         * @param number index\n         * @param org.apache.arrow.flatbuf.KeyValue= obj\n         * @returns org.apache.arrow.flatbuf.KeyValue\n         */\n        customMetadata(index: number, obj?: NS7624605610262437867.org.apache.arrow.flatbuf.KeyValue): NS7624605610262437867.org.apache.arrow.flatbuf.KeyValue | null {\n            let offset = this.bb!.__offset(this.bb_pos, 12);\n            return offset ? (obj || new NS7624605610262437867.org.apache.arrow.flatbuf.KeyValue).__init(this.bb!.__indirect(this.bb!.__vector(this.bb_pos + offset) + index * 4), this.bb!) : null;\n        }\n\n        /**\n         * @returns number\n         */\n        customMetadataLength(): number {\n            let offset = this.bb!.__offset(this.bb_pos, 12);\n            return offset ? this.bb!.__vector_len(this.bb_pos + offset) : 0;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         */\n        static startMessage(builder: flatbuffers.Builder) {\n            builder.startObject(5);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.MetadataVersion version\n         */\n        static addVersion(builder: flatbuffers.Builder, version: NS7624605610262437867.org.apache.arrow.flatbuf.MetadataVersion) {\n            builder.addFieldInt16(0, version, NS7624605610262437867.org.apache.arrow.flatbuf.MetadataVersion.V1);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param org.apache.arrow.flatbuf.MessageHeader headerType\n         */\n        static addHeaderType(builder: flatbuffers.Builder, headerType: org.apache.arrow.flatbuf.MessageHeader) {\n            builder.addFieldInt8(1, headerType, org.apache.arrow.flatbuf.MessageHeader.NONE);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset headerOffset\n         */\n        static addHeader(builder: flatbuffers.Builder, headerOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(2, headerOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Long bodyLength\n         */\n        static addBodyLength(builder: flatbuffers.Builder, bodyLength: flatbuffers.Long) {\n            builder.addFieldInt64(3, bodyLength, builder.createLong(0, 0));\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset customMetadataOffset\n         */\n        static addCustomMetadata(builder: flatbuffers.Builder, customMetadataOffset: flatbuffers.Offset) {\n            builder.addFieldOffset(4, customMetadataOffset, 0);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param Array.<flatbuffers.Offset> data\n         * @returns flatbuffers.Offset\n         */\n        static createCustomMetadataVector(builder: flatbuffers.Builder, data: flatbuffers.Offset[]): flatbuffers.Offset {\n            builder.startVector(4, data.length, 4);\n            for (let i = data.length - 1; i >= 0; i--) {\n                builder.addOffset(data[i]);\n            }\n            return builder.endVector();\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param number numElems\n         */\n        static startCustomMetadataVector(builder: flatbuffers.Builder, numElems: number) {\n            builder.startVector(4, numElems, 4);\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @returns flatbuffers.Offset\n         */\n        static endMessage(builder: flatbuffers.Builder): flatbuffers.Offset {\n            let offset = builder.endObject();\n            return offset;\n        }\n\n        /**\n         * @param flatbuffers.Builder builder\n         * @param flatbuffers.Offset offset\n         */\n        static finishMessageBuffer(builder: flatbuffers.Builder, offset: flatbuffers.Offset) {\n            builder.finish(offset);\n        }\n\n        static createMessage(builder: flatbuffers.Builder, version: NS7624605610262437867.org.apache.arrow.flatbuf.MetadataVersion, headerType: org.apache.arrow.flatbuf.MessageHeader, headerOffset: flatbuffers.Offset, bodyLength: flatbuffers.Long, customMetadataOffset: flatbuffers.Offset): flatbuffers.Offset {\n            Message.startMessage(builder);\n            Message.addVersion(builder, version);\n            Message.addHeaderType(builder, headerType);\n            Message.addHeader(builder, headerOffset);\n            Message.addBodyLength(builder, bodyLength);\n            Message.addCustomMetadata(builder, customMetadataOffset);\n            return Message.endMessage(builder);\n        }\n    }\n}\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\nimport * as Schema_ from './fb/Schema';\nimport * as Message_ from './fb/Message';\n\nexport import ArrowType = Schema_.org.apache.arrow.flatbuf.Type;\nexport import DateUnit = Schema_.org.apache.arrow.flatbuf.DateUnit;\nexport import TimeUnit = Schema_.org.apache.arrow.flatbuf.TimeUnit;\nexport import Precision = Schema_.org.apache.arrow.flatbuf.Precision;\nexport import UnionMode = Schema_.org.apache.arrow.flatbuf.UnionMode;\nexport import IntervalUnit = Schema_.org.apache.arrow.flatbuf.IntervalUnit;\nexport import MessageHeader = Message_.org.apache.arrow.flatbuf.MessageHeader;\nexport import MetadataVersion = Schema_.org.apache.arrow.flatbuf.MetadataVersion;\n\n/**\n * Main data type enumeration.\n *\n * Data types in this library are all *logical*. They can be expressed as\n * either a primitive physical type (bytes or bits of some fixed size), a\n * nested type consisting of other data types, or another data type (e.g. a\n * timestamp encoded as an int64).\n *\n * **Note**: Only enum values 0-17 (NONE through Map) are written to an Arrow\n * IPC payload.\n *\n * The rest of the values are specified here so TypeScript can narrow the type\n * signatures further beyond the base Arrow Types. The Arrow DataTypes include\n * metadata like `bitWidth` that impact the type signatures of the values we\n * accept and return.\n *\n * For example, the `Int8Vector` reads 1-byte numbers from an `Int8Array`, an\n * `Int32Vector` reads a 4-byte number from an `Int32Array`, and an `Int64Vector`\n * reads a pair of 4-byte lo, hi 32-bit integers as a zero-copy slice from the\n * underlying `Int32Array`.\n *\n * Library consumers benefit by knowing the narrowest type, since we can ensure\n * the types across all public methods are propagated, and never bail to `any`.\n * These values are _never_ used at runtime, and they will _never_ be written\n * to the flatbuffers metadata of serialized Arrow IPC payloads.\n */\nexport enum Type {\n    /** The default placeholder type */\n    NONE            =  0,\n    /** A NULL type having no physical storage */\n    Null            =  1,\n    /** Signed or unsigned 8, 16, 32, or 64-bit little-endian integer */\n    Int             =  2,\n    /** 2, 4, or 8-byte floating point value */\n    Float           =  3,\n    /** Variable-length bytes (no guarantee of UTF8-ness) */\n    Binary          =  4,\n    /** UTF8 variable-length string as List<Char> */\n    Utf8            =  5,\n    /** Boolean as 1 bit, LSB bit-packed ordering */\n    Bool            =  6,\n    /** Precision-and-scale-based decimal type. Storage type depends on the parameters. */\n    Decimal         =  7,\n    /** int32_t days or int64_t milliseconds since the UNIX epoch */\n    Date            =  8,\n    /** Time as signed 32 or 64-bit integer, representing either seconds, milliseconds, microseconds, or nanoseconds since midnight since midnight */\n    Time            =  9,\n    /** Exact timestamp encoded with int64 since UNIX epoch (Default unit millisecond) */\n    Timestamp       = 10,\n    /** YEAR_MONTH or DAY_TIME interval in SQL style */\n    Interval        = 11,\n    /** A list of some logical data type */\n    List            = 12,\n    /** Struct of logical types */\n    Struct          = 13,\n    /** Union of logical types */\n    Union           = 14,\n    /** Fixed-size binary. Each value occupies the same number of bytes */\n    FixedSizeBinary = 15,\n    /** Fixed-size list. Each value occupies the same number of bytes */\n    FixedSizeList   = 16,\n    /** Map of named logical types */\n    Map             = 17,\n\n    /** Dictionary aka Category type */\n    Dictionary            = -1,\n    Int8                  = -2,\n    Int16                 = -3,\n    Int32                 = -4,\n    Int64                 = -5,\n    Uint8                 = -6,\n    Uint16                = -7,\n    Uint32                = -8,\n    Uint64                = -9,\n    Float16               = -10,\n    Float32               = -11,\n    Float64               = -12,\n    DateDay               = -13,\n    DateMillisecond       = -14,\n    TimestampSecond       = -15,\n    TimestampMillisecond  = -16,\n    TimestampMicrosecond  = -17,\n    TimestampNanosecond   = -18,\n    TimeSecond            = -19,\n    TimeMillisecond       = -20,\n    TimeMicrosecond       = -21,\n    TimeNanosecond        = -22,\n    DenseUnion            = -23,\n    SparseUnion           = -24,\n    IntervalDayTime       = -25,\n    IntervalYearMonth     = -26,\n}\n\nexport enum BufferType {\n    /**\n     * used in List type, Dense Union and variable length primitive types (String, Binary)\n     */\n    OFFSET = 0,\n\n    /**\n     * actual data, either wixed width primitive types in slots or variable width delimited by an OFFSET vector\n     */\n    DATA = 1,\n\n    /**\n     * Bit vector indicating if each value is null\n     */\n    VALIDITY = 2,\n\n    /**\n     * Type vector used in Union type\n     */\n    TYPE = 3\n  }\n",
         "// Licensed to the Apache Software Foundation (ASF) under one\n// or more contributor license agreements.  See the NOTICE file\n// distributed with this work for additional information\n// regarding copyright ownership.  The ASF licenses this file\n// to you under the Apache License, Version 2.0 (the\n// \"License\"); you may not use this file except in compliance\n// with the License.  You may obtain a copy of the License at\n//\n//   http://www.apache.org/licenses/LICENSE-2.0\n//\n// Unless required by applicable law or agreed to in writing,\n// software distributed under the License is distributed on an\n// \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n// KIND, either express or implied.  See the License for the\n// specific language governing permissions and limitations\n// under the License.\n\n/** @ignore */\nexport function getBool(_data: any, _index: number, byte: number, bit: number) {\n    return (byte & 1 << bit) !== 0;\n}\n\n/** @ignore */\nexport function getBit(_data: any, _index: number, byte: number, bit: number): 0 | 1 {\n    return (byte & 1 << bit) >> bit as (0 | 1);\n}\n\n/** @ignore */\nexport function setBool(bytes: Uint8Array, index: number, value: any) {\n    return value ?\n        !!(bytes[index >> 3] |=  (1 << (index % 8))) || true :\n        !(bytes[index >> 3] &= ~(1 << (index % 8))) && false ;\n}\n\n/** @ignore */\nexport function truncateBitmap(offset: number, length: number, bitmap: Uint8Array) {\n    const alignedSize = (bitmap.byteLength + 7) & ~7;\n    if (offset > 0 || bitmap.byteLength < alignedSize) {\n        const bytes = new Uint8Array(alignedSize);\n        // If the offset is a multiple of 8 bits, it's safe to slice the bitmap\n        bytes.set(offset % 8 === 0 ? bitmap.subarray(offset >> 3) :\n            // Otherwise iterate each bit from the offset and return a new one\n            packBools(iterateBits(bitmap, offset, length, null, getBool)).subarray(0, alignedSize));\n        return bytes;\n    }\n    return bitmap;\n}\n\n/** @ignore */\nexport function packBools(values: Iterable<any>) {\n    let xs: number[] = [];\n    let i = 0, bit = 0, byte = 0;\n    for (const value of values) {\n        value && (byte |= 1 << bit);\n        if (++bit === 8) {\n            xs[i++] = byte;\n            byte = bit = 0;\n        }\n    }\n    if (i === 0 || bit > 0) { xs[i++] = byte; }\n    let b = new Uint8Array((xs.length + 7) & ~7);\n    b.set(xs);\n    return b;\n}\n\n/** @ignore */\nexport function* iterateBits<T>(bytes: Uint8Array, begin: number, length: number, context: any,\n                                get: (context: any, index: number, byte: number, bit: number) => T) {\n    let bit = begin % 8;\n    let byteIndex = begin >> 3;\n    let index = 0, remaining = length;\n    for (; remaining > 0; bit = 0) {\n        let byte = bytes[byteIndex++];\n        do {\n            yield get(context, index++, byte, bit);\n        } while (--remaining > 0 && ++bit < 8);\n    }\n}\n\n/**\n * Compute the population count (the number of bits set to 1) for a range of bits in a Uint8Array.\n * @param vector The Uint8Array of bits for which to compute the population count.\n * @param lhs The range's left-hand side (or start) bit\n * @param rhs The range's right-hand side (or end) bit\n */\n/** @ignore */\nexport function popcnt_bit_range(data: Uint8Array, lhs: number, rhs: number): number {\n    if (rhs - lhs <= 0) { return 0; }\n    // If the bit range is less than one byte, sum the 1 bits in the bit range\n    if (rhs - lhs < 8) {\n        let sum = 0;\n        for (const bit of iterateBits(data, lhs, rhs - lhs, data, getBit)) {\n            sum += bit;\n        }\n        return sum;\n    }\n    // Get the next lowest multiple of 8 from the right hand side\n    const rhsInside = rhs >> 3 << 3;\n    // Get the next highest multiple of 8 from the left hand side\n    const lhsInside = lhs + (lhs % 8 === 0 ? 0 : 8 - lhs % 8);\n    return (\n        // Get the popcnt of bits between the left hand side, and the next highest multiple of 8\n        popcnt_bit_range(data, lhs, lhsInside) +\n        // Get the popcnt of bits between the right hand side, and the next lowest multiple of 8\n        popcnt_bit_range(data, rhsInside, rhs) +\n        // Get the popcnt of all bits between the left and right hand sides' multiples of 8\n        popcnt_array(data, lhsInside >> 3, (rhsInside - lhsInside) >> 3)\n    );\n}\n\n/** @ignore */\nexport function popcnt_array(arr: ArrayBufferView, byteOffset?: number, byteLength?: number) {\n    let cnt = 0, pos = byteOffset! | 0;\n    const view = new DataView(arr.buffer, arr.byteOffset, arr.byteLength);\n    const len =  byteLength === void 0 ? arr.byteLength : pos + byteLength;\n    while (len - pos >= 4) {\n        cnt += popcnt_uint32(view.getUint32(pos));\n        pos += 4;\n    }\n    while (len - pos >= 2) {\n        cnt += popcnt_uint32(view.getUint16(pos));\n        pos += 2;\n    }\n    while (len - pos >= 1) {\n        cnt += popcnt_uint32(view.getUint8(pos));\n        pos += 1;\n    }\n    return cnt;\n}\n\n/** @ignore */\nexport function popcnt_uint32(uint32: number): number {\n    let i = uint32 | 0;\n    i = i - ((i >>> 1) & 0x55555555);\n    i = (i & 0x33333333) + ((i >>> 2) & 0x33333333);\n    return (((i + (i >>> 4)) & 0x0F0F0F0F) * 0x01010101) >>> 24;\n}\n",
```

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/main.d75feb69.chunk.js` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/main.78d08be9.chunk.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,105 +1,132 @@
 (this.webpackJsonpstreamlit_lang_tts = this.webpackJsonpstreamlit_lang_tts || []).push([
     [0], {
-        24: function(e, t, s) {
+        26: function(e, t, n) {
             "use strict";
-            s.r(t);
-            var n = s(6),
-                r = s.n(n),
-                i = s(15),
-                c = s.n(i),
-                o = s(0),
-                a = s(1),
-                l = s(2),
-                p = s(3),
-                d = s(13),
-                h = s(5),
-                u = function(e) {
-                    Object(l.a)(s, e);
-                    var t = Object(p.a)(s);
+            n.r(t);
+            var s = n(8),
+                i = n.n(s),
+                r = n(17),
+                c = n.n(r),
+                o = n(5),
+                a = n(0),
+                l = n(1),
+                d = n(2),
+                p = n(3),
+                b = n(15),
+                h = n(7),
+                j = function(e) {
+                    Object(d.a)(n, e);
+                    var t = Object(p.a)(n);
 
-                    function s() {
+                    function n() {
                         var e;
-                        Object(a.a)(this, s);
-                        for (var n = arguments.length, r = new Array(n), i = 0; i < n; i++) r[i] = arguments[i];
-                        return (e = t.call.apply(t, [this].concat(r))).state = {
+                        Object(l.a)(this, n);
+                        for (var s = arguments.length, i = new Array(s), r = 0; r < s; r++) i[r] = arguments[r];
+                        return (e = t.call.apply(t, [this].concat(i))).state = {
                             textToSpeak: e.props.args.name,
                             isFocused: !1
                         }, e.render = function() {
                             var t = e.props.args.name,
-                                s = e.props.args.label || "AI:",
-                                n = e.props.args.translation,
-                                r = e.props.theme,
-                                i = {};
-                            if (r) {
-                                var c = "0px solid ".concat(e.state.isFocused ? r.primaryColor : "gray");
-                                i.border = c, i.outline = c, i.border = "1px solid gray", i.fontSize = "20px", i.padding = "3px", i.background = "lightgray", i.borderRadius = "5px", i.width = "70px", i.height = "70px", i.marginLeft = "10px"
-                            }
-                            return Object(h.jsx)("div", {
+                                n = e.props.args.label || "AI:",
+                                s = e.props.args.translation,
+                                i = e.props.theme,
+                                r = {};
+                            return i && (r = Object(o.a)(Object(o.a)({}, r), {}, {
+                                display: "inline-flex",
+                                WebkitBoxAlign: "center",
+                                alignItems: "center",
+                                WebkitBoxPack: "center",
+                                justifyContent: "center",
+                                fontWeight: 400,
+                                fontSize: "15px",
+                                borderRadius: "0.25rem",
+                                borderWidth: "1px",
+                                borderStyle: "solid",
+                                borderColor: e.state.isFocused ? i.primaryColor : "rgba(49, 51, 63, 0.2)",
+                                marginTop: 0,
+                                marginLeft: "5px",
+                                lineHeight: 1.6,
+                                color: "inherit",
+                                width: "auto",
+                                height: "40px",
+                                WebkitUserSelect: "none",
+                                backgroundColor: "rgb(255, 255, 255)"
+                            })), Object(h.jsx)("div", {
                                 children: Object(h.jsxs)("div", {
                                     style: {
                                         display: "flex"
                                     },
                                     children: [Object(h.jsx)("div", {
                                         style: {
-                                            width: "70px"
+                                            width: "35px"
                                         },
                                         children: Object(h.jsx)("p", {
                                             children: Object(h.jsx)("span", {
                                                 style: {
                                                     fontWeight: "bold"
                                                 },
-                                                children: s
+                                                children: n
                                             })
                                         })
                                     }), Object(h.jsxs)("div", {
                                         style: {
                                             flex: "1"
                                         },
-                                        children: [Object(h.jsxs)("p", {
-                                            children: [t, " \xa0"]
+                                        children: [Object(h.jsx)("p", {
+                                            children: t
                                         }), Object(h.jsx)("p", {
                                             style: {
                                                 fontStyle: "italic"
                                             },
-                                            children: n
+                                            children: s
                                         })]
-                                    }), Object(h.jsx)("button", {
-                                        style: i,
-                                        onClick: e.onClicked,
-                                        disabled: e.props.disabled,
-                                        onFocus: e._onFocus,
-                                        onBlur: e._onBlur,
-                                        children: "\ud83d\udde3"
+                                    }), Object(h.jsx)("div", {
+                                        style: {
+                                            width: "45px"
+                                        },
+                                        children: Object(h.jsx)("button", {
+                                            style: r,
+                                            onClick: e.onClicked,
+                                            disabled: e.props.disabled,
+                                            onFocus: e._onFocus,
+                                            onBlur: e._onBlur,
+                                            children: Object(h.jsx)("p", {
+                                                style: {
+                                                    margin: 0
+                                                },
+                                                children: "\ud83d\udde3"
+                                            })
+                                        })
                                     })]
                                 })
                             })
                         }, e.onClicked = function() {
                             e.state.textToSpeak;
                             var t = new window.SpeechSynthesisUtterance,
-                                s = window.speechSynthesis.getVoices().filter((function(e) {
+                                n = window.speechSynthesis.getVoices().filter((function(e) {
                                     return "com.apple.voice.compact.es-ES.Monica" === e.voiceURI
                                 }))[0];
-                            t.text = e.props.args.name, t.voice = s, t.rate = .8, window.speechSynthesis.speak(t)
+                            t.text = e.props.args.name, t.voice = n, t.rate = .8, window.speechSynthesis.speak(t)
                         }, e._onFocus = function() {
                             e.setState({
                                 isFocused: !0
                             })
                         }, e._onBlur = function() {
                             e.setState({
                                 isFocused: !1
                             })
                         }, e
                     }
-                    return Object(o.a)(s)
-                }(d.a),
-                b = Object(d.b)(u);
-            c.a.render(Object(h.jsx)(r.a.StrictMode, {
-                children: Object(h.jsx)(b, {})
+                    return Object(a.a)(n)
+                }(b.a),
+                u = Object(b.b)(j);
+            c.a.render(Object(h.jsx)(i.a.StrictMode, {
+                children: Object(h.jsx)(u, {})
             }), document.getElementById("root"))
         }
     },
     [
-        [24, 1, 2]
+        [26, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.d75feb69.chunk.js.map
+//# sourceMappingURL=main.78d08be9.chunk.js.map
```

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/main.d75feb69.chunk.js.map` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/main.78d08be9.chunk.js.map`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7880952380952381%*

 * *Differences: {"'file'": "'static/js/main.78d08be9.chunk.js'",*

 * * "'mappings'": "'uNAgBMA,EAAW,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GA6Gd,OA7GcP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACRM,MAAQ,CAAEC,YAAaZ,EAAKa,MAAMR,KAAW,KAAGS,WAAW,GAAOd,EAElEe,OAAS,WAGd,IAAMC,EAAOhB,EAAKa,MAAMR,KAAW,KAC7BY,EAAQjB,EAAKa,MAAMR,KAAY,OAAK,MACpCa,EAAclB,EAAKa,MAAMR,KAAkB,YAKzCc,EAAUnB,EAAKa,MA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.d75feb69.chunk.js",
-    "mappings": "gNAgBMA,EAAW,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GA8Fd,OA9FcP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACRM,MAAQ,CAAEC,YAAaZ,EAAKa,MAAMR,KAAW,KAAGS,WAAW,GAAOd,EAElEe,OAAS,WAGd,IAAMC,EAAOhB,EAAKa,MAAMR,KAAW,KAC7BY,EAAQjB,EAAKa,MAAMR,KAAY,OAAK,MACpCa,EAAclB,EAAKa,MAAMR,KAAkB,YAKzCc,EAAUnB,EAAKa,MAAfM,MACFC,EAA6B,CAAC,EAIpC,GAAID,EAAO,CAGT,IAAME,EAAa,aAAAX,OACjBV,EAAKW,MAAMG,UAAYK,EAAMG,aAAe,QAE9CF,EAAMG,OAASF,EACfD,EAAMI,QAAUH,EAChBD,EAAMG,OAAS,iBACfH,EAAMK,SAAW,OACjBL,EAAMM,QAAU,MAChBN,EAAMO,WAAa,YACnBP,EAAMQ,aAAe,MACrBR,EAAMS,MAAQ,OACdT,EAAMU,OAAS,OACfV,EAAMW,WAAa,MACrB,CAMA,OACEC,cAAA,OAAAC,SACEC,eAAA,OAAKd,MAAO,CAACe,QAAS,QAAQF,SAAA,CAC5BD,cAAA,OAAKZ,MAAO,CAACS,MAAO,QAAQI,SAC1BD,cAAA,KAAAC,SACED,cAAA,QAAMZ,MAAO,CAACgB,WAAY,QAAQH,SAAEhB,QAGxCiB,eAAA,OAAKd,MAAO,CAACiB,KAAM,KAAKJ,SAAA,CACtBC,eAAA,KAAAD,SAAA,CAAIjB,EAAK,WACTgB,cAAA,KAAGZ,MAAO,CAACkB,UAAW,UAAUL,SAAEf,OAEpCc,cAAA,UACEZ,MAAOA,EACPmB,QAASvC,EAAKwC,UACdC,SAAUzC,EAAKa,MAAM4B,SACrBC,QAAS1C,EAAK2C,SACdC,OAAQ5C,EAAK6C,QAAQZ,SACtB,qBAMT,EAEAjC,EACQwC,UAAY,WAGMxC,EAAKW,MAArBC,YAAR,IACMkC,EAAM,IAAIC,OAAOC,yBACjBC,EAASF,OAAOG,gBAAgBC,YAAYC,QAChD,SAACC,GAAK,MAAwB,yCAAnBA,EAAMC,QAAmD,IAAE,GACxER,EAAIS,KAAOvD,EAAKa,MAAMR,KAAW,KACjCyC,EAAIO,MAAQJ,EAEZH,EAAIU,KAAO,GACXT,OAAOG,gBAAgBO,MAAMX,EAM/B,EAEA9C,EACQ2C,SAAW,WACjB3C,EAAK0D,SAAS,CAAE5C,WAAW,GAC7B,EAEAd,EACQ6C,QAAU,WAChB7C,EAAK0D,SAAS,CAAE5C,WAAW,GAC7B,EAACd,CAAA,QAAA2D,YAAAhE,EAAA,CA9Fc,CAASiE,KAsGXC,cAAwBlE,GClHvCmE,IAAS/C,OACPiB,cAAC+B,IAAMC,WAAU,CAAA/B,SACfD,cAACrC,EAAW,MAEdsE,SAASC,eAAe,Q",
+    "file": "static/js/main.78d08be9.chunk.js",
+    "mappings": "uNAgBMA,EAAW,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GA6Gd,OA7GcP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACRM,MAAQ,CAAEC,YAAaZ,EAAKa,MAAMR,KAAW,KAAGS,WAAW,GAAOd,EAElEe,OAAS,WAGd,IAAMC,EAAOhB,EAAKa,MAAMR,KAAW,KAC7BY,EAAQjB,EAAKa,MAAMR,KAAY,OAAK,MACpCa,EAAclB,EAAKa,MAAMR,KAAkB,YAKzCc,EAAUnB,EAAKa,MAAfM,MACJC,EAA6B,CAAC,EAsClC,OAlCID,IAIFC,EAAKC,wBAAA,GACAD,GAAK,IACRE,QAAS,cACTC,eAAgB,SAChBC,WAAY,SACZC,cAAe,SACfC,eAAgB,SAChBC,WAAY,IACZC,SAAU,OACVC,aAAc,UACdC,YAAa,MACbC,YAAa,QACbC,YAAahC,EAAKW,MAAMG,UAAYK,EAAMc,aAAe,wBACzDC,UAAW,EACXC,WAAY,MACZC,WAAY,IACZC,MAAO,UACPC,MAAO,OACPC,OAAQ,OACRC,iBAAkB,OAClBC,gBAAiB,wBAWnBC,cAAA,OAAAC,SACEC,eAAA,OAAKxB,MAAO,CAACE,QAAS,QAAQqB,SAAA,CAC5BD,cAAA,OAAKtB,MAAO,CAACkB,MAAO,QAAQK,SAC1BD,cAAA,KAAAC,SACED,cAAA,QAAMtB,MAAO,CAACO,WAAY,QAAQgB,SAAE1B,QAGxC2B,eAAA,OAAKxB,MAAO,CAACyB,KAAM,KAAKF,SAAA,CACtBD,cAAA,KAAAC,SAAI3B,IACJ0B,cAAA,KAAGtB,MAAO,CAAC0B,UAAW,UAAUH,SAAEzB,OAEpCwB,cAAA,OAAKtB,MAAO,CAACkB,MAAO,QAAQK,SAC1BD,cAAA,UACItB,MAAOA,EACP2B,QAAS/C,EAAKgD,UACdC,SAAUjD,EAAKa,MAAMoC,SACrBC,QAASlD,EAAKmD,SACdC,OAAQpD,EAAKqD,QAAQV,SAEvBD,cAAA,KAAGtB,MAAO,CAAEkC,OAAQ,GAAGX,SAAC,yBAOpC,EAEA3C,EACQgD,UAAY,WAGMhD,EAAKW,MAArBC,YAAR,IACM2C,EAAM,IAAIC,OAAOC,yBACjBC,EAASF,OAAOG,gBAAgBC,YAAYC,QAChD,SAACC,GAAK,MAAwB,yCAAnBA,EAAMC,QAAmD,IAAE,GACxER,EAAIS,KAAOhE,EAAKa,MAAMR,KAAW,KACjCkD,EAAIO,MAAQJ,EAEZH,EAAIU,KAAO,GACXT,OAAOG,gBAAgBO,MAAMX,EAM/B,EAEAvD,EACQmD,SAAW,WACjBnD,EAAKmE,SAAS,CAAErD,WAAW,GAC7B,EAEAd,EACQqD,QAAU,WAChBrD,EAAKmE,SAAS,CAAErD,WAAW,GAC7B,EAACd,CAAA,QAAAoE,YAAAzE,EAAA,CA7Gc,CAAS0E,KAqHXC,cAAwB3E,GCjIvC4E,IAASxD,OACP2B,cAAC8B,IAAMC,WAAU,CAAA9B,SACfD,cAAC/C,EAAW,MAEd+E,SAASC,eAAe,Q",
     "names": [
         "MyComponent",
         "_StreamlitComponentBa",
         "_inherits",
         "_super",
         "_createSuper",
         "_this",
@@ -24,39 +24,48 @@
         "isFocused",
         "render",
         "name",
         "label",
         "translation",
         "theme",
         "style",
-        "borderStyling",
-        "primaryColor",
-        "border",
-        "outline",
+        "_objectSpread",
+        "display",
+        "WebkitBoxAlign",
+        "alignItems",
+        "WebkitBoxPack",
+        "justifyContent",
+        "fontWeight",
         "fontSize",
-        "padding",
-        "background",
         "borderRadius",
+        "borderWidth",
+        "borderStyle",
+        "borderColor",
+        "primaryColor",
+        "marginTop",
+        "marginLeft",
+        "lineHeight",
+        "color",
         "width",
         "height",
-        "marginLeft",
+        "WebkitUserSelect",
+        "backgroundColor",
         "_jsx",
         "children",
         "_jsxs",
-        "display",
-        "fontWeight",
         "flex",
         "fontStyle",
         "onClick",
         "onClicked",
         "disabled",
         "onFocus",
         "_onFocus",
         "onBlur",
         "_onBlur",
+        "margin",
         "msg",
         "window",
         "SpeechSynthesisUtterance",
         "monica",
         "speechSynthesis",
         "getVoices",
         "filter",
@@ -77,12 +86,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "MyComponent.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\n\ninterface State {\n  textToSpeak: string;\n  isFocused: boolean;\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nclass MyComponent extends StreamlitComponentBase<State> {\n  public state = { textToSpeak: this.props.args[\"name\"], isFocused: false }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`. Here, we access the \"name\" arg.\n    const name = this.props.args[\"name\"]\n    const label = this.props.args[\"label\"] || 'AI:'\n    const translation = this.props.args[\"translation\"]\n\n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    const style: React.CSSProperties = {}\n\n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (theme) {\n      // Use the theme object to style our button border. Alternatively, the\n      // theme style is defined in CSS vars.\n      const borderStyling = `0px solid ${\n        this.state.isFocused ? theme.primaryColor : \"gray\"\n      }`\n      style.border = borderStyling\n      style.outline = borderStyling\n      style.border = '1px solid gray'\n      style.fontSize = '20px';\n      style.padding = '3px';\n      style.background = 'lightgray';\n      style.borderRadius = '5px';\n      style.width = '70px';\n      style.height = '70px';\n      style.marginLeft = '10px';\n    }\n\n    // Show a button and some text.\n    // When the button is clicked, we'll increment our \"numClicks\" state\n    // variable, and send its new value back to Streamlit, where it'll\n    // be available to the Python program.\n    return (\n      <div>\n        <div style={{display: 'flex'}}>\n          <div style={{width: '70px'}}>\n            <p>\n              <span style={{fontWeight: 'bold'}}>{label}</span>\n            </p>\n          </div>\n          <div style={{flex: '1'}}>\n            <p>{name} &nbsp;</p>\n            <p style={{fontStyle: 'italic'}}>{translation}</p>\n          </div>\n          <button\n            style={style}\n            onClick={this.onClicked}\n            disabled={this.props.disabled}\n            onFocus={this._onFocus}\n            onBlur={this._onBlur}\n          >\n            \ud83d\udde3\n          </button>\n        </div>\n      </div>\n    )\n  }\n\n  /** Click handler for our \"Click Me!\" button. */\n  private onClicked = (): void => {\n    // Increment state.numClicks, and pass the new value back to\n    // Streamlit via `Streamlit.setComponentValue`.\n    const { textToSpeak } = this.state;\n    const msg = new window.SpeechSynthesisUtterance();\n    const monica = window.speechSynthesis.getVoices().filter(\n      (voice) => voice.voiceURI === 'com.apple.voice.compact.es-ES.Monica')[0];\n    msg.text = this.props.args[\"name\"];\n    msg.voice = monica;\n    // Slower speech rate is easier for learning\n    msg.rate = 0.8;\n    window.speechSynthesis.speak(msg);\n\n//     this.setState(\n//       prevState => ({ textToSpeak: prevState.textToSpeak }),\n//       () => Streamlit.setComponentValue(textToSpeak)\n//     )\n  }\n\n  /** Focus handler for our \"Click Me!\" button. */\n  private _onFocus = (): void => {\n    this.setState({ isFocused: true })\n  }\n\n  /** Blur handler for our \"Click Me!\" button. */\n  private _onBlur = (): void => {\n    this.setState({ isFocused: false })\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(MyComponent)\n",
+        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\n\ninterface State {\n  textToSpeak: string;\n  isFocused: boolean;\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nclass MyComponent extends StreamlitComponentBase<State> {\n  public state = { textToSpeak: this.props.args[\"name\"], isFocused: false }\n\n  public render = (): ReactNode => {\n    // Arguments that are passed to the plugin in Python are accessible\n    // via `this.props.args`. Here, we access the \"name\" arg.\n    const name = this.props.args[\"name\"]\n    const label = this.props.args[\"label\"] || 'AI:'\n    const translation = this.props.args[\"translation\"]\n\n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    let style: React.CSSProperties = {}\n\n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (theme) {\n      // Use the theme object to style our button border. Alternatively, the\n      // theme style is defined in CSS vars.\n\n      style = {\n        ...style,\n        display: \"inline-flex\",\n        WebkitBoxAlign: \"center\",\n        alignItems: \"center\",\n        WebkitBoxPack: \"center\",\n        justifyContent: \"center\",\n        fontWeight: 400,\n        fontSize: \"15px\",\n        borderRadius: \"0.25rem\",\n        borderWidth: \"1px\",\n        borderStyle: \"solid\",\n        borderColor: this.state.isFocused ? theme.primaryColor : \"rgba(49, 51, 63, 0.2)\",\n        marginTop: 0,\n        marginLeft: \"5px\",\n        lineHeight: 1.6,\n        color: \"inherit\",\n        width: \"auto\",\n        height: \"40px\",\n        WebkitUserSelect: \"none\",\n        backgroundColor: \"rgb(255, 255, 255)\",\n      }\n\n\n    }\n\n    // Show a button and some text.\n    // When the button is clicked, we'll increment our \"numClicks\" state\n    // variable, and send its new value back to Streamlit, where it'll\n    // be available to the Python program.\n    return (\n      <div>\n        <div style={{display: 'flex'}}>\n          <div style={{width: '35px'}}>\n            <p>\n              <span style={{fontWeight: 'bold'}}>{label}</span>\n            </p>\n          </div>\n          <div style={{flex: '1'}}>\n            <p>{name}</p>\n            <p style={{fontStyle: 'italic'}}>{translation}</p>\n          </div>\n          <div style={{width: '45px'}}>\n            <button\n                style={style}\n                onClick={this.onClicked}\n                disabled={this.props.disabled}\n                onFocus={this._onFocus}\n                onBlur={this._onBlur}\n              >\n              <p style={{ margin: 0}}>\ud83d\udde3</p>\n            </button>\n          </div>\n\n        </div>\n      </div>\n    )\n  }\n\n  /** Click handler for our \"Click Me!\" button. */\n  private onClicked = (): void => {\n    // Increment state.numClicks, and pass the new value back to\n    // Streamlit via `Streamlit.setComponentValue`.\n    const { textToSpeak } = this.state;\n    const msg = new window.SpeechSynthesisUtterance();\n    const monica = window.speechSynthesis.getVoices().filter(\n      (voice) => voice.voiceURI === 'com.apple.voice.compact.es-ES.Monica')[0];\n    msg.text = this.props.args[\"name\"];\n    msg.voice = monica;\n    // Slower speech rate is easier for learning\n    msg.rate = 0.8;\n    window.speechSynthesis.speak(msg);\n\n//     this.setState(\n//       prevState => ({ textToSpeak: prevState.textToSpeak }),\n//       () => Streamlit.setComponentValue(textToSpeak)\n//     )\n  }\n\n  /** Focus handler for our \"Click Me!\" button. */\n  private _onFocus = (): void => {\n    this.setState({ isFocused: true })\n  }\n\n  /** Blur handler for our \"Click Me!\" button. */\n  private _onBlur = (): void => {\n    this.setState({ isFocused: false })\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(MyComponent)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport MyComponent from \"./MyComponent\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <MyComponent />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_lang_tts-0.0.3/streamlit_lang_tts.egg-info/SOURCES.txt` & `streamlit_lang_tts-0.0.4/streamlit_lang_tts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 streamlit_lang_tts.egg-info/SOURCES.txt
 streamlit_lang_tts.egg-info/dependency_links.txt
 streamlit_lang_tts.egg-info/requires.txt
 streamlit_lang_tts.egg-info/top_level.txt
 streamlit_lang_tts/frontend/build/asset-manifest.json
 streamlit_lang_tts/frontend/build/bootstrap.min.css
 streamlit_lang_tts/frontend/build/index.html
-streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js
-streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js.LICENSE.txt
-streamlit_lang_tts/frontend/build/static/js/2.cfa3d2aa.chunk.js.map
-streamlit_lang_tts/frontend/build/static/js/main.d75feb69.chunk.js
-streamlit_lang_tts/frontend/build/static/js/main.d75feb69.chunk.js.map
+streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js
+streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js.LICENSE.txt
+streamlit_lang_tts/frontend/build/static/js/2.38865783.chunk.js.map
+streamlit_lang_tts/frontend/build/static/js/main.78d08be9.chunk.js
+streamlit_lang_tts/frontend/build/static/js/main.78d08be9.chunk.js.map
 streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js
 streamlit_lang_tts/frontend/build/static/js/runtime-main.0a6aa703.js.map
```
