# Comparing `tmp/streamp3-0.1.8.tar.gz` & `tmp/streamp3-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/streamp3-0.1.8.tar", last modified: Mon Apr 24 21:17:33 2023, max compression
+gzip compressed data, was "streamp3-0.1.9.tar", last modified: Mon Apr 24 21:22:00 2023, max compression
```

## Comparing `streamp3-0.1.8.tar` & `streamp3-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/
--rw-r--r--   0 brent      (501) staff       (20)       38 2019-07-03 00:24:06.000000 streamp3-0.1.8/MANIFEST.in
--rw-r--r--   0 brent      (501) staff       (20)     4559 2023-04-24 21:17:33.000000 streamp3-0.1.8/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)     3242 2020-10-19 14:24:34.000000 streamp3-0.1.8/README.md
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/lame/
--rw-r--r--   0 brent      (501) staff       (20)        0 2019-07-03 00:24:06.000000 streamp3-0.1.8/lame/__init__.py
--rw-r--r--   0 brent      (501) staff       (20)     2429 2019-07-03 00:24:06.000000 streamp3-0.1.8/lame/hip.pyx
--rw-r--r--   0 brent      (501) staff       (20)      487 2019-07-03 00:24:06.000000 streamp3-0.1.8/lame/lame.pxd
--rw-r--r--   0 brent      (501) staff       (20)       38 2023-04-24 21:17:33.000000 streamp3-0.1.8/setup.cfg
--rw-r--r--   0 brent      (501) staff       (20)      888 2023-04-24 21:17:22.000000 streamp3-0.1.8/setup.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3/
--rw-r--r--   0 brent      (501) staff       (20)     7427 2020-09-16 18:14:48.000000 streamp3-0.1.8/streamp3/__init__.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/
--rw-r--r--   0 brent      (501) staff       (20)     4559 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)      264 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (501) staff       (20)        1 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (501) staff       (20)       15 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/requires.txt
--rw-r--r--   0 brent      (501) staff       (20)       14 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/top_level.txt
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:22:00.258761 streamp3-0.1.9/
+-rw-r--r--   0 brent      (501) staff       (20)    11343 2019-07-03 00:24:06.000000 streamp3-0.1.9/LICENSE
+-rw-r--r--   0 brent      (501) staff       (20)       38 2019-07-03 00:24:06.000000 streamp3-0.1.9/MANIFEST.in
+-rw-r--r--   0 brent      (501) staff       (20)     3682 2023-04-24 21:22:00.258855 streamp3-0.1.9/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)     3242 2020-10-19 14:24:34.000000 streamp3-0.1.9/README.md
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:22:00.256686 streamp3-0.1.9/lame/
+-rw-r--r--   0 brent      (501) staff       (20)        0 2019-07-03 00:24:06.000000 streamp3-0.1.9/lame/__init__.py
+-rw-r--r--   0 brent      (501) staff       (20)     2429 2019-07-03 00:24:06.000000 streamp3-0.1.9/lame/hip.pyx
+-rw-r--r--   0 brent      (501) staff       (20)      487 2019-07-03 00:24:06.000000 streamp3-0.1.9/lame/lame.pxd
+-rw-r--r--   0 brent      (501) staff       (20)       38 2023-04-24 21:22:00.259318 streamp3-0.1.9/setup.cfg
+-rw-r--r--   0 brent      (501) staff       (20)      884 2023-04-24 21:19:50.000000 streamp3-0.1.9/setup.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:22:00.256927 streamp3-0.1.9/streamp3/
+-rw-r--r--   0 brent      (501) staff       (20)     7427 2020-09-16 18:14:48.000000 streamp3-0.1.9/streamp3/__init__.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:22:00.258403 streamp3-0.1.9/streamp3.egg-info/
+-rw-r--r--   0 brent      (501) staff       (20)     3682 2023-04-24 21:22:00.000000 streamp3-0.1.9/streamp3.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)      272 2023-04-24 21:22:00.000000 streamp3-0.1.9/streamp3.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (501) staff       (20)        1 2023-04-24 21:22:00.000000 streamp3-0.1.9/streamp3.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (501) staff       (20)       13 2023-04-24 21:22:00.000000 streamp3-0.1.9/streamp3.egg-info/requires.txt
+-rw-r--r--   0 brent      (501) staff       (20)       14 2023-04-24 21:22:00.000000 streamp3-0.1.9/streamp3.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `streamp3-0.1.8/PKG-INFO` & `streamp3-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,128 @@
 Metadata-Version: 2.1
 Name: streamp3
-Version: 0.1.8
+Version: 0.1.9
 Summary: streaming mp3 decoder
 Home-page: https://github.com/pylon/streamp3/
 Author: Brent M. Spell
 Author-email: brent@pylon.com
 License: UNKNOWN
-Description: # streamp3
-        
-        This library implements streaming MP3 decompression using the LAME library.
-        
-        ## Status
-        [![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
-        [![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
-        [![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
-        
-        ## Installation
-        
-        First, make sure you have the LAME libraries and headers installed.
-        
-        #### macOS
-        
-        ```bash
-        brew install lame
-        ```
-        
-        #### Debian/Ubuntu
-        
-        ```bash
-        apt install libmp3lame-dev
-        ```
-        
-        ### Install with pip
-        ```bash
-        pip install streamp3
-        ```
-        
-        ## Usage
-        To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
-        stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
-        and `num_channels` properties for information about the MP3.
-        
-        ```python
-        from streamp3 import MP3Decoder
-        
-        with open('my.mp3', 'rb') as mp3_file:
-            decoder = MP3Decoder(mp3_file)
-            print(decoder.bit_rate, decoder.sample_rate, decoder.num_channels)
-        ```
-        
-        You can then read samples from the stream directly using the `read()` method
-        or use the decoder as an iterator. Samples are returned as `bytes` objects,
-        which are 16-bit PCM encoded, with samples interleaved across channels. This
-        example streams an MP3 file to the system speaker using
-        [PyAudio](https://pypi.org/project/PyAudio/).
-        
-        ```python
-        import pyaudio
-        from streamp3 import MP3Decoder
-        
-        with open('my.mp3', 'rb') as mp3_file:
-            decoder = MP3Decoder(mp3_file)
-        
-            audio = pyaudio.PyAudio()
-            device = audio.get_default_output_device_info()
-            speaker = audio.open(output=True,
-                                 input_device_index=device['index'],
-                                 format=pyaudio.paInt16,
-                                 channels=decoder.num_channels,
-                                 rate=decoder.sample_rate)
-        
-            for chunk in decoder:
-                speaker.write(chunk)
-        ```
-        
-        ## Development
-        
-        ### Setup
-        We generally use pyenv to create virtual environments. The following script
-        creates a virtual environment for the project and installs dependencies.
-        
-        ```bash
-        pyenv install 3.6.4
-        pyenv virtualenv 3.6.4 streamp3
-        pip install -r requirements.txt
-        ```
-        
-        ### Deployment
-        The project uses setup.py for installation and is deployed to
-        [PyPI](https://pypi.org). The project can be built for installation with
-        the following command:
-        
-        ```bash
-        python setup.py clean --all; rm -r ./dist
-        python setup.py sdist bdist_wheel
-        ```
-        
-        The wheel and source distribution can then be uploaded to PyPI using twine.
-        
-        ```bash
-        twine upload --repository-url=https://upload.pypi.org/legacy/ dist/*
-        ```
-        
-        ## License
-        
-        Copyright 2018 Pylon, Inc.
-        
-          Licensed under the Apache License, Version 2.0 (the "License");
-          you may not use this file except in compliance with the License.
-          You may obtain a copy of the License at
-        
-              http://www.apache.org/licenses/LICENSE-2.0
-        
-          Unless required by applicable law or agreed to in writing, software
-          distributed under the License is distributed on an "AS IS" BASIS,
-          WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-          See the License for the specific language governing permissions and
-          limitations under the License.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# streamp3
+
+This library implements streaming MP3 decompression using the LAME library.
+
+## Status
+[![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
+[![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
+[![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
+
+## Installation
+
+First, make sure you have the LAME libraries and headers installed.
+
+#### macOS
+
+```bash
+brew install lame
+```
+
+#### Debian/Ubuntu
+
+```bash
+apt install libmp3lame-dev
+```
+
+### Install with pip
+```bash
+pip install streamp3
+```
+
+## Usage
+To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
+stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
+and `num_channels` properties for information about the MP3.
+
+```python
+from streamp3 import MP3Decoder
+
+with open('my.mp3', 'rb') as mp3_file:
+    decoder = MP3Decoder(mp3_file)
+    print(decoder.bit_rate, decoder.sample_rate, decoder.num_channels)
+```
+
+You can then read samples from the stream directly using the `read()` method
+or use the decoder as an iterator. Samples are returned as `bytes` objects,
+which are 16-bit PCM encoded, with samples interleaved across channels. This
+example streams an MP3 file to the system speaker using
+[PyAudio](https://pypi.org/project/PyAudio/).
+
+```python
+import pyaudio
+from streamp3 import MP3Decoder
+
+with open('my.mp3', 'rb') as mp3_file:
+    decoder = MP3Decoder(mp3_file)
+
+    audio = pyaudio.PyAudio()
+    device = audio.get_default_output_device_info()
+    speaker = audio.open(output=True,
+                         input_device_index=device['index'],
+                         format=pyaudio.paInt16,
+                         channels=decoder.num_channels,
+                         rate=decoder.sample_rate)
+
+    for chunk in decoder:
+        speaker.write(chunk)
+```
+
+## Development
+
+### Setup
+We generally use pyenv to create virtual environments. The following script
+creates a virtual environment for the project and installs dependencies.
+
+```bash
+pyenv install 3.6.4
+pyenv virtualenv 3.6.4 streamp3
+pip install -r requirements.txt
+```
+
+### Deployment
+The project uses setup.py for installation and is deployed to
+[PyPI](https://pypi.org). The project can be built for installation with
+the following command:
+
+```bash
+python setup.py clean --all; rm -r ./dist
+python setup.py sdist bdist_wheel
+```
+
+The wheel and source distribution can then be uploaded to PyPI using twine.
+
+```bash
+twine upload --repository-url=https://upload.pypi.org/legacy/ dist/*
+```
+
+## License
+
+Copyright 2018 Pylon, Inc.
+
+  Licensed under the Apache License, Version 2.0 (the "License");
+  you may not use this file except in compliance with the License.
+  You may obtain a copy of the License at
+
+      http://www.apache.org/licenses/LICENSE-2.0
+
+  Unless required by applicable law or agreed to in writing, software
+  distributed under the License is distributed on an "AS IS" BASIS,
+  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+  See the License for the specific language governing permissions and
+  limitations under the License.
+
+
```

### Comparing `streamp3-0.1.8/README.md` & `streamp3-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `streamp3-0.1.8/lame/hip.pyx` & `streamp3-0.1.9/lame/hip.pyx`

 * *Files identical despite different names*

### Comparing `streamp3-0.1.8/setup.py` & `streamp3-0.1.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 
 import setuptools
 from distutils.core import setup
 from distutils.extension import Extension
 
 setup(name='streamp3',
-      version='0.1.8',
+      version='0.1.9',
       description="streaming mp3 decoder",
       long_description=open('README.md', 'r').read(),
       long_description_content_type='text/markdown',
       url='https://github.com/pylon/streamp3/',
       author="Brent M. Spell",
       author_email='brent@pylon.com',
       packages=setuptools.find_packages(),
-      setup_requires=['Cython==0.28.5'],
-      install_requires=['Cython==0.28.5'],
+      setup_requires=['Cython==0.29'],
+      install_requires=['Cython==0.29'],
       ext_modules=[Extension('lame.hip',
                              ['lame/hip.pyx'],
                              libraries=['mp3lame'])],
       classifiers=("Programming Language :: Python :: 3",
                    "License :: OSI Approved :: Apache Software License",
                    "Operating System :: OS Independent"))
```

### Comparing `streamp3-0.1.8/streamp3/__init__.py` & `streamp3-0.1.9/streamp3/__init__.py`

 * *Files identical despite different names*

### Comparing `streamp3-0.1.8/streamp3.egg-info/PKG-INFO` & `streamp3-0.1.9/streamp3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,128 @@
 Metadata-Version: 2.1
 Name: streamp3
-Version: 0.1.8
+Version: 0.1.9
 Summary: streaming mp3 decoder
 Home-page: https://github.com/pylon/streamp3/
 Author: Brent M. Spell
 Author-email: brent@pylon.com
 License: UNKNOWN
-Description: # streamp3
-        
-        This library implements streaming MP3 decompression using the LAME library.
-        
-        ## Status
-        [![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
-        [![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
-        [![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
-        
-        ## Installation
-        
-        First, make sure you have the LAME libraries and headers installed.
-        
-        #### macOS
-        
-        ```bash
-        brew install lame
-        ```
-        
-        #### Debian/Ubuntu
-        
-        ```bash
-        apt install libmp3lame-dev
-        ```
-        
-        ### Install with pip
-        ```bash
-        pip install streamp3
-        ```
-        
-        ## Usage
-        To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
-        stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
-        and `num_channels` properties for information about the MP3.
-        
-        ```python
-        from streamp3 import MP3Decoder
-        
-        with open('my.mp3', 'rb') as mp3_file:
-            decoder = MP3Decoder(mp3_file)
-            print(decoder.bit_rate, decoder.sample_rate, decoder.num_channels)
-        ```
-        
-        You can then read samples from the stream directly using the `read()` method
-        or use the decoder as an iterator. Samples are returned as `bytes` objects,
-        which are 16-bit PCM encoded, with samples interleaved across channels. This
-        example streams an MP3 file to the system speaker using
-        [PyAudio](https://pypi.org/project/PyAudio/).
-        
-        ```python
-        import pyaudio
-        from streamp3 import MP3Decoder
-        
-        with open('my.mp3', 'rb') as mp3_file:
-            decoder = MP3Decoder(mp3_file)
-        
-            audio = pyaudio.PyAudio()
-            device = audio.get_default_output_device_info()
-            speaker = audio.open(output=True,
-                                 input_device_index=device['index'],
-                                 format=pyaudio.paInt16,
-                                 channels=decoder.num_channels,
-                                 rate=decoder.sample_rate)
-        
-            for chunk in decoder:
-                speaker.write(chunk)
-        ```
-        
-        ## Development
-        
-        ### Setup
-        We generally use pyenv to create virtual environments. The following script
-        creates a virtual environment for the project and installs dependencies.
-        
-        ```bash
-        pyenv install 3.6.4
-        pyenv virtualenv 3.6.4 streamp3
-        pip install -r requirements.txt
-        ```
-        
-        ### Deployment
-        The project uses setup.py for installation and is deployed to
-        [PyPI](https://pypi.org). The project can be built for installation with
-        the following command:
-        
-        ```bash
-        python setup.py clean --all; rm -r ./dist
-        python setup.py sdist bdist_wheel
-        ```
-        
-        The wheel and source distribution can then be uploaded to PyPI using twine.
-        
-        ```bash
-        twine upload --repository-url=https://upload.pypi.org/legacy/ dist/*
-        ```
-        
-        ## License
-        
-        Copyright 2018 Pylon, Inc.
-        
-          Licensed under the Apache License, Version 2.0 (the "License");
-          you may not use this file except in compliance with the License.
-          You may obtain a copy of the License at
-        
-              http://www.apache.org/licenses/LICENSE-2.0
-        
-          Unless required by applicable law or agreed to in writing, software
-          distributed under the License is distributed on an "AS IS" BASIS,
-          WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-          See the License for the specific language governing permissions and
-          limitations under the License.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# streamp3
+
+This library implements streaming MP3 decompression using the LAME library.
+
+## Status
+[![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
+[![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
+[![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
+
+## Installation
+
+First, make sure you have the LAME libraries and headers installed.
+
+#### macOS
+
+```bash
+brew install lame
+```
+
+#### Debian/Ubuntu
+
+```bash
+apt install libmp3lame-dev
+```
+
+### Install with pip
+```bash
+pip install streamp3
+```
+
+## Usage
+To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
+stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
+and `num_channels` properties for information about the MP3.
+
+```python
+from streamp3 import MP3Decoder
+
+with open('my.mp3', 'rb') as mp3_file:
+    decoder = MP3Decoder(mp3_file)
+    print(decoder.bit_rate, decoder.sample_rate, decoder.num_channels)
+```
+
+You can then read samples from the stream directly using the `read()` method
+or use the decoder as an iterator. Samples are returned as `bytes` objects,
+which are 16-bit PCM encoded, with samples interleaved across channels. This
+example streams an MP3 file to the system speaker using
+[PyAudio](https://pypi.org/project/PyAudio/).
+
+```python
+import pyaudio
+from streamp3 import MP3Decoder
+
+with open('my.mp3', 'rb') as mp3_file:
+    decoder = MP3Decoder(mp3_file)
+
+    audio = pyaudio.PyAudio()
+    device = audio.get_default_output_device_info()
+    speaker = audio.open(output=True,
+                         input_device_index=device['index'],
+                         format=pyaudio.paInt16,
+                         channels=decoder.num_channels,
+                         rate=decoder.sample_rate)
+
+    for chunk in decoder:
+        speaker.write(chunk)
+```
+
+## Development
+
+### Setup
+We generally use pyenv to create virtual environments. The following script
+creates a virtual environment for the project and installs dependencies.
+
+```bash
+pyenv install 3.6.4
+pyenv virtualenv 3.6.4 streamp3
+pip install -r requirements.txt
+```
+
+### Deployment
+The project uses setup.py for installation and is deployed to
+[PyPI](https://pypi.org). The project can be built for installation with
+the following command:
+
+```bash
+python setup.py clean --all; rm -r ./dist
+python setup.py sdist bdist_wheel
+```
+
+The wheel and source distribution can then be uploaded to PyPI using twine.
+
+```bash
+twine upload --repository-url=https://upload.pypi.org/legacy/ dist/*
+```
+
+## License
+
+Copyright 2018 Pylon, Inc.
+
+  Licensed under the Apache License, Version 2.0 (the "License");
+  you may not use this file except in compliance with the License.
+  You may obtain a copy of the License at
+
+      http://www.apache.org/licenses/LICENSE-2.0
+
+  Unless required by applicable law or agreed to in writing, software
+  distributed under the License is distributed on an "AS IS" BASIS,
+  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+  See the License for the specific language governing permissions and
+  limitations under the License.
+
+
```

