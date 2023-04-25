# Comparing `tmp/animethemes-batch-encoder-1.0.1.tar.gz` & `tmp/animethemes-batch-encoder-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\animethemes-batch-encoder-1.0.1.tar", last modified: Mon Oct 26 05:06:27 2020, max compression
+gzip compressed data, was "animethemes-batch-encoder-1.1.tar", last modified: Tue Apr 25 03:56:26 2023, max compression
```

## Comparing `animethemes-batch-encoder-1.0.1.tar` & `animethemes-batch-encoder-1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2020-10-26 05:06:27.813158 animethemes-batch-encoder-1.0.1/
--rw-rw-rw-   0        0        0     4544 2020-10-26 05:06:27.813158 animethemes-batch-encoder-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3090 2020-10-26 05:03:36.000000 animethemes-batch-encoder-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2020-10-26 05:06:27.719431 animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     4544 2020-10-26 05:06:27.000000 animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2020-10-26 05:06:27.000000 animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-26 05:06:27.000000 animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2020-10-26 05:06:27.000000 animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2020-10-26 05:06:27.000000 animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-10-26 05:06:27.813158 animethemes-batch-encoder-1.0.1/batch_encoder/
--rw-rw-rw-   0        0        0        0 2020-10-22 22:58:23.000000 animethemes-batch-encoder-1.0.1/batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     6132 2020-10-26 04:36:38.000000 animethemes-batch-encoder-1.0.1/batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2020-10-22 23:13:09.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2020-10-22 23:26:02.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    10458 2020-10-22 23:37:34.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     2849 2020-10-22 23:54:25.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     2527 2020-10-22 23:25:54.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      711 2020-10-22 23:47:59.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     5615 2020-10-22 23:52:18.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6593 2020-10-22 23:46:21.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2020-10-22 23:57:03.000000 animethemes-batch-encoder-1.0.1/batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2020-10-26 05:06:27.813158 animethemes-batch-encoder-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1096 2020-10-26 05:05:13.000000 animethemes-batch-encoder-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:56:26.935955 animethemes-batch-encoder-1.1/
+-rw-rw-rw-   0        0        0     1088 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/LICENSE
+-rw-rw-rw-   0        0        0     4216 2023-04-25 03:56:26.934953 animethemes-batch-encoder-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3313 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 03:56:26.927863 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     4216 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 03:56:26.933954 animethemes-batch-encoder-1.1/batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     6340 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    12926 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     3434 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     2527 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      711 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     5615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6593 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:56:26.935955 animethemes-batch-encoder-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/setup.py
```

### Comparing `animethemes-batch-encoder-1.0.1/PKG-INFO` & `animethemes-batch-encoder-1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 Metadata-Version: 2.1
 Name: animethemes-batch-encoder
-Version: 1.0.1
+Version: 1.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
-Author: paranarimasu
-Author-email: paranarimasu@gmail.com
-License: UNKNOWN
-Description: ### Description
-        
-        Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
-        
-        Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
-        
-        Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
-        
-        ### Install
-        
-        **Requirements:**
-        
-        * FFmpeg
-        * Python >= 3.6
-        
-        **Install:**
-        
-            pip install animethemes-batch-encoder
-        
-        ### Usage
-        
-                python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
-        
-        **Mode**
-        
-        `--mode 1` generates commands from input files in the current directory.
-        
-        The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
-        
-        `--mode 2` executes commands from file in the current directory line-by-line.
-        
-        By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
-        
-        `--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
-        
-        The `--file` argument will be ignored in this case.
-        
-        **File**
-        
-        The file that commands are written to or read from.
-        
-        By default, the program will write to or read from `commands.txt` in the current directory.
-        
-        **Config File**
-        
-        The configuration file in which our encoding properties are defined.
-        
-        By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
-        
-        Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
-        
-        **Encoding Properties**
-        
-        `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
-        
-        `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
-        
-        Available bitrate control modes are:
-        
-        * `CBR` Constant Bitrate Mode
-        * `VBR` Variable Bitrate Mode
-        * `CQ` Constrained Quality Mode
-        
-        `CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
-        
-        `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing.
-        
-        `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
-        
-        **Logging**
-        
-        Determines the level of the logging for the program.
-        
-        `--loglevel error` will only output error messages.
-        
-        `--loglevel info` will output error messages and script progression info messages.
-        
-        `--loglevel debug` will output all messages, including variable dumps.
-        
-Platform: UNKNOWN
+Author: AnimeThemes
+Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Description
+
+Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
+
+Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
+
+Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
+
+### Install
+
+**Requirements:**
+
+* FFmpeg
+* Python >= 3.6
+
+**Install:**
+
+    pip install animethemes-batch-encoder
+
+### Usage
+
+        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+
+**Mode**
+
+`--mode 1` generates commands from input files in the current directory.
+
+The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
+
+`--mode 2` executes commands from file in the current directory line-by-line.
+
+By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
+
+`--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
+
+The `--file` argument will be ignored in this case.
+
+**File**
+
+The file that commands are written to or read from.
+
+By default, the program will write to or read from `commands.txt` in the current directory.
+
+**Config File**
+
+The configuration file in which our encoding properties are defined.
+
+By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
+
+Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+
+**Encoding Properties**
+
+`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
+
+`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
+
+Available bitrate control modes are:
+
+* `CBR` Constant Bitrate Mode
+* `VBR` Variable Bitrate Mode
+* `CQ` Constrained Quality Mode
+
+`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
+
+`Threads` is the number of threads used to encode. Default is 4.
+
+`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
+
+`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
+
+`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
+
+**Logging**
+
+Determines the level of the logging for the program.
+
+`--loglevel error` will only output error messages.
+
+`--loglevel info` will output error messages and script progression info messages.
+
+`--loglevel debug` will output all messages, including variable dumps.
```

### Comparing `animethemes-batch-encoder-1.0.1/README.md` & `animethemes-batch-encoder-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,19 @@
 
 * `CBR` Constant Bitrate Mode
 * `VBR` Variable Bitrate Mode
 * `CQ` Constrained Quality Mode
 
 `CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
 
-`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing.
+`Threads` is the number of threads used to encode. Default is 4.
+
+`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
+
+`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/PKG-INFO` & `animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 Metadata-Version: 2.1
 Name: animethemes-batch-encoder
-Version: 1.0.1
+Version: 1.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
-Author: paranarimasu
-Author-email: paranarimasu@gmail.com
-License: UNKNOWN
-Description: ### Description
-        
-        Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
-        
-        Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
-        
-        Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
-        
-        ### Install
-        
-        **Requirements:**
-        
-        * FFmpeg
-        * Python >= 3.6
-        
-        **Install:**
-        
-            pip install animethemes-batch-encoder
-        
-        ### Usage
-        
-                python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
-        
-        **Mode**
-        
-        `--mode 1` generates commands from input files in the current directory.
-        
-        The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
-        
-        `--mode 2` executes commands from file in the current directory line-by-line.
-        
-        By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
-        
-        `--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
-        
-        The `--file` argument will be ignored in this case.
-        
-        **File**
-        
-        The file that commands are written to or read from.
-        
-        By default, the program will write to or read from `commands.txt` in the current directory.
-        
-        **Config File**
-        
-        The configuration file in which our encoding properties are defined.
-        
-        By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
-        
-        Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
-        
-        **Encoding Properties**
-        
-        `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
-        
-        `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
-        
-        Available bitrate control modes are:
-        
-        * `CBR` Constant Bitrate Mode
-        * `VBR` Variable Bitrate Mode
-        * `CQ` Constrained Quality Mode
-        
-        `CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
-        
-        `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing.
-        
-        `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
-        
-        **Logging**
-        
-        Determines the level of the logging for the program.
-        
-        `--loglevel error` will only output error messages.
-        
-        `--loglevel info` will output error messages and script progression info messages.
-        
-        `--loglevel debug` will output all messages, including variable dumps.
-        
-Platform: UNKNOWN
+Author: AnimeThemes
+Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Description
+
+Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
+
+Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
+
+Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
+
+### Install
+
+**Requirements:**
+
+* FFmpeg
+* Python >= 3.6
+
+**Install:**
+
+    pip install animethemes-batch-encoder
+
+### Usage
+
+        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+
+**Mode**
+
+`--mode 1` generates commands from input files in the current directory.
+
+The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
+
+`--mode 2` executes commands from file in the current directory line-by-line.
+
+By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
+
+`--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
+
+The `--file` argument will be ignored in this case.
+
+**File**
+
+The file that commands are written to or read from.
+
+By default, the program will write to or read from `commands.txt` in the current directory.
+
+**Config File**
+
+The configuration file in which our encoding properties are defined.
+
+By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
+
+Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+
+**Encoding Properties**
+
+`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
+
+`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
+
+Available bitrate control modes are:
+
+* `CBR` Constant Bitrate Mode
+* `VBR` Variable Bitrate Mode
+* `CQ` Constrained Quality Mode
+
+`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
+
+`Threads` is the number of threads used to encode. Default is 4.
+
+`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
+
+`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
+
+`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
+
+**Logging**
+
+Determines the level of the logging for the program.
+
+`--loglevel error` will only output error messages.
+
+`--loglevel info` will output error messages and script progression info messages.
+
+`--loglevel debug` will output all messages, including variable dumps.
```

### Comparing `animethemes-batch-encoder-1.0.1/animethemes_batch_encoder.egg-info/SOURCES.txt` & `animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 animethemes_batch_encoder.egg-info/PKG-INFO
 animethemes_batch_encoder.egg-info/SOURCES.txt
 animethemes_batch_encoder.egg-info/dependency_links.txt
 animethemes_batch_encoder.egg-info/requires.txt
 animethemes_batch_encoder.egg-info/top_level.txt
```

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/__main__.py` & `animethemes-batch-encoder-1.1/batch_encoder/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     config = configparser.ConfigParser()
     dirs = AppDirs('batch_encoder', 'AnimeThemes')
     config_file = os.path.join(dirs.user_config_dir, args.configfile)
     if not os.path.exists(config_file):
         config['Encoding'] = {EncodingConfig.config_allowed_filetypes: EncodingConfig.default_allowed_filetypes,
                               EncodingConfig.config_encoding_modes: EncodingConfig.default_encoding_modes,
                               EncodingConfig.config_crfs: EncodingConfig.default_crfs,
+                              EncodingConfig.config_threads: EncodingConfig.default_threads,
+                              EncodingConfig.config_limit_size_enable: EncodingConfig.default_limit_size_enable,
                               EncodingConfig.config_include_unfiltered: EncodingConfig.default_include_unfiltered,
                               EncodingConfig.config_default_video_stream: '',
                               EncodingConfig.config_default_audio_stream: ''}
         config['VideoFilters'] = EncodingConfig.default_video_filters
 
         os.makedirs(os.path.dirname(config_file), exist_ok=True)
         with open(config_file, 'w', encoding='utf8') as f:
```

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_bitrate_mode.py` & `animethemes-batch-encoder-1.1/batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_colorspace.py` & `animethemes-batch-encoder-1.1/batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_encode_webm.py` & `animethemes-batch-encoder-1.1/batch_encoder/_encode_webm.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,37 +78,62 @@
         elif resolution >= 720:
             return '4200k'
         elif resolution >= 576:
             return '3700k'
         else:
             return '3200k'
 
+    # Limiting file size based on resolution and duration
+    def get_limit_file_size(self, video_filters=''):
+        source_file_duration = float(self.source_file.file_format['format']['duration'])
+
+        start_time = string_to_seconds(self.seek.ss) if self.seek.ss else 0
+        end_time = string_to_seconds(self.seek.to) if self.seek.to else source_file_duration
+        duration = end_time - start_time
+
+        for filter in video_filters.split(','):
+            if 'scale=-1:' in filter:
+                resolution = int(filter.split(':')[1])
+                break
+            else:
+                resolution = int(self.source_file.video_format['streams'][0]['height'])
+        
+        logging.debug(f'[EncodeWebm.get_limit_file_size] resolution: \'{resolution}\'')
+
+        max_allowed_bitrate = resolution * 6100 + 475000
+        max_allowed_size = max_allowed_bitrate * duration
+        limit_size = max_allowed_size / 8
+
+        return str(round(limit_size))
+
     # First-pass encode
-    def get_first_pass(self, encoding_mode, crf=None):
+    def get_first_pass(self, encoding_mode, crf=None, threads=4):
         return f'ffmpeg {self.seek.get_seek_string()} ' \
                f'-pass 1 -passlogfile {self.seek.output_name} ' \
                f'-map 0:v:{self.source_file.selected_video_stream} ' \
                f'-map 0:a:{self.source_file.selected_audio_stream} ' \
                f'-c:v libvpx-vp9 ' \
                f'{encoding_mode.first_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
-               f'-cpu-used 4 -g {self.g} -threads 4 -tile-columns 6 -frame-parallel 0 -auto-alt-ref 1 ' \
+               f'-cpu-used 4 -g {self.g} -threads {threads} -tile-columns 6 -frame-parallel 0 -auto-alt-ref 1 ' \
                f'-lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p {self.colorspace.get_args()} -an -sn -f webm -y NUL'
 
     # Second-pass encode
-    def get_second_pass(self, encoding_mode, crf=None, video_filters='', webm_filename=''):
+    def get_second_pass(self, encoding_mode, crf=None, threads=4, video_filters='', limit_size_enable=True, webm_filename=''):
+        limit_size = '-fs ' + EncodeWebM.get_limit_file_size(self, video_filters=video_filters) + ' ' if limit_size_enable else ''
         return f'ffmpeg {self.seek.get_seek_string()} ' \
                f'-pass 2 -passlogfile {self.seek.output_name} ' \
                f'-map 0:v:{self.source_file.selected_video_stream} ' \
                f'-map 0:a:{self.source_file.selected_audio_stream} ' \
                f'-c:v libvpx-vp9 ' \
                f'{encoding_mode.second_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
-               f'-cpu-used 0 -g {self.g} -threads 4 {self.get_audio_filters()}{video_filters} -tile-columns 6 ' \
+               f'-cpu-used 0 -g {self.g} -threads {threads} {self.get_audio_filters()}{video_filters} -tile-columns 6 ' \
                f'-frame-parallel 0 -auto-alt-ref 1 -lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p ' \
                f'{self.colorspace.get_args()} ' \
                f'-c:a libopus -b:a {self.audio_bitrate} -ar 48k ' \
+               f'{limit_size}' \
                f'-map_metadata -1 -map_chapters -1 -sn -f webm -y {webm_filename}.webm'
 
     # Build audio filtergraph for encodes
     def get_audio_filters(self):
         audio_filters = []
         self.source_file.apply_audio_resampling(audio_filters)
         audio_filters.append(self.loudnorm_filter.get_normalization_filter())
@@ -151,54 +176,64 @@
             f'[EncodeWebm.get_commands] encoding_modes: \'{encoding_config.encoding_modes}\', '
             f'crfs: \'{encoding_config.crfs}\', '
             f'include_unfiltered: \'{encoding_config.include_unfiltered}\', '
             f'video_filters: \'{encoding_config.video_filters}\'')
 
         for encoding_mode in encoding_config.encoding_modes:
             if BitrateMode.CBR.name == encoding_mode.upper():
-                file_commands.append(self.get_first_pass(BitrateMode.CBR))
+                file_commands.append(self.get_first_pass(BitrateMode.CBR, threads=encoding_config.threads))
                 if encoding_config.include_unfiltered:
                     file_commands.append(self.get_second_pass(BitrateMode.CBR,
+                                                              threads=encoding_config.threads,
                                                               video_filters=EncodeWebM.get_video_filters(),
+                                                              limit_size_enable=encoding_config.limit_size_enable,
                                                               webm_filename=self.get_webm_filename(
                                                                   cbr_bitrate=self.cbr_bitrate)))
                 for filter_name, filter_value in encoding_config.video_filters:
                     file_commands.append(self.get_second_pass(BitrateMode.CBR,
+                                                              threads=encoding_config.threads,
                                                               video_filters=EncodeWebM.get_video_filters(
                                                                   config_filter=filter_value),
+                                                              limit_size_enable=encoding_config.limit_size_enable,
                                                               webm_filename=self.get_webm_filename(
                                                                   cbr_bitrate=self.cbr_bitrate,
                                                                   filter_name=filter_name)))
             elif BitrateMode.VBR.name == encoding_mode.upper():
                 for crf in encoding_config.crfs:
-                    file_commands.append(self.get_first_pass(BitrateMode.VBR, crf=crf))
+                    file_commands.append(self.get_first_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads))
                     if encoding_config.include_unfiltered:
                         file_commands.append(
-                            self.get_second_pass(BitrateMode.VBR, crf=crf, video_filters=EncodeWebM.get_video_filters(),
+                            self.get_second_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads, video_filters=EncodeWebM.get_video_filters(),
+                                                 limit_size_enable=encoding_config.limit_size_enable,
                                                  webm_filename=self.get_webm_filename(crf=crf)))
                     for filter_name, filter_value in encoding_config.video_filters:
                         file_commands.append(self.get_second_pass(BitrateMode.VBR, crf=crf,
+                                                                  threads=encoding_config.threads,
                                                                   video_filters=EncodeWebM.get_video_filters(
                                                                       config_filter=filter_value),
+                                                                  limit_size_enable=encoding_config.limit_size_enable,
                                                                   webm_filename=self.get_webm_filename(
                                                                       crf=crf,
                                                                       filter_name=filter_name)))
             elif BitrateMode.CQ.name == encoding_mode.upper():
                 for crf in encoding_config.crfs:
-                    file_commands.append(self.get_first_pass(BitrateMode.CQ, crf=crf))
+                    file_commands.append(self.get_first_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads))
                     if encoding_config.include_unfiltered:
                         file_commands.append(
-                            self.get_second_pass(BitrateMode.CQ, crf=crf, video_filters=self.get_video_filters(),
+                            self.get_second_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads, video_filters=self.get_video_filters(),
+                                                 limit_size_enable=encoding_config.limit_size_enable,
                                                  webm_filename=self.get_webm_filename(crf=crf,
                                                                                       cbr_bitrate=self.cbr_bitrate)))
                     for filter_name, filter_value in encoding_config.video_filters:
                         file_commands.append(self.get_second_pass(BitrateMode.CQ, crf=crf,
+                                                                  threads=encoding_config.threads,
                                                                   video_filters=EncodeWebM.get_video_filters(
                                                                       config_filter=filter_value),
+                                                                  limit_size_enable=encoding_config.limit_size_enable,
                                                                   webm_filename=self.get_webm_filename(
                                                                       crf=crf,
                                                                       cbr_bitrate=self.cbr_bitrate,
                                                                       filter_name=filter_name)))
 
         logging.debug(f'[EncodeWebm.get_commands] # of file_commands: \'{len(file_commands)}\'')
-
-        return file_commands
+        
+        return file_commands
```

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_encoding_config.py` & `animethemes-batch-encoder-1.1/batch_encoder/_encoding_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,55 +2,64 @@
 
 
 class EncodingConfig:
     # Config keys
     config_allowed_filetypes = 'AllowedFileTypes'
     config_encoding_modes = 'EncodingModes'
     config_crfs = 'CRFs'
+    config_threads = 'Threads'
+    config_limit_size_enable = 'LimitSizeEnable'
     config_include_unfiltered = 'IncludeUnfiltered'
 
     # Default Config keys
     config_default_video_stream = 'DefaultVideoStream'
     config_default_audio_stream = 'DefaultAudioStream'
 
     # Default config values
     default_allowed_filetypes = '.avi,.m2ts,.mkv,.mp4,.wmv'
     default_encoding_modes = f'{BitrateMode.VBR.name},{BitrateMode.CBR.name}'
     default_crfs = '12,15,18,21,24'
+    default_limit_size_enable = True
+    default_threads = '4'
     default_include_unfiltered = True
     default_video_filters = {'filtered': 'hqdn3d=0:0:3:3,gradfun,unsharp',
                              'lightdenoise': 'hqdn3d=0:0:3:3',
                              'heavydenoise': 'hqdn3d=1.5:1.5:6:6',
                              'unsharp': 'unsharp'}
 
-    def __init__(self, allowed_filetypes, encoding_modes, crfs, include_unfiltered, video_filters, default_video_stream,
+    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, include_unfiltered, video_filters, default_video_stream,
                  default_audio_stream):
         self.allowed_filetypes = allowed_filetypes
         self.encoding_modes = encoding_modes
         self.crfs = crfs
+        self.threads = threads
+        self.limit_size_enable = limit_size_enable
         self.include_unfiltered = include_unfiltered
         self.video_filters = video_filters
         self.default_video_stream = default_video_stream
         self.default_audio_stream = default_audio_stream
 
     @classmethod
     def from_config(cls, config):
         allowed_filetypes = config['Encoding'].get(EncodingConfig.config_allowed_filetypes,
                                                    EncodingConfig.default_allowed_filetypes).split(',')
         encoding_modes = config['Encoding'].get(EncodingConfig.config_encoding_modes,
                                                 EncodingConfig.default_encoding_modes).split(',')
         crfs = config['Encoding'].get(EncodingConfig.config_crfs, EncodingConfig.default_crfs).split(',')
+        threads = config['Encoding'].get(EncodingConfig.config_threads,
+                                         EncodingConfig.default_threads)
+        limit_size_enable = config.getboolean('Encoding', EncodingConfig.config_limit_size_enable, fallback=EncodingConfig.default_limit_size_enable)
         include_unfiltered = config.getboolean('Encoding', EncodingConfig.config_include_unfiltered,
                                                fallback=EncodingConfig.default_include_unfiltered)
         video_filters = config.items('VideoFilters', EncodingConfig.default_video_filters)
 
         default_video_stream = config['Encoding'].get(EncodingConfig.config_default_video_stream)
         default_audio_stream = config['Encoding'].get(EncodingConfig.config_default_audio_stream)
 
-        return cls(allowed_filetypes, encoding_modes, crfs, include_unfiltered, video_filters, default_video_stream,
+        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, include_unfiltered, video_filters, default_video_stream,
                    default_audio_stream)
 
     def get_default_stream(self, stream_type):
         if stream_type == 'video':
             return self.default_video_stream
         elif stream_type == 'audio':
             return self.default_audio_stream
```

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_loudnorm_filter.py` & `animethemes-batch-encoder-1.1/batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_seek.py` & `animethemes-batch-encoder-1.1/batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_seek_collector.py` & `animethemes-batch-encoder-1.1/batch_encoder/_seek_collector.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_source_file.py` & `animethemes-batch-encoder-1.1/batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/batch_encoder/_utils.py` & `animethemes-batch-encoder-1.1/batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.0.1/setup.py` & `animethemes-batch-encoder-1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-batch-encoder',
-    version='1.0.1',
-    author='paranarimasu',
-    author_email='paranarimasu@gmail.com',
+    version='1.1',
+    author='AnimeThemes',
+    author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=[
         'appdirs',
```

