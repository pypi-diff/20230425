# Comparing `tmp/DownloadDMARCAttachmentsFromGmail-0.1.0.tar.gz` & `tmp/DownloadDMARCAttachmentsFromGmail-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DownloadDMARCAttachmentsFromGmail-0.1.0.tar", last modified: Mon Feb 13 07:16:08 2023, max compression
+gzip compressed data, was "DownloadDMARCAttachmentsFromGmail-0.2.0.tar", last modified: Tue Apr 25 10:25:27 2023, max compression
```

## Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0.tar` & `DownloadDMARCAttachmentsFromGmail-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 07:16:08.605749 DownloadDMARCAttachmentsFromGmail-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 07:16:08.605749 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-02-13 07:16:08.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-13 07:16:08.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 07:16:08.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-13 07:16:08.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-13 07:16:08.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-13 07:16:08.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 07:16:08.605749 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/GmailAuth.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/GmailLabelQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-02-13 07:16:08.605749 DownloadDMARCAttachmentsFromGmail-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 07:16:08.605749 DownloadDMARCAttachmentsFromGmail-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 07:16:08.605749 DownloadDMARCAttachmentsFromGmail-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-13 07:15:40.000000 DownloadDMARCAttachmentsFromGmail-0.1.0/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:27.238551 DownloadDMARCAttachmentsFromGmail-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:27.234551 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 10:25:27.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-25 10:25:27.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:25:27.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 10:25:27.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-25 10:25:27.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 10:25:27.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:27.238551 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/GmailAuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/GmailLabelQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 10:25:27.238551 DownloadDMARCAttachmentsFromGmail-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:25:27.238551 DownloadDMARCAttachmentsFromGmail-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:27.238551 DownloadDMARCAttachmentsFromGmail-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-25 10:25:01.000000 DownloadDMARCAttachmentsFromGmail-0.2.0/tests/test_all.py
```

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/PKG-INFO` & `DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DownloadDMARCAttachmentsFromGmail
-Version: 0.1.0
+Version: 0.2.0
 Summary: Downloads DMARC attachments from Gmail
 Home-page: https://github.com/MozaicWorks/DownloadDMARCAttachmentsFromGmail
 Author: Mozaic Works
 Author-email: alex.bolboaca@mozaicworks.com
 Project-URL: Bug Reports, https://github.com/MozaicWorks/DownloadDMARCAttachmentsFromGmail/issues
 Project-URL: Source, https://github.com/MozaicWorks/DownloadDMARCAttachmentsFromGmail/
 Keywords: DMARC Gmail
@@ -20,14 +20,21 @@
 
 # Download DMARC Attachments From Gmail
 
 ## Description
 
 A tool to download DMARC from Gmail email attachments. Consider it under development, so use with care. Feedback and PRs are welcome!
 
+## Installation
+
+```bash
+pip3 install DownloadDMARCAttachmentsFromGmail
+DownloadDMARCFilesFromGmail --help
+```
+
 ## How To Use
 
 First, you need to give the tool access to your Gmail account through the API. Here's how to do it for a workspace account:
 
 * Access [https://console.cloud.google.com/](https://console.cloud.google.com/)
 * Create a new project, for example named "DownloadDMARCAttachments"
 * Select the newly created project
@@ -80,15 +87,15 @@
 
 * Make sure you have python 3.10
 * Install [pipenv](https://pipenv.pypa.io/en/latest/#install-pipenv-today)
 
 With default arguments, i.e. `--labelName DMARC --processedLabelName PROCESSED_DMARC`
 
 ```bash
-make install
+make install-dev
 make run
 ```
 
 To pass arguments:
 
 ```bash
 make run args="--labelName dmarc --processedLabelName processed-dmarc"
```

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/SOURCES.txt` & `DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCAttachmentsFromGmail.egg-info/requires.txt` & `DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCAttachmentsFromGmail.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/GmailAuth.py` & `DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/GmailAuth.py`

 * *Files identical despite different names*

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/GmailLabelQuery.py` & `DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/GmailLabelQuery.py`

 * *Files identical despite different names*

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/DownloadDMARCFilesFromGmail/download.py` & `DownloadDMARCAttachmentsFromGmail-0.2.0/DownloadDMARCFilesFromGmail/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
 import sys
 import os
 
+import filetype
+
 from DownloadDMARCFilesFromGmail.GmailAuth import GmailAuth
 from DownloadDMARCFilesFromGmail.GmailLabelQuery import GmailLabelQuery
 
 
 def main():
     parser = argparse.ArgumentParser(
         description='Download DMARC attachments from your Gmail account. '
@@ -62,16 +64,17 @@
     createDownloadPath(downloadPath)
 
     for message in messages:
         try:
             processMessage(
                 service, message["id"], labelId, replaceWithLabelId, downloadPath
             )
-        except Exception:
+        except Exception as e:
             print("Error at message {message}".format(message=message))
+            print(repr(e))
 
 
 def processMessage(service, messageId, labelId, replaceWithLabelId, downloadPath):
     downloadAttachment(service, messageId, downloadPath)
     markMessageAsProcessed(service, messageId, labelId, replaceWithLabelId)
 
 
@@ -112,16 +115,18 @@
     return result.get("messages", [])
 
 
 def downloadAttachment(service, messageId, downloadPath):
     import base64
 
     message = service.users().messages().get(userId="me", id=messageId).execute()
-    if message["payload"]["filename"]:
+    if "filename" in message["payload"] and "parts" not in message["payload"]:
         fileName = message["payload"]["filename"]
+        if not fileName:
+            fileName = f"noname-{messageId}"
         print("Processing file {fileName}".format(fileName=fileName))
         attachmentId = message["payload"]["body"]["attachmentId"]
     else:
         part = next(
             it
             for it in message["payload"]["parts"]
             if it["mimeType"] == "application/octet-stream"
@@ -142,13 +147,20 @@
     data = attachment['data']
 
     file_data = base64.urlsafe_b64decode(data.encode('UTF-8'))
 
     filePath = os.path.join(downloadPath, fileName)
     with open(filePath, 'wb') as f:
         f.write(file_data)
+    ext = os.path.splitext(filePath)[1]
+    if not ext:
+        print(f"Determining file extension for {fileName}")
+        kind = filetype.guess(filePath)
+        fileName = f"{fileName}.{kind.extension}"
+        newFilePath = os.path.join(downloadPath, fileName)
+        os.rename(filePath, newFilePath)
 
     print("File {fileName} written".format(fileName=fileName))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/LICENSE` & `DownloadDMARCAttachmentsFromGmail-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/PKG-INFO` & `DownloadDMARCAttachmentsFromGmail-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DownloadDMARCAttachmentsFromGmail
-Version: 0.1.0
+Version: 0.2.0
 Summary: Downloads DMARC attachments from Gmail
 Home-page: https://github.com/MozaicWorks/DownloadDMARCAttachmentsFromGmail
 Author: Mozaic Works
 Author-email: alex.bolboaca@mozaicworks.com
 Project-URL: Bug Reports, https://github.com/MozaicWorks/DownloadDMARCAttachmentsFromGmail/issues
 Project-URL: Source, https://github.com/MozaicWorks/DownloadDMARCAttachmentsFromGmail/
 Keywords: DMARC Gmail
@@ -20,14 +20,21 @@
 
 # Download DMARC Attachments From Gmail
 
 ## Description
 
 A tool to download DMARC from Gmail email attachments. Consider it under development, so use with care. Feedback and PRs are welcome!
 
+## Installation
+
+```bash
+pip3 install DownloadDMARCAttachmentsFromGmail
+DownloadDMARCFilesFromGmail --help
+```
+
 ## How To Use
 
 First, you need to give the tool access to your Gmail account through the API. Here's how to do it for a workspace account:
 
 * Access [https://console.cloud.google.com/](https://console.cloud.google.com/)
 * Create a new project, for example named "DownloadDMARCAttachments"
 * Select the newly created project
@@ -80,15 +87,15 @@
 
 * Make sure you have python 3.10
 * Install [pipenv](https://pipenv.pypa.io/en/latest/#install-pipenv-today)
 
 With default arguments, i.e. `--labelName DMARC --processedLabelName PROCESSED_DMARC`
 
 ```bash
-make install
+make install-dev
 make run
 ```
 
 To pass arguments:
 
 ```bash
 make run args="--labelName dmarc --processedLabelName processed-dmarc"
```

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/README.md` & `DownloadDMARCAttachmentsFromGmail-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Download DMARC Attachments From Gmail
 
 ## Description
 
 A tool to download DMARC from Gmail email attachments. Consider it under development, so use with care. Feedback and PRs are welcome!
 
+## Installation
+
+```bash
+pip3 install DownloadDMARCAttachmentsFromGmail
+DownloadDMARCFilesFromGmail --help
+```
+
 ## How To Use
 
 First, you need to give the tool access to your Gmail account through the API. Here's how to do it for a workspace account:
 
 * Access [https://console.cloud.google.com/](https://console.cloud.google.com/)
 * Create a new project, for example named "DownloadDMARCAttachments"
 * Select the newly created project
@@ -60,15 +67,15 @@
 
 * Make sure you have python 3.10
 * Install [pipenv](https://pipenv.pypa.io/en/latest/#install-pipenv-today)
 
 With default arguments, i.e. `--labelName DMARC --processedLabelName PROCESSED_DMARC`
 
 ```bash
-make install
+make install-dev
 make run
 ```
 
 To pass arguments:
 
 ```bash
 make run args="--labelName dmarc --processedLabelName processed-dmarc"
```

### Comparing `DownloadDMARCAttachmentsFromGmail-0.1.0/setup.py` & `DownloadDMARCAttachmentsFromGmail-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_description = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="DownloadDMARCAttachmentsFromGmail",  # Required
-    version="0.1.0",  # Required
+    version="0.2.0",  # Required
     description="Downloads DMARC attachments from Gmail",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
```

