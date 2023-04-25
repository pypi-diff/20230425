# Comparing `tmp/cppiniter-1.0.4.tar.gz` & `tmp/cppiniter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppiniter-1.0.4.tar", last modified: Thu Feb 17 06:31:20 2022, max compression
+gzip compressed data, was "cppiniter-1.0.5.tar", last modified: Tue Apr 25 02:19:08 2023, max compression
```

## Comparing `cppiniter-1.0.4.tar` & `cppiniter-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:31:20.106600 cppiniter-1.0.4/
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)     1051 2022-02-17 06:30:44.000000 cppiniter-1.0.4/LICENSE
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       30 2022-02-17 06:30:47.000000 cppiniter-1.0.4/MANIFEST.in
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      404 2022-02-17 06:31:20.106600 cppiniter-1.0.4/PKG-INFO
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)     1602 2022-02-17 06:30:49.000000 cppiniter-1.0.4/README.md
-drwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:31:20.096600 cppiniter-1.0.4/cppiniter/
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:30:44.000000 cppiniter-1.0.4/cppiniter/__init__.py
--rwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)     3072 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/cppiniter.py
-drwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:31:20.106600 cppiniter-1.0.4/cppiniter/files/
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)     2062 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/.clang-format
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)     8926 2022-02-17 06:30:45.000000 cppiniter-1.0.4/cppiniter/files/.gitignore
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)     1747 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       21 2022-02-17 06:30:44.000000 cppiniter-1.0.4/cppiniter/files/README.md
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       45 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/conanfile.txt
-drwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:31:20.106600 cppiniter-1.0.4/cppiniter/files/src/
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      588 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/src/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      145 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/src/main.cpp
-drwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:31:20.106600 cppiniter-1.0.4/cppiniter/files/test/
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      399 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/test/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      147 2022-02-17 06:30:49.000000 cppiniter-1.0.4/cppiniter/files/test/main_cpp
-drwxr-xr-x   0 xyz1001   (1001) xyz1001   (1001)        0 2022-02-17 06:31:20.106600 cppiniter-1.0.4/cppiniter.egg-info/
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      404 2022-02-17 06:31:19.000000 cppiniter-1.0.4/cppiniter.egg-info/PKG-INFO
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      557 2022-02-17 06:31:19.000000 cppiniter-1.0.4/cppiniter.egg-info/SOURCES.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)        1 2022-02-17 06:31:19.000000 cppiniter-1.0.4/cppiniter.egg-info/dependency_links.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       56 2022-02-17 06:31:19.000000 cppiniter-1.0.4/cppiniter.egg-info/entry_points.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       25 2022-02-17 06:31:19.000000 cppiniter-1.0.4/cppiniter.egg-info/requires.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       10 2022-02-17 06:31:19.000000 cppiniter-1.0.4/cppiniter.egg-info/top_level.txt
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)       38 2022-02-17 06:31:20.106600 cppiniter-1.0.4/setup.cfg
--rw-r--r--   0 xyz1001   (1001) xyz1001   (1001)      808 2022-02-17 06:30:49.000000 cppiniter-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:19:08.266915 cppiniter-1.0.5/
+-rw-rw-rw-   0        0        0     1051 2023-04-25 01:45:21.000000 cppiniter-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-04-25 01:32:54.000000 cppiniter-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      399 2023-04-25 02:19:08.266915 cppiniter-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1668 2023-04-25 01:59:35.000000 cppiniter-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 02:19:08.251288 cppiniter-1.0.5/cppiniter/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:32:54.000000 cppiniter-1.0.5/cppiniter/__init__.py
+-rw-rw-rw-   0        0        0     3227 2023-04-25 02:05:34.000000 cppiniter-1.0.5/cppiniter/cppiniter.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:19:08.266915 cppiniter-1.0.5/cppiniter/files/
+-rw-rw-rw-   0        0        0     2062 2023-04-25 01:32:54.000000 cppiniter-1.0.5/cppiniter/files/.clang-format
+-rw-rw-rw-   0        0        0     8926 2023-04-25 01:32:54.000000 cppiniter-1.0.5/cppiniter/files/.gitignore
+-rw-rw-rw-   0        0        0     2168 2023-04-25 01:44:22.000000 cppiniter-1.0.5/cppiniter/files/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1388 2023-04-25 01:49:55.000000 cppiniter-1.0.5/cppiniter/files/CMakeSettings.json
+-rw-rw-rw-   0        0        0       21 2023-04-25 01:32:54.000000 cppiniter-1.0.5/cppiniter/files/README.md
+-rw-rw-rw-   0        0        0       55 2023-04-25 02:17:17.000000 cppiniter-1.0.5/cppiniter/files/conanfile.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 02:19:08.266915 cppiniter-1.0.5/cppiniter/files/src/
+-rw-rw-rw-   0        0        0      588 2023-04-25 01:32:54.000000 cppiniter-1.0.5/cppiniter/files/src/CMakeLists.txt
+-rw-rw-rw-   0        0        0      145 2023-04-25 01:32:54.000000 cppiniter-1.0.5/cppiniter/files/src/main.cpp
+drwxrwxrwx   0        0        0        0 2023-04-25 02:19:08.266915 cppiniter-1.0.5/cppiniter/files/test/
+-rw-rw-rw-   0        0        0      399 2023-04-25 01:42:20.000000 cppiniter-1.0.5/cppiniter/files/test/CMakeLists.txt
+-rw-rw-rw-   0        0        0      147 2023-04-25 01:42:20.000000 cppiniter-1.0.5/cppiniter/files/test/main_cpp
+drwxrwxrwx   0        0        0        0 2023-04-25 02:19:08.266915 cppiniter-1.0.5/cppiniter.egg-info/
+-rw-rw-rw-   0        0        0      399 2023-04-25 02:19:08.000000 cppiniter-1.0.5/cppiniter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-04-25 02:19:08.000000 cppiniter-1.0.5/cppiniter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 02:19:08.000000 cppiniter-1.0.5/cppiniter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-25 02:19:08.000000 cppiniter-1.0.5/cppiniter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-04-25 02:19:08.000000 cppiniter-1.0.5/cppiniter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 02:19:08.000000 cppiniter-1.0.5/cppiniter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 02:19:08.266915 cppiniter-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-04-25 01:58:46.000000 cppiniter-1.0.5/setup.py
```

### Comparing `cppiniter-1.0.4/LICENSE` & `cppiniter-1.0.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020 xyz1001
+Copyright (c) 2022 xyz1001
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cppiniter-1.0.4/README.md` & `cppiniter-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 │
 ├── .clang-format # clang format 格式化配置
 │
 ├── .gitignore # git 忽略文件
 │
 ├── CMakeLists.txt # 顶层 CMake 构建脚本
 │
+├── CMakeSettings.json # Visual Studio CMake 配置
+│
 ├── conanfile.txt # conan 包依赖配置
 │
 ├── README.md # 用来介绍这个项目
 │
 ├── src # 存放项目的源码，包括 .cpp 文件和 .h 文件
 │   │
 │   ├── CMakeLists.txt
@@ -54,8 +56,8 @@
 │   │
 │   └── main_cpp # 加快catch2的编译速度
 │
 ├── doc # 文档保存目录
 │
 └── build # 我们应该保持一棵干净的源码树，所有编译动作应该单独在这个目录进行。这个目录应加入gitignore
     │
-    └── out # 在没有指定安装目录时默认安装目录，避免安装到系统目录。
+    └── install # 在没有指定安装目录时默认安装目录，避免安装到系统目录。
```

### Comparing `cppiniter-1.0.4/cppiniter/cppiniter.py` & `cppiniter-1.0.5/cppiniter/cppiniter.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import os
 import sys
 import shutil
 import inquirer
 import pystache
 import subprocess
+import platform
 from docopt import docopt
 from datetime import datetime
 
 IGNORE_FILES = set([".git", "LICENSE"])
 EMPTY_DIR = ("build", "doc")
 
 
@@ -80,15 +81,18 @@
         else:
             exit(-1)
     return {"project_name": project_name, "project_dir": project_dir, "is_lib": is_lib, "date_time": date_time, "author": author, "email": email}
 
 
 def execute(dir):
     subprocess.run(["conan", "install", ".."], cwd=os.path.join(dir, "build"))
-    subprocess.run(["cmake", ".."], cwd=os.path.join(dir, "build"))
+    if platform.system() == "Windows":
+        subprocess.run(["cmake","-G", "Ninja", ".."], cwd=os.path.join(dir, "build"))
+    else:
+        subprocess.run(["cmake", ".."], cwd=os.path.join(dir, "build"))
 
 
 def main():
     args = docopt(__doc__, version="1.0")
     args = preprocess(args)
     install(args)
     render(args["project_dir"], args)
```

### Comparing `cppiniter-1.0.4/cppiniter/files/.clang-format` & `cppiniter-1.0.5/cppiniter/files/.clang-format`

 * *Files identical despite different names*

### Comparing `cppiniter-1.0.4/cppiniter/files/.gitignore` & `cppiniter-1.0.5/cppiniter/files/.gitignore`

 * *Files identical despite different names*

### Comparing `cppiniter-1.0.4/cppiniter/files/CMakeLists.txt` & `cppiniter-1.0.5/cppiniter/files/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 ######################################################################
 # Automatically generated by cppiniter {{{date_time}}}
 ######################################################################
 
-cmake_minimum_required(VERSION 3.6)
+cmake_minimum_required(VERSION 3.10)
 project ({{{project_name}}})
 
 if(EXISTS ${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
     include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
 else()
     include(${PROJECT_SOURCE_DIR}/build/conanbuildinfo.cmake)
 endif()
+set(CONAN_SYSTEM_INCLUDES ON)
 conan_basic_setup()
 
-# include header
 include_directories(${PROJECT_SOURCE_DIR}/src)
 include_directories(${PROJECT_SOURCE_DIR}/test)
 
-# c++11
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
 if(UNIX AND NOT ANDROID AND NOT APPLE)
     set(LINUX true)
 endif()
 
-if(MSVC)
-    add_definitions (-D_SCL_SECURE_NO_WARNINGS=1)
-    add_definitions (-D_CRT_SECURE_NO_WARNINGS=1)
+if ("${CMAKE_CXX_COMPILER_ID}" MATCHES "Clang" OR "${CMAKE_CXX_COMPILER_ID}" STREQUAL "GNU")
+    set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS_DEBUG} -Og -g3 -Werror -Wall -Wextra -Wno-unused-function -Wno-sign-compare")
+    set(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS_RELEASE} -O2")
+elseif ("${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC")
+    add_definitions(-D_SCL_SECURE_NO_WARNINGS=1)
+    add_definitions(-D_CRT_SECURE_NO_WARNINGS=1)
 
     set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS TRUE)
-    set(CMAKE_VS_INCLUDE_INSTALL_TO_DEFAULT_BUILD 1)
+    set(CMAKE_VS_INCLUDE_INSTALL_TO_DEFAULT_BUILD TRUE)
 
-    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} /EHsc /utf-8 /MP")
-    set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} /Zi")
+    string (REGEX REPLACE "/W[0-4]" "/W4" CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")
+    set(CMAKE_CXX_FLAGS "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS} /EHsc /utf-8 /MP /Zc:__cplusplus")
+    set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS_DEBUG}  /WX /wd4244 /wd4018 /wd4267")
+    set(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS_RELEASE} /Zi")
+
+    set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} /SAFESEH:NO")
     set(CMAKE_SHARED_LINKER_FLAGS_RELEASE "${CMAKE_SHARED_LINKER_FLAGS_RELEASE} /DEBUG /OPT:REF /OPT:ICF")
-elseif(LINUX)
-    set(CMAKE_CXX_FLAGS "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS} -Wall -Wextra -Werror")
-    set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} ${CMAKE_CXX_FLAGS_DEBUG} -O0 -Wall -g2 -ggdb")
-    set(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3 -Wall")
 endif()
 
 if (CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
-    set(CMAKE_INSTALL_PREFIX ${CMAKE_BINARY_DIR}/out CACHE PATH "default install prefix" FORCE)
+    set(CMAKE_INSTALL_PREFIX ${CMAKE_BINARY_DIR}/install CACHE PATH "default install prefix" FORCE)
 endif()
 
 add_subdirectory(src)
 {{#is_lib}}
 if(BUILD_TEST)
     add_subdirectory (test)
 endif()
```

### Comparing `cppiniter-1.0.4/cppiniter/files/src/CMakeLists.txt` & `cppiniter-1.0.5/cppiniter/files/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cppiniter-1.0.4/cppiniter.egg-info/SOURCES.txt` & `cppiniter-1.0.5/cppiniter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 cppiniter.egg-info/dependency_links.txt
 cppiniter.egg-info/entry_points.txt
 cppiniter.egg-info/requires.txt
 cppiniter.egg-info/top_level.txt
 cppiniter/files/.clang-format
 cppiniter/files/.gitignore
 cppiniter/files/CMakeLists.txt
+cppiniter/files/CMakeSettings.json
 cppiniter/files/README.md
 cppiniter/files/conanfile.txt
 cppiniter/files/src/CMakeLists.txt
 cppiniter/files/src/main.cpp
 cppiniter/files/test/CMakeLists.txt
 cppiniter/files/test/main_cpp
```

### Comparing `cppiniter-1.0.4/setup.py` & `cppiniter-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='cppiniter',
-    version="1.0.4",
+    version="1.0.5",
     description="C++项目脚手架",
     long_description="""用于提供C++项目开发环境的初始化""",
     keywords='c++ scaffolding',
     author='xyz1001',
     author_email='zgzf1001@gmail.com',
     url='https://github.com/xyz1001/cppiniter',
     license='MIT',
```

