# Comparing `tmp/Video_Audio_Image_Downloader-0.0.9.tar.gz` & `tmp/Video_Audio_Image_Downloader-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Video_Audio_Image_Downloader-0.0.9.tar", last modified: Mon Apr 24 06:33:50 2023, max compression
+gzip compressed data, was "Video_Audio_Image_Downloader-0.1.0.tar", last modified: Tue Apr 25 11:27:18 2023, max compression
```

## Comparing `Video_Audio_Image_Downloader-0.0.9.tar` & `Video_Audio_Image_Downloader-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2165 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1770 2023-04-24 05:55:53.000000 Video_Audio_Image_Downloader-0.0.9/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2165 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      413 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      889 2023-04-24 06:33:07.000000 Video_Audio_Image_Downloader-0.0.9/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 10:56:32.000000 Video_Audio_Image_Downloader-0.0.9/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2209 2023-04-24 06:30:32.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/Command_function.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2748 2023-04-24 05:51:48.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/help.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4510 2023-04-24 06:23:30.000000 Video_Audio_Image_Downloader-0.0.9/source/source.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 11:27:18.686221 Video_Audio_Image_Downloader-0.1.0/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3753 2023-04-25 11:27:18.686221 Video_Audio_Image_Downloader-0.1.0/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3466 2023-04-25 11:22:55.000000 Video_Audio_Image_Downloader-0.1.0/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 11:27:18.686221 Video_Audio_Image_Downloader-0.1.0/Video_Audio_Image_Downloader.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3753 2023-04-25 11:27:18.000000 Video_Audio_Image_Downloader-0.1.0/Video_Audio_Image_Downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      413 2023-04-25 11:27:18.000000 Video_Audio_Image_Downloader-0.1.0/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-25 11:27:18.000000 Video_Audio_Image_Downloader-0.1.0/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-25 11:27:18.000000 Video_Audio_Image_Downloader-0.1.0/Video_Audio_Image_Downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-25 11:27:18.000000 Video_Audio_Image_Downloader-0.1.0/Video_Audio_Image_Downloader.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-25 11:27:18.686221 Video_Audio_Image_Downloader-0.1.0/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      914 2023-04-25 11:26:49.000000 Video_Audio_Image_Downloader-0.1.0/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 11:27:18.686221 Video_Audio_Image_Downloader-0.1.0/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 11:22:56.000000 Video_Audio_Image_Downloader-0.1.0/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-25 11:27:18.686221 Video_Audio_Image_Downloader-0.1.0/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-25 11:22:57.000000 Video_Audio_Image_Downloader-0.1.0/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2171 2023-04-25 11:22:57.000000 Video_Audio_Image_Downloader-0.1.0/source/lib/Command_function.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-25 11:22:57.000000 Video_Audio_Image_Downloader-0.1.0/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2844 2023-04-25 11:22:57.000000 Video_Audio_Image_Downloader-0.1.0/source/lib/help.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4463 2023-04-25 11:22:56.000000 Video_Audio_Image_Downloader-0.1.0/source/source.py
```

### Comparing `Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/PKG-INFO` & `Video_Audio_Image_Downloader-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,120 @@
 Metadata-Version: 2.1
-Name: Video-Audio-Image-Downloader
-Version: 0.0.9
+Name: Video_Audio_Image_Downloader
+Version: 0.1.0
 Summary: In this tool is help to Download the Youtube Video,Audio and Any type of Google and other site's Images
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/audio_video_image_downloder-1
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
+# Downloder - To download Video and Audio and Any type of Images
 
-## Download
+`Downloader` is a Downloading tool,is used to `download the Youtube Video's`With specified path with specified Resolution.
+It is used to `download the Audio's` with specified path with specified name of the Audio file and `Download the images` with any type of image's with their image source address or image address
 
-#### Prerequisites
+## Prerequisites
 
 
 On Ubuntu/Debian:
 
 
     sudo apt install update
     sudo apt install upgrade
 
 
-#### Usage
+## Installation
 
+Use pip/pip3 to install from PyPI
 
-To download the Youtube video's and Audio's And Download Any type of Image's.
+    $ pip install Video-Audio-Image-Downloader
 
-    Downloader [Option..]
+You can also use Python from your command prompt
 
+    $ python -m pip install Video-Audio-Image-Downloader
 
+## Usage of `Downloader`
 
 
-## Table of Contents
+To download the Youtube video's and Audio's And Download Any type of Image's.
 
+    Downloader [Option..]
 
 
+With `Downloader`, you can download any YouTube Video and Audio you want, over a few commands. The following section of the documentation is to guide you on how to use `Downloder` tool.
 
-## Installation
 
-Use pip/pip3 to install from PyPI
+### Download YouTube Videos
 
-    $ pip install <Tool NAME>
+To Download a YouTube Video from your default web browser or Direct from Youtube Platform , use the following syntax:
 
-You can also use Python from your command prompt
+    Usage: Downloader Youtube Video [-source="Youtube video link" -resolution="Youtube video resolution" -path="file path"]
 
-    $ python -m pip install <Tool NAME>
+    Positional arguments:
 
-## Features
-1.  Download the youtube video with specified Resolution
-2.  Downlaod the Youtube audio with specified name with specified path name
-3.  Download the youtube video with or without specified the youtube resolution's
-4.  Downlaod Image with specified Image copy address with specified path
-5.  
-6.
-7.
+            -source
+                        Source or Link of the Video file
 
-## Usage
+    optional arguments:
 
-With Downloader, you can download any YouTube Video and Audio you want, over a few commands. The following section of the documentation is to guide you on how to use Downloders.
+            -resolution
+                            The Resolution of the Video's to Download.
+                            For now, the default value 730p.
 
+            -path           
+                            The Path of the Video's to download.
+                            For now,The default path is your Current Working Directory
 
-### Download YouTube Videos
+            -h,--help
+                            List information about the Command
+
+
+##### Get the Resolution of the Video file
+To get a YouTube Video Resolution of the Video file, use the following syntax:
+
+    Usage: Downloader Youtube Video  -get_resolution [-get_url="Source of the Video file"]
+        
+        
+    Positional arguments:
 
-To Download a YouTube Video from your default web browser or DIrect from Youtube Platform , use the following syntax:
+            -get_url
+                    We provide the source of the Video file's
 
-    Usage: Downloader Youtube video [-source="Youtube video link" -resolution="Youtube video resolution" ]
+    optional arguments:
+            -h,--help
+                    List information about the Command
+            
 
 
 ### Download YouTube Audios
 
 To Download a YouTube Audio from your default web browser or DIrect from Youtube Platform , use the following syntax:
 
-    Usage: Downloader Youtube Audio [-source="Youtube video link" -path="which path the file to be saved" -filename="Your Audio filename"]
+    Usage: Downloader Youtube Audio [-source="Youtube Audio link" -path="which path the file to be saved" -filename="Your Audio filename"]
+    
+    Positional arguments:
+
+            -source
+                        Source or Link of the Audio file
+
+    optional arguments:
+    
+            -resolution
+                            The Resolution of the Audio's to Download.
+                            For now, the default value 730p.
+
+            -path           
+                            The Path of the Audio's to download.
+                            For now,The default path is your Current Working Directory
+
+
 
-### Download Any type of Images
+##### Download Any type of Images
 
 To Download Any type of Images from your default web browser or Any type of online  Platform , use the following syntax:
 
     Usage: Downloader Image [-source="Image address link" -path="which path the file to be saved" -filename="Your Image filename"]
```

### Comparing `Video_Audio_Image_Downloader-0.0.9/source/lib/Argument.py` & `Video_Audio_Image_Downloader-0.1.0/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.0.9/source/lib/Command_function.py` & `Video_Audio_Image_Downloader-0.1.0/source/lib/Command_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
                 return_value = resolutions.append(stream.resolution)
         if resolutions is not None:
             return resolutions
         else:
             return False
     
 
-    def Youtube_Download_Audio(self,url,user_path,user_filename):
+    def Youtube_Download_Audio(self,url,user_path):
         print(f"Wait untill few seconds.. Your Downloader is Processing..")
         yt = YouTube(url)
         audio = yt.streams.filter(only_audio=True).first()
-        return_value = audio.download(output_path=user_path, filename=user_filename)
+        return_value = audio.download(output_path=user_path)
         if return_value:
             return True
         else:
             return False
 
     # def Other_Downloading_Resources(url):
     #     print(f"Wait untill few seconds.. Your Downloader is Processing..")
```

### Comparing `Video_Audio_Image_Downloader-0.0.9/source/lib/help.py` & `Video_Audio_Image_Downloader-0.1.0/source/lib/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,41 +13,42 @@
         print("   -get_resolution       Show's the Resolution of the Youtube")
         print()
         print("Optional arguments : ")
         print("-h, --help   show this help message and exit")
         
         
     def Youtube_Download_video_help(self):
-        print(f"Usage: <downloder> youtube video [Options]...")
+        
+        print(f"Usage: <Downloader> Youtube Video [Options]...")
         print()
         print("Description :: ")
-        print("In this command is used to Download Youtube Video's with Specified Path with Specifed Resolution")
+        print("             In this command is used to Download Youtube Video's with Specified Path with Specifed Resolution")
         print()
         print("Options  are :")
         print()
-        print("positional arguments : ")
-        print("   -source       Source of our Youtube Video")
-        print("   -resolution   Resolution of our Youtube Video")
-        print("   -path         which path the file to be saved")
+        print("positional arguments :: ")
+        print("         -source             Source of our Youtube Video")
         print()
-        print("Optional arguments : ")
-        print("-h, --help   show this help message and exit")
+        print("Optional arguments :: ")
+        print("         -resolution         Resolution of our Youtube Video")
+        print("         -path               which path the file to be saved")
+        print("-h,      --help              show this help message and exit")
         
     def Youtube_Download_Audio_help(self):
         print("Usage: <downloder> youtube audio [Options]...")
         print()
         print("Description :: ")
         print("In this command is used to Download Youtube Audio's with Specified Path with Specifed Resolution")
         print()
         print("Options  are :")
         print()
         print("positional arguments : ")
-        print("   -source       Source of our Youtube Audio")
-        print("   -filename     Name of the Audio File")
-        print("   -path         which path the file to be saved")
+        print("         -source       Source of our Youtube Audio")
+        print("         -filename     Name of the Audio File")
+        print("         -path         which path the file to be saved")
         print()
         print("Optional arguments : ")
         print("   -h, --help   show this help message and exit")
 
     def Image_Download_help(self):
         print("Usage: <downloder> Image [Options]...")
         print()
```

### Comparing `Video_Audio_Image_Downloader-0.0.9/source/source.py` & `Video_Audio_Image_Downloader-0.1.0/source/source.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,57 +15,61 @@
 
 def Help():
     print("<Downloder> [Options].. ")
 
 
 
 def main():
-    
+    #TODO: if no resolution is not mentioned means download default resloution
     if Argument.hasCommands(['Youtube']):
-        if Argument.hasCommands(['video']): # Check the option has video or audio
+        if Argument.hasCommands(['Video']): 
+            resolution = None
+            path = None
             if Argument.hasOptionValue('-source'):
+                url = Argument.getoptionvalue('-source')
+                if Argument.hasOptionValue('-path'):
+                    path = Argument.getoptionvalue('-path')
+                else:
+                    path = '.'
                 if Argument.hasOptionValue('-resolution'):
-                    if Argument.hasOptionValue('-path'):
-                        if Argument.hasOptionValue('-resolution'):
-                            url = Argument.getoptionvalue('-source')
-                            resolution = Argument.getoptionvalue('-resolution')
-                            path = Argument.getoptionvalue('-path')
-                            if Youtube_Download_video(url,resolution,path):
-                                print("Your Video is succesfully Downloaded")
-                            else:
-                                print("Your Video downloading operation is failed")
+                    resolution = Argument.getoptionvalue('-resolution') 
+                else:
+                    resolution = '720p'
+                if Command_function.Youtube_Download_video(url,resolution,path):
+                    print("Your Video is succesfully Downloaded")
+                else:
+                    print("Your Video downloading operation is failed")
                                     
             elif Argument.hasOption(['-h']) or Argument.hasOption(['--help']):
                 help.Youtube_Download_video_help() 
                 
             elif Argument.hasOption(['-get_resolution']):
                 if Argument.hasOptionValue('-get_url'):
                     url = Argument.getoptionvalue('-get_url')
-                    resolution = Youtube_Download_video_Resolution(url)
+                    resolution = Command_function.Youtube_Download_video_Resolution(url)
                     print(f"Available Resolution :: {resolution}")
                 elif Argument.hasOption(['-h']) or Argument.hasOption(['--help']):
                     help.Youtube_Download_video_Resolution_help()
-                    
-        else:
-            help.Youtube_Download_video_help()
+            else:
+                help.Youtube_Download_video_help()
         
                                 
         if Argument.hasCommands(['Audio']):
             if Argument.hasOptionValue('-source'):
-                if Argument.hasOptionValue('-filename'):
-                    if Argument.hasOptionValue('-path'):
-                        url = Argument.getoptionvalue('-source')
-                        path = Argument.getoptionvalue('-path')
-                        filename = Argument.getoptionvalue('-filename')
-                        if Youtube_Download_Audio(url,path,filename):
-                            print("Your Audio file is Successfully Downloaded")
-                            print(f"Your Audio file is saved in this Location :: {Argument.getoptionvalue('-path')}")
-                            print(f"Your Audio file name is :: {Argument.getoptionvalue('-filename')}")
-                        else:
-                            print("Your Audio downloading operation is failed")
+                url = Argument.getoptionvalue('-source')
+                if Argument.hasOptionValue('-path'):
+                    path = Argument.getoptionvalue('-path')
+                else:
+                    path = '.'
+                if Command_function.Youtube_Download_Audio(url,path):
+                    print("Your Audio file is Successfully Downloaded")
+                    print(f"Your Audio file is saved in this Location :: {Argument.getoptionvalue('-path')}")
+                    print(f"Your Audio file name is :: {Argument.getoptionvalue('-filename')}")
+                else:
+                    print("Your Audio downloading operation is failed")
             elif Argument.hasOption(['-h']) or Argument.hasOption(['--help']):
                 help.Youtube_Download_Audio_help()
             else:
                 help.Youtube_Download_Audio_help()
                     
     if Argument.hasCommands(['Image']):  #TODO: to download any type of picture formates like .png, .jpg ...
         if Argument.hasOptionValue('-source'):
```

