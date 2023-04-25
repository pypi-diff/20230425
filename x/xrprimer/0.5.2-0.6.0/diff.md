# Comparing `tmp/xrprimer-0.5.2.tar.gz` & `tmp/xrprimer-0.6.0-cp39-cp39-manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xrprimer-0.5.2.tar", last modified: Fri Aug 26 07:05:51 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

