# Comparing `tmp/hkhklab-0.0.2.tar.gz` & `tmp/hkhklab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkhklab-0.0.2.tar", last modified: Tue Apr 25 07:11:13 2023, max compression
+gzip compressed data, was "hkhklab-0.0.3.tar", last modified: Tue Apr 25 07:18:17 2023, max compression
```

## Comparing `hkhklab-0.0.2.tar` & `hkhklab-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 07:11:13.760107 hkhklab-0.0.2/
--rw-rw-rw-   0        0        0      226 2023-04-25 07:11:13.758110 hkhklab-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 07:11:13.729108 hkhklab-0.0.2/hkhklab/
--rw-rw-rw-   0        0        0     1225 2023-04-25 06:56:52.000000 hkhklab-0.0.2/hkhklab/__init__.py
--rw-rw-rw-   0        0        0      372 2023-04-25 07:09:43.000000 hkhklab-0.0.2/hkhklab/commonFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-25 07:11:13.755110 hkhklab-0.0.2/hkhklab.egg-info/
--rw-rw-rw-   0        0        0      226 2023-04-25 07:11:13.000000 hkhklab-0.0.2/hkhklab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-25 07:11:13.000000 hkhklab-0.0.2/hkhklab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 07:11:13.000000 hkhklab-0.0.2/hkhklab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 07:11:13.000000 hkhklab-0.0.2/hkhklab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 07:11:13.760107 hkhklab-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-04-25 07:10:16.000000 hkhklab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:18:17.646537 hkhklab-0.0.3/
+-rw-rw-rw-   0        0        0      226 2023-04-25 07:18:17.644537 hkhklab-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 07:18:17.622551 hkhklab-0.0.3/hkhklab/
+-rw-rw-rw-   0        0        0     1225 2023-04-25 06:56:52.000000 hkhklab-0.0.3/hkhklab/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-04-25 07:17:56.000000 hkhklab-0.0.3/hkhklab/commonFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:18:17.641538 hkhklab-0.0.3/hkhklab.egg-info/
+-rw-rw-rw-   0        0        0      226 2023-04-25 07:18:16.000000 hkhklab-0.0.3/hkhklab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-25 07:18:17.000000 hkhklab-0.0.3/hkhklab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:18:16.000000 hkhklab-0.0.3/hkhklab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 07:18:16.000000 hkhklab-0.0.3/hkhklab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:18:17.647536 hkhklab-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-04-25 07:18:06.000000 hkhklab-0.0.3/setup.py
```

### Comparing `hkhklab-0.0.2/hkhklab/__init__.py` & `hkhklab-0.0.3/hkhklab/__init__.py`

 * *Files identical despite different names*

### Comparing `hkhklab-0.0.2/setup.py` & `hkhklab-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 module_name = item
             packages[module_name] = dir
             packages.update(find_packages(dir, module_name))
     return packages
 
 # 패키지 폴더명 작성
 setup(name="hkhklab", # 패키지 폴더명으로 수정
-      version="0.0.2", # 버전은 처음 0.0.1 이후 증가
+      version="0.0.3", # 버전은 처음 0.0.1 이후 증가
       url="http://github.com/hyokwan/hkhklab", # 코드 저장한 url 정의
       license="MIT", # 기본세팅
       author="kimhyokwan", #본인정보로 수정
       author_email="haiteam@kopo.ac.kr", #본인정보로 수정
       keywords=["listsum"], #본인정보로 수정
       description="calculate list sum and so on", #본인정보로 수정
       packages=find_packages("."),
```

