# Comparing `tmp/dune_harmonizer-0.6.0.tar.gz` & `tmp/dune_harmonizer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_harmonizer-0.6.0.tar", max compression
+gzip compressed data, was "dune_harmonizer-0.7.0.tar", max compression
```

## Comparing `dune_harmonizer-0.6.0.tar` & `dune_harmonizer-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1061 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/LICENSE
--rw-r--r--   0        0        0     2378 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/README.md
--rw-r--r--   0        0        0      440 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/__init__.py
--rw-r--r--   0        0        0      849 2023-04-24 08:27:37.515846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19435 2023-04-24 08:27:37.519846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
--rw-r--r--   0        0        0      630 2023-04-24 08:27:37.523846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     3103 2023-04-24 08:27:37.519846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3544 2023-04-24 08:27:37.515846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/constants.py
--rw-r--r--   0        0        0    16901 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/custom_transforms.py
--rw-r--r--   0        0        0     4082 2023-04-24 08:27:37.519846 dune_harmonizer-0.6.0/dune/harmonizer/dialects/__pycache__/dunesql.cpython-311.pyc
--rw-r--r--   0        0        0     2715 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/dialects/dunesql.py
--rw-r--r--   0        0        0      105 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/errors.py
--rw-r--r--   0        0        0     2018 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/table_replacements.py
--rw-r--r--   0        0        0     2916 2023-04-24 08:27:11.291843 dune_harmonizer-0.6.0/dune/harmonizer/translate.py
--rw-r--r--   0        0        0      570 2023-04-24 08:27:11.291843 dune_harmonizer-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2378 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/README.md
+-rw-r--r--   0        0        0      440 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-25 10:42:47.596641 dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    18865 2023-04-25 10:42:47.600641 dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2023-04-25 10:42:47.604641 dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     3103 2023-04-25 10:42:47.600641 dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3544 2023-04-25 10:42:47.600641 dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/constants.py
+-rw-r--r--   0        0        0    16529 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/custom_transforms.py
+-rw-r--r--   0        0        0     4841 2023-04-25 10:42:47.604641 dune_harmonizer-0.7.0/dune/harmonizer/dialects/__pycache__/dunesql.cpython-311.pyc
+-rw-r--r--   0        0        0     3339 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/dialects/dunesql.py
+-rw-r--r--   0        0        0      105 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/table_replacements.py
+-rw-r--r--   0        0        0     2916 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/dune/harmonizer/translate.py
+-rw-r--r--   0        0        0      570 2023-04-25 10:42:29.544133 dune_harmonizer-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.7.0/PKG-INFO
```

### Comparing `dune_harmonizer-0.6.0/LICENSE` & `dune_harmonizer-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.6.0/README.md` & `dune_harmonizer-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc` & `dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
+moddate:  0x95ae4764 (Tue Apr 25 10:42:29 2023 UTC)
 files sz: 440
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc` & `dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
-files sz: 16901
+moddate:  0x95ae4764 (Tue Apr 25 10:42:29 2023 UTC)
+files sz: 16529
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -14,15 +14,15 @@
       0aac08a6020000ab0200000000000000005a0b020065026508640bac08a6
       020000ab0200000000000000005a0c020065026508640cac08a6020000ab
       0200000000000000005a0d640d84005a0e640e5a0f640f5a106410650f9b
       009d025a1165109b0064109d025a126411650f9b009d025a1365109b0064
       119d025a14641284005a15641384005a16641484005a17641584005a1864
       1684005a19641784005a1a641884005a1b641984005a1c641a84005a1d64
       1b84005a1e641c84005a1f641d84005a20641e84005a21641f84005a2264
-      2084005a23642184005a24642284005a2564015300
+      2084005a23642184005a2464015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -184,31 +184,27 @@
                312 MAKE_FUNCTION            0
                314 STORE_NAME              32 (postgres_transforms)
    
    350         316 LOAD_CONST              30 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 350>)
                318 MAKE_FUNCTION            0
                320 STORE_NAME              33 (remove_quotes_around_0x_strings)
    
-   359         322 LOAD_CONST              31 (<code object spark_function_replacements, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 359>)
+   359         322 LOAD_CONST              31 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 359>)
                324 MAKE_FUNCTION            0
-               326 STORE_NAME              34 (spark_function_replacements)
+               326 STORE_NAME              34 (spark_transforms)
    
-   367         328 LOAD_CONST              32 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 367>)
+   377         328 LOAD_CONST              32 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 377>)
                330 MAKE_FUNCTION            0
-               332 STORE_NAME              35 (spark_transforms)
+               332 STORE_NAME              35 (add_warnings_and_banner)
    
-   386         334 LOAD_CONST              33 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 386>)
+   409         334 LOAD_CONST              33 (<code object parameter_placeholder, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 409>)
                336 MAKE_FUNCTION            0
-               338 STORE_NAME              36 (add_warnings_and_banner)
-   
-   418         340 LOAD_CONST              34 (<code object parameter_placeholder, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 418>)
-               342 MAKE_FUNCTION            0
-               344 STORE_NAME              37 (parameter_placeholder)
-               346 LOAD_CONST               1 (None)
-               348 RETURN_VALUE
+               338 STORE_NAME              36 (parameter_placeholder)
+               340 LOAD_CONST               1 (None)
+               342 RETURN_VALUE
    consts
       0
       None
       ('partial',)
       ('postgres_table_replacements',)
       code
          argcount  : 1
@@ -2137,212 +2133,141 @@
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'remove_quotes_around_0x_strings'
          firstlineno 350
          lnotab 0x020404014401
       code
          argcount  : 1
-         nlocals   : 2
-         stacksize : 6
-         flags     : 3
-         code
-            0x97007c00a00000000000000000000000000000000000000000006401ac
-            02a6010000ab0100000000000000007d0164037c01a00100000000000000
-            00000000000000000000000000a6000000ab000000000000000000760072
-            227405000000000000000000006a030000000000000000640464057c0174
-            04000000000000000000006a040000000000000000ac06a6040000ab0400
-            000000000000007d01740b000000000000000000006a0600000000000000
-            007c016401ac07a6020000ab0200000000000000005300
-         359           0 RESUME                   0
-         
-         361           2 LOAD_FAST                0 (node)
-                       4 LOAD_METHOD              0 (sql)
-                      26 LOAD_CONST               1 ('trino')
-                      28 KW_NAMES                 2
-                      30 PRECALL                  1
-                      34 CALL                     1
-                      44 STORE_FAST               1 (query)
-         
-         362          46 LOAD_CONST               3 ('timestamp(')
-                      48 LOAD_FAST                1 (query)
-                      50 LOAD_METHOD              1 (lower)
-                      72 PRECALL                  0
-                      76 CALL                     0
-                      86 CONTAINS_OP              0
-                      88 POP_JUMP_FORWARD_IF_FALSE    34 (to 158)
-         
-         363          90 LOAD_GLOBAL              5 (NULL + re)
-                     102 LOAD_ATTR                3 (sub)
-                     112 LOAD_CONST               4 ('timestamp')
-                     114 LOAD_CONST               5 ('from_unixtime')
-                     116 LOAD_FAST                1 (query)
-                     118 LOAD_GLOBAL              4 (re)
-                     130 LOAD_ATTR                4 (IGNORECASE)
-                     140 KW_NAMES                 6
-                     142 PRECALL                  4
-                     146 CALL                     4
-                     156 STORE_FAST               1 (query)
-         
-         364     >>  158 LOAD_GLOBAL             11 (NULL + sqlglot)
-                     170 LOAD_ATTR                6 (parse_one)
-                     180 LOAD_FAST                1 (query)
-                     182 LOAD_CONST               1 ('trino')
-                     184 KW_NAMES                 7
-                     186 PRECALL                  2
-                     190 CALL                     2
-                     200 RETURN_VALUE
-         consts
-            "Replace the Spark timestamp() function with Trino's from_unixtime() function"
-            'trino'
-            ('dialect',)
-            'timestamp('
-            'timestamp'
-            'from_unixtime'
-            ('flags',)
-            ('read',)
-         names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
-         varnames   ('node', 'query')
-         freevars   ()
-         cellvars   ()
-         filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
-         name       'spark_function_replacements'
-         firstlineno 359
-         lnotab 0x02022c012c014401
-      code
-         argcount  : 1
          nlocals   : 4
-         stacksize : 7
+         stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c006401ac
             02a6020000ab0200000000000000007d0174040000000000000000000074
             0600000000000000000000740800000000000000000000740a0000000000
-            0000000000740c00000000000000000000740e0000000000000000000074
-            100000000000000000000066077d027c0244005d177d037c01a009000000
-            00000000000000000000000000000000007c03a6010000ab010000000000
-            0000007d018c187c015300
-         367           0 RESUME                   0
+            0000000000740c00000000000000000000740e0000000000000000000066
+            067d027c0244005d177d037c01a008000000000000000000000000000000
+            00000000007c03a6010000ab0100000000000000007d018c187c015300
+         359           0 RESUME                   0
          
-         371           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         363           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               1 (query_tree)
          
-         373          46 LOAD_GLOBAL              4 (fix_boolean)
-         
-         374          58 LOAD_GLOBAL              6 (cast_numeric)
+         365          46 LOAD_GLOBAL              4 (fix_boolean)
          
-         375          70 LOAD_GLOBAL              8 (cast_timestamp)
+         366          58 LOAD_GLOBAL              6 (cast_numeric)
          
-         376          82 LOAD_GLOBAL             10 (warn_unnest)
+         367          70 LOAD_GLOBAL              8 (cast_timestamp)
          
-         377          94 LOAD_GLOBAL             12 (warn_sequence)
+         368          82 LOAD_GLOBAL             10 (warn_unnest)
          
-         378         106 LOAD_GLOBAL             14 (bytea2numeric)
+         369          94 LOAD_GLOBAL             12 (warn_sequence)
          
-         379         118 LOAD_GLOBAL             16 (spark_function_replacements)
+         370         106 LOAD_GLOBAL             14 (bytea2numeric)
          
-         372         130 BUILD_TUPLE              7
-                     132 STORE_FAST               2 (transforms)
+         364         118 BUILD_TUPLE              6
+                     120 STORE_FAST               2 (transforms)
          
-         381         134 LOAD_FAST                2 (transforms)
-                     136 GET_ITER
-                 >>  138 FOR_ITER                23 (to 186)
-                     140 STORE_FAST               3 (f)
+         372         122 LOAD_FAST                2 (transforms)
+                     124 GET_ITER
+                 >>  126 FOR_ITER                23 (to 174)
+                     128 STORE_FAST               3 (f)
          
-         382         142 LOAD_FAST                1 (query_tree)
-                     144 LOAD_METHOD              9 (transform)
-                     166 LOAD_FAST                3 (f)
-                     168 PRECALL                  1
-                     172 CALL                     1
-                     182 STORE_FAST               1 (query_tree)
-                     184 JUMP_BACKWARD           24 (to 138)
+         373         130 LOAD_FAST                1 (query_tree)
+                     132 LOAD_METHOD              8 (transform)
+                     154 LOAD_FAST                3 (f)
+                     156 PRECALL                  1
+                     160 CALL                     1
+                     170 STORE_FAST               1 (query_tree)
+                     172 JUMP_BACKWARD           24 (to 126)
          
-         383     >>  186 LOAD_FAST                1 (query_tree)
-                     188 RETURN_VALUE
+         374     >>  174 LOAD_FAST                1 (query_tree)
+                     176 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'trino'
             ('read',)
-         names      ('sqlglot', 'parse_one', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'spark_function_replacements', 'transform')
+         names      ('sqlglot', 'parse_one', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'transform')
          varnames   ('query', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'spark_transforms'
-         firstlineno 367
-         lnotab 0x02042c020c010c010c010c010c010c010cf9040908012c01
+         firstlineno 359
+         lnotab 0x02042c020c010c010c010c010c010cfa040808012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017c00a0000000000000000000000000000000000000000000a6
             000000ab0000000000000000007600720564027c007a0000007d00740300
             0000000000000000006a02000000000000000064037c00a6020000ab0200
             00000000000000720564047c007a0000007d0064057c00a0000000000000
             000000000000000000000000000000a6000000ab00000000000000000076
             00720564067c007a0000007d0064077c007a0000005300
-         386           0 RESUME                   0
+         377           0 RESUME                   0
          
-         388           2 LOAD_CONST               1 ("lower('{{")
+         379           2 LOAD_CONST               1 ("lower('{{")
                        4 LOAD_FAST                0 (query)
                        6 LOAD_METHOD              0 (lower)
                       28 PRECALL                  0
                       32 CALL                     0
                       42 CONTAINS_OP              0
                       44 POP_JUMP_FORWARD_IF_FALSE     5 (to 56)
          
-         390          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
+         381          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
          
-         393          48 LOAD_FAST                0 (query)
+         384          48 LOAD_FAST                0 (query)
          
-         389          50 BINARY_OP                0 (+)
+         380          50 BINARY_OP                0 (+)
                       54 STORE_FAST               0 (query)
          
-         396     >>   56 LOAD_GLOBAL              3 (NULL + re)
+         387     >>   56 LOAD_GLOBAL              3 (NULL + re)
                       68 LOAD_ATTR                2 (search)
                       78 LOAD_CONST               3 ('\\[.*\\]')
                       80 LOAD_FAST                0 (query)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE     5 (to 108)
          
-         398          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
+         389          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
          
-         401         100 LOAD_FAST                0 (query)
+         392         100 LOAD_FAST                0 (query)
          
-         397         102 BINARY_OP                0 (+)
+         388         102 BINARY_OP                0 (+)
                      106 STORE_FAST               0 (query)
          
-         403     >>  108 LOAD_CONST               5 ('dune_user_generated')
+         394     >>  108 LOAD_CONST               5 ('dune_user_generated')
                      110 LOAD_FAST                0 (query)
                      112 LOAD_METHOD              0 (lower)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 CONTAINS_OP              0
                      150 POP_JUMP_FORWARD_IF_FALSE     5 (to 162)
          
-         405         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
+         396         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
          
-         408         154 LOAD_FAST                0 (query)
+         399         154 LOAD_FAST                0 (query)
          
-         404         156 BINARY_OP                0 (+)
+         395         156 BINARY_OP                0 (+)
                      160 STORE_FAST               0 (query)
          
-         412     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
+         403     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
          
-         415         164 LOAD_FAST                0 (query)
+         406         164 LOAD_FAST                0 (query)
          
-         411         166 BINARY_OP                0 (+)
+         402         166 BINARY_OP                0 (+)
                      170 RETURN_VALUE
          consts
             "Add a success banner at the top, and look for a few cases of things we don't fix and add a warning if present"
             "lower('{{"
             "/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n"
             '\\[.*\\]'
             '/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n'
@@ -2351,15 +2276,15 @@
             "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n"
          names      ('lower', 're', 'search')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'add_warnings_and_banner'
-         firstlineno 386
+         firstlineno 377
          lnotab
             0x02022c02020302fc06072a02020302fc06062c02020302fc0608020302
             fc
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -2369,65 +2294,65 @@
             0200000000000000000000a6020000ab020000000000000000a000000000
             000000000000000000000000000000000064027404000000000000000000
             00a6020000ab020000000000000000a00000000000000000000000000000
             0000000000000064036404a6020000ab020000000000000000a000000000
             000000000000000000000000000000000064056404a6020000ab02000000
             0000000000a0030000000000000000000000000000000000000000a60000
             00ab0000000000000000005300
-         418           0 RESUME                   0
+         409           0 RESUME                   0
          
-         420           2 LOAD_FAST                0 (p)
+         411           2 LOAD_FAST                0 (p)
                        4 LOAD_METHOD              0 (replace)
                       26 LOAD_CONST               1 ('{{')
                       28 LOAD_GLOBAL              2 (param_left_placeholder)
                       40 PRECALL                  2
                       44 CALL                     2
          
-         421          54 LOAD_METHOD              0 (replace)
+         412          54 LOAD_METHOD              0 (replace)
                       76 LOAD_CONST               2 ('}}')
                       78 LOAD_GLOBAL              4 (param_right_placeholder)
                       90 PRECALL                  2
                       94 CALL                     2
          
-         422         104 LOAD_METHOD              0 (replace)
+         413         104 LOAD_METHOD              0 (replace)
                      126 LOAD_CONST               3 (' ')
                      128 LOAD_CONST               4 ('_')
                      130 PRECALL                  2
                      134 CALL                     2
          
-         423         144 LOAD_METHOD              0 (replace)
+         414         144 LOAD_METHOD              0 (replace)
                      166 LOAD_CONST               5 ('-')
                      168 LOAD_CONST               4 ('_')
                      170 PRECALL                  2
                      174 CALL                     2
          
-         424         184 LOAD_METHOD              3 (lower)
+         415         184 LOAD_METHOD              3 (lower)
                      206 PRECALL                  0
                      210 CALL                     0
          
-         419         220 RETURN_VALUE
+         410         220 RETURN_VALUE
          consts
             None
             '{{'
             '}}'
             ' '
             '_'
             '-'
          names      ('replace', 'param_left_placeholder', 'param_right_placeholder', 'lower')
          varnames   ('p',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'parameter_placeholder'
-         firstlineno 418
+         firstlineno 409
          lnotab 0x0202340132012801280124fb
-   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_function_replacements', 'spark_transforms', 'add_warnings_and_banner', 'parameter_placeholder')
+   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_transforms', 'add_warnings_and_banner', 'parameter_placeholder')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c0208020c030613065906121a011a011a011a011a0306
       2c040104010a010a010a010a03061b0609060f060a060e060e0605060e06
-      060609060a06170609060806130620
+      060609060a0617060906120620
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc` & `dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
+moddate:  0x95ae4764 (Tue Apr 25 10:42:29 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc` & `dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
+moddate:  0x95ae4764 (Tue Apr 25 10:42:29 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc` & `dune_harmonizer-0.7.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
+moddate:  0x95ae4764 (Tue Apr 25 10:42:29 2023 UTC)
 files sz: 2916
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/custom_transforms.py` & `dune_harmonizer-0.7.0/dune/harmonizer/custom_transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -352,35 +352,26 @@
 
     This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"""
     pattern = r"'0x(.*?)'"
     substituted = re.sub(pattern, r"0x\1", query, flags=re.IGNORECASE)
     return substituted
 
 
-def spark_function_replacements(node):
-    """Replace the Spark timestamp() function with Trino's from_unixtime() function"""
-    query = node.sql(dialect="trino")
-    if "timestamp(" in query.lower():
-        query = re.sub("timestamp", "from_unixtime", query, flags=re.IGNORECASE)
-    return sqlglot.parse_one(query, read="trino")
-
-
 def spark_transforms(query):
     """Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.
 
     Each transform takes and returns a sqlglot.Expression"""
     query_tree = sqlglot.parse_one(query, read="trino")
     transforms = (
         fix_boolean,
         cast_numeric,
         cast_timestamp,
         warn_unnest,
         warn_sequence,
         bytea2numeric,
-        spark_function_replacements,
     )
     for f in transforms:
         query_tree = query_tree.transform(f)
     return query_tree
 
 
 def add_warnings_and_banner(query):
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/dialects/__pycache__/dunesql.cpython-311.pyc` & `dune_harmonizer-0.7.0/dune/harmonizer/dialects/__pycache__/dunesql.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
-files sz: 2715
+moddate:  0x95ae4764 (Tue Apr 25 10:42:29 2023 UTC)
+files sz: 3339
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -34,17 +34,17 @@
                 36 LOAD_NAME                2 (exp)
                 38 LOAD_ATTR                6 (Expression)
                 48 BUILD_TUPLE              2
                 50 LOAD_CONST               4 (<code object explode_to_unnest, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 5>)
                 52 MAKE_FUNCTION            4 (annotations)
                 54 STORE_NAME               7 (explode_to_unnest)
    
-    38          56 PUSH_NULL
+    53          56 PUSH_NULL
                 58 LOAD_BUILD_CLASS
-                60 LOAD_CONST               5 (<code object DuneSQL, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 38>)
+                60 LOAD_CONST               5 (<code object DuneSQL, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 53>)
                 62 MAKE_FUNCTION            0
                 64 LOAD_CONST               6 ('DuneSQL')
                 66 LOAD_NAME                5 (Trino)
                 68 PRECALL                  3
                 72 CALL                     3
                 82 STORE_NAME               8 (DuneSQL)
                 84 LOAD_CONST               7 (None)
@@ -52,263 +52,359 @@
    consts
       0
       ('TokenType', 'exp', 'transforms')
       ('Trino',)
       'expression'
       code
          argcount  : 1
-         nlocals   : 10
-         stacksize : 8
+         nlocals   : 6
+         stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000007c007402000000000000000000006a
-            020000000000000000a6020000ab020000000000000000900172487c006a
+            020000000000000000a6020000ab0200000000000000009002724d7c006a
             030000000000000000a00400000000000000000000000000000000000000
-            0064016700a6020000ab020000000000000000440090015d2b7d0164027d
-            027401000000000000000000007c017402000000000000000000006a0500
-            00000000000000a6020000ab020000000000000000724a74010000000000
-            00000000007c016a03000000000000000064031900000000000000000074
-            02000000000000000000006a060000000000000000a6020000ab02000000
-            000000000072247c016a0700000000000000007d027c016a030000000000
-            0000006403190000000000000000007d037c017d047c036a030000000000
-            0000006403190000000000000000007d056e2e8c69740100000000000000
-            0000007c017402000000000000000000006a060000000000000000a60200
-            00ab02000000000000000072127c017d037c017d047c036a030000000000
-            0000006403190000000000000000007d056e018c9664047d067c02700164
-            057d077403000000000000000000006a0800000000000000007c0567017c
-            069b0064067c079b0064079d04ac08a6020000ab0200000000000000007d
-            087403000000000000000000006a0900000000000000007c086409ac0aa6
-            020000ab0200000000000000007d097c006a030000000000000000640119
-            000000000000000000a00a00000000000000000000000000000000000000
-            007c04a6010000ab01000000000000000001007c00a00b00000000000000
-            000000000000000000000000007c07a6010000ab010000000000000000a0
-            0c00000000000000000000000000000000000000006700ac0ba6010000ab
-            010000000000000000a00d00000000000000000000000000000000000000
-            007c09a6010000ab0100000000000000007d0090018c2d7c005300
+            0064016700a6020000ab020000000000000000440090025d307d01740100
+            0000000000000000007c017402000000000000000000006a050000000000
+            000000a6020000ab02000000000000000072c97c016a0300000000000000
+            006402190000000000000000007d027c006a030000000000000000640119
+            000000000000000000a00600000000000000000000000000000000000000
+            007c01a6010000ab01000000000000000001007403000000000000000000
+            006a0700000000000000007c02670164036404ac05a6030000ab03000000
+            00000000007d037c006a030000000000000000a004000000000000000000
+            00000000000000000000006406a6010000ab010000000000000000814074
+            03000000000000000000006a0800000000000000007c036408ac09a60200
+            00ab0200000000000000007d047c00a00900000000000000000000000000
+            00000000000000640a640ba6020000ab020000000000000000a00a000000
+            00000000000000000000000000000000007c04a6010000ab010000000000
+            0000007d006e297c00a00900000000000000000000000000000000000000
+            00640a640ba6020000ab020000000000000000a00b000000000000000000
+            00000000000000000000007c03a6010000ab0100000000000000007d008c
+            e67401000000000000000000007c017402000000000000000000006a0c00
+            00000000000000a6020000ab0200000000000000007210640b7d057c016a
+            0300000000000000006402190000000000000000007d026e637401000000
+            000000000000007c017402000000000000000000006a0d00000000000000
+            00a6020000ab02000000000000000072477401000000000000000000007c
+            016a03000000000000000064021900000000000000000074020000000000
+            00000000006a0c0000000000000000a6020000ab02000000000000000073
+            0290018c517c016a0e00000000000000007d057c016a0300000000000000
+            006402190000000000000000006a03000000000000000064021900000000
+            00000000007d026e0290018c737c006a0300000000000000006401190000
+            00000000000000a00600000000000000000000000000000000000000007c
+            01a6010000ab01000000000000000001007403000000000000000000006a
+            0700000000000000007c026701640c7c059b00640d9d03ac0ea6020000ab
+            0200000000000000007d037c006a030000000000000000a0040000000000
+            0000000000000000000000000000006406a6010000ab0100000000000000
+            0081407403000000000000000000006a0800000000000000007c036408ac
+            09a6020000ab0200000000000000007d047c00a009000000000000000000
+            00000000000000000000007c05a6010000ab010000000000000000a00a00
+            000000000000000000000000000000000000007c04a6010000ab01000000
+            00000000007d0090028c087c00a009000000000000000000000000000000
+            00000000007c05a6010000ab010000000000000000a00b00000000000000
+            000000000000000000000000007c03a6010000ab0100000000000000007d
+            0090028c327c005300
            5           0 RESUME                   0
          
            7           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (expression)
                       16 LOAD_GLOBAL              2 (exp)
                       28 LOAD_ATTR                2 (Select)
                       38 PRECALL                  2
                       42 CALL                     2
-                      52 EXTENDED_ARG             1
-                      54 POP_JUMP_FORWARD_IF_FALSE   328 (to 712)
+                      52 EXTENDED_ARG             2
+                      54 POP_JUMP_FORWARD_IF_FALSE   589 (to 1234)
          
            8          56 LOAD_FAST                0 (expression)
                       58 LOAD_ATTR                3 (args)
                       68 LOAD_METHOD              4 (get)
                       90 LOAD_CONST               1 ('expressions')
                       92 BUILD_LIST               0
                       94 PRECALL                  2
                       98 CALL                     2
                      108 GET_ITER
-                 >>  110 EXTENDED_ARG             1
-                     112 FOR_ITER               299 (to 712)
+                 >>  110 EXTENDED_ARG             2
+                     112 FOR_ITER               560 (to 1234)
                      114 STORE_FAST               1 (e)
          
-          10         116 LOAD_CONST               2 (None)
-                     118 STORE_FAST               2 (explode_alias)
+           9         116 LOAD_GLOBAL              1 (NULL + isinstance)
+                     128 LOAD_FAST                1 (e)
+                     130 LOAD_GLOBAL              2 (exp)
+                     142 LOAD_ATTR                5 (Posexplode)
+                     152 PRECALL                  2
+                     156 CALL                     2
+                     166 POP_JUMP_FORWARD_IF_FALSE   201 (to 570)
+         
+          10         168 LOAD_FAST                1 (e)
+                     170 LOAD_ATTR                3 (args)
+                     180 LOAD_CONST               2 ('this')
+                     182 BINARY_SUBSCR
+                     192 STORE_FAST               2 (explode_expression)
+         
+          13         194 LOAD_FAST                0 (expression)
+                     196 LOAD_ATTR                3 (args)
+                     206 LOAD_CONST               1 ('expressions')
+                     208 BINARY_SUBSCR
+                     218 LOAD_METHOD              6 (remove)
+                     240 LOAD_FAST                1 (e)
+                     242 PRECALL                  1
+                     246 CALL                     1
+                     256 POP_TOP
+         
+          17         258 LOAD_GLOBAL              3 (NULL + exp)
+                     270 LOAD_ATTR                7 (Unnest)
+                     280 LOAD_FAST                2 (explode_expression)
+                     282 BUILD_LIST               1
+                     284 LOAD_CONST               3 ('array_column(col, pos)')
+                     286 LOAD_CONST               4 (True)
+                     288 KW_NAMES                 5
+                     290 PRECALL                  3
+                     294 CALL                     3
+                     304 STORE_FAST               3 (unnest)
+         
+          18         306 LOAD_FAST                0 (expression)
+                     308 LOAD_ATTR                3 (args)
+                     318 LOAD_METHOD              4 (get)
+                     340 LOAD_CONST               6 ('from')
+                     342 PRECALL                  1
+                     346 CALL                     1
+                     356 POP_JUMP_FORWARD_IF_NONE    64 (to 486)
+         
+          19         358 LOAD_GLOBAL              3 (NULL + exp)
+                     370 LOAD_ATTR                8 (Join)
+                     380 LOAD_FAST                3 (unnest)
+                     382 LOAD_CONST               8 ('CROSS')
+                     384 KW_NAMES                 9
+                     386 PRECALL                  2
+                     390 CALL                     2
+                     400 STORE_FAST               4 (join)
+         
+          20         402 LOAD_FAST                0 (expression)
+                     404 LOAD_METHOD              9 (select)
+                     426 LOAD_CONST              10 ('pos')
+                     428 LOAD_CONST              11 ('col')
+                     430 PRECALL                  2
+                     434 CALL                     2
+                     444 LOAD_METHOD             10 (join)
+                     466 LOAD_FAST                4 (join)
+                     468 PRECALL                  1
+                     472 CALL                     1
+                     482 STORE_FAST               0 (expression)
+                     484 JUMP_FORWARD            41 (to 568)
+         
+          22     >>  486 LOAD_FAST                0 (expression)
+                     488 LOAD_METHOD              9 (select)
+                     510 LOAD_CONST              10 ('pos')
+                     512 LOAD_CONST              11 ('col')
+                     514 PRECALL                  2
+                     518 CALL                     2
+                     528 LOAD_METHOD             11 (from_)
+                     550 LOAD_FAST                3 (unnest)
+                     552 PRECALL                  1
+                     556 CALL                     1
+                     566 STORE_FAST               0 (expression)
+         
+          23     >>  568 JUMP_BACKWARD          230 (to 110)
+         
+          25     >>  570 LOAD_GLOBAL              1 (NULL + isinstance)
+                     582 LOAD_FAST                1 (e)
+                     584 LOAD_GLOBAL              2 (exp)
+                     596 LOAD_ATTR               12 (Explode)
+                     606 PRECALL                  2
+                     610 CALL                     2
+                     620 POP_JUMP_FORWARD_IF_FALSE    16 (to 654)
+         
+          26         622 LOAD_CONST              11 ('col')
+                     624 STORE_FAST               5 (unnested_column_name)
+         
+          27         626 LOAD_FAST                1 (e)
+                     628 LOAD_ATTR                3 (args)
+                     638 LOAD_CONST               2 ('this')
+                     640 BINARY_SUBSCR
+                     650 STORE_FAST               2 (explode_expression)
+                     652 JUMP_FORWARD            99 (to 852)
+         
+          29     >>  654 LOAD_GLOBAL              1 (NULL + isinstance)
+                     666 LOAD_FAST                1 (e)
+                     668 LOAD_GLOBAL              2 (exp)
+                     680 LOAD_ATTR               13 (Alias)
+                     690 PRECALL                  2
+                     694 CALL                     2
+                     704 POP_JUMP_FORWARD_IF_FALSE    71 (to 848)
+         
+          30         706 LOAD_GLOBAL              1 (NULL + isinstance)
+                     718 LOAD_FAST                1 (e)
+                     720 LOAD_ATTR                3 (args)
+                     730 LOAD_CONST               2 ('this')
+                     732 BINARY_SUBSCR
+                     742 LOAD_GLOBAL              2 (exp)
+                     754 LOAD_ATTR               12 (Explode)
+                     764 PRECALL                  2
+                     768 CALL                     2
+                     778 POP_JUMP_FORWARD_IF_TRUE     2 (to 784)
+         
+          31         780 EXTENDED_ARG             1
+                     782 JUMP_BACKWARD          337 (to 110)
+         
+          32     >>  784 LOAD_FAST                1 (e)
+                     786 LOAD_ATTR               14 (alias)
+                     796 STORE_FAST               5 (unnested_column_name)
+         
+          33         798 LOAD_FAST                1 (e)
+                     800 LOAD_ATTR                3 (args)
+                     810 LOAD_CONST               2 ('this')
+                     812 BINARY_SUBSCR
+                     822 LOAD_ATTR                3 (args)
+                     832 LOAD_CONST               2 ('this')
+                     834 BINARY_SUBSCR
+                     844 STORE_FAST               2 (explode_expression)
+                     846 JUMP_FORWARD             2 (to 852)
+         
+          37     >>  848 EXTENDED_ARG             1
+                     850 JUMP_BACKWARD          371 (to 110)
+         
+          40     >>  852 LOAD_FAST                0 (expression)
+                     854 LOAD_ATTR                3 (args)
+                     864 LOAD_CONST               1 ('expressions')
+                     866 BINARY_SUBSCR
+                     876 LOAD_METHOD              6 (remove)
+                     898 LOAD_FAST                1 (e)
+                     900 PRECALL                  1
+                     904 CALL                     1
+                     914 POP_TOP
+         
+          44         916 LOAD_GLOBAL              3 (NULL + exp)
+                     928 LOAD_ATTR                7 (Unnest)
+                     938 LOAD_FAST                2 (explode_expression)
+                     940 BUILD_LIST               1
+                     942 LOAD_CONST              12 ('array_column(')
+                     944 LOAD_FAST                5 (unnested_column_name)
+                     946 FORMAT_VALUE             0
+                     948 LOAD_CONST              13 (')')
+                     950 BUILD_STRING             3
+                     952 KW_NAMES                14
+                     954 PRECALL                  2
+                     958 CALL                     2
+                     968 STORE_FAST               3 (unnest)
+         
+          45         970 LOAD_FAST                0 (expression)
+                     972 LOAD_ATTR                3 (args)
+                     982 LOAD_METHOD              4 (get)
+                    1004 LOAD_CONST               6 ('from')
+                    1006 PRECALL                  1
+                    1010 CALL                     1
+                    1020 POP_JUMP_FORWARD_IF_NONE    64 (to 1150)
+         
+          46        1022 LOAD_GLOBAL              3 (NULL + exp)
+                    1034 LOAD_ATTR                8 (Join)
+                    1044 LOAD_FAST                3 (unnest)
+                    1046 LOAD_CONST               8 ('CROSS')
+                    1048 KW_NAMES                 9
+                    1050 PRECALL                  2
+                    1054 CALL                     2
+                    1064 STORE_FAST               4 (join)
+         
+          47        1066 LOAD_FAST                0 (expression)
+                    1068 LOAD_METHOD              9 (select)
+                    1090 LOAD_FAST                5 (unnested_column_name)
+                    1092 PRECALL                  1
+                    1096 CALL                     1
+                    1106 LOAD_METHOD             10 (join)
+                    1128 LOAD_FAST                4 (join)
+                    1130 PRECALL                  1
+                    1134 CALL                     1
+                    1144 STORE_FAST               0 (expression)
+                    1146 EXTENDED_ARG             2
+                    1148 JUMP_BACKWARD          520 (to 110)
+         
+          49     >> 1150 LOAD_FAST                0 (expression)
+                    1152 LOAD_METHOD              9 (select)
+                    1174 LOAD_FAST                5 (unnested_column_name)
+                    1176 PRECALL                  1
+                    1180 CALL                     1
+                    1190 LOAD_METHOD             11 (from_)
+                    1212 LOAD_FAST                3 (unnest)
+                    1214 PRECALL                  1
+                    1218 CALL                     1
+                    1228 STORE_FAST               0 (expression)
+                    1230 EXTENDED_ARG             2
+                    1232 JUMP_BACKWARD          562 (to 110)
          
-          11         120 LOAD_GLOBAL              1 (NULL + isinstance)
-                     132 LOAD_FAST                1 (e)
-                     134 LOAD_GLOBAL              2 (exp)
-                     146 LOAD_ATTR                5 (Alias)
-                     156 PRECALL                  2
-                     160 CALL                     2
-                     170 POP_JUMP_FORWARD_IF_FALSE    74 (to 320)
-         
-          12         172 LOAD_GLOBAL              1 (NULL + isinstance)
-                     184 LOAD_FAST                1 (e)
-                     186 LOAD_ATTR                3 (args)
-                     196 LOAD_CONST               3 ('this')
-                     198 BINARY_SUBSCR
-                     208 LOAD_GLOBAL              2 (exp)
-                     220 LOAD_ATTR                6 (Explode)
-                     230 PRECALL                  2
-                     234 CALL                     2
-                     244 POP_JUMP_FORWARD_IF_FALSE    36 (to 318)
-         
-          13         246 LOAD_FAST                1 (e)
-                     248 LOAD_ATTR                7 (alias)
-                     258 STORE_FAST               2 (explode_alias)
-         
-          14         260 LOAD_FAST                1 (e)
-                     262 LOAD_ATTR                3 (args)
-                     272 LOAD_CONST               3 ('this')
-                     274 BINARY_SUBSCR
-                     284 STORE_FAST               3 (explode)
-         
-          15         286 LOAD_FAST                1 (e)
-                     288 STORE_FAST               4 (to_remove)
-         
-          16         290 LOAD_FAST                3 (explode)
-                     292 LOAD_ATTR                3 (args)
-                     302 LOAD_CONST               3 ('this')
-                     304 BINARY_SUBSCR
-                     314 STORE_FAST               5 (explode_expression)
-                     316 JUMP_FORWARD            46 (to 410)
-         
-          18     >>  318 JUMP_BACKWARD          105 (to 110)
-         
-          19     >>  320 LOAD_GLOBAL              1 (NULL + isinstance)
-                     332 LOAD_FAST                1 (e)
-                     334 LOAD_GLOBAL              2 (exp)
-                     346 LOAD_ATTR                6 (Explode)
-                     356 PRECALL                  2
-                     360 CALL                     2
-                     370 POP_JUMP_FORWARD_IF_FALSE    18 (to 408)
-         
-          20         372 LOAD_FAST                1 (e)
-                     374 STORE_FAST               3 (explode)
-         
-          21         376 LOAD_FAST                1 (e)
-                     378 STORE_FAST               4 (to_remove)
-         
-          22         380 LOAD_FAST                3 (explode)
-                     382 LOAD_ATTR                3 (args)
-                     392 LOAD_CONST               3 ('this')
-                     394 BINARY_SUBSCR
-                     404 STORE_FAST               5 (explode_expression)
-                     406 JUMP_FORWARD             1 (to 410)
-         
-          24     >>  408 JUMP_BACKWARD          150 (to 110)
-         
-          26     >>  410 LOAD_CONST               4 ('array_column')
-                     412 STORE_FAST               6 (array_column_name)
-         
-          27         414 LOAD_FAST                2 (explode_alias)
-                     416 JUMP_IF_TRUE_OR_POP      1 (to 420)
-                     418 LOAD_CONST               5 ('col')
-                 >>  420 STORE_FAST               7 (unnested_column_name)
-         
-          28         422 LOAD_GLOBAL              3 (NULL + exp)
-                     434 LOAD_ATTR                8 (Unnest)
-                     444 LOAD_FAST                5 (explode_expression)
-                     446 BUILD_LIST               1
-                     448 LOAD_FAST                6 (array_column_name)
-                     450 FORMAT_VALUE             0
-                     452 LOAD_CONST               6 ('(')
-                     454 LOAD_FAST                7 (unnested_column_name)
-                     456 FORMAT_VALUE             0
-                     458 LOAD_CONST               7 (')')
-                     460 BUILD_STRING             4
-                     462 KW_NAMES                 8
-                     464 PRECALL                  2
-                     468 CALL                     2
-                     478 STORE_FAST               8 (unnest)
-         
-          29         480 LOAD_GLOBAL              3 (NULL + exp)
-                     492 LOAD_ATTR                9 (Join)
-                     502 LOAD_FAST                8 (unnest)
-                     504 LOAD_CONST               9 ('CROSS')
-                     506 KW_NAMES                10
-                     508 PRECALL                  2
-                     512 CALL                     2
-                     522 STORE_FAST               9 (join)
-         
-          31         524 LOAD_FAST                0 (expression)
-                     526 LOAD_ATTR                3 (args)
-                     536 LOAD_CONST               1 ('expressions')
-                     538 BINARY_SUBSCR
-                     548 LOAD_METHOD             10 (remove)
-                     570 LOAD_FAST                4 (to_remove)
-                     572 PRECALL                  1
-                     576 CALL                     1
-                     586 POP_TOP
-         
-          34         588 LOAD_FAST                0 (expression)
-                     590 LOAD_METHOD             11 (select)
-                     612 LOAD_FAST                7 (unnested_column_name)
-                     614 PRECALL                  1
-                     618 CALL                     1
-                     628 LOAD_METHOD             12 (from_)
-                     650 BUILD_LIST               0
-                     652 KW_NAMES                11
-                     654 PRECALL                  1
-                     658 CALL                     1
-                     668 LOAD_METHOD             13 (join)
-                     690 LOAD_FAST                9 (join)
-                     692 PRECALL                  1
-                     696 CALL                     1
-                     706 STORE_FAST               0 (expression)
-                     708 EXTENDED_ARG             1
-                     710 JUMP_BACKWARD          301 (to 110)
-         
-          35     >>  712 LOAD_FAST                0 (expression)
-                     714 RETURN_VALUE
+          50     >> 1234 LOAD_FAST                0 (expression)
+                    1236 RETURN_VALUE
          consts
-            'Convert explode to cross join unnest'
+            'Convert posexplode, explode, and aliased explode to unnest'
             'expressions'
-            None
             'this'
-            'array_column'
+            'array_column(col, pos)'
+            True
+            ('expressions', 'alias', 'ordinality')
+            'from'
+            None
+            'CROSS'
+            ('this', 'kind')
+            'pos'
             'col'
-            '('
+            'array_column('
             ')'
             ('expressions', 'alias')
-            'CROSS'
-            ('this', 'kind')
-            ('expressions',)
-         names      ('isinstance', 'exp', 'Select', 'args', 'get', 'Alias', 'Explode', 'alias', 'Unnest', 'Join', 'remove', 'select', 'from_', 'join')
-         varnames   ('expression', 'e', 'explode_alias', 'explode', 'to_remove', 'explode_expression', 'array_column_name', 'unnested_column_name', 'unnest', 'join')
+         names      ('isinstance', 'exp', 'Select', 'args', 'get', 'Posexplode', 'remove', 'Unnest', 'Join', 'select', 'join', 'from_', 'Explode', 'Alias', 'alias')
+         varnames   ('expression', 'e', 'explode_expression', 'unnest', 'join', 'unnested_column_name')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
          name       'explode_to_unnest'
          firstlineno 5
          lnotab
-            0x020236013c02040134014a010e011a0104011c0202013401040104011c
-            020202040108013a012c0240037c01
+            0x020236013c0134011a034004300134012c01540252010202340104011c
+            0234014a0104010e01320404034004360134012c0154025401
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a030200470064028400640365046a0500
             00000000000000a6030000ab0300000000000000005a0502004700640484
             00640565046a060000000000000000a6030000ab0300000000000000005a
             060200470064068400640765046a070000000000000000a6030000ab0300
             000000000000005a0764085300
-          38           0 RESUME                   0
+          53           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DuneSQL')
                        8 STORE_NAME               2 (__qualname__)
          
-          39          10 LOAD_CONST               1 ("The DuneSQL dialect is the dialect used to execute SQL queries on Dune's crypto data sets\n\n    DuneSQL is the Trino dialect with slight modifications.")
+          54          10 LOAD_CONST               1 ("The DuneSQL dialect is the dialect used to execute SQL queries on Dune's crypto data sets\n\n    DuneSQL is the Trino dialect with slight modifications.")
                       12 STORE_NAME               3 (__doc__)
          
-          43          14 PUSH_NULL
+          58          14 PUSH_NULL
                       16 LOAD_BUILD_CLASS
-                      18 LOAD_CONST               2 (<code object Tokenizer, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 43>)
+                      18 LOAD_CONST               2 (<code object Tokenizer, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 58>)
                       20 MAKE_FUNCTION            0
                       22 LOAD_CONST               3 ('Tokenizer')
                       24 LOAD_NAME                4 (Trino)
                       26 LOAD_ATTR                5 (Tokenizer)
                       36 PRECALL                  3
                       40 CALL                     3
                       50 STORE_NAME               5 (Tokenizer)
          
-          52          52 PUSH_NULL
+          67          52 PUSH_NULL
                       54 LOAD_BUILD_CLASS
-                      56 LOAD_CONST               4 (<code object Parser, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 52>)
+                      56 LOAD_CONST               4 (<code object Parser, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 67>)
                       58 MAKE_FUNCTION            0
                       60 LOAD_CONST               5 ('Parser')
                       62 LOAD_NAME                4 (Trino)
                       64 LOAD_ATTR                6 (Parser)
                       74 PRECALL                  3
                       78 CALL                     3
                       88 STORE_NAME               6 (Parser)
          
-          57          90 PUSH_NULL
+          72          90 PUSH_NULL
                       92 LOAD_BUILD_CLASS
-                      94 LOAD_CONST               6 (<code object Generator, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 57>)
+                      94 LOAD_CONST               6 (<code object Generator, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 72>)
                       96 MAKE_FUNCTION            0
                       98 LOAD_CONST               7 ('Generator')
                      100 LOAD_NAME                4 (Trino)
                      102 LOAD_ATTR                7 (Generator)
                      112 PRECALL                  3
                      116 CALL                     3
                      126 STORE_NAME               7 (Generator)
@@ -322,39 +418,39 @@
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a0264015a036402640367025a0465056a06000000
                   00000000006a07000000000000000065086a09000000000000000065086a
                   0a000000000000000064049c027a0700005a0764055300
-                43           0 RESUME                   0
+                58           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('DuneSQL.Tokenizer')
                              8 STORE_NAME               2 (__qualname__)
                
-                44          10 LOAD_CONST               1 ('Text -> Tokens')
+                59          10 LOAD_CONST               1 ('Text -> Tokens')
                             12 STORE_NAME               3 (__doc__)
                
-                46          14 LOAD_CONST               2 ('0x')
+                61          14 LOAD_CONST               2 ('0x')
                             16 LOAD_CONST               3 (("X'", "'"))
                             18 BUILD_LIST               2
                             20 STORE_NAME               4 (HEX_STRINGS)
                
-                47          22 LOAD_NAME                5 (Trino)
+                62          22 LOAD_NAME                5 (Trino)
                             24 LOAD_ATTR                6 (Tokenizer)
                             34 LOAD_ATTR                7 (KEYWORDS)
                
-                48          44 LOAD_NAME                8 (TokenType)
+                63          44 LOAD_NAME                8 (TokenType)
                             46 LOAD_ATTR                9 (UBIGINT)
                
-                49          56 LOAD_NAME                8 (TokenType)
+                64          56 LOAD_NAME                8 (TokenType)
                             58 LOAD_ATTR               10 (BIGINT)
                
-                47          68 LOAD_CONST               4 (('UINT256', 'INT256'))
+                62          68 LOAD_CONST               4 (('UINT256', 'INT256'))
                             70 BUILD_CONST_KEY_MAP      2
                             72 BINARY_OP                7 (|)
                             76 STORE_NAME               7 (KEYWORDS)
                             78 LOAD_CONST               5 (None)
                             80 RETURN_VALUE
                consts
                   'DuneSQL.Tokenizer'
@@ -365,36 +461,36 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'HEX_STRINGS', 'Trino', 'Tokenizer', 'KEYWORDS', 'TokenType', 'UBIGINT', 'BIGINT')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
                name       'Tokenizer'
-               firstlineno 43
+               firstlineno 58
                lnotab 0x0a010402080116010c010cfe
             'Tokenizer'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a0264015a0365046a0500000000000000006a0600
                   0000000000000065076a08000000000000000065076a0900000000000000
                   0068027a0700005a0664025300
-                52           0 RESUME                   0
+                67           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('DuneSQL.Parser')
                              8 STORE_NAME               2 (__qualname__)
                
-                53          10 LOAD_CONST               1 ('Tokens -> AST')
+                68          10 LOAD_CONST               1 ('Tokens -> AST')
                             12 STORE_NAME               3 (__doc__)
                
-                55          14 LOAD_NAME                4 (Trino)
+                70          14 LOAD_NAME                4 (Trino)
                             16 LOAD_ATTR                5 (Parser)
                             26 LOAD_ATTR                6 (TYPE_TOKENS)
                             36 LOAD_NAME                7 (TokenType)
                             38 LOAD_ATTR                8 (UBIGINT)
                             48 LOAD_NAME                7 (TokenType)
                             50 LOAD_ATTR                9 (BIGINT)
                             60 BUILD_SET                2
@@ -408,15 +504,15 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'Trino', 'Parser', 'TYPE_TOKENS', 'TokenType', 'UBIGINT', 'BIGINT')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
                name       'Parser'
-               firstlineno 52
+               firstlineno 67
                lnotab 0x0a010402
             'Parser'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 7
                flags     : 0
@@ -424,63 +520,63 @@
                   0x970065005a0164005a0264015a0365046a0500000000000000006a0600
                   0000000000000065076a0800000000000000006402840065076a09000000
                   00000000000200650a6a0b0000000000000000650c6701a6010000ab0100
                   0000000000000069027a0700005a0665046a0500000000000000006a0d00
                   0000000000000065076a0e00000000000000006a0f00000000000000006a
                   100000000000000000640365076a0e00000000000000006a0f0000000000
                   0000006a110000000000000000640469027a0700005a0d64055300
-                57           0 RESUME                   0
+                72           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('DuneSQL.Generator')
                              8 STORE_NAME               2 (__qualname__)
                
-                58          10 LOAD_CONST               1 ('AST -> SQL')
+                73          10 LOAD_CONST               1 ('AST -> SQL')
                             12 STORE_NAME               3 (__doc__)
                
-                60          14 LOAD_NAME                4 (Trino)
+                75          14 LOAD_NAME                4 (Trino)
                             16 LOAD_ATTR                5 (Generator)
                             26 LOAD_ATTR                6 (TRANSFORMS)
                
-                62          36 LOAD_NAME                7 (exp)
+                77          36 LOAD_NAME                7 (exp)
                             38 LOAD_ATTR                8 (HexString)
-                            48 LOAD_CONST               2 (<code object <lambda>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 62>)
+                            48 LOAD_CONST               2 (<code object <lambda>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py", line 77>)
                             50 MAKE_FUNCTION            0
                
-                63          52 LOAD_NAME                7 (exp)
+                78          52 LOAD_NAME                7 (exp)
                             54 LOAD_ATTR                9 (Select)
                             64 PUSH_NULL
                             66 LOAD_NAME               10 (transforms)
                             68 LOAD_ATTR               11 (preprocess)
                             78 LOAD_NAME               12 (explode_to_unnest)
                             80 BUILD_LIST               1
                             82 PRECALL                  1
                             86 CALL                     1
                
-                60          96 BUILD_MAP                2
+                75          96 BUILD_MAP                2
                             98 BINARY_OP                7 (|)
                            102 STORE_NAME               6 (TRANSFORMS)
                
-                66         104 LOAD_NAME                4 (Trino)
+                81         104 LOAD_NAME                4 (Trino)
                            106 LOAD_ATTR                5 (Generator)
                            116 LOAD_ATTR               13 (TYPE_MAPPING)
                
-                67         126 LOAD_NAME                7 (exp)
+                82         126 LOAD_NAME                7 (exp)
                            128 LOAD_ATTR               14 (DataType)
                            138 LOAD_ATTR               15 (Type)
                            148 LOAD_ATTR               16 (UBIGINT)
                            158 LOAD_CONST               3 ('UINT256')
                
-                68         160 LOAD_NAME                7 (exp)
+                83         160 LOAD_NAME                7 (exp)
                            162 LOAD_ATTR               14 (DataType)
                            172 LOAD_ATTR               15 (Type)
                            182 LOAD_ATTR               17 (BIGINT)
                            192 LOAD_CONST               4 ('INT256')
                
-                66         194 BUILD_MAP                2
+                81         194 BUILD_MAP                2
                            196 BINARY_OP                7 (|)
                            200 STORE_NAME              13 (TYPE_MAPPING)
                            202 LOAD_CONST               5 (None)
                            204 RETURN_VALUE
                consts
                   'DuneSQL.Generator'
                   'AST -> SQL'
@@ -489,15 +585,15 @@
                      nlocals   : 2
                      stacksize : 5
                      flags     : 3
                      code
                         0x97007401000000000000000000007403000000000000000000007c016a
                         020000000000000000a6010000ab010000000000000000a6010000ab0100
                         000000000000005300
-                      62           0 RESUME                   0
+                      77           0 RESUME                   0
                                    2 LOAD_GLOBAL              1 (NULL + hex)
                                   14 LOAD_GLOBAL              3 (NULL + int)
                                   26 LOAD_FAST                1 (e)
                                   28 LOAD_ATTR                2 (name)
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 PRECALL                  1
@@ -507,40 +603,40 @@
                         None
                      names      ('hex', 'int', 'name')
                      varnames   ('self', 'e')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
                      name       '<lambda>'
-                     firstlineno 62
+                     firstlineno 77
                      lnotab 0x
                   'UINT256'
                   'INT256'
                   None
                names      ('__name__', '__module__', '__qualname__', '__doc__', 'Trino', 'Generator', 'TRANSFORMS', 'exp', 'HexString', 'Select', 'transforms', 'preprocess', 'explode_to_unnest', 'TYPE_MAPPING', 'DataType', 'Type', 'UBIGINT', 'BIGINT')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
                name       'Generator'
-               firstlineno 57
+               firstlineno 72
                lnotab 0x0a010402160210012cfd08061601220122fe
             'Generator'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Trino', 'Tokenizer', 'Parser', 'Generator')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
          name       'DuneSQL'
-         firstlineno 38
+         firstlineno 53
          lnotab 0x0a01040426092605
       'DuneSQL'
       None
    names      ('sqlglot', 'TokenType', 'exp', 'transforms', 'sqlglot.dialects.trino', 'Trino', 'Expression', 'explode_to_unnest', 'DuneSQL')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/dialects/dunesql.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020114010c031621
+   lnotab 0x00ff020114010c031630
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/dialects/dunesql.py` & `dune_harmonizer-0.7.0/dune/harmonizer/dialects/dunesql.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 from sqlglot import TokenType, exp, transforms
 from sqlglot.dialects.trino import Trino
 
 
 def explode_to_unnest(expression: exp.Expression):
-    """Convert explode to cross join unnest"""
+    """Convert posexplode, explode, and aliased explode to unnest"""
     if isinstance(expression, exp.Select):
         for e in expression.args.get("expressions", []):
-            # Handle either an aliased explode select, or a plain explode select
-            explode_alias = None
-            if isinstance(e, exp.Alias):
-                if isinstance(e.args["this"], exp.Explode):
-                    explode_alias = e.alias
-                    explode = e.args["this"]
-                    to_remove = e
-                    explode_expression = explode.args["this"]
+            if isinstance(e, exp.Posexplode):
+                explode_expression = e.args["this"]
+
+                # Remove the `posexplode()` expression from the select
+                expression.args["expressions"].remove(e)
+
+                # If the SELECT has a FROM, do a CROSS JOIN with the UNNEST,
+                # otherwise, just do SELECT ... FROM UNNEST
+                unnest = exp.Unnest(expressions=[explode_expression], alias="array_column(col, pos)", ordinality=True)
+                if expression.args.get("from") is not None:
+                    join = exp.Join(this=unnest, kind="CROSS")
+                    expression = expression.select("pos", "col").join(join)
                 else:
-                    continue
+                    expression = expression.select("pos", "col").from_(unnest)
+                continue
+
             elif isinstance(e, exp.Explode):
-                explode = e
-                to_remove = e
-                explode_expression = explode.args["this"]
+                unnested_column_name = "col"
+                explode_expression = e.args["this"]
+
+            elif isinstance(e, exp.Alias):
+                if not isinstance(e.args["this"], exp.Explode):
+                    continue
+                unnested_column_name = e.alias
+                explode_expression = e.args["this"].args["this"]
+
+            # This is not a (pos)explode expression
             else:
                 continue
 
-            array_column_name = "array_column"
-            unnested_column_name = explode_alias or "col"
-            unnest = exp.Unnest(expressions=[explode_expression], alias=f"{array_column_name}({unnested_column_name})")
-            join = exp.Join(this=unnest, kind="CROSS")
             # Remove the `explode()` expression from the select
-            expression.args["expressions"].remove(to_remove)
-            # Add an empty FROM expression so that there's always a FROM even if we don't select from a table,
-            # e.g. if the original expression is `select explode(sequence(...)))`
-            expression = expression.select(unnested_column_name).from_(expressions=[]).join(join)
+            expression.args["expressions"].remove(e)
+
+            # If the SELECT has a FROM, do a CROSS JOIN with the UNNEST,
+            # otherwise, just do SELECT ... FROM UNNEST
+            unnest = exp.Unnest(expressions=[explode_expression], alias=f"array_column({unnested_column_name})")
+            if expression.args.get("from") is not None:
+                join = exp.Join(this=unnest, kind="CROSS")
+                expression = expression.select(unnested_column_name).join(join)
+            else:
+                expression = expression.select(unnested_column_name).from_(unnest)
     return expression
 
 
 class DuneSQL(Trino):
     """The DuneSQL dialect is the dialect used to execute SQL queries on Dune's crypto data sets
 
     DuneSQL is the Trino dialect with slight modifications."""
```

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/table_replacements.py` & `dune_harmonizer-0.7.0/dune/harmonizer/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.6.0/dune/harmonizer/translate.py` & `dune_harmonizer-0.7.0/dune/harmonizer/translate.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.6.0/pyproject.toml` & `dune_harmonizer-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "dune-harmonizer"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-sqlglot = "^11.5.5"
+sqlglot = "^11.5.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 ruff = "^0.0.259"
 black = "^23.1.0"
 
 [build-system]
```

### Comparing `dune_harmonizer-0.6.0/PKG-INFO` & `dune_harmonizer-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dune-harmonizer
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sqlglot (>=11.5.5,<12.0.0)
+Requires-Dist: sqlglot (>=11.5.7,<12.0.0)
 Description-Content-Type: text/markdown
 
 # Harmonizer
 
 Harmonizer is a library we have developed at Dune to translate Dune queries from PostgreSQL and Spark SQL to DuneSQL.
 We currently use this library in our migration service in the app.
```

