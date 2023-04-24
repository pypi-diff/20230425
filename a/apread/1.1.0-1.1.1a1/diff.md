# Comparing `tmp/apread-1.1.0.tar.gz` & `tmp/apread-1.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apread-1.1.0.tar", last modified: Sun May 22 17:33:03 2022, max compression
+gzip compressed data, was "apread-1.1.1a1.tar", last modified: Mon Apr 24 19:27:19 2023, max compression
```

## Comparing `apread-1.1.0.tar` & `apread-1.1.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 17:33:03.610499 apread-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-05-22 17:32:52.000000 apread-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9541 2022-05-22 17:33:03.606499 apread-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9135 2022-05-22 17:32:52.000000 apread-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 17:33:03.606499 apread-1.1.0/apread/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-22 17:32:52.000000 apread-1.1.0/apread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-05-22 17:32:52.000000 apread-1.1.0/apread/apreader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-05-22 17:32:52.000000 apread-1.1.0/apread/binaryReader.py
--rw-r--r--   0 runner    (1001) docker     (121)    15637 2022-05-22 17:32:52.000000 apread-1.1.0/apread/entries.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-05-22 17:32:52.000000 apread-1.1.0/apread/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-05-22 17:32:52.000000 apread-1.1.0/apread/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 17:33:03.606499 apread-1.1.0/apread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9541 2022-05-22 17:33:03.000000 apread-1.1.0/apread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-05-22 17:33:03.000000 apread-1.1.0/apread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-22 17:33:03.000000 apread-1.1.0/apread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-22 17:33:03.000000 apread-1.1.0/apread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-22 17:33:03.000000 apread-1.1.0/apread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-22 17:33:03.610499 apread-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-05-22 17:32:52.000000 apread-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 17:33:03.606499 apread-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-22 17:32:52.000000 apread-1.1.0/test/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:27:19.192274 apread-1.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 19:27:07.000000 apread-1.1.1a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-24 19:27:19.192274 apread-1.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-04-24 19:27:07.000000 apread-1.1.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:27:19.192274 apread-1.1.1a1/apread/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 19:27:07.000000 apread-1.1.1a1/apread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-04-24 19:27:07.000000 apread-1.1.1a1/apread/apreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-24 19:27:07.000000 apread-1.1.1a1/apread/binaryReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-04-24 19:27:07.000000 apread-1.1.1a1/apread/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-24 19:27:07.000000 apread-1.1.1a1/apread/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-24 19:27:07.000000 apread-1.1.1a1/apread/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:27:19.192274 apread-1.1.1a1/apread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-24 19:27:19.000000 apread-1.1.1a1/apread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-24 19:27:19.000000 apread-1.1.1a1/apread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:27:19.000000 apread-1.1.1a1/apread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 19:27:19.000000 apread-1.1.1a1/apread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 19:27:19.000000 apread-1.1.1a1/apread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:27:19.192274 apread-1.1.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 19:27:07.000000 apread-1.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:27:19.192274 apread-1.1.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 19:27:07.000000 apread-1.1.1a1/test/testing.py
```

### Comparing `apread-1.1.0/LICENSE.txt` & `apread-1.1.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apread-1.1.0/PKG-INFO` & `apread-1.1.1a1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,109 @@
-Metadata-Version: 2.1
-Name: apread
-Version: 1.1.0
-Summary: Import data from CatmanAP binary files.
-Home-page: https://github.com/leonbohmann/apreader
-Author: Leon Bohmann
-Author-email: mail@leonbohmann.de
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
+# **apread** (Catman AP Reader)
 
 [![PyPi Upload](https://github.com/leonbohmann/APReader/actions/workflows/python-publish.yml/badge.svg)](https://github.com/leonbohmann/APReader/actions/workflows/python-publish.yml)
 ![pyPI - Version](https://img.shields.io/pypi/v/apread?label=package%20version)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/apread?color=green&label=PyPi%20Downloads&style=plastic)
 
-# **apread** (Catman AP Reader)
 > Read binary files produced from catmanAP projects directly into python.
 
 CatmanAP procudes .bin files after each measurement. While it is possible to export as a different format (i.e. txt or asc) it's not efficient because one has to change the export format after every measurement. Here comes the treat: Just export as binary and use this package to work with binary files directly.
 
 After reading all channels from the binary file, the channels are analyzed and every measure-channel will receive a reference to a time channel, depending on the amount of entries in the channels and the fact, that the time-channel has to contain "time" or "zeit" in its name. What that means is, that a channel with x entries and the name "time - 1" will be regarded as the time-channel of any other channel with x Data Entries.
 
 Here is an example plot, generated directly from a binary file:
 ![apread_demo_out_1](https://user-images.githubusercontent.com/13386367/169707732-240a916e-228f-4ef9-8c3c-e560a2647c97.png)
 
-
 ## Installation/Update
 
 Anywhere with python (note the uppercase U):
 
 ```sh
 pip install -U apread
 ```
 
 ## How it works
+
 The workflow of the package is straight-forward. You supply a binary file created with CatmanAP and the script will read that into python.
 
 First of all, the binary data is analyzed and packaged into seperate `Channel` objects. When all `Channels` are created, each `Channel.Name` will be checked against `([T|t]ime)|([Z|z]eit)`, which mark time channels which usually are the reference.
 
 These `Channels` marked as `istime` are the basis for `Groups`. Inside a group you will find the `ChannelX` (time channel) and a bunch of other channels in `ChannelsY`, which are the channels containing data in that time domain. The corresponding channels inside a `Group` are found by analyzing their length. Since the total time measured is the same for all groups, it is assumed that `Channels` with the same data-length belong to the same group. Connecting the matching channels to the group give a structured representation of your measurement data.
 
 Now that the Data is available in python you are free to do with that whatever you want. Until Version `1.0.x` there were some features in which you can save the data but that feature has been removed.
 
 ## Usage
 
-Lets say you produced a file called `measurements.bin` and you put it in the directory of your python script, then you can create the `APReader` on that file. It's that simple. The Initialization may take some time depending on how large your .bin-File is. 
+Lets say you produced a file called `measurements.bin` and you put it in the directory of your python script, then you can create the `APReader` on that file. It's that simple. The Initialization may take some time depending on how large your .bin-File is.
 
 ```python
 from apread import APReader
 
 reader = APReader('measurements.bin')   # this will read in the file
-``` 
+```
 
 ### Print channels
+
 Afterwards you can access the `Channels` by accessing the `APReader.Channels` Member. `Channel` and `Group` implement `__str__` which will return the name and the length of data inside it.
 
 ```python
 for channel in reader.Channels:
     print(channel)
 
 # "Timechannel 1 - Standard" (120341 Entries)
 # "T12_ref" (120341 Entries)
 # "T33" (120341 Entries)
 # "Timechannel 1 - Quick" (3022344 Entries)
 # "F1" (3022344 Entries)
 # "ast089" (3022344 Entries)
-``` 
+```
 
 ```python
 for group in reader.Groups:
     print(group)
 
 # "Timechannel 1 - Standard" (2 Data-channels, 120341 Entries)
 # "Timechannel 1 - Quick" (2 Data-channels, 3022344 Entries)
-``` 
+```
 
 ### Plot Channels/Groups
+
 To review your data on the fly, you can plot every entity in the data structure by calling `.plot()`. When plotting, every group will get its own figure window, in which all connected channels are plotted.
 
 ```python
 # plot the readers data
 reader.plot()
 # plot all groups
 for group in reader.Groups:
     group.plot()
 # plot all channels
 for channel in reader.Channels:
     channel.plot()
-``` 
+```
 
 As you can see, you can access the channels from the reader, which contains all channels (including time channels) or you can access them from the groups.
 
 There are some more functions to plot specific data. When plotting multiple channels each channel gets its own y-axis.
+
 ```python
 group.plotChannel(0)           # specific channel
 group.plotChannels(0,3)        # channel 1 to 3 (1,2,3)
 group.plot([0, 2, 4])          # channel 1, 3 and 5
-``` 
+```
 
 The same can be applied to the `APReader`. The only difference is that you can plot specific groups instead of channels.
+
 ```python
 reader.plotGroup(0)           # specific group
 reader.plotGroups(0,3)        # group 1 to 3 (1,2,3)
 reader.plot([0, 2, 4])        # group 1, 3 and 5
 ``` 
+
 ### External Header
+
 Thanks to ([hakonbars PR13](https://github.com/leonbohmann/APReader/pull/13)) you are now able to access external header information using `channel.exthdr`, a dicitionary containing all keys as described in [this sheet](https://github.com/leonbohmann/APReader/blob/dev-2/test/catmanBinaryFormat.xls).
 
 ```python
 ['T0']                 # ACQ timestamp info (NOW format) 
 ['dt']                 # ACQ delta t in ms
 ['SensorType']         # IDS code of sensor type
 ['SupplyVoltage']      # IDS code supply voltage
@@ -138,67 +130,116 @@
 ['SoftwareTareVal']    # Software tare (zero) for channels carrying a user scale
 ['WriteProtected']     # If true, write access is denied
 ['NominalRange']       # CAV value
 ['CLCFactor']          # Cable length compensation factor (CANHEAD only)
 ['ExportFormat']       # 0=8-Byte Double, 1=4-Byte Single, 2=2-Byte Integer (FOR CATMAN BINARY EXPORT ONLY!)    
 ```
 
+### Parallel reading of data
+
+> Only available from version `v1.1.1-alpha1` and above
+
+See `test/testing.py` for a full example. Modify the following around your `APReader` call:
+
+```python
+import multiprocessing as mp
+...
+
 
+if __name__ == '__main__': # this line has to be included!
+    # without 'processes=...'!
+    pool = mp.Pool() 
 
+    # pass the pool to the reader
+    reader = APReader(file, parallelPool=pool)
+
+    # make sure to close the pool after you are done with it
+    mp.close()
+    mp.join()
+```
+
+For the parallel loading to work, you have to define a parallel pool of processes in your top-level script. These processes will be accessed from within `APReader`-Functions. When passing no arguments to `mp.Pool()` it will automatically create as many processes as possible, according to the amount of threads your CPU allows (cores + virtual cores). It does not make sense to pass in more, since the `APReader` spawns the same amount of processes as there are CPU Threads. Increasing the amount of processes in your pool does not increase the amount of parallelism. It is fixed.
+
+> Keep in mind, that parallelisation is not always faster. Spawning of processes is expensive and can be wasteful for small files.
+
+The results from `APReader` stay the same and you can continue your analysis.
 
 ## Release History
-### **Version 1.1**
 
-#### Breaking changes
+### Version 1.1.1-alpha1
+
+* Added converted timestamp property on channels (`Channel.date`)
+  * *Property `Channel.time` will be deleted at some point in the future...*
+* Parallel reading of binary files
+  * Max degree of parallelism is defined with maximum amount of processors
+* ----------------------------
+* ----------------------------
+  
+#### Version 1.1
+
+##### Breaking changes
 
 * Removed saving functions, this will be up to the user
     > Since these function change a lot based on current needs, I decided to remove the post-processing functionality completely. The user now needs to do the post-processing on his own, meaning the creation of plots using time and data channels...
 
-#### Changes
+##### Changes
+
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Differentiate floating point precision
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Reading additional header information
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Supplying binary format reference
 * Fixed null returning string conversion function
 * Using regex to find time channels
 * Improved plotting with multiple axes
 * Printing channels and groups will now give a summary instead of all data
 
-
 #### Version 1.0.22
+
 * Fixed an issue with groups where time channels are not recognized
-*  now, user is prompted, when suspected time channel is found
-*  plotting is not possible when there is no time-channel found
-*  save groups and channels even when there is no time channel
+* now, user is prompted, when suspected time channel is found  
+* plotting is not possible when there is no time-channel found
+* save groups and channels even when there is no time channel
+
 #### Version 1.0.21
+
 * Updated serialisation-procedures to always encode in `UTF-8`
+
 #### Version 1.0.20
+
 * Switched to explicit type hinting with `typing` package (compatibility issues with python <3.9.x)  
+
 #### Version 1.0.15/16
+
 * Fixed an issue with saving and non-existent directories
 * Added `getas` to generate formatted string without saving
+
 #### Version 1.0.14
+
 * Output file-names updated
+
 #### Version 1.0.12/13
+
 * Group channels with their time-channel into "groups"
 * Multiple plot modes:
-    * Whole file
-    * Channel/Group only
+  * Whole file
+  * Channel/Group only
 * Output data
-    * json
-    * csv
+  * json
+  * csv
 
 #### Version 1.0.11
+
 * Progressbars indicate read-progress of files
 * Multiple plot modes
 
 #### Version 1.0.0
+
 * Convert catman files to channels
 
 ## Meta
 
 Leon Bohmann – mail@leonbohmann.de
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
 
-[https://github.com/leonbohmann/apreader](https://github.com/leonbohmann/apreader)
-
+This software comes with no warranty, expressed or implied. Use at your own risk!
 
+[https://github.com/leonbohmann/apreader](https://github.com/leonbohmann/apreader)
```

### Comparing `apread-1.1.0/README.md` & `apread-1.1.1a1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,122 @@
+Metadata-Version: 2.1
+Name: apread
+Version: 1.1.1a1
+Summary: Import data from CatmanAP binary files.
+Home-page: https://github.com/leonbohmann/apreader
+Author: Leon Bohmann
+Author-email: mail@leonbohmann.de
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# **apread** (Catman AP Reader)
 
 [![PyPi Upload](https://github.com/leonbohmann/APReader/actions/workflows/python-publish.yml/badge.svg)](https://github.com/leonbohmann/APReader/actions/workflows/python-publish.yml)
 ![pyPI - Version](https://img.shields.io/pypi/v/apread?label=package%20version)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/apread?color=green&label=PyPi%20Downloads&style=plastic)
 
-# **apread** (Catman AP Reader)
 > Read binary files produced from catmanAP projects directly into python.
 
 CatmanAP procudes .bin files after each measurement. While it is possible to export as a different format (i.e. txt or asc) it's not efficient because one has to change the export format after every measurement. Here comes the treat: Just export as binary and use this package to work with binary files directly.
 
 After reading all channels from the binary file, the channels are analyzed and every measure-channel will receive a reference to a time channel, depending on the amount of entries in the channels and the fact, that the time-channel has to contain "time" or "zeit" in its name. What that means is, that a channel with x entries and the name "time - 1" will be regarded as the time-channel of any other channel with x Data Entries.
 
 Here is an example plot, generated directly from a binary file:
 ![apread_demo_out_1](https://user-images.githubusercontent.com/13386367/169707732-240a916e-228f-4ef9-8c3c-e560a2647c97.png)
 
-
 ## Installation/Update
 
 Anywhere with python (note the uppercase U):
 
 ```sh
 pip install -U apread
 ```
 
 ## How it works
+
 The workflow of the package is straight-forward. You supply a binary file created with CatmanAP and the script will read that into python.
 
 First of all, the binary data is analyzed and packaged into seperate `Channel` objects. When all `Channels` are created, each `Channel.Name` will be checked against `([T|t]ime)|([Z|z]eit)`, which mark time channels which usually are the reference.
 
 These `Channels` marked as `istime` are the basis for `Groups`. Inside a group you will find the `ChannelX` (time channel) and a bunch of other channels in `ChannelsY`, which are the channels containing data in that time domain. The corresponding channels inside a `Group` are found by analyzing their length. Since the total time measured is the same for all groups, it is assumed that `Channels` with the same data-length belong to the same group. Connecting the matching channels to the group give a structured representation of your measurement data.
 
 Now that the Data is available in python you are free to do with that whatever you want. Until Version `1.0.x` there were some features in which you can save the data but that feature has been removed.
 
 ## Usage
 
-Lets say you produced a file called `measurements.bin` and you put it in the directory of your python script, then you can create the `APReader` on that file. It's that simple. The Initialization may take some time depending on how large your .bin-File is. 
+Lets say you produced a file called `measurements.bin` and you put it in the directory of your python script, then you can create the `APReader` on that file. It's that simple. The Initialization may take some time depending on how large your .bin-File is.
 
 ```python
 from apread import APReader
 
 reader = APReader('measurements.bin')   # this will read in the file
-``` 
+```
 
 ### Print channels
+
 Afterwards you can access the `Channels` by accessing the `APReader.Channels` Member. `Channel` and `Group` implement `__str__` which will return the name and the length of data inside it.
 
 ```python
 for channel in reader.Channels:
     print(channel)
 
 # "Timechannel 1 - Standard" (120341 Entries)
 # "T12_ref" (120341 Entries)
 # "T33" (120341 Entries)
 # "Timechannel 1 - Quick" (3022344 Entries)
 # "F1" (3022344 Entries)
 # "ast089" (3022344 Entries)
-``` 
+```
 
 ```python
 for group in reader.Groups:
     print(group)
 
 # "Timechannel 1 - Standard" (2 Data-channels, 120341 Entries)
 # "Timechannel 1 - Quick" (2 Data-channels, 3022344 Entries)
-``` 
+```
 
 ### Plot Channels/Groups
+
 To review your data on the fly, you can plot every entity in the data structure by calling `.plot()`. When plotting, every group will get its own figure window, in which all connected channels are plotted.
 
 ```python
 # plot the readers data
 reader.plot()
 # plot all groups
 for group in reader.Groups:
     group.plot()
 # plot all channels
 for channel in reader.Channels:
     channel.plot()
-``` 
+```
 
 As you can see, you can access the channels from the reader, which contains all channels (including time channels) or you can access them from the groups.
 
 There are some more functions to plot specific data. When plotting multiple channels each channel gets its own y-axis.
+
 ```python
 group.plotChannel(0)           # specific channel
 group.plotChannels(0,3)        # channel 1 to 3 (1,2,3)
 group.plot([0, 2, 4])          # channel 1, 3 and 5
-``` 
+```
 
 The same can be applied to the `APReader`. The only difference is that you can plot specific groups instead of channels.
+
 ```python
 reader.plotGroup(0)           # specific group
 reader.plotGroups(0,3)        # group 1 to 3 (1,2,3)
 reader.plot([0, 2, 4])        # group 1, 3 and 5
 ``` 
+
 ### External Header
+
 Thanks to ([hakonbars PR13](https://github.com/leonbohmann/APReader/pull/13)) you are now able to access external header information using `channel.exthdr`, a dicitionary containing all keys as described in [this sheet](https://github.com/leonbohmann/APReader/blob/dev-2/test/catmanBinaryFormat.xls).
 
 ```python
 ['T0']                 # ACQ timestamp info (NOW format) 
 ['dt']                 # ACQ delta t in ms
 ['SensorType']         # IDS code of sensor type
 ['SupplyVoltage']      # IDS code supply voltage
@@ -124,65 +143,116 @@
 ['SoftwareTareVal']    # Software tare (zero) for channels carrying a user scale
 ['WriteProtected']     # If true, write access is denied
 ['NominalRange']       # CAV value
 ['CLCFactor']          # Cable length compensation factor (CANHEAD only)
 ['ExportFormat']       # 0=8-Byte Double, 1=4-Byte Single, 2=2-Byte Integer (FOR CATMAN BINARY EXPORT ONLY!)    
 ```
 
+### Parallel reading of data
+
+> Only available from version `v1.1.1-alpha1` and above
+
+See `test/testing.py` for a full example. Modify the following around your `APReader` call:
+
+```python
+import multiprocessing as mp
+...
 
 
+if __name__ == '__main__': # this line has to be included!
+    # without 'processes=...'!
+    pool = mp.Pool() 
+
+    # pass the pool to the reader
+    reader = APReader(file, parallelPool=pool)
+
+    # make sure to close the pool after you are done with it
+    mp.close()
+    mp.join()
+```
+
+For the parallel loading to work, you have to define a parallel pool of processes in your top-level script. These processes will be accessed from within `APReader`-Functions. When passing no arguments to `mp.Pool()` it will automatically create as many processes as possible, according to the amount of threads your CPU allows (cores + virtual cores). It does not make sense to pass in more, since the `APReader` spawns the same amount of processes as there are CPU Threads. Increasing the amount of processes in your pool does not increase the amount of parallelism. It is fixed.
+
+> Keep in mind, that parallelisation is not always faster. Spawning of processes is expensive and can be wasteful for small files.
+
+The results from `APReader` stay the same and you can continue your analysis.
 
 ## Release History
-### **Version 1.1**
 
-#### Breaking changes
+### Version 1.1.1-alpha1
+
+* Added converted timestamp property on channels (`Channel.date`)
+  * *Property `Channel.time` will be deleted at some point in the future...*
+* Parallel reading of binary files
+  * Max degree of parallelism is defined with maximum amount of processors
+* ----------------------------
+* ----------------------------
+  
+#### Version 1.1
+
+##### Breaking changes
 
 * Removed saving functions, this will be up to the user
     > Since these function change a lot based on current needs, I decided to remove the post-processing functionality completely. The user now needs to do the post-processing on his own, meaning the creation of plots using time and data channels...
 
-#### Changes
+##### Changes
+
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Differentiate floating point precision
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Reading additional header information
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Supplying binary format reference
 * Fixed null returning string conversion function
 * Using regex to find time channels
 * Improved plotting with multiple axes
 * Printing channels and groups will now give a summary instead of all data
 
-
 #### Version 1.0.22
+
 * Fixed an issue with groups where time channels are not recognized
-*  now, user is prompted, when suspected time channel is found
-*  plotting is not possible when there is no time-channel found
-*  save groups and channels even when there is no time channel
+* now, user is prompted, when suspected time channel is found  
+* plotting is not possible when there is no time-channel found
+* save groups and channels even when there is no time channel
+
 #### Version 1.0.21
+
 * Updated serialisation-procedures to always encode in `UTF-8`
+
 #### Version 1.0.20
+
 * Switched to explicit type hinting with `typing` package (compatibility issues with python <3.9.x)  
+
 #### Version 1.0.15/16
+
 * Fixed an issue with saving and non-existent directories
 * Added `getas` to generate formatted string without saving
+
 #### Version 1.0.14
+
 * Output file-names updated
+
 #### Version 1.0.12/13
+
 * Group channels with their time-channel into "groups"
 * Multiple plot modes:
-    * Whole file
-    * Channel/Group only
+  * Whole file
+  * Channel/Group only
 * Output data
-    * json
-    * csv
+  * json
+  * csv
 
 #### Version 1.0.11
+
 * Progressbars indicate read-progress of files
 * Multiple plot modes
 
 #### Version 1.0.0
+
 * Convert catman files to channels
 
 ## Meta
 
 Leon Bohmann – mail@leonbohmann.de
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
 
+This software comes with no warranty, expressed or implied. Use at your own risk!
+
 [https://github.com/leonbohmann/apreader](https://github.com/leonbohmann/apreader)
```

### Comparing `apread-1.1.0/apread/apreader.py` & `apread-1.1.1a1/apread/apreader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import multiprocessing as mp
 import os
+import re
+
 # binary imports
 from os import SEEK_SET
 from typing import List
-# import this to show warnings
-import warnings
-import random
+
 from matplotlib import pyplot as plt
 from tqdm import tqdm
-import re
 
-# channel definition
-from apread.entries import Channel, Group
 # binary reader to read binary files
 from apread.binaryReader import BinaryReader
-from apread.tools import deprecated
+
+# channel definition
+from apread.entries import Channel, Group
+
 
 def align_yaxis(ax1, v1, ax2, v2):
     """adjust ax2 ylimit so that v2 in ax2 is aligned to v1 in ax1"""
     _, y1 = ax1.transData.transform((0, v1))
     _, y2 = ax2.transData.transform((0, v2))
     inv = ax2.transData.inverted()
     _, dy = inv.transform((0, 0)) - inv.transform((0, y1-y2))
@@ -36,29 +37,34 @@
     """
     Channels: List[Channel]
     """
     Grouped channels.    
     """
     Groups: List[Group]
 
-    def __init__(self, path, verbose=False, filterData=False, fastload=True):
+    def __init__(self, path, verbose=False, parallelPool = None):
         """Creates a new APReader based on a .binary file (path).
 
         Args:
             path (str): path to a catmanAP binary file.
             verbose (boolean): Show debug output.
-            filterData (boolean): Filter input data.
+            parallelPool (multiprocessing.Pool): If passed, the loading of files will be
+                done on the threads in the pool.
         """
         self.verbose = verbose
-        self.filterData = filterData
-        self.fastload = fastload
         self.filepath = path
         self.fileName = os.path.splitext(os.path.basename(path))[0]
+        self.parallelLoad = parallelPool is not None
+        self.parallelPool = parallelPool
         self.Channels = []
         self.Groups = []
+        
+        if self.parallelLoad:
+            print(f'INFO: Using {len(mp.active_children())} processes to load data.')
+        
         self.read()
         self.connect()
 
     def connect(self):
         """
         Find channels with equal data length and filter the name for "time" to 
         connect the time-channel with every value-channel (Channel -> channel.Time).
@@ -69,15 +75,15 @@
 
         # create dictionary entries for every length of channels
         # Dictionary: [int: channel.Length, List: Channels]
         channelGroups = {}
         # loop through channels
         for channel in self.Channels:
             # if the current channel length has not been analyzed yet
-            if not channel.length in channelGroups:
+            if channel.length not in channelGroups:
                 # add a new dictionary entry
                 channelGroups[channel.length] = []
             
             # append the channel to the dictionary's entry
             channelGroups[channel.length].append(channel)
                 
         # now, for each channel-group find the time-channel (only if length of the gorup > 0)
@@ -100,14 +106,16 @@
                     break
 
                 # instead of assuming, ask the user if the timechannel is the one with "seconds"
                 if "s" == channel.unit:
                     if input(f"Is '{channel.Name}' your time/reference channel? [y/n] ") == "y":
                         timeChannel = channel
                         break
+# %%
+
             #%% sdasd
             # set the time-channel on every channel but itself
             if timeChannel != None:
                 for channel in group:
                     if channel is not timeChannel:
                         channel.Time = timeChannel
                         channel.isTime = False
@@ -116,14 +124,18 @@
             else:
                 print("\t [ERROR] Channel-group does not contain a time-channel!")
                 print("\t  The current group will not be included in this output.")
                 continue
             
             # create new group based on the groups listed
             self.Groups.append(Group(group, self.fileName, self.verbose))
+        
+        if len(self.Channels) > 0:
+            self.date = self.Channels[0].date
+        
         pass
 
     def __iter__(self):
         """Iterates over everything in this reader.
 
         Yields:
             Any(Channel, Group): Yields all channels and groups.
@@ -149,35 +161,36 @@
             self.dataOffset = reader.read_int32()
             # read comment
             self.comment = reader.read_string(reader.read_int16())
 
             # readaway
             for i in range(32):
                 lresakt = reader.read_int16()
-                resString = reader.read_string(lresakt)
+                _ = reader.read_string(lresakt)
 
             # total number of channels
             self.numChannels = reader.read_int16()
             if self.verbose:
                 print(f"\t[ {self.fileName} ] Found {self.numChannels} Channels.")
             # maximum channel length (usually 0 meaning unlimited)
             self.maxLength = reader.read_int32()
 
             # readaway
             for i in range(self.numChannels):
                 reader.read_int32()
             
             # reduced factor (unused)
-            redfac = reader.read_int32()
+            _ = reader.read_int32()
 
             # loop channels
             for i in range(self.numChannels):
                 # create new channel on top of reader
                 #! be careful with current stream position
-                channel = Channel(reader, self.fileName, self.verbose, self.filterData, self.fastload)
+                channel = Channel(reader, self.fileName, self.filepath,\
+                    self.verbose, self.parallelPool)
 
                 if not channel.broken and channel.length > 0:                    
                     self.Channels.append(channel)
                 elif self.verbose:
                     print(f'\t[ {self.fileName} ] Skipping channel (zero length or invalid data)')
 
             # seek stream pointer to start of data
@@ -193,20 +206,14 @@
             if self.verbose:
                 print(f'\t[ {self.fileName} ] Done. {len(self.Channels)} Channels left after filtering.') 
                 
                 
     def plot(self, groupIndices=None):
         """Plots the complete file.
         """
-        name = os.path.basename(self.filepath)
-        
-        groups = self.Groups
-        if groupIndices is not None:
-            groups = [self.Groups[x] for x in groupIndices]
-
         for group in self.Groups:
             group.plot()     
             
     def plotGroup(self, channelIndex):
         """Plot a specific channel
 
         Args:
```

### Comparing `apread-1.1.0/apread/binaryReader.py` & `apread-1.1.1a1/apread/binaryReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import struct
 from os import SEEK_CUR
 from typing import BinaryIO
 
+
 ENDIAN_PREFIXES = ("@", "<", ">", "=", "!")
 
 
 class BinaryReader:
     """
     Base class to read binary files.
     """
@@ -63,8 +64,10 @@
     def read_float(self) -> float:
         return struct.unpack(self.endian + "f", self.read(4))[0]
 
     def read_double(self) -> float:
         return struct.unpack(self.endian + "d", self.read(8))[0]
     # Aliases
     def read_int(self) -> int:
-        return self.read_int32()
+        return self.read_int32()
+    
+
```

### Comparing `apread-1.1.0/apread/entries.py` & `apread-1.1.1a1/apread/entries.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,52 @@
 # binary reader import
+# parallel processing
+import multiprocessing as mp
 import os
-from time import time
-from apread.binaryReader import BinaryReader
+from datetime import datetime
+from multiprocessing.pool import Pool as mpPool
+
+# typing
+from typing import List
 
 # plotting
 import matplotlib.pyplot as plt
-import plotly.express as px
-import scipy.signal as sig
-
-# serialization
-import json
 
 # progress
-from tqdm import tqdm
-from apread.loader import Loader
 import numpy as np
-# filtering
-from scipy.signal import lfilter
 
-# typing
-from typing import List
+from apread.binaryReader import BinaryReader
 
-from apread.tools import deprecated
 
+def read_chunk_from_file(file_path, start, end, typ, buf_loc) -> np.ndarray:
+    """Reads a chunk of a file by opening a binary reader.
+
+    Args:
+        file_path (str): Filepath to the file.
+        start (int): Start buffer location in entries.
+        end (int): End buffer location in entries.
+        typ (nd.dtype): The type of data.
+        cur_loc (int): Current buffer location in bytes.
+
+    Returns:
+        np.ndarray: The chunk of the file as a numbered array.
+    """
+    # open the file and seek the buffer to the start of channel entries
+    with open(file_path, 'rb') as f:
+        f.seek(buf_loc)
+        # read the chunk of data from the file
+        chunk = np.fromfile(f, dtype=typ, offset=start * typ.itemsize, count=end-start)
+        
+    return chunk    
+
+def toTimestamp(serialFormat):
+    return (serialFormat - 25569) * 86400.0
+
+def toDatetime(timestamp):
+    return datetime.utcfromtimestamp(timestamp)
 
 def get_clr(n, name='hsv'):
     '''Returns a function that maps each index in 0, 1, ..., n-1 to a distinct 
     RGB color; the keyword argument name must be a standard mpl colormap name.'''
     return plt.cm.get_cmap(name, n)
 
 class Channel:
@@ -41,26 +61,37 @@
             If there is more than one channel having the same amount of entries, every channel will 
             get the same reference to the time channel.
     """        
     # data: List[float]
     verbose: bool
     # Defines if data should be filtered.
     filterData: bool
-
-    def __init__(self, reader: BinaryReader, fileName='unknown', verbose=False, filterData=False, fastload=True):
+    
+    # Specifies if channel entries should be loaded in parallel.
+    parallelLoad: bool
+    # Amount of parallel processes that can be used to load data.
+    parallelProcs: int
+    # The parallel pool which holds parallel processes.
+    parallelPool: mpPool
+    
+    def __init__(self, reader: BinaryReader, fileName='unknown', filepath='', \
+        verbose=False, parallelPool=None):
         """
         Creates the Channel.
 
         Uses a reader (BinaryReader) to read the data from the file accessed by "APReader.__init__".
         """
-        self.fastload = fastload
+        
+        # parallel stuff
+        self.parallelLoad = parallelPool is not None
+        self.parallelPool = parallelPool
+        self.parallelProcs = len(mp.active_children())
+        
         # defines, if the apreader should output verbose debug messages
         self.verbose = verbose
-        # defines, wether read data should be filtered
-        self.filterData = filterData
 
         # referenced time channel (dummy, since this may stay None)
         self.Time = None
         self.isTime = False
         # save the reader for later use
         self.reader = reader
 
@@ -71,28 +102,29 @@
         # get name of channel
         self.Name = reader.read_string(reader.read_int16())
 
         # the original file name of the group
         self.fileName = os.path.splitext(os.path.basename(fileName))[0]
         tName = self.Name.replace(' ',"_")  # temporary name
         self.fullName = f"{fileName}.{tName}"
-
+        self.filePath = filepath
         # retrieve unit of channel                
         
         self.unit = reader.read_string(reader.read_int16())
         
         # get comment of channel                
         self.comment = reader.read_string(reader.read_int16())
 
         # 0: numeric, 1: string, 2: binary object
         self.format  = reader.read_int16()
         # get format of channel (8: numeric, >8: string)
         self.dw = reader.read_int16()
         # time of reading
         self.time = reader.read_double()
+        self.date = toDatetime(self.time)
         # extended channel header
         self.nHdrBytes = reader.read_int32()
         self.extHeader = self.readExtHeader(reader)
         
         precDict = {0:8, 1:4, 2:2} # key: Attribute "Exportformat", value: precision in bytes
         try:
             self.precision = precDict[self.extHeader['ExportFormat']]
@@ -165,20 +197,20 @@
         exthdr['MeasSig'] = rdr.read_int16() # 118
         exthdr['AmpInput'] = rdr.read_int16() # 120
         exthdr['HPFilt'] = rdr.read_int16() # 122
         exthdr['OLImportInfo'] = rdr.read_byte() # 123
         exthdr['ScaleType'] = rdr.read_byte() # 124
         exthdr['SoftwareTareVal'] = rdr.read_float() # 128        
         exthdr['WriteProtected'] = rdr.read_byte() # 129
-        padding = rdr.read_string(3) # 132
+        rdr.read_string(3) # 132
         
         exthdr['NominalRange'] = rdr.read_float() # 136 
         exthdr['CLCFactor'] = rdr.read_float() # 140
         exthdr['ExportFormat'] = rdr.read_byte() # 141
-        reserve = rdr.read_string(7) # 148
+        rdr.read_string(7) # 148
         # reserve = rdr.read_string(10)        
         posN = rdr.tell()
         
         if (posN-pos0) != self.nHdrBytes:
             print("""
                   WARNING:
                   The number of bytes read in the extended header of the channel
@@ -200,48 +232,32 @@
 
         IMPORTANT
             The stream offset has to be set before calling this function!
         """
         # if something was wrong previously, nothing will happen here
         if self.broken:
             return
-        
-        if self.fastload:
-            # The data is stored channelwise. We therefore only need to pass pointers to the first and last byte.
-            if self.precision == 8 or self.precision == 4:
-                self.data = np.fromfile(self.reader.buf, dtype=np.dtype('f{}'.format(self.precision)), count=self.length)
-            elif self.precision == 2:
-                MinValue = self.reader.read_double()
-                MaxValue = self.reader.read_double()
-                sf = (MaxValue - MinValue)/32767 # scale factor
-                self.data = np.fromfile(self.reader.buf, dtype=np.dtype('u2'), count=self.length)*sf + MinValue
-        else:
-            # initialize data
-            self.data = []
-
-            # read all channel data            
-            if self.precision == 8:
-                for i in tqdm(range(self.length), leave=False):
-                    self.data.append(self.reader.read_double())
-            elif self.precision == 4:
-                for i in tqdm(range(self.length), leave=False):
-                    self.data.append(self.reader.read_float())
-            elif self.precision == 2:                
-                MinValue = self.reader.read_double()
-                MaxValue = self.reader.read_double()
-                sf = (MaxValue - MinValue)/32767 # scale factor
+                        
+        # The data is stored channelwise. We therefore only need to pass pointers to the first and last byte.
+        if self.precision == 8 or self.precision == 4:
+            datatype = np.dtype('f{}'.format(self.precision))                
+            # parallel loading will split up the incoming bin array
+            if self.parallelLoad:
+                self.data = self.read_data_parallel(datatype)
                 
-                for i in tqdm(range(self.length), leave=False):
-                    self.data.append(self.reader.read_int16()*sf + MinValue)
-
-        # filter data
-        if self.filterData:
-            with Loader('Filtering data...'):
-                self.data = self.filter()
-
+            # default loading will load all entries at once
+            else:
+                self.data = np.fromfile(self.reader.buf, dtype=datatype, count=self.length)
+                
+        elif self.precision == 2:
+            MinValue = self.reader.read_double()
+            MaxValue = self.reader.read_double()
+            sf = (MaxValue - MinValue)/32767 # scale factor
+            self.data = np.fromfile(self.reader.buf, dtype=np.dtype('u2'), count=self.length)*sf + MinValue
+    
     def __str__(self):
         """
         Default conversion to string.
         """
         return f'Channel "{self.Name}" ({self.length} Entries)'        
 
     def __getitem__(self, key) -> float:
@@ -276,29 +292,66 @@
         plotbase = axes if axes is not None else plt
         
         
         if self.verbose:
             print(f'\t[ APREAD/PLOT ] Plotting {self.Name}')
         
         if not governed:
-            fig = plt.figure(self.Name)
+            plt.figure(self.Name)
             plt.xlabel('Time [s]')
             plt.ylabel(self.unit)
 
         line = plotbase.plot(self.Time.data, self.data, color=clr, label=self.Name )
         
         
         if not governed:
             plt.title(self.Name)
             plt.draw()
             plt.legend()        
             plt.show()
             
         return line
-  
+    
+    
+
+    def read_data_parallel(self, dtype):
+        """Reads in the underlying binary data using multiple parallel tasks.
+
+        Args:
+            dtype (nd.dtype): The type of the underlying layer data entries (f4, f8, ...).
+
+        Returns:
+            ndarray: Array of the binary data.
+        """
+        # chunk the total length of this channel
+        chunk_size = self.length // self.parallelProcs        
+                
+        # current location of the buffered binary reader
+        cur_loc = self.reader.tell()
+
+        # chunk the length
+        chunks = [(start, min(start + chunk_size, self.length)) for start in range(0, self.length, chunk_size)]
+        results = [self.parallelPool.apply_async(read_chunk_from_file, args=(self.filePath, start, end, dtype, cur_loc)) for (start, end) in chunks]
+
+        # wait for results to finish and check if they finished successfully
+        for r in results:
+            r.wait()
+            if not r.successful():
+                print('Error in loading task!')
+        
+        # concatenate the data structure
+        data = np.empty(self.length, dtype)
+        for result, (start, end) in zip(results, chunks):
+            data[start:end] = result.get()
+        
+        # push the underlying original reader to after the channel items
+        self.reader.seek(cur_loc + self.length * dtype.itemsize)
+        return data
+
+
 class Group:
     """
     Groups channels together.
 
     Helps calling plot functions..
     """
     # all (unsorted) channels in this group
```

### Comparing `apread-1.1.0/apread/loader.py` & `apread-1.1.1a1/apread/loader.py`

 * *Files identical despite different names*

### Comparing `apread-1.1.0/apread/tools.py` & `apread-1.1.1a1/apread/tools.py`

 * *Files identical despite different names*

### Comparing `apread-1.1.0/apread.egg-info/PKG-INFO` & `apread-1.1.1a1/apread.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,122 @@
 Metadata-Version: 2.1
 Name: apread
-Version: 1.1.0
+Version: 1.1.1a1
 Summary: Import data from CatmanAP binary files.
 Home-page: https://github.com/leonbohmann/apreader
 Author: Leon Bohmann
 Author-email: mail@leonbohmann.de
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+# **apread** (Catman AP Reader)
 
 [![PyPi Upload](https://github.com/leonbohmann/APReader/actions/workflows/python-publish.yml/badge.svg)](https://github.com/leonbohmann/APReader/actions/workflows/python-publish.yml)
 ![pyPI - Version](https://img.shields.io/pypi/v/apread?label=package%20version)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/apread?color=green&label=PyPi%20Downloads&style=plastic)
 
-# **apread** (Catman AP Reader)
 > Read binary files produced from catmanAP projects directly into python.
 
 CatmanAP procudes .bin files after each measurement. While it is possible to export as a different format (i.e. txt or asc) it's not efficient because one has to change the export format after every measurement. Here comes the treat: Just export as binary and use this package to work with binary files directly.
 
 After reading all channels from the binary file, the channels are analyzed and every measure-channel will receive a reference to a time channel, depending on the amount of entries in the channels and the fact, that the time-channel has to contain "time" or "zeit" in its name. What that means is, that a channel with x entries and the name "time - 1" will be regarded as the time-channel of any other channel with x Data Entries.
 
 Here is an example plot, generated directly from a binary file:
 ![apread_demo_out_1](https://user-images.githubusercontent.com/13386367/169707732-240a916e-228f-4ef9-8c3c-e560a2647c97.png)
 
-
 ## Installation/Update
 
 Anywhere with python (note the uppercase U):
 
 ```sh
 pip install -U apread
 ```
 
 ## How it works
+
 The workflow of the package is straight-forward. You supply a binary file created with CatmanAP and the script will read that into python.
 
 First of all, the binary data is analyzed and packaged into seperate `Channel` objects. When all `Channels` are created, each `Channel.Name` will be checked against `([T|t]ime)|([Z|z]eit)`, which mark time channels which usually are the reference.
 
 These `Channels` marked as `istime` are the basis for `Groups`. Inside a group you will find the `ChannelX` (time channel) and a bunch of other channels in `ChannelsY`, which are the channels containing data in that time domain. The corresponding channels inside a `Group` are found by analyzing their length. Since the total time measured is the same for all groups, it is assumed that `Channels` with the same data-length belong to the same group. Connecting the matching channels to the group give a structured representation of your measurement data.
 
 Now that the Data is available in python you are free to do with that whatever you want. Until Version `1.0.x` there were some features in which you can save the data but that feature has been removed.
 
 ## Usage
 
-Lets say you produced a file called `measurements.bin` and you put it in the directory of your python script, then you can create the `APReader` on that file. It's that simple. The Initialization may take some time depending on how large your .bin-File is. 
+Lets say you produced a file called `measurements.bin` and you put it in the directory of your python script, then you can create the `APReader` on that file. It's that simple. The Initialization may take some time depending on how large your .bin-File is.
 
 ```python
 from apread import APReader
 
 reader = APReader('measurements.bin')   # this will read in the file
-``` 
+```
 
 ### Print channels
+
 Afterwards you can access the `Channels` by accessing the `APReader.Channels` Member. `Channel` and `Group` implement `__str__` which will return the name and the length of data inside it.
 
 ```python
 for channel in reader.Channels:
     print(channel)
 
 # "Timechannel 1 - Standard" (120341 Entries)
 # "T12_ref" (120341 Entries)
 # "T33" (120341 Entries)
 # "Timechannel 1 - Quick" (3022344 Entries)
 # "F1" (3022344 Entries)
 # "ast089" (3022344 Entries)
-``` 
+```
 
 ```python
 for group in reader.Groups:
     print(group)
 
 # "Timechannel 1 - Standard" (2 Data-channels, 120341 Entries)
 # "Timechannel 1 - Quick" (2 Data-channels, 3022344 Entries)
-``` 
+```
 
 ### Plot Channels/Groups
+
 To review your data on the fly, you can plot every entity in the data structure by calling `.plot()`. When plotting, every group will get its own figure window, in which all connected channels are plotted.
 
 ```python
 # plot the readers data
 reader.plot()
 # plot all groups
 for group in reader.Groups:
     group.plot()
 # plot all channels
 for channel in reader.Channels:
     channel.plot()
-``` 
+```
 
 As you can see, you can access the channels from the reader, which contains all channels (including time channels) or you can access them from the groups.
 
 There are some more functions to plot specific data. When plotting multiple channels each channel gets its own y-axis.
+
 ```python
 group.plotChannel(0)           # specific channel
 group.plotChannels(0,3)        # channel 1 to 3 (1,2,3)
 group.plot([0, 2, 4])          # channel 1, 3 and 5
-``` 
+```
 
 The same can be applied to the `APReader`. The only difference is that you can plot specific groups instead of channels.
+
 ```python
 reader.plotGroup(0)           # specific group
 reader.plotGroups(0,3)        # group 1 to 3 (1,2,3)
 reader.plot([0, 2, 4])        # group 1, 3 and 5
 ``` 
+
 ### External Header
+
 Thanks to ([hakonbars PR13](https://github.com/leonbohmann/APReader/pull/13)) you are now able to access external header information using `channel.exthdr`, a dicitionary containing all keys as described in [this sheet](https://github.com/leonbohmann/APReader/blob/dev-2/test/catmanBinaryFormat.xls).
 
 ```python
 ['T0']                 # ACQ timestamp info (NOW format) 
 ['dt']                 # ACQ delta t in ms
 ['SensorType']         # IDS code of sensor type
 ['SupplyVoltage']      # IDS code supply voltage
@@ -138,67 +143,116 @@
 ['SoftwareTareVal']    # Software tare (zero) for channels carrying a user scale
 ['WriteProtected']     # If true, write access is denied
 ['NominalRange']       # CAV value
 ['CLCFactor']          # Cable length compensation factor (CANHEAD only)
 ['ExportFormat']       # 0=8-Byte Double, 1=4-Byte Single, 2=2-Byte Integer (FOR CATMAN BINARY EXPORT ONLY!)    
 ```
 
+### Parallel reading of data
+
+> Only available from version `v1.1.1-alpha1` and above
+
+See `test/testing.py` for a full example. Modify the following around your `APReader` call:
+
+```python
+import multiprocessing as mp
+...
+
+
+if __name__ == '__main__': # this line has to be included!
+    # without 'processes=...'!
+    pool = mp.Pool() 
+
+    # pass the pool to the reader
+    reader = APReader(file, parallelPool=pool)
+
+    # make sure to close the pool after you are done with it
+    mp.close()
+    mp.join()
+```
+
+For the parallel loading to work, you have to define a parallel pool of processes in your top-level script. These processes will be accessed from within `APReader`-Functions. When passing no arguments to `mp.Pool()` it will automatically create as many processes as possible, according to the amount of threads your CPU allows (cores + virtual cores). It does not make sense to pass in more, since the `APReader` spawns the same amount of processes as there are CPU Threads. Increasing the amount of processes in your pool does not increase the amount of parallelism. It is fixed.
 
+> Keep in mind, that parallelisation is not always faster. Spawning of processes is expensive and can be wasteful for small files.
 
+The results from `APReader` stay the same and you can continue your analysis.
 
 ## Release History
-### **Version 1.1**
 
-#### Breaking changes
+### Version 1.1.1-alpha1
+
+* Added converted timestamp property on channels (`Channel.date`)
+  * *Property `Channel.time` will be deleted at some point in the future...*
+* Parallel reading of binary files
+  * Max degree of parallelism is defined with maximum amount of processors
+* ----------------------------
+* ----------------------------
+  
+#### Version 1.1
+
+##### Breaking changes
 
 * Removed saving functions, this will be up to the user
     > Since these function change a lot based on current needs, I decided to remove the post-processing functionality completely. The user now needs to do the post-processing on his own, meaning the creation of plots using time and data channels...
 
-#### Changes
+##### Changes
+
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Differentiate floating point precision
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Reading additional header information
 * ([hakonbar PR13](https://github.com/leonbohmann/APReader/pull/13)) Supplying binary format reference
 * Fixed null returning string conversion function
 * Using regex to find time channels
 * Improved plotting with multiple axes
 * Printing channels and groups will now give a summary instead of all data
 
-
 #### Version 1.0.22
+
 * Fixed an issue with groups where time channels are not recognized
-*  now, user is prompted, when suspected time channel is found
-*  plotting is not possible when there is no time-channel found
-*  save groups and channels even when there is no time channel
+* now, user is prompted, when suspected time channel is found  
+* plotting is not possible when there is no time-channel found
+* save groups and channels even when there is no time channel
+
 #### Version 1.0.21
+
 * Updated serialisation-procedures to always encode in `UTF-8`
+
 #### Version 1.0.20
+
 * Switched to explicit type hinting with `typing` package (compatibility issues with python <3.9.x)  
+
 #### Version 1.0.15/16
+
 * Fixed an issue with saving and non-existent directories
 * Added `getas` to generate formatted string without saving
+
 #### Version 1.0.14
+
 * Output file-names updated
+
 #### Version 1.0.12/13
+
 * Group channels with their time-channel into "groups"
 * Multiple plot modes:
-    * Whole file
-    * Channel/Group only
+  * Whole file
+  * Channel/Group only
 * Output data
-    * json
-    * csv
+  * json
+  * csv
 
 #### Version 1.0.11
+
 * Progressbars indicate read-progress of files
 * Multiple plot modes
 
 #### Version 1.0.0
+
 * Convert catman files to channels
 
 ## Meta
 
 Leon Bohmann – mail@leonbohmann.de
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
 
-[https://github.com/leonbohmann/apreader](https://github.com/leonbohmann/apreader)
-
+This software comes with no warranty, expressed or implied. Use at your own risk!
 
+[https://github.com/leonbohmann/apreader](https://github.com/leonbohmann/apreader)
```

### Comparing `apread-1.1.0/setup.py` & `apread-1.1.1a1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="apread",
-    version="1.1.0",
+    version="1.1.1-alpha1",
     description="Import data from CatmanAP binary files.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/leonbohmann/apreader",
     author="Leon Bohmann",
     author_email="mail@leonbohmann.de",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
     ],
     packages=['apread'],
-    install_requires=['matplotlib', 'plotly', 'scipy', 'typing', 'tqdm', 'pandas'],
+    install_requires=['matplotlib', 'typing', 'tqdm', 'pandas', 'multiprocessing'],
     include_package_data=True,
 )
```

