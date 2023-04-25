# Comparing `tmp/flet2-0.0.0.1.tar.gz` & `tmp/flet2-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet2-0.0.0.1.tar", last modified: Tue Apr 25 13:16:26 2023, max compression
+gzip compressed data, was "flet2-0.0.1.tar", last modified: Tue Apr 25 13:18:40 2023, max compression
```

## Comparing `flet2-0.0.0.1.tar` & `flet2-0.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 flet2-0.0.0.1/LICENSE
--rw-r--r--   0        0        0      124 2023-04-25 13:15:54.966697 flet2-0.0.0.1/flet2.py
--rw-r--r--   0        0        0      322 2023-04-25 13:15:54.966697 flet2-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0      170 1970-01-01 00:00:00.000000 flet2-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10943 2023-04-25 13:18:06.439303 flet2-0.0.1/LICENSE
+-rw-r--r--   0        0        0      124 2023-04-25 13:15:54.966697 flet2-0.0.1/flet2.py
+-rw-r--r--   0        0        0      312 2023-04-25 13:18:15.927340 flet2-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      160 1970-01-01 00:00:00.000000 flet2-0.0.1/PKG-INFO
```

### Comparing `flet2-0.0.0.1/LICENSE` & `flet2-0.0.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
    
 
-   Copyright [2023] [许灿标]
+   Copyright [2023] [x]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

