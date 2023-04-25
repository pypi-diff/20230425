# Comparing `tmp/cobli-libi-0.0.1.tar.gz` & `tmp/cobli_libi-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobli-libi-0.0.1.tar", last modified: Tue Sep 14 19:49:43 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

