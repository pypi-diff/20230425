# Comparing `tmp/jmcomic-1.6.0.tar.gz` & `tmp/jmcomic-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-rlqqn138/jmcomic-1.6.0.tar", last modified: Fri Apr 21 08:02:13 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-gp4omas4/jmcomic-1.7.0.tar", last modified: Tue Apr 25 03:16:19 2023, max compression
```

## Comparing `jmcomic-1.6.0.tar` & `jmcomic-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 08:02:02.000000 jmcomic-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-21 08:02:13.000000 jmcomic-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-21 08:02:02.000000 jmcomic-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:02:13.000000 jmcomic-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-21 08:02:02.000000 jmcomic-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 03:16:07.000000 jmcomic-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-25 03:16:19.000000 jmcomic-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-25 03:16:07.000000 jmcomic-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 03:16:19.000000 jmcomic-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 03:16:07.000000 jmcomic-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-04-25 03:16:07.000000 jmcomic-1.7.0/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 03:16:19.000000 jmcomic-1.7.0/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-1.6.0/LICENSE` & `jmcomic-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-1.6.0/PKG-INFO` & `jmcomic-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,15 +34,14 @@
 
   ```shell
   pip install jmcomic -i https://pypi.org/project --upgrade
   ```
 * 本地安装
 
   ```shell
-  cd ./modules/core/
   pip install -e ./
   ```
 
 ## 快速上手
 
 使用下面的两行代码，即可实现功能：把某个本子集（album）里的所有本子（photo）下载到本地
```

### Comparing `jmcomic-1.6.0/README.md` & `jmcomic-1.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
   ```shell
   pip install jmcomic -i https://pypi.org/project --upgrade
   ```
 * 本地安装
 
   ```shell
-  cd ./modules/core/
   pip install -e ./
   ```
 
 ## 快速上手
 
 使用下面的两行代码，即可实现功能：把某个本子集（album）里的所有本子（photo）下载到本地
```

### Comparing `jmcomic-1.6.0/setup.py` & `jmcomic-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.6.0/src/jmcomic/api.py` & `jmcomic-1.7.0/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.6.0/src/jmcomic/jm_client.py` & `jmcomic-1.7.0/src/jmcomic/jm_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -179,14 +179,20 @@
             )(func)
 
             setattr(self, func_name, wrap_func)
 
         wrap_func_cache('get_photo_detail', 'album_cache_dict')
         wrap_func_cache('get_album_detail', 'photo_cache_dict')
 
+    def get_jmcomic_url(self, postman=None):
+        return JmModuleConfig.get_jmcomic_url(postman or self)
+
+    def get_jmcomic_url_all(self, postman=None):
+        return JmModuleConfig.get_jmcomic_url_all(postman or self)
+
 
 # 爬取策略
 class FetchStrategy:
 
     def __init__(self,
                  from_index,
                  photo_len,
```

### Comparing `jmcomic-1.6.0/src/jmcomic/jm_config.py` & `jmcomic-1.7.0/src/jmcomic/jm_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -70,23 +70,41 @@
     @classmethod
     def disable_jm_debug(cls):
         cls.enable_jm_debug = False
 
     @classmethod
     def get_jmcomic_url(cls, postman=None):
         """
-        访问禁漫的永久网域，从而得到一个可用的禁漫网址，
+        访问禁漫的永久网域，从而得到一个可用的禁漫网址
+        @return: https://jm-comic2.cc
         """
         if postman is None:
             from common import Postmans
             postman = Postmans.get_impl_clazz('cffi_Session').create()
 
-        domain = postman.with_redirect_catching().get(cls.JM_REDIRECT_URL)
-        cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{domain}]')
-        return domain
+        url = postman.with_redirect_catching().get(cls.JM_REDIRECT_URL)
+        cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{url}]')
+        return url
+
+    @classmethod
+    def get_jmcomic_url_all(cls, postman=None):
+        """
+        访问禁漫发布页，得到所有禁漫的域名
+        @return：['18comic.vip', ..., 'jm365.xyz/ZNPJam'], 最后一个是【APP軟件下載】
+        """
+        if postman is None:
+            from common import Postmans
+            postman = Postmans.get_impl_clazz('cffi').create()
+
+        resp = postman.get(cls.JM_PUB_URL)
+        if resp.status_code != 200:
+            raise AssertionError(resp.text)
+
+        from .jm_toolkit import JmcomicText
+        return JmcomicText.analyse_jm_pub_html(resp.text)
 
     @classmethod
     def check_html(cls, html: str, url=None):
         html = html.strip()
         error_msg = cls.JM_ERROR_RESPONSE_HTML.get(html, None)
         if error_msg is None:
             return
```

### Comparing `jmcomic-1.6.0/src/jmcomic/jm_entity.py` & `jmcomic-1.7.0/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.6.0/src/jmcomic/jm_option.py` & `jmcomic-1.7.0/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.6.0/src/jmcomic/jm_service.py` & `jmcomic-1.7.0/src/jmcomic/jm_service.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.6.0/src/jmcomic/jm_toolkit.py` & `jmcomic-1.7.0/src/jmcomic/jm_toolkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .jm_entity import *
 
 
 class JmcomicText:
     pattern_jm_domain = compile('https://([\w.-]+)')
     pattern_jm_pa_id = compile('/(photos?|album)/(\d+)')
+    pattern_html_jm_pub_domain = compile('[\w-]+\.\w+/?\w+')
 
     pattern_html_photo_photo_id = compile('<meta property="og:url" content=".*?/photo/(\d+)/?.*?">')
     pattern_html_photo_scramble_id = compile('var scramble_id = (\d+);')
     pattern_html_photo_title = compile('<title>(.*?)\|.*</title>')
     # pattern_html_photo_data_original_list = compile('data-original="(.*?)" id="album_photo_.+?"')
     pattern_html_photo_data_original_domain = compile('src="https://(.*?)/media/albums/blank')
     pattern_html_photo_keywords = compile('<meta name="keywords" content="(.*?)" />')
@@ -70,14 +71,23 @@
             return match[2]
 
     @classmethod
     def parse_to_album_id(cls, text) -> str:
         return cls.parse_to_photo_id(text)
 
     @classmethod
+    def analyse_jm_pub_html(cls, html: str, domain_keyword=('jm', 'comic')) -> List[str]:
+        domain_ls = cls.pattern_html_jm_pub_domain.findall(html)
+
+        return list(filter(
+            lambda domain: any(kw in domain for kw in domain_keyword),
+            domain_ls
+        ))
+
+    @classmethod
     def analyse_jm_photo_html(cls, html: str) -> JmPhotoDetail:
         return cls.reflect_new_instance(
             html,
             "pattern_html_photo_",
             JmPhotoDetail
         )
```

### Comparing `jmcomic-1.6.0/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-1.7.0/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,15 +34,14 @@
 
   ```shell
   pip install jmcomic -i https://pypi.org/project --upgrade
   ```
 * 本地安装
 
   ```shell
-  cd ./modules/core/
   pip install -e ./
   ```
 
 ## 快速上手
 
 使用下面的两行代码，即可实现功能：把某个本子集（album）里的所有本子（photo）下载到本地
```

