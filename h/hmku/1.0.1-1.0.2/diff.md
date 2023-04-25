# Comparing `tmp/hmku-1.0.1.tar.gz` & `tmp/hmku-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmku-1.0.1.tar", last modified: Tue Apr 25 03:12:44 2023, max compression
+gzip compressed data, was "hmku-1.0.2.tar", last modified: Tue Apr 25 03:33:14 2023, max compression
```

## Comparing `hmku-1.0.1.tar` & `hmku-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:12:44.278647 hmku-1.0.1/
--rw-rw-rw-   0        0        0      479 2023-04-25 03:12:44.277654 hmku-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-04-25 03:10:34.000000 hmku-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 03:12:44.259612 hmku-1.0.1/hmku/
--rw-rw-rw-   0        0        0       51 2023-04-25 03:11:00.000000 hmku-1.0.1/hmku/__init__.py
--rw-rw-rw-   0        0        0     6512 2023-04-25 02:10:37.000000 hmku-1.0.1/hmku/demo.py
-drwxrwxrwx   0        0        0        0 2023-04-25 03:12:44.275652 hmku-1.0.1/hmku.egg-info/
--rw-rw-rw-   0        0        0      479 2023-04-25 03:12:44.000000 hmku-1.0.1/hmku.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-25 03:12:44.000000 hmku-1.0.1/hmku.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:12:44.000000 hmku-1.0.1/hmku.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-25 03:12:44.000000 hmku-1.0.1/hmku.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 03:12:44.000000 hmku-1.0.1/hmku.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 03:12:44.278647 hmku-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-25 03:12:40.000000 hmku-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:33:14.136991 hmku-1.0.2/
+-rw-rw-rw-   0        0        0      515 2023-04-25 03:33:14.135988 hmku-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-04-25 03:31:52.000000 hmku-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 03:33:14.125986 hmku-1.0.2/hmku/
+-rw-rw-rw-   0        0        0       51 2023-04-25 03:11:00.000000 hmku-1.0.2/hmku/__init__.py
+-rw-rw-rw-   0        0        0     6443 2023-04-25 03:30:15.000000 hmku-1.0.2/hmku/demo.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:33:14.133987 hmku-1.0.2/hmku.egg-info/
+-rw-rw-rw-   0        0        0      515 2023-04-25 03:33:14.000000 hmku-1.0.2/hmku.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-25 03:33:14.000000 hmku-1.0.2/hmku.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:33:14.000000 hmku-1.0.2/hmku.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-25 03:33:14.000000 hmku-1.0.2/hmku.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 03:33:14.000000 hmku-1.0.2/hmku.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:33:14.136991 hmku-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-04-25 03:32:22.000000 hmku-1.0.2/setup.py
```

### Comparing `hmku-1.0.1/hmku/demo.py` & `hmku-1.0.2/hmku/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # 单本书采用多线程，开启多线程采集每一话的所有page
 
 def get_json(mid):  # 得到一本漫画的所有章节
 
     json_url = f'https://www.hmku.top/index.php/api/comic/chapter?callback=jQuery22409895390228187688_1682343459921&mid={mid}'
     # 'jQuery22409895390228187688_1682343459921'
-    resp = session.get(json_url,headers=hh).text
+    resp = session.get(json_url, headers=hh).text
     mark = False
     new_resp = []
     for line in resp:
         if '(' == line:
             mark = True
             continue
         if mark == True:
@@ -45,15 +45,15 @@
     # print(resp['data'])
 
 
 def get_mid_name(home_url):
 
     # home_url='https://www.hmku.top/index.php/manga/shendujiaoliuhui'
 
-    resp = session.get(home_url,headers=hh).text
+    resp = session.get(home_url, headers=hh).text
 
     # with open('tt.html','w',encoding='utf-8')as g:
     #     g.write(resp)
     resp1 = resp.replace('<!--', '').replace('-->', '')
     book_id = ''.join(etree.HTML(resp1).xpath(
         "//*[@class='send-gift']/@data-mid"))
     bookname = convert(''.join(etree.HTML(resp).xpath(
@@ -65,15 +65,15 @@
 
     # 设置多线程
     thread = []
     if not os.path.exists(f'./manga/{bookname}'):
         os.makedirs(f'./manga/{bookname}')
     for line in all_chapter:
         chapter_name = line['chapter_name'].replace(
-            '&hellip;', '').replace('&ldquo;', '').replace('&rdquo;','').replace('?','？').replace(':','').replace('.','_')
+            '&hellip;', '').replace('&ldquo;', '').replace('&rdquo;', '').replace('?', '？').replace(':', '').replace('.', '_')
         chapter_url = line['chapter_url']
         thread.append(threading.Thread(target=download,
                       args=(bookname, chapter_name, chapter_url)))
 
     # 启动多线程
     for line in thread:
         line.start()
@@ -85,15 +85,15 @@
 
 
 def get_alone_chapter_all_page(url):
 
     # url='https://www.hmku.top/index.php/chapter/10812'
     while True:
         try:
-            resp = session.get(url,timeout=5,verify=False,headers=hh).text
+            resp = session.get(url, timeout=5, verify=False, headers=hh).text
             break
         except:
             time.sleep(3)
     all_page = etree.HTML(resp).xpath(
         "//*[@class='read-container']/div[@class='rd-article-wr clearfix']/div/img/@data-original")
 
     # print(all_page)
@@ -105,62 +105,66 @@
 
     page_list = get_alone_chapter_all_page(url)
     print(name)
     num = 0
     new_down = []
     for line in page_list:
         # print(line,name,num)
-        num+=1
+        num += 1
         # continue
-        new_down.append(threading.Thread(target=new_download, args=(line,bookname,name,num)))#不影响更新
+        new_down.append(threading.Thread(target=new_download,
+                        args=(line, bookname, name, num)))  # 不影响更新
         # threading.Thread(target=new_download, args=(line,bookname,name,num)).start()
         # num+=1
     for ii in new_down:
         ii.start()
-    
+
     for ii in new_down:
         ii.join()
-    
+
     os.system('cls')
-hh={
-   'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+    return
+
+
+hh = {
+    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
 }
 
-def new_download(line,bookname,name,num):
-    if line=='':
-        return
-    elif line==None:
-        return
+
+def new_download(line, bookname, name, num):
+
     while True:
         if os.path.exists(f'./manga/{bookname}/{name}/{num}.jpg'):
-            if os.path.getsize(f'./manga/{bookname}/{name}/{num}.jpg')<=5:
+            if os.path.getsize(f'./manga/{bookname}/{name}/{num}.jpg') <= 5:
                 pass
             else:
-                print(f'./manga/{bookname}/{name}/{num}.jpg','已存在，pass')
+                print(f'./manga/{bookname}/{name}/{num}.jpg', '已存在，pass')
                 return
         # print(line)
         try:
-            content = session.get(line,headers=hh,verify=False,timeout=5).content
+            content = session.get(
+                line, headers=hh, verify=False, timeout=5).content
             break
         except Exception as e:
             # print(e)
-            print(e,'waiting 3s')
+            print(e, 'waiting 3s')
             time.sleep(3)
             # content = session.get(line).content
     try:
         if not os.path.exists(f'./manga/{bookname}/{name}'):
             os.makedirs(f'./manga/{bookname}/{name}')
     except:
         pass
-    
+
     with open(f'./manga/{bookname}/{name}/{num}.jpg', 'wb')as g:
         g.write(content)
         g.close()
-    
-    print(f'{bookname}/{name}/{num}.jpg','done!')
+
+    print(f'{bookname}/{name}/{num}.jpg', 'done!')
+    return
 
 # get_alone_chapter_all_page()
 # get_json(1726l)
 # get_mid_name()
 
 
 # if __name__ == '__main__':
@@ -173,33 +177,32 @@
     #     'https://www.hmku.top/index.php/comic/diaojiaokaiguan',
     #     'https://www.hmku.top/index.php/comic/zhichangxianjing',
     #     'https://www.hmku.top/index.php/comic/zizimendediaojiao',
     #     'https://www.hmku.top/index.php/comic/jimudepengyoumen',
     #     'https://www.hmku.top/index.php/comic/diwangapp',
     #     'https://www.hmku.top/index.php/comic/shechanhuazi',
     # ]
-    
-    # # resp=imghdr.what('manga\\深度交流会\\第1话-正妹学姐睡在我床上\\41.jpg')
+
     # # print(resp)
     # # exit()
     # for line in home_url:
 
     #     name=get_mid_name(line)
     #     print(name,'下载完成！')
 def main(home_url):
-    name=get_mid_name(home_url)
-    all_comic=os.listdir('./manga')
+    name = get_mid_name(home_url)
+    all_comic = os.listdir('./manga')
 
     for ii in all_comic:
         # print(ii)
-        ll=os.listdir(f'./manga/{ii}')
+        ll = os.listdir(f'./manga/{ii}')
         for pp in ll:
-            all_pic=os.listdir(f'./manga/{ii}/{pp}')
+            all_pic = os.listdir(f'./manga/{ii}/{pp}')
             for oo in all_pic:
-                file_name=(f'./manga/{ii}/{pp}/{oo}').replace('/',r'\\')
+                file_name = (f'./manga/{ii}/{pp}/{oo}').replace('/', r'\\')
                 # print(file_name)
-                if imghdr.what(file_name)!='jpeg':
+                if imghdr.what(file_name) == None:
                     # print(file_name,'kkkkkkkk')
                     os.remove(file_name)
                     pass
 
-    print(name,'下载完成！')
+    print(name, '下载完成！')
```

### Comparing `hmku-1.0.1/setup.py` & `hmku-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hmku",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.1",  # 包版本号，便于维护版本
+    version="1.0.2",  # 包版本号，便于维护版本
     author="Yuki",  # 作者，可以写自己的姓名
     author_email="3026408975@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="下载韩漫库主页漫画",  # 包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     # url="https://github.com/pypa/sampleproject",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

