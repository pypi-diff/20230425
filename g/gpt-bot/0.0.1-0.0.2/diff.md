# Comparing `tmp/gpt_bot-0.0.1-py3-none-any.whl.zip` & `tmp/gpt_bot-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4680 bytes, number of entries: 7
+Zip file size: 4676 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 05:12 gpt_bot/__init__.py
 -rw-r--r--  2.0 unx     4849 b- defN 23-Apr-25 05:12 gpt_bot/__main__.py
 -rw-r--r--  2.0 unx     2318 b- defN 23-Apr-22 13:21 gpt_bot/record.py
--rw-r--r--  2.0 unx     1087 b- defN 23-Apr-25 05:34 gpt_bot-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 05:34 gpt_bot-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-25 05:34 gpt_bot-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      520 b- defN 23-Apr-25 05:34 gpt_bot-0.0.1.dist-info/RECORD
-7 files, 8874 bytes uncompressed, 3760 bytes compressed:  57.6%
+-rw-r--r--  2.0 unx     1079 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      520 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/RECORD
+7 files, 8866 bytes uncompressed, 3756 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gpt_bot/__main__.py
 Comment: 
 
 Filename: gpt_bot/record.py
 Comment: 
 
-Filename: gpt_bot-0.0.1.dist-info/METADATA
+Filename: gpt_bot-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gpt_bot-0.0.1.dist-info/WHEEL
+Filename: gpt_bot-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gpt_bot-0.0.1.dist-info/top_level.txt
+Filename: gpt_bot-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gpt_bot-0.0.1.dist-info/RECORD
+Filename: gpt_bot-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gpt_bot-0.0.1.dist-info/METADATA` & `gpt_bot-0.0.2.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: gpt-bot
-Version: 0.0.1
+Version: 0.0.2
 Summary: GPT Commandline interface bot
 Home-page: https://github.com/hzhangxyz/gpt-bot
 Author: Hao Zhang
 Author-email: zh970205@mail.ustc.edu.cn
 License: GPLv3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: fire
 Requires-Dist: numpy
 Requires-Dist: openai
 Requires-Dist: prompt-toolkit
 Requires-Dist: pyaudio
 Requires-Dist: tiktoken
 
-# gpt-cli-bot
+# gpt-bot
 
 A GPT Command line interface bot.
 
 This is only for gpt-3.5-turbo currently.
 You need to set `OPENAI_API_KEY` in environment variable.
 And maybe `OPENAI_PROXY` is also useful if you need proxy.
 
 ## Usage
 
-`python -m gpt_cli_bot` and enjoy.
+`python -m gpt_bot` and enjoy.
 
 ## Command
 
 - `/multiline`: toggle multiline input.
 - `/prompt`: change [system content](https://platform.openai.com/docs/guides/chat) during chatting.
 - `/rollback`: rollback the last conversation.
 - `/history`: show chat history.
```

