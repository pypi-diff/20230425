# Comparing `tmp/jupylite_duckdb-0.0.18a2-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.18a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7346 bytes, number of entries: 10
+Zip file size: 8887 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-22 23:21 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-24 11:35 jupylite_duckdb/_version.py
 -rw-rw-rw-  2.0 fat     9216 b- defN 23-Apr-22 17:53 jupylite_duckdb/jdw.py
--rw-rw-rw-  2.0 fat     2149 b- defN 23-Apr-22 23:17 jupylite_duckdb/jdw_magic.py
+-rw-rw-rw-  2.0 fat     4973 b- defN 23-Apr-23 18:54 jupylite_duckdb/jdw_magic.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2559 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      850 b- defN 23-Apr-22 23:21 jupylite_duckdb-0.0.18a2.dist-info/RECORD
-10 files, 17507 bytes uncompressed, 5880 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-24 11:39 jupylite_duckdb-0.0.18a3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4787 b- defN 23-Apr-24 11:39 jupylite_duckdb-0.0.18a3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 11:39 jupylite_duckdb-0.0.18a3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 11:39 jupylite_duckdb-0.0.18a3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      850 b- defN 23-Apr-24 11:39 jupylite_duckdb-0.0.18a3.dist-info/RECORD
+10 files, 22559 bytes uncompressed, 7421 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jupylite_duckdb/jdw_magic.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a2.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.18a3.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a2.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.18a3.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a2.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.18a3.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a2.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.18a3.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.18a2.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.18a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.18a2"
+__version__="0.0.18a3"
```

## jupylite_duckdb/jdw_magic.py

```diff
@@ -1,7 +1,30 @@
+# Still a work in progress:
+# The basic problem is properly handling the Pyodide Future. 
+# Couldn't handle it in the usual ways (event loop), and simplest solution
+# is to "await" the operation. 
+# But, since Cell/Line magics don't support async, needed to come up with a way to await them.
+# 
+# The monkey patch approach patches the iPython line and cell transformers to rewrite the magics directly
+# to the syntax we want: "await <function>(params)" 
+# instead of its usual behavior which is to rewrite a cell magic to: get_ipython().run_<cell|line>_magic(line, cell)
+#
+# So, the cell/line magic here is only used for registration purposes... but is never called.
+# 
+# The last complexity is that there are three paths for rewriting:
+# Cell Magics: Cells starting with %%magic
+# Line Magics: lines starting with %magic
+# Line Magics with Assignment: lines starting with xyz = %magic
+#
+# Only the first two cases are dealt with here. The assignment case is a bit weird. For now, %dql -o <xyz> instead of xyz = %dql.
+# 
+# ref: https://github.com/ipython/ipython/blob/main/IPython/core/interactiveshell.py
+# https://github.com/ipython/ipython/blob/main/IPython/core/inputtransformer2.py
+# 
+
 from IPython.core.magic import register_line_magic, register_cell_magic
 from IPython.core import magic_arguments
 from IPython.display import display
 import ipywidgets as widgets
 import asyncio
 import jupylite_duckdb as jd
 import functools
@@ -18,48 +41,103 @@
                     display(f"Output type: {type(result)}")
                 display(result)
                 if outputvar is not None: 
                     get_ipython().user_ns[outputvar] = result  # type: ignore
         except Exception as e:
             print(e)
 
-#@register_line_magic
+@register_line_magic
 @register_cell_magic
 @magic_arguments.magic_arguments()
-@magic_arguments.argument('-output', nargs=1, help="Output.", type=str)
+@magic_arguments.argument('-o', '--output', nargs=1, help="Output.", type=str)
 #@magic_arguments.argument('query', nargs="+", help="Query.", type=str)
 def dql(line = "", cell = ""):
-    outputvar = None
-    if line:
-        args = magic_arguments.parse_argstring(dql, line)
-        outputvar = args.output[0]
-        #sql = ' '.join(args.query)
-
-    sql = cell
+    raise ValueError("Invalid syntax")
+    pass
 
-    s_out = widgets.Output(layout={'border': '1px solid black'})
-    display(s_out)
-
-    with s_out:
-            r = asyncio.get_event_loop().run_until_complete(jd.query(sql=sql, return_future=False))
-            r.then(functools.partial(display_result, outputvar = outputvar, output=s_out))
 
+def transform_dql_line(line: str) -> str:
+    outputobj = None
+    try:
+        if line.startswith("-o"):
+            a = line.split(" ")
+            if len(a) < 3:
+                print("Warning: Missing option after -o or query")
+            else:
+                outputobj = a[1]
+                rest = " ".join(a[2:])
+        else:
+            rest = line
+
+        if outputobj is not None: 
+            pre = f"{outputobj} = "
+        else:
+            pre = ""
+
+        rest = rest.replace("'", "\'")
+        result =  f"{pre}await jd.query(sql='{rest}')\n"
+        return result
+    except Exception as e:
+        print(f"Error {e}")
+
+def transform_dql_cell(orig_cell: str) -> str:
+    lines = orig_cell.split("\n")
+    first_line=lines[0]
+    first_line=first_line.replace("%%dql", "").replace("-o", "").strip()
+    rest = "\\n".join(lines[1:])
+    rest=rest.replace("'", "\\'")
+    if len(first_line) >0:
+        first_line = f"{first_line} = "
+    result= f"{first_line}await jd.query(sql='{rest}')"
+    return result
 
-def patch_magic():
-    # Monkey patching a transformation to stick an "await" ahead of this cell magic
-    
+def patch_transformer():
     
     shell = get_ipython()
+    transformermanager = shell.input_transformer_manager
+    
+    if not hasattr(transformermanager, "_orig_transform_cell"):
+        transformermanager._orig_transform_cell = transformermanager.transform_cell
+        
+    def jd_transform_cell(*args, **kwargs) -> bool:
+        orig_cell = args[0]
+        if orig_cell.startswith("%%dql"):
+            return transform_dql_cell(orig_cell)
+        else:
+            result=get_ipython().input_transformer_manager._orig_transform_cell(*args, **kwargs)
+            #print(result)
+            return result
+    
+    transformermanager.transform_cell = jd_transform_cell
 
-    if not hasattr(shell, "_orig_transform_cell"):
-        shell._orig_transform_cell = shell.transform_cell
 
-    def transform_cell(*args, **kwargs) -> bool:
-            #print(args)
-            #print(kwargs)
-            
-            result=shell._orig_transform_cell(*args, **kwargs)
-            if result.startswith("get_ipython().run_cell_magic('dql',"):
-                result="await" + result
-            return result
+def patch_magic_assign():
+    from IPython.core.inputtransformer2 import MagicAssign
+    from typing import List
+
+    if not hasattr(MagicAssign, "_orig_transform"):
+        MagicAssign._orig_transform = MagicAssign.transform
+
+    def transform(a, lines: List[str]):
+        return a._orig_transform(lines)
+
+    MagicAssign.transform=transform
+
+def patch_tr_magic():
+    import IPython.core.inputtransformer2 as it
+
+    if not hasattr(it, "_orig_tr_magic"):
+        it._orig_tr_magic = it.tr[it.ESC_MAGIC]
+
+    def _tr_magic(content):
+        if content.startswith("dql "):
+            result=transform_dql_line(content[4:])
+        else:
+            result= it._orig_tr_magic(content)
+        return result
+
+    it.tr[it.ESC_MAGIC] = _tr_magic
     
-patch_magic()
+patch_transformer()
+patch_tr_magic()
+# Disabled for now: xyz = %dql won't work. 
+# patch_magic_assign()
```

## Comparing `jupylite_duckdb-0.0.18a2.dist-info/LICENSE` & `jupylite_duckdb-0.0.18a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.18a2.dist-info/RECORD` & `jupylite_duckdb-0.0.18a3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 jupylite_duckdb/__init__.py,sha256=-Z_P6KBbWKDsMsnvKal14k3bbGljgWmFQPEvz7zrLVU,128
-jupylite_duckdb/_version.py,sha256=8kjh-5-0HwdjXERHb01s3MfdAh7atVwueZwVp9JKo_g,23
+jupylite_duckdb/_version.py,sha256=jdgiQKn2jcm_N9qti4hd31Qj1fj-Wfixy8mirEyACto,23
 jupylite_duckdb/jdw.py,sha256=LzIoBx4_3j3iUlp5lviHuISdCClNdHEKb9_O8X1-cpg,9216
-jupylite_duckdb/jdw_magic.py,sha256=EBbz8IhYUc4Wubrfjb5jQcxsHblPj-BdwerktkUWxBo,2149
+jupylite_duckdb/jdw_magic.py,sha256=UiGfV4kVd-6PjmYJt6Pe7AciMKgpqFO2vUbHlj_rrCY,4973
 jupylite_duckdb/magic.py,sha256=okWgdHbcu0ul2BOYNdu9NHwRSoyAG_0m6RiGnw2Bj_k,979
-jupylite_duckdb-0.0.18a2.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.18a2.dist-info/METADATA,sha256=GiT31739aHPaVigBw0mvlsTALlZCXtvjR88Qzm6GiVQ,2559
-jupylite_duckdb-0.0.18a2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.18a2.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.18a2.dist-info/RECORD,,
+jupylite_duckdb-0.0.18a3.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.18a3.dist-info/METADATA,sha256=2KIy1t4rzEmw-LIw2UM9C1jMwJsF-U4mA8svXXGwF_Y,4787
+jupylite_duckdb-0.0.18a3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.18a3.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.18a3.dist-info/RECORD,,
```

