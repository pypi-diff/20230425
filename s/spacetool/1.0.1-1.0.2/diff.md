# Comparing `tmp/spacetool-1.0.1.tar.gz` & `tmp/spacetool-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-1.0.1.tar", last modified: Mon Apr 24 06:25:09 2023, max compression
+gzip compressed data, was "spacetool-1.0.2.tar", last modified: Tue Apr 25 08:53:42 2023, max compression
```

## Comparing `spacetool-1.0.1.tar` & `spacetool-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-24 06:25:09.610072 spacetool-1.0.1/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.1/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-24 06:25:09.609947 spacetool-1.0.1/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.1/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2023-04-24 06:25:09.610121 spacetool-1.0.1/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2527 2023-04-24 06:14:48.000000 spacetool-1.0.1/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-24 06:25:09.608683 spacetool-1.0.1/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.1/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.1/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)    41089 2023-04-24 06:23:47.000000 spacetool-1.0.1/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-24 06:25:09.609752 spacetool-1.0.1/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       68 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-25 08:53:42.281538 spacetool-1.0.2/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.2/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-25 08:53:42.281413 spacetool-1.0.2/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.2/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-04-25 08:53:42.281584 spacetool-1.0.2/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2519 2023-04-25 08:53:13.000000 spacetool-1.0.2/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-25 08:53:42.280187 spacetool-1.0.2/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.2/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.2/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    50834 2023-04-25 05:52:01.000000 spacetool-1.0.2/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-25 08:53:42.281220 spacetool-1.0.2/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       60 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-1.0.1/LICENSE` & `spacetool-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-1.0.1/setup.py` & `spacetool-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import find_packages
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="spacetool",
-    version="1.0.1",
+    version="1.0.2",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
-    install_requires=["requests==2.28.1", "cos-python-sdk-v5==1.9.23", "qcloud-python-sts==3.1.3"],
+    install_requires=["requests", "cos-python-sdk-v5==1.9.23", "qcloud-python-sts==3.1.3"],
     python_requires=">=3.6,<3.11",
     keywords=['data', "spacedata"],
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `spacetool-1.0.1/spacetool/main_tool.py` & `spacetool-1.0.2/spacetool/main_tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding:utf-8 -*-
 import requests
 import json
 import os
 import logging
 import hashlib
 from urllib import parse
+from datetime import datetime
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from qcloud_cos import CosServiceError
 # from qcloud_cos import CosClientError
 # from sts.sts import Sts
 import sys
 # import json
@@ -40,14 +41,16 @@
     """
     获取停车场信息；
     上传停车场信息；
     获取停车场采集记录信息；
     上传停车场采集记录信息；
     """
     def __init__(self, name, code, host="http://127.0.0.1:8000/"):
+        now = datetime.now().strftime("%m-%d-%Y:%H-%M-%S")
+        self._log_file_name = f"./walk_{now}.log.txt"
         self.name = name               # 用户name
         self.code = code               # 用户code
         self.uid = None                # 用户ID
         self.authorization = None
         # self.temp_carparking_name = "carparking_name"
         # self.temp_unique_time_string = "unique_time_string"
         self.host = host               # api Domain
@@ -66,14 +69,15 @@
         self.collection_record_serial_id = None
 
         self.qcloud_sts_url = parse.urljoin(self.host, "api/v1/cloud_sts/qcloud_sts/")
         # self.check_code()              # 用户校验
         self.check_set_token()           # 设置token
         # headers = {"Authorization":"bearer a809655f-e4bf-41b8-9088-85a1d3780d6d"}
         self.car_p_ser_path = {}
+        self.error_car_p_ser_path = {}
 
     def check_set_token(self):
         res = requests_post(self.usercenter_token_url, {"username": self.name, "password": self.code})
         # {
         #     "refresh": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoicmVmcmVzaCIsImV4cCI6MTY4MTk4OTkzMiwiaWF0IjoxNjgxOTAzNTMyLCJqdGkiOiI3ZWNlZmRjZGE4Y2Q0ZmFlYjhkZDRlNzVhZDRhNWNkNSIsInVzZXJfaWQiOjEwfQ.MtZ_vdnjTyVXaqqvFsvuyRjG4eUkZ20noyULz9znRHw",
         #     "access": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNjgxOTA1MzMyLCJpYXQiOjE2ODE5MDM1MzIsImp0aSI6ImVkY2NiMzljODMxNDRhYzBhMmVmMDU0NGY0YmI4NDRmIiwidXNlcl9pZCI6MTB9.F6JH8JAHsuua0pR8kC7U6OjdUtzEIxggadDoaOW_HdM"
         # }
@@ -202,28 +206,40 @@
         # value: relative dir for all files
         handle_type = 1 追势
         handle_type = 2 泽尔
         handle_type = 3 其他
         """
         if car_p_encoding in self.car_p_ser_path:
             return self.car_p_ser_path[car_p_encoding]
+        elif car_p_encoding in self.error_car_p_ser_path:
+            return False
         else:
             carparking_name = car_p_encoding.split("/")[0]
             unique_time_string = car_p_encoding.split("/")[1]
-            carparking_serial = self.get_car_parking_info(carparking_name)["data"]["carparking_serial"]
-            collection_record_serial = self.get_carparking_collection_record_info(carparking_serial, unique_time_string)["data"]["collection_record_serial"]
+            try:
+                carparking_serial = self.get_car_parking_info(carparking_name)["data"]["carparking_serial"]  # get_car_parking_info: {'code': 4004, 'data': '', 'msg': '暂无此停车场信息录入'}
+                collection_record_serial = self.get_carparking_collection_record_info(carparking_serial, unique_time_string)["data"]["collection_record_serial"]
+            except Exception:
+                logging.info("######error#######")
+                logging.info(f"get_car_parking_info: {carparking_name} {self.get_car_parking_info(carparking_name)}")
+                self.error_car_p_ser_path[car_p_encoding] = {
+                    "carparking_name": carparking_name, 
+                    "unique_time_string": unique_time_string
+                }
+                return False
             self.car_p_ser_path[car_p_encoding] = {
                 "carparking_name": carparking_name,
                 "carparking_serial": carparking_serial,
                 "unique_time_string": unique_time_string,
                 "collection_record_serial": collection_record_serial,
                 "handle_type": handle_type,
                 "handle_path": handle_path,
                 "handle_status": False
             }
+        return True
 
     def walk_dir(self, origin_dir):
         """
         # 读取文件路径，获取停车场名称和唯一时间戳
         # walk记录运行到多少行, 跳过重复处理位置
 
         # 格式1:
@@ -388,14 +404,94 @@
         }
         res = requests_post(self.collection_data_upload_url, requests_payload, {"Authorization": self.authorization})
         res_reason = res.reason
         assert res.status_code == 200, f"请求有错, errmsg【{res_reason}】"
         json_data = json.loads(res.text)
         return json_data
 
+    def file_collection_data_upload(self, line, total_num, match_num, handle_num):
+        total_num += 1
+        if "/data/" in line:
+            match_num += 1
+            fir_split_line_texts = line.split("##")
+            origin_full_file_path = fir_split_line_texts[1].replace("/ ", "/")
+            full_f_name = "offline" + origin_full_file_path.replace("/data/", f"/data{fir_split_line_texts[0]}/")
+            carparking_name = full_f_name.split(os.path.sep)[3]
+            unique_time_string = full_f_name.split(os.path.sep)[4]
+            car_p_encoding = f"{carparking_name}/{unique_time_string}"
+            if car_p_encoding in self.car_p_ser_path:
+                # self.car_p_ser_path[car_p_encoding] = {
+                #     "carparking_name": carparking_name,
+                #     "carparking_serial": carparking_serial,
+                #     "unique_time_string": unique_time_string,
+                #     "collection_record_serial": collection_record_serial,
+                #     "handle_type": handle_type,
+                #     "handle_path": handle_path,
+                #     "handle_status": False
+                # }
+                carparking_serial = self.car_p_ser_path[car_p_encoding]['carparking_serial']
+                collection_record_serial = self.car_p_ser_path[car_p_encoding]['collection_record_serial']
+                handle_type = self.car_p_ser_path[car_p_encoding]['handle_type']
+                md5 = fir_split_line_texts[2]
+                suffix = fir_split_line_texts[3]
+                size = fir_split_line_texts[4]
+                file = full_f_name.split("/")[-1]
+                if handle_type == 2:
+                    if full_f_name.endswith(".blf"):
+                        handle_num += 1
+                        target_file_path_key = f"origin/{carparking_serial}-{collection_record_serial}/{carparking_serial}-{collection_record_serial}-{file}"
+                        self.collection_data_upload(carparking_serial, collection_record_serial, target_file_path_key, md5, suffix, size, full_f_name)
+                    elif full_f_name.endswith("raw.csv"):
+                        if "/raw/" in full_f_name:
+                            handle_num += 1
+                            target_file_path_key = f"origin/{carparking_serial}-{collection_record_serial}/{carparking_serial}-{collection_record_serial}-{file}"
+                            self.collection_data_upload(carparking_serial, collection_record_serial, target_file_path_key, md5, suffix, size, full_f_name)
+                        else:
+                            self.write_log(f"#file_collection_data_upload#0#{line}")
+                            pass
+                    elif full_f_name.endswith(".csv"):
+                        if "/video/" in full_f_name:
+                            handle_num += 1
+                            target_file_path_key = f"origin/{carparking_serial}-{collection_record_serial}/{carparking_serial}-{collection_record_serial}-{file}"
+                            self.collection_data_upload(carparking_serial, collection_record_serial, target_file_path_key, md5, suffix, size, full_f_name)
+                        else:
+                            self.write_log(f"#file_collection_data_upload#1#{line}")
+                            pass
+                    elif full_f_name.endswith("raw.avi"):
+                        handle_num += 1
+                        target_file_path_key = f"origin/{carparking_serial}-{collection_record_serial}/{carparking_serial}-{collection_record_serial}-{file}"
+                        self.collection_data_upload(carparking_serial, collection_record_serial, target_file_path_key, md5, suffix, size, full_f_name)
+                    else:
+                        self.write_log(f"#file_collection_data_upload#2#{line}")
+                        pass
+                else:
+                    self.write_log(f"#file_collection_data_upload#3#{line}")
+            else:
+                self.write_log(f"#file_collection_data_upload#4#{line}")
+                # 当前停车场信息未入库
+                pass
+        return total_num, match_num, handle_num
+
+    def collection_data_upload(self, carparking_serial, collection_record_serial, target_file_path_key, md5, suffix, size, full_f_name):
+        requests_payload = {
+            "carparking_serial": carparking_serial,
+            "collection_record_serial": collection_record_serial,
+            "qcloud_sts_request_key": None,
+            "target_file_path_key": target_file_path_key,
+            "md5": md5,
+            "suffix": suffix,
+            "size": size,
+            "full_f_name": full_f_name,
+        }
+        res = requests_post(self.collection_data_upload_url, requests_payload, {"Authorization": self.authorization})
+        res_reason = res.reason
+        assert res.status_code == 200, f"请求有错, errmsg【{res_reason}】"
+        json_data = json.loads(res.text)
+        return json_data
+
     def try_get_smc(self, handle_path):
         smc_path = os.path.join(handle_path, f"2、Config{os.path.sep}PC")
         smc_file = None
         for file in os.listdir(smc_path):
             if file.endswith(".bin"):
                 smc_file = os.path.join(smc_path, file)
                 break
@@ -423,21 +519,102 @@
             return "error"
 
     def get_file_size(self, fname):
         # os.stat_result(st_mode=33188, st_ino=14412668, st_dev=16777229, st_nlink=1, st_uid=501, st_gid=20, st_size=2515, st_atime=1681784164, st_mtime=1681784151, st_ctime=1681784163)
         # return os.stat(fname).st_size
         return os.path.getsize(fname)
 
+    def walk_log_file(self, file_name):
+        """
+        1、先运行walk_log_file
+        2、再运行walk_log_and_upload_info
+        """
+        total_num = 0
+        match_num = 0
+        handle_num = 0
+        with open(file_name, 'r') as file:
+            while True:
+                line = file.readline()
+                if line:
+                    total_num, match_num, handle_num = self.line_handle(line, total_num, match_num, handle_num)
+                    if total_num % 500 == 0:
+                        logging.info(f"进度第{total_num}行")
+                else:
+                    break
+        return total_num, match_num, handle_num
+
+    def walk_log_and_upload_info(self, file_name):
+        """
+        1、先运行walk_log_file
+        2、再运行walk_log_and_upload_info
+        """
+        total_num = 0
+        match_num = 0
+        handle_num = 0
+        with open(file_name, 'r') as file:
+            while True:
+                line = file.readline()
+                if line:
+                    total_num, match_num, handle_num = self.file_collection_data_upload(line, total_num, match_num, handle_num)
+                    if total_num % 500 == 0:
+                        logging.info(f"进度第{total_num}行")
+                else:
+                    break
+        return self.car_p_ser_path
+
+    def write_log(self, to_write_text):
+        f = open(self._log_file_name, "a+", encoding='utf-8')
+        f.writelines(to_write_text+"\n")
+        f.close()
+
+    def line_handle(self, line, total_num, match_num, handle_num):
+        total_num += 1
+        if "/data/" in line:
+            fir_split_line_texts = line.split("##")
+            origin_full_file_path = fir_split_line_texts[1].replace("/ ", "/")
+            full_f_name = "offline" + origin_full_file_path.replace("/data/", f"/data{fir_split_line_texts[0]}/")
+            if full_f_name.endswith("mp4"):
+                pass
+                # # 格式检查
+                # if "1、Raw_Video" in full_f_name:
+                #     # 追势自有格式
+                #     carparking_name = full_f_name.split(os.path.sep)[-3]
+                #     unique_time_string = file_name.split(".")[0]
+                #     handle_path = os.path.sep.join(full_f_name.split(os.path.sep)[:-2])
+                #     self.set_car_p_ser_handle_path(f"{carparking_name}/{unique_time_string}", handle_type=1, handle_path=handle_path)
+                # else:
+                #     # 追势自有格式错误
+                #     # todo log
+                #     f.write(f"#line{num}[WARNING]:{full_f_name}\n")
+                #     logging.warning(f"#line{num} {full_f_name}")  # 创建一条严重级别为WARNING的日志记录
+            elif full_f_name.endswith("raw.csv"):
+                match_num += 1
+                if f"input{os.path.sep}raw" in full_f_name:
+                    # 泽尔格式
+                    carparking_name = full_f_name.split(os.path.sep)[3]
+                    unique_time_string = full_f_name.split(os.path.sep)[4]
+                    handle_path = os.path.sep.join(full_f_name.split(os.path.sep)[:5])  # 'offline/data/20220721/唯亭旺角停车场/20220721-19-58-42'
+                    res = self.set_car_p_ser_handle_path(f"{carparking_name}/{unique_time_string}", handle_type=2, handle_path=handle_path)
+                    if res:
+                        handle_num += 1
+                    else:
+                        self.write_log(f"#line_handle#{line}")
+                        pass
+                else:
+                    # 泽尔格式错误
+                    # todo log
+                    logging.warning(f"#{line}")  # 创建一条严重级别为WARNING的日志记录
+        return total_num, match_num, handle_num
+
 
 class QCloudHandle:
     '''
     # 功能点，读取文件路径，获取入库信息
     # 如果您一定要使用永久密钥来生成预签名，建议永久密钥的权限范围仅限于上传或下载操作，以规避风险。并且所生成的签名有效时长设置为完成本次上传或下载操作所需的最短期限，因为，当指定预签名 URL 的有效时间过期后，请求会中断；申请新的签名后，需要重新执行失败请求，不支持断点续传。
     # 分别封装永久密钥和临时密钥方案
-
     '''
     def __init__(self, secret_id, secret_key, region, bucket_name, if_ever=False, token=None):
         self.if_ever = if_ever            # 密钥状态，False: 临时, True: 永久
         self.secret_id = secret_id
         self.secret_key = secret_key
         self.region = region
         self.bucket_name = bucket_name
@@ -468,15 +645,15 @@
             meta_data = {}
         response = self.client.upload_file(
             Bucket=self.bucket_name,      # Bucket='examplebucket-1250000000',
             LocalFilePath=tmp_file_path,  # 'local.txt'
             Key=target_file_path,         # 对象键（Key）是对象在存储桶中的唯一标识。例如，在对象的访问域名 examplebucket-1250000000.cos.ap-guangzhou.myqcloud.com/doc/pic.jpg 中，对象键为 doc/pic.jpg
             PartSize=1,                   # 分块上传的分块大小，默认为1MB
             MAXThread=10,                 # 分块上传的并发数量，默认为5个线程上传分块
-            EnableMD5=False,              # 是否需要 SDK 计算 Content-MD5，默认关闭，打开后会增加上传耗时
+            EnableMD5=True,              # 是否需要 SDK 计算 Content-MD5，默认关闭，打开后会增加上传耗时
             progress_callback=self.percentage,       # 上传进度的回调函数，可以通过自定义此函数，来获取上传进度
             Metadata=meta_data,                  # 用户自定义的对象元数据
         )
         return response
 
     def head_object(self, object_key):
         response = self.client.head_object(
@@ -791,19 +968,25 @@
 
 pip install spacetool, requests
 import sys,os,json
 pp2 = os.path.abspath(".")
 sys.path.append(pp2)
 
 import main_tool
-d = main_tool.DataTool(name="test", code="space666!", host="http://127.0.0.1:8000/")
+d = main_tool.DataTool(name="", code="", host="http://127.0.0.1:8000/")
 to_handle_dir = "/Users/leo/Documents/data/test数据格式样本/紫横家园东区"
 car_p_ser_path = d.walk_dir(to_handle_dir)
 res = d.handle_local()
 
+import main_tool
+d = main_tool.DataTool(name="", code="", host="http://127.0.0.1:8000/")
+f = "/Users/leo/Downloads/追势数据4号盘.txt"
+res = d.walk_log_file(f)
+res2 = d.walk_log_and_upload_info(f)
+
 """
 
 
 """
 qcloud 测试
 if __name__ == "__main__":
     # 进入异步任务队列
```

