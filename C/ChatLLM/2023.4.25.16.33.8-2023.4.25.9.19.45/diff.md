# Comparing `tmp/ChatLLM-2023.4.25.16.33.8.tar.gz` & `tmp/ChatLLM-2023.4.25.9.19.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.25.16.33.8.tar", last modified: Tue Apr 25 08:33:08 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.25.9.19.45.tar", last modified: Tue Apr 25 01:19:46 2023, max compression
```

## Comparing `ChatLLM-2023.4.25.16.33.8.tar` & `ChatLLM-2023.4.25.9.19.45.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.609853 ChatLLM-2023.4.25.16.33.8/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.25.16.33.8/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.579282 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2128 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1532 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 08:33:08.000000 ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2128 2023-04-25 08:33:08.609709 ChatLLM-2023.4.25.16.33.8/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1312 2023-04-25 08:31:06.000000 ChatLLM-2023.4.25.16.33.8/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/README.rst
--rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 ChatLLM-2023.4.25.16.33.8/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.579644 ChatLLM-2023.4.25.16.33.8/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.581052 ChatLLM-2023.4.25.16.33.8/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/ann4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)     2773 2023-04-25 08:31:42.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      542 2023-04-25 08:23:38.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-25 01:23:41.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/crawler4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.25.16.33.8/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.581713 ChatLLM-2023.4.25.16.33.8/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      571 2023-04-25 02:29:53.000000 ChatLLM-2023.4.25.16.33.8/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1429 2023-04-25 08:29:49.000000 ChatLLM-2023.4.25.16.33.8/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.582768 ChatLLM-2023.4.25.16.33.8/chatllm/his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.25.16.33.8/chatllm/his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.25.16.33.8/chatllm/his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.25.16.33.8/chatllm/his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.25.16.33.8/chatllm/his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.583652 ChatLLM-2023.4.25.16.33.8/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.25.16.33.8/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 ChatLLM-2023.4.25.16.33.8/chatllm/parse_utils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.25.16.33.8/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3256 2023-04-25 08:17:51.000000 ChatLLM-2023.4.25.16.33.8/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.584296 ChatLLM-2023.4.25.16.33.8/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.25.16.33.8/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.16.33.8/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.25.16.33.8/chatllm/webui/nice_ui.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.588041 ChatLLM-2023.4.25.16.33.8/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.591793 ChatLLM-2023.4.25.16.33.8/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.25.16.33.8/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.25.16.33.8/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.16.33.8/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.16.33.8/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.16.33.8/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.25.16.33.8/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.16.33.8/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.609151 ChatLLM-2023.4.25.16.33.8/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1342 2023-04-25 08:31:06.000000 ChatLLM-2023.4.25.16.33.8/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.25.16.33.8/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatLLM-2023.4.25.16.33.8/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatLLM-2023.4.25.16.33.8/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.25.16.33.8/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-25 08:33:08.609915 ChatLLM-2023.4.25.16.33.8/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-04-25 02:27:49.000000 ChatLLM-2023.4.25.16.33.8/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 08:33:08.609473 ChatLLM-2023.4.25.16.33.8/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.16.33.8/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.062485 ChatLLM-2023.4.25.9.19.45/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.25.9.19.45/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.041945 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2137 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1551 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 01:19:45.000000 ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2137 2023-04-25 01:19:46.062634 ChatLLM-2023.4.25.9.19.45/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1320 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/README.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 ChatLLM-2023.4.25.9.19.45/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.042461 ChatLLM-2023.4.25.9.19.45/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.043570 ChatLLM-2023.4.25.9.19.45/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      333 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/ann4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2809 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/chat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/crawler4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.25.9.19.45/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1846 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.043984 ChatLLM-2023.4.25.9.19.45/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/chatllm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.044412 ChatLLM-2023.4.25.9.19.45/chatllm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      299 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 ChatLLM-2023.4.25.9.19.45/chatllm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.25.9.19.45/chatllm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.044840 ChatLLM-2023.4.25.9.19.45/chatllm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.25.9.19.45/chatllm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 ChatLLM-2023.4.25.9.19.45/chatllm/kb/kbqa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.045126 ChatLLM-2023.4.25.9.19.45/chatllm/knowledge_base/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 ChatLLM-2023.4.25.9.19.45/chatllm/knowledge_base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 ChatLLM-2023.4.25.9.19.45/chatllm/knowledge_base/lite.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.045406 ChatLLM-2023.4.25.9.19.45/chatllm/textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 ChatLLM-2023.4.25.9.19.45/chatllm/textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 ChatLLM-2023.4.25.9.19.45/chatllm/textsplitter/chinese_text_splitter.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.045663 ChatLLM-2023.4.25.9.19.45/chatllm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.25.9.19.45/chatllm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/chatllm/uis/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 ChatLLM-2023.4.25.9.19.45/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.046178 ChatLLM-2023.4.25.9.19.45/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.049967 ChatLLM-2023.4.25.9.19.45/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.25.9.19.45/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.25.9.19.45/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.9.19.45/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.9.19.45/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.9.19.45/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.25.9.19.45/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.062073 ChatLLM-2023.4.25.9.19.45/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1331 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.25.9.19.45/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatLLM-2023.4.25.9.19.45/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatLLM-2023.4.25.9.19.45/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-25 01:19:46.063025 ChatLLM-2023.4.25.9.19.45/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-04-25 01:19:43.000000 ChatLLM-2023.4.25.9.19.45/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 01:19:46.062344 ChatLLM-2023.4.25.9.19.45/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.25.9.19.45/tox.ini
```

### Comparing `ChatLLM-2023.4.25.16.33.8/.gitignore` & `ChatLLM-2023.4.25.9.19.45/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/.travis.yml` & `ChatLLM-2023.4.25.9.19.45/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/CONTRIBUTING.rst` & `ChatLLM-2023.4.25.9.19.45/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.25.16.33.8
+Version: 2023.4.25.9.19.45
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
-Keywords: chatllm
+Keywords: llm4chat
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -20,32 +20,32 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 
 
-<h1 align = "center">🔥ChatLLM🔥</h1>
+<h1 align = "center">🔥LLM4GPT 为大模型而生🔥</h1>
 
 ---
 
 # Install
 
 ```python
 pip install -U llm4gpt
 ```
 
 # [Docs](https://jie-yuan.github.io/llm4gpt/)
 
 # Usages
 
 ```python
-from chatllm.his._qa import QA
-from chatllm.his import FaissANN
-from chatllm.his._chatllm import ChatLLM
+from chatllm.qa import QA
+from chatllm.kb import FaissANN
+from chatllm.chatllm import ChatLLM
 from chatllm.utils import llm_load
 
 from meutils.pipe import *
 
 # 解析知识库
 texts = []
 metadatas = []
```

### Comparing `ChatLLM-2023.4.25.16.33.8/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.25.9.19.45/ChatLLM.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,53 +9,54 @@
 Makefile
 README.md
 README.rst
 TODO.md
 git_init.sh
 pypi.sh
 requirements.txt
-requirements_pdf.txt
+requirements_dev.txt
+setup.cfg
 setup.py
 tox.ini
 ChatLLM.egg-info/PKG-INFO
 ChatLLM.egg-info/SOURCES.txt
 ChatLLM.egg-info/dependency_links.txt
 ChatLLM.egg-info/entry_points.txt
 ChatLLM.egg-info/not-zip-safe
 ChatLLM.egg-info/requires.txt
 ChatLLM.egg-info/top_level.txt
 chatllm/__init__.py
-chatllm/embedding.py
+chatllm/chatllm.py
+chatllm/qa.py
 chatllm/utils.py
 chatllm/applications/Question2Answer.py
 chatllm/applications/__init__.py
 chatllm/applications/ann4qa.py
-chatllm/applications/chatbase.py
-chatllm/applications/chatdoc.py
+chatllm/applications/chat.py
 chatllm/applications/chatpdf.py
-chatllm/applications/chatweb.py
 chatllm/applications/crawler4qa.py
 chatllm/applications/pipeline.py
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
-chatllm/his/FaissANN.py
-chatllm/his/__init__.py
-chatllm/his/_chatllm.py
-chatllm/his/_qa.py
-chatllm/parse_utils/__init__.py
-chatllm/parse_utils/doc_embedding.py
-chatllm/parse_utils/doc_parse.py
-chatllm/webui/__init__.py
-chatllm/webui/gradio_ui.py
-chatllm/webui/nice_ui.py
+chatllm/docutils/__init__.py
+chatllm/docutils/doc_embedding.py
+chatllm/docutils/doc_parse.py
+chatllm/kb/FaissANN.py
+chatllm/kb/__init__.py
+chatllm/kb/kbqa.py
+chatllm/knowledge_base/__init__.py
+chatllm/knowledge_base/lite.py
+chatllm/textsplitter/__init__.py
+chatllm/textsplitter/chinese_text_splitter.py
+chatllm/uis/__init__.py
+chatllm/uis/gradio_ui.py
 data/姚明.txt
 data/王治郅.txt
 data/科比.txt
-data/财报.pdf
 data/马保国.txt
 data/医/500种中药现代研究.txt
 data/医/古今医统大全.txt
 docs/Makefile
 docs/README.md
 docs/_config.yml
 docs/authors.rst
```

### Comparing `ChatLLM-2023.4.25.16.33.8/LICENSE` & `ChatLLM-2023.4.25.9.19.45/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/Makefile` & `ChatLLM-2023.4.25.9.19.45/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/PKG-INFO` & `ChatLLM-2023.4.25.9.19.45/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.25.16.33.8
+Version: 2023.4.25.9.19.45
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
-Keywords: chatllm
+Keywords: llm4chat
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -20,32 +20,32 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 
 
-<h1 align = "center">🔥ChatLLM🔥</h1>
+<h1 align = "center">🔥LLM4GPT 为大模型而生🔥</h1>
 
 ---
 
 # Install
 
 ```python
 pip install -U llm4gpt
 ```
 
 # [Docs](https://jie-yuan.github.io/llm4gpt/)
 
 # Usages
 
 ```python
-from chatllm.his._qa import QA
-from chatllm.his import FaissANN
-from chatllm.his._chatllm import ChatLLM
+from chatllm.qa import QA
+from chatllm.kb import FaissANN
+from chatllm.chatllm import ChatLLM
 from chatllm.utils import llm_load
 
 from meutils.pipe import *
 
 # 解析知识库
 texts = []
 metadatas = []
```

### Comparing `ChatLLM-2023.4.25.16.33.8/README.md` & `ChatLLM-2023.4.25.9.19.45/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 
 
-<h1 align = "center">🔥ChatLLM🔥</h1>
+<h1 align = "center">🔥LLM4GPT 为大模型而生🔥</h1>
 
 ---
 
 # Install
 
 ```python
 pip install -U llm4gpt
 ```
 
 # [Docs](https://jie-yuan.github.io/llm4gpt/)
 
 # Usages
 
 ```python
-from chatllm.his._qa import QA
-from chatllm.his import FaissANN
-from chatllm.his._chatllm import ChatLLM
+from chatllm.qa import QA
+from chatllm.kb import FaissANN
+from chatllm.chatllm import ChatLLM
 from chatllm.utils import llm_load
 
 from meutils.pipe import *
 
 # 解析知识库
 texts = []
 metadatas = []
```

### Comparing `ChatLLM-2023.4.25.16.33.8/README.rst` & `ChatLLM-2023.4.25.9.19.45/README.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/applications/ann4qa.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/applications/ann4qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/applications/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 # @Software     : PyCharm
 # @Description  :
 import types
 from meutils.pipe import *
 from meutils.decorators import clear_cuda_cache
 
 
-class ChatBase(object):
+class Chat(object):
 
     def __init__(self, chat_func, prompt_template=None):
         self.chat_func = chat_func
-        self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
 
-        #
         self.history = []
         self.knowledge_base = None
 
+        self.prompt_template = prompt_template
+        if prompt_template is None:
+            self.prompt_template = self.default_document_prompt
+
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
 
+    @abstractmethod  # 重写
     def qa(self, query, knowledge_base='', **kwargs):
-        """可重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
-    def set_chat_kwargs(self, **kwargs):
-        self.chat_func = partial(self.chat_func, **kwargs)
-
     @clear_cuda_cache
     def _qa(self, query, knowledge_base='', max_turns=1):
         if knowledge_base:
             self.knowledge_base = knowledge_base
             query = self.prompt_template.format(context=knowledge_base, question=query)
 
         result = self.chat_func(query=query, history=self.history[-max_turns:])
@@ -63,19 +62,22 @@
             如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的相关信息"，不允许在答案中添加编造成分，答案请使用中文。
             已知内容: {context}
             问题: {question}
             """.strip()
 
         return prompt_template
 
+    def set_chat_kwargs(self, **kwargs):
+        self.chat_func = partial(self.chat_func, **kwargs)
+
 
 if __name__ == '__main__':
     from chatllm.utils import llm_load4chat
 
     chat_func = llm_load4chat(
         model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm",
         device='mps')
 
-    qa = ChatBase(chat_func=chat_func)
+    qa = Chat(chat_func=chat_func)
 
     for i, _ in qa(query='提取关键词', knowledge_base='我今天去听了周杰伦的演唱会'):
         print(i, flush=True)
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/applications/crawler4qa.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/applications/crawler4qa.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # @Software     : PyCharm
 # @Description  :
 
 
 from meutils.pipe import *
 from meutils.request_utils.crawler import Crawler
 
-from chatllm.applications import ChatBase
+from chatllm.applications import Chat
 
 
-class Crawler4QA(ChatBase):
+class Crawler4QA(Chat):
 
     def __init__(self, chat_func):
         super().__init__(chat_func)
 
     def qa(self, query,
            url="https://top.baidu.com/board?tab=realtime",
            xpath='//*[@id="sanRoot"]/main/div[2]/div/div[2]/div[*]/div[2]/a/div[1]//text()', **kwargs):
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/clis/cli.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/clis/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # @Description  : python meutils/clis/__init__.py
 
 
 import typer
 
 from meutils.pipe import *
 
-cli = typer.Typer(name="ChatLLM CLI")
+cli = typer.Typer(name="llm4gpt CLI")
 
 
 @cli.command(help="help")  # help会覆盖docstring
-def clitest(name: str = 'TEST'):
+def clitest(name: str='TEST'):
     """
 
     @param name: name
     @return:
     """
     typer.echo(f"Hello {name}")
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/embedding.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/docutils/doc_embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from sentence_transformers import SentenceTransformer
 from meutils.docarray_ import Document, DocumentArray
 
 
 # 增加 docarray v2
 # 增加 ann后端
-class SentenceEmbedding(object):
+class DocEmbedding(object):
     def __init__(self, model_name_or_path="shibing624/text2vec-base-chinese", device=None):
         """
             disk_cache()(DocEmbedding().encode)
         :param model_name_or_path:
         :param device:
         """
         self.st = SentenceTransformer(model_name_or_path, device)
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/his/FaissANN.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/his/_chatllm.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/chatllm.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
 
 if __name__ == '__main__':
     from chatllm.utils import llm_load
 
-    model, tokenizer = llm_load("/CHAT_MODEL/chatglm")
+    model, tokenizer = llm_load("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
     glm = ChatLLM()
     glm.chat_func = partial(model.chat, tokenizer=tokenizer)
     glm.chat_func = partial(model.stream_chat, tokenizer=tokenizer)
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/his/_qa.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # @Description  :
 
 from langchain.chains import RetrievalQA
 from langchain.prompts.prompt import PromptTemplate
 from langchain.vectorstores import FAISS
 
 # ME
-from chatllm.his._chatllm import ChatLLM
+from meutils.pipe import *
+from chatllm.chatllm import ChatLLM
 
 RetrievalQA.return_source_documents = True
 
 
 class QA(object):
     def __init__(self, chatllm: ChatLLM, faiss_ann: FAISS = None, document_prompt: PromptTemplate = None):
         """
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/utils.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,56 +4,18 @@
 # @File         : utils
 # @Time         : 2023/4/20 12:50
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 import torch
-from transformers import AutoTokenizer, AutoModel
+from transformers import AutoTokenizer, AutoModel, AutoConfig
 
 from meutils.pipe import *
 
-DEVICE = "cuda" if torch.cuda.is_available() else "mps" if torch.backends.mps.is_available() else "cpu"
-
-
-def textsplitter(text, window_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
-    return text.lower().split() | xjoin(sep) | xgroup(window_size, overlap_rate)
-
-
-def llm_load4chat(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
-    model, tokenizer = llm_load(model_name_or_path, device, **kwargs)
-    if stream:
-        return partial(model.stream_chat, tokenizer=tokenizer)
-    else:
-        return partial(model.chat, tokenizer=tokenizer)
-
-
-def llm_load(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, device_map: Optional[Dict[str, int]] = None,
-             **kwargs):
-    tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, trust_remote_code=True)
-    model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True, **kwargs)
-
-    if torch.cuda.is_available() and device.lower().startswith("cuda"):
-        # 根据当前设备GPU数量决定是否进行多卡部署
-        num_gpus = torch.cuda.device_count()
-        if num_gpus < 2 and device_map is None:
-            model = model.half().cuda()
-        else:
-            from accelerate import dispatch_model
-            # 可传入device_map自定义每张卡的部署情况
-            if device_map is None:
-                device_map = auto_configure_device_map(num_gpus)
-
-            model = dispatch_model(model, device_map=device_map).half().cuda()
-
-    else:
-        model = model.float().to(device)
-
-    return model.eval(), tokenizer
-
 
 def auto_configure_device_map(num_gpus: int) -> Dict[str, int]:
     # transformer.word_embeddings 占用1层
     # transformer.final_layernorm 和 lm_head 占用1层
     # transformer.layers 占用 28 层
     # 总共30层分配到num_gpus张卡上
     num_trans_layers = 28
@@ -77,9 +39,41 @@
         assert gpu_target < num_gpus
         device_map[f'transformer.layers.{i}'] = gpu_target
         used += 1
 
     return device_map
 
 
+def llm_load(model_name_or_path="THUDM/chatglm-6b", device='cpu', device_map: Optional[Dict[str, int]] = None,
+             **kwargs):
+    tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, trust_remote_code=True)
+    model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True, **kwargs)
+
+    if torch.cuda.is_available() and device.lower().startswith("cuda"):
+        # 根据当前设备GPU数量决定是否进行多卡部署
+        num_gpus = torch.cuda.device_count()
+        if num_gpus < 2 and device_map is None:
+            model = model.half().cuda()
+        else:
+            from accelerate import dispatch_model
+            # 可传入device_map自定义每张卡的部署情况
+            if device_map is None:
+                device_map = auto_configure_device_map(num_gpus)
+
+            model = dispatch_model(model, device_map=device_map).half().cuda()
+
+    else:
+        model = model.float().to(device)
+
+    return model.eval(), tokenizer
+
+
+def llm_load4chat(model_name_or_path="THUDM/chatglm-6b", device='cpu', stream=True, **kwargs):
+    model, tokenizer = llm_load(model_name_or_path, device, **kwargs)
+    if stream:
+        return partial(model.stream_chat, tokenizer=tokenizer)
+    else:
+        return partial(model.chat, tokenizer=tokenizer)
+
+
 if __name__ == '__main__':
     a = llm_load("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
```

### Comparing `ChatLLM-2023.4.25.16.33.8/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.25.9.19.45/chatllm/uis/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.25.9.19.45/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/data/医/古今医统大全.txt` & `ChatLLM-2023.4.25.9.19.45/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/data/姚明.txt` & `ChatLLM-2023.4.25.9.19.45/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/data/王治郅.txt` & `ChatLLM-2023.4.25.9.19.45/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/data/科比.txt` & `ChatLLM-2023.4.25.9.19.45/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/docs/Makefile` & `ChatLLM-2023.4.25.9.19.45/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/docs/README.md` & `ChatLLM-2023.4.25.9.19.45/docs/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 ```
 
 # [Docs](https://yuanjie-ai.github.io/LLM4GPT/)
 
 # Usages
 
 ```python
-from chatllm.his._qa import QA
+from chatllm.qa import QA
 from chatllm.utils import llm_load
-from chatllm.his._chatllm import ChatLLM
-from chatllm.his.FaissANN import FaissANN
+from chatllm.chatllm import ChatLLM
+from chatllm.kb.FaissANN import FaissANN
 
 from meutils.pipe import *
 
 # 解析知识库
 texts = []
 metadatas = []
 for p in Path('data').glob('*.txt'):
```

### Comparing `ChatLLM-2023.4.25.16.33.8/docs/conf.py` & `ChatLLM-2023.4.25.9.19.45/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/docs/img.png` & `ChatLLM-2023.4.25.9.19.45/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/docs/installation.rst` & `ChatLLM-2023.4.25.9.19.45/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/docs/make.bat` & `ChatLLM-2023.4.25.9.19.45/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.25.16.33.8/setup.py` & `ChatLLM-2023.4.25.9.19.45/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,16 @@
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
-    keywords='chatllm',
+    keywords='llm4chat',
     name='ChatLLM',
-    # name='ChatSearch', # 抢占包
-
     packages=find_packages(include=['chatllm', 'llm.*']),
 
     test_suite='tests',
     url='https://github.com/yuanjie-ai/llm4gpt',
     version=version, # '0.0.0',
     zip_safe=False,
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ChatLLM-2023.4.25.16.33.8/tests/test_llm4gpt.py` & `ChatLLM-2023.4.25.9.19.45/tests/test_llm4gpt.py`

 * *Files identical despite different names*

