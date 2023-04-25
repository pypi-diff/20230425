# Comparing `tmp/cnki_html2json-0.1.3.tar.gz` & `tmp/cnki_html2json-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.3.tar", last modified: Mon Apr 24 18:45:03 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.4.tar", last modified: Tue Apr 25 04:38:40 2023, max compression
```

## Comparing `cnki_html2json-0.1.3.tar` & `cnki_html2json-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.503498 cnki_html2json-0.1.3/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.165607 cnki_html2json-0.1.4/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.3/LICENSE` & `cnki_html2json-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.3/PKG-INFO` & `cnki_html2json-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
 - 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
 
-核心功能：¥
+核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
   - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
   - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
   - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
@@ -86,16 +86,16 @@
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 命令行工具参数说明：
-| 简写参数 | 参数 | 说明 |
-| --- | --- | --- |
+|  | 参数 | 说明 |
+| :-: | :-- | -- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
 | -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
@@ -118,14 +118,14 @@
 |  | abstract |  |论文摘要|
 |  | keywords |  |论文关键词|
 |  | funds |  |基金资助|
 |  | class_num |  |分类号|
 |  | source |  |发表期刊|
 |  | issue |  |发表刊号|
 | body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |citation对应本章节的参考文献索引；text对应本章节的文本|
+|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |reference对应本章节的参考文献索引；text对应本章节的文本|
 |  | 2.xxx | 2.1xxx ||
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
 ## 开源协议
 本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.3/README.md` & `cnki_html2json-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
 - 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
 
-核心功能：¥
+核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
   - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
   - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
   - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
@@ -63,16 +63,16 @@
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 命令行工具参数说明：
-| 简写参数 | 参数 | 说明 |
-| --- | --- | --- |
+|  | 参数 | 说明 |
+| :-: | :-- | -- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
 | -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
@@ -95,14 +95,14 @@
 |  | abstract |  |论文摘要|
 |  | keywords |  |论文关键词|
 |  | funds |  |基金资助|
 |  | class_num |  |分类号|
 |  | source |  |发表期刊|
 |  | issue |  |发表刊号|
 | body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |citation对应本章节的参考文献索引；text对应本章节的文本|
+|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |reference对应本章节的参考文献索引；text对应本章节的文本|
 |  | 2.xxx | 2.1xxx ||
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
 ## 开源协议
 本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.3/cnki_html2json/cli.py` & `cnki_html2json-0.1.4/cnki_html2json/cli.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.3/cnki_html2json/crawl.py` & `cnki_html2json-0.1.4/cnki_html2json/crawl.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # 调用判断验证码函数
         recogize_count = process_slider(driver)
         
         if recogize_count > 0:
             logger.info(f'验证码识别{recogize_count}次后通过')
 
         paper_raw_html = driver.page_source
-        paper_dict = html2json.ExtractContent(paper_raw_html,mode).extract_all()
+        paper_dict = html2json._ExtractContent(paper_raw_html,mode).extract_all()
         driver.close()
         if not paper_dict:
             logger.error('无法解析html页面')
         return concat_content(metadata,paper_dict)
       
     finally:
         driver.switch_to.window(handles[0]) 
@@ -114,39 +114,37 @@
     end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
     mode: 模式，structure|plain|raw，默认为structure
     save_path: 下载文件的保存路径，默认为当前目录的data文件夹
     log: 是否保存日志，默认为True
     wait_time: 为检索预留的等待时间，单位为秒
     browser_type: Chrome(默认)|Firefox|Edge|Safari
     """
-    if log:
-        if not os.path.exists(f'{save_path}/log'):
-            os.makedirs(f'{save_path}/log')
-            logger.info(f'已在{save_path}文件夹下创建log文件夹')
-
-        current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
-        logger.add(f"{save_path}/log/{current_time}.log",format="{time} {level} {message}",level="INFO",mode='w')
-        logger.info('本次任务记录日志')
-    else:
-        logger.info('本次任务不记录日志')
-
-    visited_urls = set()
 
     if not os.path.exists(save_path):
-        # os.mkdir(save_path)
-        # logger.info(f'已在当前目录创建{save_path}文件夹')
-        pass
+        os.makedirs(save_path)
+        logger.info(f'已创建{save_path}文件夹')
     else:
         save_path_files = [i for i in os.listdir(save_path) if i.endswith('.json')]
         if save_path_files and start_paper_index==1:
             cover_risk = input(f'{save_path}文件夹中已存在json文件, 覆盖请输入y, 不覆盖请输入n, 程序将退出, 请输入: ')
             if cover_risk == 'y':
                 logger.warning(f'新下载的文件将覆盖{save_path}文件夹里的文件')
             else:
                 sys.exit('程序已退出')
+    
+    if log:
+        if not os.path.exists(f'{save_path}/log'):
+            os.mkdir(f'{save_path}/log')
+            logger.info(f'已在{save_path}文件夹下创建log文件夹')
+
+        current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+        logger.add(f"{save_path}/log/{current_time}.log",format="{time} {level} {message}",level="INFO",mode='w')
+        logger.info('本次任务记录日志')
+    else:
+        logger.info('本次任务不记录日志')
             
     # 启动浏览器
     if browser_type=='Chrome':
         driver = webdriver.Chrome()
     elif browser_type=='Firefox':
         driver = webdriver.Firefox()
     elif browser_type=='Edge':
@@ -199,15 +197,15 @@
     if minutes < 60:
         logger.info(f'预计耗时 {minutes} 分钟')
     else:
         logger.info(f'预计耗时 {minutes//60} 小时 {minutes%60} 分钟')
     
     # 下载文献数据
     current_paper_index = start_paper_index
-
+    visited_urls = set()
     while current_paper_index < avaiable_records_num+1:
         current_url_list = obtain_page_papers_url(driver)[current_paper_index%papers_per_page-1:]  
         for url in current_url_list:
             
             # 避免重复下载
             if url in visited_urls:
                 logger.error(f'已下载过 {url}')
```

### Comparing `cnki_html2json-0.1.3/cnki_html2json/html2json.py` & `cnki_html2json-0.1.4/cnki_html2json/html2json.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.3/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.4/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.3/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.4/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.3/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.4/cnki_html2json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
 - 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
 
-核心功能：¥
+核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
   - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
   - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
   - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
@@ -86,16 +86,16 @@
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 命令行工具参数说明：
-| 简写参数 | 参数 | 说明 |
-| --- | --- | --- |
+|  | 参数 | 说明 |
+| :-: | :-- | -- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
 | -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
 | -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
 | -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
 | -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
@@ -118,14 +118,14 @@
 |  | abstract |  |论文摘要|
 |  | keywords |  |论文关键词|
 |  | funds |  |基金资助|
 |  | class_num |  |分类号|
 |  | source |  |发表期刊|
 |  | issue |  |发表刊号|
 | body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |citation对应本章节的参考文献索引；text对应本章节的文本|
+|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |reference对应本章节的参考文献索引；text对应本章节的文本|
 |  | 2.xxx | 2.1xxx ||
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
 ## 开源协议
 本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.3/setup.py` & `cnki_html2json-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.3",
+    version="0.1.4",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=["cnki_html2json"],
```

### Comparing `cnki_html2json-0.1.3/tests/test_html2json.py` & `cnki_html2json-0.1.4/tests/test_html2json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,29 @@
 from cnki_html2json import html2json
 
-def test_html2json():
+def test_fulltext():
     with open('tests/fulltext.html','r') as f:
         content = f.read()
 
     text_structure = html2json._ExtractContent(content,'structure').extract_all()
     assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT('
     assert text_structure['body_text']['1 引言']['reference'][0]==1
 
     text_plain = html2json._ExtractContent(content,'plain').extract_all()
+    assert text_plain['body_text'][:14] == '近年来，以Chat GPT('
+
+    text_raw = html2json._ExtractContent(content,'raw').extract_all()
+    assert '[1]' in text_raw['body_text']['1 引言']['text']
+
+def test_fulltext_crawl():
+    with open('tests/fulltext_crawl.html','r') as f:
+        content = f.read()
+
+    text_structure = html2json._ExtractContent(content,'structure').extract_all()
+    assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT('
+    assert text_structure['body_text']['1 引言']['reference'][0]==1
+
+    text_plain = html2json._ExtractContent(content,'plain').extract_all()
     assert text_plain['body_text'][:14] == '近年来，以Chat GPT('
 
     text_raw = html2json._ExtractContent(content,'raw').extract_all()
     assert '[1]' in text_raw['body_text']['1 引言']['text']
```

