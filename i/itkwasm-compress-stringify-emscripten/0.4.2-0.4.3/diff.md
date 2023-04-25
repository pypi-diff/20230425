# Comparing `tmp/itkwasm_compress_stringify_emscripten-0.4.2.tar.gz` & `tmp/itkwasm_compress_stringify_emscripten-0.4.3.tar.gz`

## Comparing `itkwasm_compress_stringify_emscripten-0.4.2.tar` & `itkwasm_compress_stringify_emscripten-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/_version.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/compress_stringify_async.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/pyodide.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/test/test_compress_stringify.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/.gitignore
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/README.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/_version.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/compress_stringify_async.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/pyodide.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/test/test_compress_stringify.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/.gitignore
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/README.md
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.3/PKG-INFO
```

### Comparing `itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/compress_stringify_async.py` & `itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/compress_stringify_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,24 +46,19 @@
     js_module = await js_package.js_module
     web_worker = js_resources.web_worker
 
     outputs = await js_module.compressStringify(web_worker, to_js(input),  stringify=to_js(stringify), compressionLevel=to_js(compression_level), dataUrlPrefix=to_js(data_url_prefix), )
 
     output_web_worker = None
     output_list = []
-    print(dir(outputs))
     outputs_object_map = outputs.as_object_map()
     for output_name in outputs.object_keys():
         if output_name == 'webWorker':
             output_web_worker = outputs_object_map[output_name]
         else:
-            print(output_name)
-            print(type(outputs_object_map[output_name]))
-            print(outputs_object_map[output_name].constructor.name)
-            print(outputs_object_map[output_name])
             output_list.append(to_py(outputs_object_map[output_name]))
 
     js_resources.web_worker = output_web_worker
 
     if len(output_list) == 1:
         return output_list[0]
     return tuple(output_list)
```

### Comparing `itkwasm_compress_stringify_emscripten-0.4.2/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py` & `itkwasm_compress_stringify_emscripten-0.4.3/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,24 +38,19 @@
     js_module = await js_package.js_module
     web_worker = js_resources.web_worker
 
     outputs = await js_module.parseStringDecompress(web_worker, to_js(input),  parseString=to_js(parse_string), )
 
     output_web_worker = None
     output_list = []
-    print(dir(outputs))
     outputs_object_map = outputs.as_object_map()
     for output_name in outputs.object_keys():
         if output_name == 'webWorker':
             output_web_worker = outputs_object_map[output_name]
         else:
-            print(output_name)
-            print(type(outputs_object_map[output_name]))
-            print(outputs_object_map[output_name].constructor.name)
-            print(outputs_object_map[output_name])
             output_list.append(to_py(outputs_object_map[output_name]))
 
     js_resources.web_worker = output_web_worker
 
     if len(output_list) == 1:
         return output_list[0]
     return tuple(output_list)
```

### Comparing `itkwasm_compress_stringify_emscripten-0.4.2/.gitignore` & `itkwasm_compress_stringify_emscripten-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.2/README.md` & `itkwasm_compress_stringify_emscripten-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.2/pyproject.toml` & `itkwasm_compress_stringify_emscripten-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.2/PKG-INFO` & `itkwasm_compress_stringify_emscripten-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-compress-stringify-emscripten
-Version: 0.4.2
+Version: 0.4.3
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

