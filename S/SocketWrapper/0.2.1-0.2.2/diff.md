# Comparing `tmp/SocketWrapper-0.2.1.tar.gz` & `tmp/SocketWrapper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SocketWrapper-0.2.1.tar", last modified: Mon Apr 24 17:00:47 2023, max compression
+gzip compressed data, was "SocketWrapper-0.2.2.tar", last modified: Tue Apr 25 00:20:55 2023, max compression
```

## Comparing `SocketWrapper-0.2.1.tar` & `SocketWrapper-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 17:00:47.025622 SocketWrapper-0.2.1/
--rw-r--r--   0 jarredtd   (501) staff       (20)     1073 2023-04-20 23:18:46.000000 SocketWrapper-0.2.1/LICENSE
--rw-r--r--   0 jarredtd   (501) staff       (20)     1873 2023-04-24 17:00:47.025683 SocketWrapper-0.2.1/PKG-INFO
--rw-r--r--   0 jarredtd   (501) staff       (20)     1297 2023-04-24 16:56:47.000000 SocketWrapper-0.2.1/README.md
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 17:00:47.025022 SocketWrapper-0.2.1/SocketWrapper/
--rw-r--r--   0 jarredtd   (501) staff       (20)     1130 2023-04-24 16:38:21.000000 SocketWrapper-0.2.1/SocketWrapper/Client.py
--rw-r--r--   0 jarredtd   (501) staff       (20)     1106 2023-04-24 16:37:22.000000 SocketWrapper-0.2.1/SocketWrapper/Server.py
--rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 22:24:19.000000 SocketWrapper-0.2.1/SocketWrapper/__init__.py
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 17:00:47.025520 SocketWrapper-0.2.1/SocketWrapper.egg-info/
--rw-r--r--   0 jarredtd   (501) staff       (20)     1873 2023-04-24 17:00:47.000000 SocketWrapper-0.2.1/SocketWrapper.egg-info/PKG-INFO
--rw-r--r--   0 jarredtd   (501) staff       (20)      258 2023-04-24 17:00:47.000000 SocketWrapper-0.2.1/SocketWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)        1 2023-04-24 17:00:47.000000 SocketWrapper-0.2.1/SocketWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)       14 2023-04-24 17:00:47.000000 SocketWrapper-0.2.1/SocketWrapper.egg-info/top_level.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)       79 2023-04-24 17:00:47.026030 SocketWrapper-0.2.1/setup.cfg
--rw-r--r--   0 jarredtd   (501) staff       (20)     1645 2023-04-24 17:00:35.000000 SocketWrapper-0.2.1/setup.py
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 00:20:55.056917 SocketWrapper-0.2.2/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1073 2023-04-20 23:18:46.000000 SocketWrapper-0.2.2/LICENSE
+-rw-r--r--   0 jarredtd   (501) staff       (20)     2092 2023-04-25 00:20:55.057156 SocketWrapper-0.2.2/PKG-INFO
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1516 2023-04-25 00:12:39.000000 SocketWrapper-0.2.2/README.md
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 00:20:55.053839 SocketWrapper-0.2.2/SocketWrapper/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1357 2023-04-25 00:10:43.000000 SocketWrapper-0.2.2/SocketWrapper/Client.py
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1329 2023-04-25 00:10:51.000000 SocketWrapper-0.2.2/SocketWrapper/Server.py
+-rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 22:24:19.000000 SocketWrapper-0.2.2/SocketWrapper/__init__.py
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 00:20:55.056036 SocketWrapper-0.2.2/SocketWrapper.egg-info/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     2092 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 jarredtd   (501) staff       (20)      258 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)        1 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)       14 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/top_level.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)       79 2023-04-25 00:20:55.058133 SocketWrapper-0.2.2/setup.cfg
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1645 2023-04-25 00:17:23.000000 SocketWrapper-0.2.2/setup.py
```

### Comparing `SocketWrapper-0.2.1/LICENSE` & `SocketWrapper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SocketWrapper-0.2.1/PKG-INFO` & `SocketWrapper-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SocketWrapper
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/JarredTD/Socket_Wrapper
-Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.2.tar.gz
 Author: Jarred
 Author-email: jarredtdesrosiers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,15 @@
 
 Both the server and client have error checking, which throw errors in the case of invalid input for the IP or Port.
 
 ## Table of Contents
 - [Installation](#installation)
 - [Usage](#usage)
 - [Technologies](#technologies)
+- [TODO](#todo)
 
 ## Installation
 
 To use the SocketWrapper Package, follow the steps below:
 
 1. Import the package using: `pip install SocketWrapper`
 2. Import Client from Client.py: `from SocketWrapper.Client import Client`
@@ -46,14 +47,21 @@
 
 SockerWrapper was developed using the following technologies:
 
 - Python
 - socket library
 - os library
 
+## TODO
+- Create custom exceptions
+- Create default constructors (optional \__init__ parameters)
+- Create tests
+- Add more functionality
+- Add more detail to the methods and classes of input and output
+
 ## License
 
 SocketWrapper is open source software licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `SocketWrapper-0.2.1/README.md` & `SocketWrapper-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Both the server and client have error checking, which throw errors in the case of invalid input for the IP or Port.
 
 ## Table of Contents
 - [Installation](#installation)
 - [Usage](#usage)
 - [Technologies](#technologies)
+- [TODO](#todo)
 
 ## Installation
 
 To use the SocketWrapper Package, follow the steps below:
 
 1. Import the package using: `pip install SocketWrapper`
 2. Import Client from Client.py: `from SocketWrapper.Client import Client`
@@ -30,14 +31,21 @@
 
 SockerWrapper was developed using the following technologies:
 
 - Python
 - socket library
 - os library
 
+## TODO
+- Create custom exceptions
+- Create default constructors (optional \__init__ parameters)
+- Create tests
+- Add more functionality
+- Add more detail to the methods and classes of input and output
+
 ## License
 
 SocketWrapper is open source software licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `SocketWrapper-0.2.1/SocketWrapper/Server.py` & `SocketWrapper-0.2.2/SocketWrapper/Server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 '''
-Import Server interface that the Server class is a child of
+Import Server interface that the Server class is a child of Server Interface
 '''
 
 from interfaces.ServerInterface import ServerInterface
 
 ##############################
-'''
-Server class, child of Server interface. Used as a container for the collection of the server information and automatically
-using that information.
-'''
 class Server(ServerInterface):
-    def __init__(self, ip: str, port: str) -> None:
+    '''
+    Server class, child of Server interface. Used as a container for the collection of the server information and automatically
+    using that information.
+
+    Constructing this with no arguments will default both to '', which whill cause the ip to point to the loopback, and the 
+    port to default to 12000.
+    '''
+    def __init__(self, ip: str = '', port: str = '') -> None:
         super().__init__()
         self.ip = ip
         self.port_num = port
 
         self._parse_file()
 
-    '''
-    Runs as part of the initialization. Converts the port to a int. and then binds the socket.
-    '''
     def _parse_file(self) -> None:
+        '''
+        Runs as part of the initialization. Converts the port to a int. and then binds the socket.
+        '''
         if ((self._convert_port() == False) or (self._bind_socket() == False)):
             raise StopIteration
     
-    '''
-    Takes a msg and checks if it meets a requirement. If it does, false is returned.
-    '''
     def check_end_condition(self, msg:str):
+        '''
+        Takes a msg and checks if it meets a requirement. If it does, false is returned.
+        '''
         if (msg == "exit"):
             self.send_msg(msg)
             self.connectionSocket.close()
             self.close()
             return False
         
         else:
```

### Comparing `SocketWrapper-0.2.1/SocketWrapper.egg-info/PKG-INFO` & `SocketWrapper-0.2.2/SocketWrapper.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SocketWrapper
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/JarredTD/Socket_Wrapper
-Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.2.tar.gz
 Author: Jarred
 Author-email: jarredtdesrosiers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,15 @@
 
 Both the server and client have error checking, which throw errors in the case of invalid input for the IP or Port.
 
 ## Table of Contents
 - [Installation](#installation)
 - [Usage](#usage)
 - [Technologies](#technologies)
+- [TODO](#todo)
 
 ## Installation
 
 To use the SocketWrapper Package, follow the steps below:
 
 1. Import the package using: `pip install SocketWrapper`
 2. Import Client from Client.py: `from SocketWrapper.Client import Client`
@@ -46,14 +47,21 @@
 
 SockerWrapper was developed using the following technologies:
 
 - Python
 - socket library
 - os library
 
+## TODO
+- Create custom exceptions
+- Create default constructors (optional \__init__ parameters)
+- Create tests
+- Add more functionality
+- Add more detail to the methods and classes of input and output
+
 ## License
 
 SocketWrapper is open source software licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `SocketWrapper-0.2.1/setup.py` & `SocketWrapper-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'SocketWrapper',         # How you named your package folder (MyLib)
   packages = ['SocketWrapper'],   # Chose the same as "name"
-  version = '0.2.1',      # Start with a small number and increase it with every change you make
+  version = '0.2.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Jarred',                   # Type in your name
   author_email = 'jarredtdesrosiers@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/JarredTD/Socket_Wrapper',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.2.tar.gz',    # I explain this later on
   keywords = [],   # Keywords that define your package best
   install_requires=[],        # I get to this in a second,
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

