# Comparing `tmp/ChatDocument-2023.4.25.9.49.22.tar.gz` & `tmp/ChatDocument-2023.4.25.9.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatDocument-2023.4.25.9.49.22.tar", last modified: Tue Apr 25 01:49:23 2023, max compression
+gzip compressed data, was "ChatDocument-2023.4.25.9.50.0.tar", last modified: Tue Apr 25 01:50:00 2023, max compression
```

## Comparing `ChatDocument-2023.4.25.9.49.22.tar` & `ChatDocument-2023.4.25.9.50.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.009802 ChatDocument-2023.4.25.9.49.22/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatDocument-2023.4.25.9.49.22/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:22.998665 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1653 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-04-25 01:49:23.009645 ChatDocument-2023.4.25.9.49.22/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1301 2023-04-25 01:20:39.000000 ChatDocument-2023.4.25.9.49.22/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/README.rst
--rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 ChatDocument-2023.4.25.9.49.22/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:22.999205 ChatDocument-2023.4.25.9.49.22/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.000361 ChatDocument-2023.4.25.9.49.22/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      342 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/ann4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)     2813 2023-04-25 01:22:30.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/crawler4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatDocument-2023.4.25.9.49.22/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1846 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/chatllm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.000722 ChatDocument-2023.4.25.9.49.22/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/chatllm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.001064 ChatDocument-2023.4.25.9.49.22/chatllm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatDocument-2023.4.25.9.49.22/chatllm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      284 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/chatllm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 ChatDocument-2023.4.25.9.49.22/chatllm/kb/kbqa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.001302 ChatDocument-2023.4.25.9.49.22/chatllm/knowledge_base/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 ChatDocument-2023.4.25.9.49.22/chatllm/knowledge_base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 ChatDocument-2023.4.25.9.49.22/chatllm/knowledge_base/lite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.001659 ChatDocument-2023.4.25.9.49.22/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatDocument-2023.4.25.9.49.22/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 ChatDocument-2023.4.25.9.49.22/chatllm/parse_utils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatDocument-2023.4.25.9.49.22/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/chatllm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.001915 ChatDocument-2023.4.25.9.49.22/chatllm/textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 ChatDocument-2023.4.25.9.49.22/chatllm/textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 ChatDocument-2023.4.25.9.49.22/chatllm/textsplitter/chinese_text_splitter.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.002166 ChatDocument-2023.4.25.9.49.22/chatllm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatDocument-2023.4.25.9.49.22/chatllm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/chatllm/uis/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 ChatDocument-2023.4.25.9.49.22/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.002647 ChatDocument-2023.4.25.9.49.22/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.004934 ChatDocument-2023.4.25.9.49.22/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatDocument-2023.4.25.9.49.22/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatDocument-2023.4.25.9.49.22/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.49.22/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.49.22/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.49.22/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.49.22/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.009181 ChatDocument-2023.4.25.9.49.22/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1331 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.49.22/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatDocument-2023.4.25.9.49.22/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatDocument-2023.4.25.9.49.22/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatDocument-2023.4.25.9.49.22/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-25 01:49:23.009873 ChatDocument-2023.4.25.9.49.22/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1556 2023-04-25 01:49:22.000000 ChatDocument-2023.4.25.9.49.22/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:49:23.009419 ChatDocument-2023.4.25.9.49.22/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.49.22/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.561720 ChatDocument-2023.4.25.9.50.0/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatDocument-2023.4.25.9.50.0/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.549877 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1653 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-25 01:50:00.561554 ChatDocument-2023.4.25.9.50.0/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1301 2023-04-25 01:20:39.000000 ChatDocument-2023.4.25.9.50.0/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/README.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 ChatDocument-2023.4.25.9.50.0/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.550419 ChatDocument-2023.4.25.9.50.0/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.551671 ChatDocument-2023.4.25.9.50.0/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/ann4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2813 2023-04-25 01:22:30.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-25 01:23:41.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/crawler4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatDocument-2023.4.25.9.50.0/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1846 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/chatllm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.552083 ChatDocument-2023.4.25.9.50.0/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/chatllm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.552490 ChatDocument-2023.4.25.9.50.0/chatllm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatDocument-2023.4.25.9.50.0/chatllm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/chatllm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 ChatDocument-2023.4.25.9.50.0/chatllm/kb/kbqa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.552746 ChatDocument-2023.4.25.9.50.0/chatllm/knowledge_base/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 ChatDocument-2023.4.25.9.50.0/chatllm/knowledge_base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 ChatDocument-2023.4.25.9.50.0/chatllm/knowledge_base/lite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.553140 ChatDocument-2023.4.25.9.50.0/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatDocument-2023.4.25.9.50.0/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 ChatDocument-2023.4.25.9.50.0/chatllm/parse_utils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatDocument-2023.4.25.9.50.0/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/chatllm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.553411 ChatDocument-2023.4.25.9.50.0/chatllm/textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 ChatDocument-2023.4.25.9.50.0/chatllm/textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 ChatDocument-2023.4.25.9.50.0/chatllm/textsplitter/chinese_text_splitter.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.553674 ChatDocument-2023.4.25.9.50.0/chatllm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatDocument-2023.4.25.9.50.0/chatllm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/chatllm/uis/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 ChatDocument-2023.4.25.9.50.0/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.554170 ChatDocument-2023.4.25.9.50.0/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.556803 ChatDocument-2023.4.25.9.50.0/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatDocument-2023.4.25.9.50.0/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatDocument-2023.4.25.9.50.0/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.50.0/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.50.0/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.50.0/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatDocument-2023.4.25.9.50.0/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.561044 ChatDocument-2023.4.25.9.50.0/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1331 2023-04-25 01:19:43.000000 ChatDocument-2023.4.25.9.50.0/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatDocument-2023.4.25.9.50.0/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatDocument-2023.4.25.9.50.0/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatDocument-2023.4.25.9.50.0/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-25 01:50:00.561776 ChatDocument-2023.4.25.9.50.0/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1556 2023-04-25 01:50:00.000000 ChatDocument-2023.4.25.9.50.0/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:50:00.561299 ChatDocument-2023.4.25.9.50.0/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatDocument-2023.4.25.9.50.0/tox.ini
```

### Comparing `ChatDocument-2023.4.25.9.49.22/.gitignore` & `ChatDocument-2023.4.25.9.50.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/.travis.yml` & `ChatDocument-2023.4.25.9.50.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/CONTRIBUTING.rst` & `ChatDocument-2023.4.25.9.50.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/PKG-INFO` & `ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatDocument
-Version: 2023.4.25.9.49.22
+Version: 2023.4.25.9.50.0
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatDocument-2023.4.25.9.49.22/ChatDocument.egg-info/SOURCES.txt` & `ChatDocument-2023.4.25.9.50.0/ChatDocument.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/LICENSE` & `ChatDocument-2023.4.25.9.50.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/Makefile` & `ChatDocument-2023.4.25.9.50.0/Makefile`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/PKG-INFO` & `ChatDocument-2023.4.25.9.50.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatDocument
-Version: 2023.4.25.9.49.22
+Version: 2023.4.25.9.50.0
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatDocument-2023.4.25.9.49.22/README.md` & `ChatDocument-2023.4.25.9.50.0/README.md`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/README.rst` & `ChatDocument-2023.4.25.9.50.0/README.rst`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/applications/Question2Answer.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/applications/ann4qa.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/applications/ann4qa.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/applications/chatbase.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/applications/crawler4qa.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/applications/crawler4qa.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/chatllm.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/clis/cli.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/kb/FaissANN.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/parse_utils/doc_embedding.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/parse_utils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/qa.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/qa.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/textsplitter/chinese_text_splitter.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/uis/gradio_ui.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/uis/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/chatllm/utils.py` & `ChatDocument-2023.4.25.9.50.0/chatllm/utils.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/data/医/500种中药现代研究.txt` & `ChatDocument-2023.4.25.9.50.0/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/data/医/古今医统大全.txt` & `ChatDocument-2023.4.25.9.50.0/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/data/姚明.txt` & `ChatDocument-2023.4.25.9.50.0/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/data/王治郅.txt` & `ChatDocument-2023.4.25.9.50.0/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/data/科比.txt` & `ChatDocument-2023.4.25.9.50.0/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/docs/Makefile` & `ChatDocument-2023.4.25.9.50.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/docs/README.md` & `ChatDocument-2023.4.25.9.50.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/docs/conf.py` & `ChatDocument-2023.4.25.9.50.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/docs/img.png` & `ChatDocument-2023.4.25.9.50.0/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/docs/installation.rst` & `ChatDocument-2023.4.25.9.50.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/docs/make.bat` & `ChatDocument-2023.4.25.9.50.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/setup.py` & `ChatDocument-2023.4.25.9.50.0/setup.py`

 * *Files identical despite different names*

### Comparing `ChatDocument-2023.4.25.9.49.22/tests/test_llm4gpt.py` & `ChatDocument-2023.4.25.9.50.0/tests/test_llm4gpt.py`

 * *Files identical despite different names*

