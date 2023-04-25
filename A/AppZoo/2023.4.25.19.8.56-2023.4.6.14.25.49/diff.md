# Comparing `tmp/AppZoo-2023.4.25.19.8.56.tar.gz` & `tmp/AppZoo-2023.4.6.14.25.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppZoo-2023.4.25.19.8.56.tar", last modified: Tue Apr 25 11:08:57 2023, max compression
+gzip compressed data, was "AppZoo-2023.4.6.14.25.49.tar", last modified: Thu Apr  6 06:25:49 2023, max compression
```

## Comparing `AppZoo-2023.4.25.19.8.56.tar` & `AppZoo-2023.4.6.14.25.49.tar`

### file list

```diff
@@ -1,268 +1,259 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.310868 AppZoo-2023.4.25.19.8.56/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.211822 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2616 2023-04-25 11:08:57.000000 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     7763 2023-04-25 11:08:57.000000 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-25 11:08:57.000000 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       76 2023-04-25 11:08:57.000000 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-25 11:08:57.000000 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       24 2023-04-25 11:08:57.000000 AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1061 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      175 2023-03-24 08:07:08.000000 AppZoo-2023.4.25.19.8.56/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2616 2023-04-25 11:08:57.310710 AppZoo-2023.4.25.19.8.56/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1979 2022-06-22 02:12:18.000000 AppZoo-2023.4.25.19.8.56/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1401 2020-11-05 12:07:26.000000 AppZoo-2023.4.25.19.8.56/README_.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.213647 AppZoo-2023.4.25.19.8.56/appzoo/
--rw-r--r--   0 betterme   (501) staff       (20)      299 2022-06-08 09:15:07.000000 AppZoo-2023.4.25.19.8.56/appzoo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10800 2022-11-10 06:55:01.000000 AppZoo-2023.4.25.19.8.56/appzoo/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1512 2021-09-04 15:47:19.000000 AppZoo-2023.4.25.19.8.56/appzoo/app_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.217440 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/
--rw-r--r--   0 betterme   (501) staff       (20)      253 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1740 2020-11-12 06:22:43.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/ann_search_app.py
--rw-r--r--   0 betterme   (501) staff       (20)      412 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/appzoo_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      729 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/common_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1045 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     3584 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/feishu_bot_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2271 2020-12-01 09:44:39.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/gen_synonyms.py
--rw-r--r--   0 betterme   (501) staff       (20)    57560 2022-09-15 03:56:47.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/image.png
--rw-r--r--   0 betterme   (501) staff       (20)      526 2022-06-08 02:47:15.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/lite_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1265 2020-11-30 08:18:15.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/mongo_cache.py
--rw-r--r--   0 betterme   (501) staff       (20)     1106 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/mongo_item.py
--rw-r--r--   0 betterme   (501) staff       (20)     3562 2020-12-04 08:12:48.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/nh_choice_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2591 2020-11-13 06:59:11.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/ocr_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2543 2022-09-15 03:45:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/ocr_app_.py
--rw-r--r--   0 betterme   (501) staff       (20)     1826 2022-06-21 02:20:49.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/raw_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     3631 2021-03-08 07:50:48.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/simbert_app.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.218055 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2021-09-04 16:31:06.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1175 2021-12-15 03:26:41.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1045 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      377 2022-03-16 02:31:18.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/hun.py
--rw-r--r--   0 betterme   (501) staff       (20)      642 2022-09-15 06:39:47.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test.py
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/user_ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3271 2022-03-24 07:41:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/wecom_callback.py
--rw-r--r--   0 betterme   (501) staff       (20)     2699 2022-03-31 02:56:19.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/wecom_callback_.py
--rw-r--r--   0 betterme   (501) staff       (20)     2803 2023-03-03 07:27:33.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/wecom_callback_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.218637 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/
--rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-01-17 02:23:26.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/2_.png
--rw-r--r--   0 betterme   (501) staff       (20)      241 2021-09-06 01:51:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      921 2022-08-10 05:49:23.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.218777 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/
--rw-r--r--   0 betterme   (501) staff       (20)      215 2022-08-10 04:21:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/log.csv
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.219230 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/
--rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-08-10 03:14:07.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/0.png
--rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-08-10 03:14:46.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/1.png
--rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-08-10 04:21:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/2.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.207307 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/gradio_cached_examples/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.219372 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/gradio_cached_examples/17/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2022-08-10 03:10:12.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/gradio_cached_examples/17/log.csv
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.219545 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/gradio_cached_examples/18/
--rw-r--r--   0 betterme   (501) staff       (20)      430 2022-08-10 05:37:25.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/gradio_cached_examples/18/log.csv
--rw-r--r--   0 betterme   (501) staff       (20)      391 2022-09-23 03:01:33.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/x.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.220171 AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2021-09-06 02:05:47.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      241 2021-09-06 01:28:04.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-31 09:56:29.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      621 2021-09-09 02:08:05.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/gooey_gui.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.220599 AppZoo-2023.4.25.19.8.56/appzoo/apps_pywebio/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2021-11-10 07:07:07.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_pywebio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1061 2022-06-02 05:57:05.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_pywebio/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      380 2022-06-02 06:05:19.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_pywebio/demo1.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.221332 AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/
--rw-r--r--   0 betterme   (501) staff       (20)     1138 2020-12-04 08:02:12.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/RpcApp.py
--rw-r--r--   0 betterme   (501) staff       (20)      252 2020-12-04 07:35:51.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      501 2022-10-10 02:59:39.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/client.py
--rw-r--r--   0 betterme   (501) staff       (20)       39 2022-06-02 03:31:12.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/pingpong.thrift
--rw-r--r--   0 betterme   (501) staff       (20)      583 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/server.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.223818 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)      122 2022-09-21 10:32:29.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      253 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1671 2022-10-10 10:03:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1353 2021-11-03 08:35:07.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/demo_app.py
--rw-r--r--   0 betterme   (501) staff       (20)      554 2020-11-03 04:16:24.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/display_data.py
--rw-r--r--   0 betterme   (501) staff       (20)      485 2021-09-04 15:31:16.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/display_request.py
--rw-r--r--   0 betterme   (501) staff       (20)     1365 2021-10-12 13:37:11.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/example.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.224537 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2021-09-04 16:21:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      554 2022-04-19 05:40:00.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/main.py
--rw-r--r--   0 betterme   (501) staff       (20)       10 2021-09-05 08:18:44.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/packages.txt
--rw-r--r--   0 betterme   (501) staff       (20)       98 2021-09-05 08:07:04.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/requirements.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      275 2021-09-05 03:26:24.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.224966 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/
--rw-r--r--   0 betterme   (501) staff       (20)      582 2022-09-21 11:10:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1708 2022-09-21 11:10:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/home.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.225935 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/
--rw-r--r--   0 betterme   (501) staff       (20)     1435 2022-09-22 06:25:26.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/0__Demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      694 2022-10-14 07:49:24.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/0_📹_Animation_Demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2022-09-21 11:10:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/1_📈_Plotting_Demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     3846 2022-09-21 11:10:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/2_🌍_Mapping_Demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2517 2022-09-21 11:10:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/3_📊_DataFrame_Demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1435 2022-09-22 08:12:10.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/xx.py
--rwxr--r--   0 betterme   (501) staff       (20)      282 2022-09-22 06:26:24.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      251 2020-11-05 12:11:21.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/nlpzoo_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2314 2022-06-16 08:32:53.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/ocr_app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2348 2020-11-13 07:17:06.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/ocr_app_.py
--rw-r--r--   0 betterme   (501) staff       (20)      901 2022-09-29 08:58:53.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/ppocr_.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.226719 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/profile/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2021-09-05 05:37:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/profile/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      935 2021-09-05 07:52:44.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/profile/main.py
--rw-r--r--   0 betterme   (501) staff       (20)       56 2021-09-05 06:45:32.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/profile/requirements.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      277 2021-10-12 12:40:29.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/profile/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)       26 2021-09-05 05:28:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/requirements.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      410 2022-10-10 09:55:45.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.227589 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2021-09-04 16:21:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2427 2023-04-05 06:05:51.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/main.py
--rw-r--r--   0 betterme   (501) staff       (20)       10 2021-09-05 08:18:44.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/packages.txt
--rw-r--r--   0 betterme   (501) staff       (20)       98 2021-09-05 08:07:04.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/requirements.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      275 2021-09-05 03:26:24.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      304 2021-10-12 13:35:51.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/st_pandas_profiling.py
--rw-r--r--   0 betterme   (501) staff       (20)      393 2021-11-10 07:19:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/text_update.py
--rw-r--r--   0 betterme   (501) staff       (20)     2327 2020-11-12 08:20:43.000000 AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/xindao_ann_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.279689 AppZoo-2023.4.25.19.8.56/appzoo/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      283 2021-09-03 03:28:26.000000 AppZoo-2023.4.25.19.8.56/appzoo/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1587 2022-07-04 06:43:38.000000 AppZoo-2023.4.25.19.8.56/appzoo/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.280083 AppZoo-2023.4.25.19.8.56/appzoo/data/
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-25 11:08:56.000000 AppZoo-2023.4.25.19.8.56/appzoo/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)      258 2020-11-03 05:24:54.000000 AppZoo-2023.4.25.19.8.56/appzoo/data/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.280948 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/
--rw-r--r--   0 betterme   (501) staff       (20)      325 2022-08-19 09:25:31.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.281292 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2022-09-16 02:16:35.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      234 2022-09-16 03:15:15.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/main.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.281638 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/nlp_apps/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2022-09-16 02:16:00.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/nlp_apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      616 2022-09-16 03:29:01.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/nlp_apps/lac_cut.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.282391 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/ocr_apps/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2022-09-16 02:16:06.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/ocr_apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    57560 2022-09-15 03:56:47.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/ocr_apps/image.png
--rw-r--r--   0 betterme   (501) staff       (20)      434 2023-03-27 02:02:01.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/ocr_apps/paddle_ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     1657 2022-09-16 05:13:38.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/client.py
--rw-r--r--   0 betterme   (501) staff       (20)     1153 2022-09-09 01:08:52.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.283049 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/multi_apps/
--rw-r--r--   0 betterme   (501) staff       (20)      239 2022-09-08 09:57:14.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/multi_apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      256 2022-09-08 09:59:44.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/multi_apps/a.py
--rw-r--r--   0 betterme   (501) staff       (20)      256 2022-09-08 09:59:45.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/multi_apps/b.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.284195 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2022-09-01 09:17:40.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      578 2022-08-19 10:20:23.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base.proto
--rw-r--r--   0 betterme   (501) staff       (20)      725 2022-08-19 10:04:26.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base_.proto
--rw-r--r--   0 betterme   (501) staff       (20)     1818 2022-09-01 09:20:38.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base_pb2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2253 2022-09-01 09:20:39.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base_pb2_grpc.py
--rw-r--r--   0 betterme   (501) staff       (20)      568 2022-10-10 01:26:23.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/create_proto.py
--rwxr--r--   0 betterme   (501) staff       (20)      285 2022-08-19 08:31:45.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/create_proto.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.285080 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/
--rw-r--r--   0 betterme   (501) staff       (20)      254 2022-09-01 08:48:53.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      578 2022-08-19 10:20:23.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base.proto
--rw-r--r--   0 betterme   (501) staff       (20)      725 2022-08-19 10:04:26.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base_.proto
--rw-r--r--   0 betterme   (501) staff       (20)     3831 2022-08-19 10:06:46.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base_pb2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2253 2022-08-22 01:08:21.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base_pb2_grpc.py
--rwxr--r--   0 betterme   (501) staff       (20)      285 2022-08-19 08:31:45.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/create_proto.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2679 2022-09-19 01:52:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/service.py
--rw-r--r--   0 betterme   (501) staff       (20)      433 2022-09-08 08:42:39.000000 AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1396 2022-06-14 06:33:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/gunicorn.conf.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.286849 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/
--rw-r--r--   0 betterme   (501) staff       (20)      239 2022-09-09 08:59:12.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      347 2023-03-07 01:58:03.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/c.py
--rw-r--r--   0 betterme   (501) staff       (20)      743 2023-04-12 12:54:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/client.py
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-04-12 13:04:36.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/data.txt
--rw-r--r--   0 betterme   (501) staff       (20)      836 2023-04-19 09:36:14.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/demo1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1209 2023-04-24 07:05:24.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/s.py
--rw-r--r--   0 betterme   (501) staff       (20)     1976 2023-04-20 00:40:45.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/server.py
--rw-r--r--   0 betterme   (501) staff       (20)      381 2023-04-09 05:03:35.000000 AppZoo-2023.4.25.19.8.56/appzoo/jina_app/ss.py
--rw-r--r--   0 betterme   (501) staff       (20)     1467 2022-10-28 07:17:23.000000 AppZoo-2023.4.25.19.8.56/appzoo/main.py
--rw-r--r--   0 betterme   (501) staff       (20)      411 2022-10-27 05:47:22.000000 AppZoo-2023.4.25.19.8.56/appzoo/req.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.287504 AppZoo-2023.4.25.19.8.56/appzoo/scheduler/
--rw-r--r--   0 betterme   (501) staff       (20)     4706 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/scheduler/Scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/scheduler/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3499 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/scheduler/__sanic.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.287716 AppZoo-2023.4.25.19.8.56/appzoo/st_app/
--rw-r--r--   0 betterme   (501) staff       (20)      282 2022-09-22 06:29:22.000000 AppZoo-2023.4.25.19.8.56/appzoo/st_app/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.287923 AppZoo-2023.4.25.19.8.56/appzoo/static/
--rw-r--r--   0 betterme   (501) staff       (20)      248 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/static/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.288083 AppZoo-2023.4.25.19.8.56/appzoo/static/css/
--rw-r--r--   0 betterme   (501) staff       (20)      955 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/static/css/main.css
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.288255 AppZoo-2023.4.25.19.8.56/appzoo/static/js/
--rw-r--r--   0 betterme   (501) staff       (20)     1551 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/static/js/main.js
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.290513 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/
--rw-r--r--   0 betterme   (501) staff       (20)       78 2022-09-22 07:34:00.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      282 2022-09-22 06:29:22.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      680 2023-04-09 04:28:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/backend.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.209180 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.290820 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components/lda/
--rw-r--r--   0 betterme   (501) staff       (20)      996 2023-04-09 03:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components/lda/lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.291501 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/
--rw-r--r--   0 betterme   (501) staff       (20)      259 2022-10-25 02:34:56.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-09 03:20:13.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.291910 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/
--rw-r--r--   0 betterme   (501) staff       (20)     4334 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.209459 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.292899 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/
--rw-r--r--   0 betterme   (501) staff       (20)      859 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/asset-manifest.json
--rw-r--r--   0 betterme   (501) staff       (20)     2031 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/index.html
--rw-r--r--   0 betterme   (501) staff       (20)      564 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/precache-manifest.91710ed8b790b4cd059933cd5b952d13.js
--rw-r--r--   0 betterme   (501) staff       (20)     1183 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/service-worker.js
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.209593 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.296453 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/
--rw-r--r--   0 betterme   (501) staff       (20)   328155 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js
--rw-r--r--   0 betterme   (501) staff       (20)     1774 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.LICENSE.txt
--rw-r--r--   0 betterme   (501) staff       (20)  1275620 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.map
--rw-r--r--   0 betterme   (501) staff       (20)      693 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js
--rw-r--r--   0 betterme   (501) staff       (20)     2653 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js.map
--rw-r--r--   0 betterme   (501) staff       (20)     1598 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 betterme   (501) staff       (20)     8317 2022-10-17 02:34:42.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0 betterme   (501) staff       (20)     1604 2022-10-31 10:10:46.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/time.html
--rw-r--r--   0 betterme   (501) staff       (20)      221 2023-04-12 05:08:47.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/init.css
--rw-r--r--   0 betterme   (501) staff       (20)      123 2023-04-12 03:55:41.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/init.html
--rw-r--r--   0 betterme   (501) staff       (20)     1509 2023-03-26 05:08:11.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/page.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.297011 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/pics/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-03-24 07:59:23.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/pics/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)  5979276 2023-03-24 07:56:12.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/pics/夕阳.png
--rwxr--r--   0 betterme   (501) staff       (20)      392 2022-11-29 08:59:54.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.302925 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.303619 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/.streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)     7586 2022-10-19 02:58:55.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/.streamlit/_config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      510 2022-12-07 06:48:02.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/.streamlit/config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      582 2022-09-21 11:10:09.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   144311 2022-12-07 08:42:31.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/a.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.304264 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/pages/
--rw-r--r--   0 betterme   (501) staff       (20)      306 2022-12-07 08:42:21.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/pages/0__0.py
--rw-r--r--   0 betterme   (501) staff       (20)     2001 2022-12-07 07:04:25.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/pages/分词&实体识别.py
--rwxr--r--   0 betterme   (501) staff       (20)      235 2022-10-17 01:32:27.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     1241 2022-12-07 05:53:46.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/👋.py
--rw-r--r--   0 betterme   (501) staff       (20)      229 2022-09-23 00:56:37.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/test.py
--rw-r--r--   0 betterme   (501) staff       (20)     7118 2023-04-25 10:51:44.000000 AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.307019 AppZoo-2023.4.25.19.8.56/appzoo/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      251 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2022-10-24 02:35:03.000000 AppZoo-2023.4.25.19.8.56/appzoo/templates/css.py
--rw-r--r--   0 betterme   (501) staff       (20)      160 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/templates/example_template.html
--rw-r--r--   0 betterme   (501) staff       (20)      785 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/templates/index.html
--rw-r--r--   0 betterme   (501) staff       (20)     1893 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/templates/meeting.html
--rw-r--r--   0 betterme   (501) staff       (20)     1635 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/templates/upload.html
--rw-r--r--   0 betterme   (501) staff       (20)      832 2023-04-06 06:28:31.000000 AppZoo-2023.4.25.19.8.56/appzoo/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.309126 AppZoo-2023.4.25.19.8.56/appzoo/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      954 2021-10-12 12:33:57.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/Templates.py
--rw-r--r--   0 betterme   (501) staff       (20)      246 2022-09-23 07:55:19.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1465 2022-09-29 10:19:15.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/handlers.py
--rw-r--r--   0 betterme   (501) staff       (20)     1143 2020-11-12 06:17:29.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/image_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.309450 AppZoo-2023.4.25.19.8.56/appzoo/utils/log/
--rw-r--r--   0 betterme   (501) staff       (20)      504 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/log/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1661 2020-11-05 11:48:55.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/log/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1098 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/make_scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1604 2022-09-29 10:13:19.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/melog.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      414 2022-06-28 08:49:53.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      727 2022-09-29 10:43:51.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/settings.py
--rw-r--r--   0 betterme   (501) staff       (20)     1397 2022-06-28 09:21:25.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/shap_app.py
--rw-r--r--   0 betterme   (501) staff       (20)      911 2022-09-23 02:43:41.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/st_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1581 2022-06-24 07:10:14.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/streamlit_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1241 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/upload.py
--rw-r--r--   0 betterme   (501) staff       (20)      326 2022-06-28 08:44:49.000000 AppZoo-2023.4.25.19.8.56/appzoo/utils/x.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.310201 AppZoo-2023.4.25.19.8.56/appzoo/webs/
--rw-r--r--   0 betterme   (501) staff       (20)      248 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/webs/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      605 2020-11-05 11:45:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/webs/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/appzoo/webs/jinja_example.py
--rw-r--r--   0 betterme   (501) staff       (20)      886 2020-11-05 11:45:17.000000 AppZoo-2023.4.25.19.8.56/appzoo/webs/meeting.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-25 11:08:57.310356 AppZoo-2023.4.25.19.8.56/configs/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2020-11-05 11:43:58.000000 AppZoo-2023.4.25.19.8.56/configs/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-25 11:08:57.310917 AppZoo-2023.4.25.19.8.56/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2022 2022-10-27 02:44:15.000000 AppZoo-2023.4.25.19.8.56/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.992521 AppZoo-2023.4.6.14.25.49/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.946129 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2616 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     7540 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       76 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       24 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1061 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      175 2023-03-24 08:07:08.000000 AppZoo-2023.4.6.14.25.49/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2616 2023-04-06 06:25:49.992356 AppZoo-2023.4.6.14.25.49/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1979 2022-06-22 02:12:18.000000 AppZoo-2023.4.6.14.25.49/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1401 2020-11-05 12:07:26.000000 AppZoo-2023.4.6.14.25.49/README_.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.948061 AppZoo-2023.4.6.14.25.49/appzoo/
+-rw-r--r--   0 betterme   (501) staff       (20)      299 2022-06-08 09:15:07.000000 AppZoo-2023.4.6.14.25.49/appzoo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10800 2022-11-10 06:55:01.000000 AppZoo-2023.4.6.14.25.49/appzoo/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1512 2021-09-04 15:47:19.000000 AppZoo-2023.4.6.14.25.49/appzoo/app_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.951668 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/
+-rw-r--r--   0 betterme   (501) staff       (20)      253 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1740 2020-11-12 06:22:43.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/ann_search_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)      412 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/appzoo_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      729 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/common_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1045 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3584 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/feishu_bot_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2271 2020-12-01 09:44:39.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/gen_synonyms.py
+-rw-r--r--   0 betterme   (501) staff       (20)    57560 2022-09-15 03:56:47.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/image.png
+-rw-r--r--   0 betterme   (501) staff       (20)      526 2022-06-08 02:47:15.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/lite_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1265 2020-11-30 08:18:15.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/mongo_cache.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1106 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/mongo_item.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3562 2020-12-04 08:12:48.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/nh_choice_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2591 2020-11-13 06:59:11.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/ocr_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2543 2022-09-15 03:45:27.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/ocr_app_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1826 2022-06-21 02:20:49.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/raw_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3631 2021-03-08 07:50:48.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/simbert_app.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.952290 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2021-09-04 16:31:06.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1175 2021-12-15 03:26:41.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1045 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      377 2022-03-16 02:31:18.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/hun.py
+-rw-r--r--   0 betterme   (501) staff       (20)      642 2022-09-15 06:39:47.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/user_ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3271 2022-03-24 07:41:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/wecom_callback.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2699 2022-03-31 02:56:19.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/wecom_callback_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2803 2023-03-03 07:27:33.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/wecom_callback_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.952917 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/
+-rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-01-17 02:23:26.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/2_.png
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2021-09-06 01:51:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      921 2022-08-10 05:49:23.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.953119 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/
+-rw-r--r--   0 betterme   (501) staff       (20)      215 2022-08-10 04:21:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/log.csv
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.953632 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/
+-rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-08-10 03:14:07.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/0.png
+-rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-08-10 03:14:46.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/1.png
+-rw-r--r--   0 betterme   (501) staff       (20)     1501 2022-08-10 04:21:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/2.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.941096 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/gradio_cached_examples/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.953796 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/gradio_cached_examples/17/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2022-08-10 03:10:12.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/gradio_cached_examples/17/log.csv
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.953958 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/gradio_cached_examples/18/
+-rw-r--r--   0 betterme   (501) staff       (20)      430 2022-08-10 05:37:25.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/gradio_cached_examples/18/log.csv
+-rw-r--r--   0 betterme   (501) staff       (20)      391 2022-09-23 03:01:33.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/x.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.954843 AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2021-09-06 02:05:47.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2021-09-06 01:28:04.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-31 09:56:29.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      621 2021-09-09 02:08:05.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/gooey_gui.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.955320 AppZoo-2023.4.6.14.25.49/appzoo/apps_pywebio/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2021-11-10 07:07:07.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_pywebio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1061 2022-06-02 05:57:05.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_pywebio/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      380 2022-06-02 06:05:19.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_pywebio/demo1.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.956084 AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/
+-rw-r--r--   0 betterme   (501) staff       (20)     1138 2020-12-04 08:02:12.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/RpcApp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      252 2020-12-04 07:35:51.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      501 2022-10-10 02:59:39.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)       39 2022-06-02 03:31:12.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/pingpong.thrift
+-rw-r--r--   0 betterme   (501) staff       (20)      583 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/server.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.958824 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)      122 2022-09-21 10:32:29.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      253 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1671 2022-10-10 10:03:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1353 2021-11-03 08:35:07.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/demo_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)      554 2020-11-03 04:16:24.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/display_data.py
+-rw-r--r--   0 betterme   (501) staff       (20)      485 2021-09-04 15:31:16.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/display_request.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1365 2021-10-12 13:37:11.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/example.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.959707 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2021-09-04 16:21:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      554 2022-04-19 05:40:00.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/main.py
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2021-09-05 08:18:44.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/packages.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2021-09-05 08:07:04.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/requirements.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      275 2021-09-05 03:26:24.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.960238 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/
+-rw-r--r--   0 betterme   (501) staff       (20)      582 2022-09-21 11:10:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1708 2022-09-21 11:10:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/home.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.961432 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1435 2022-09-22 06:25:26.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/0__Demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      694 2022-10-14 07:49:24.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/0_📹_Animation_Demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2022-09-21 11:10:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/1_📈_Plotting_Demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3846 2022-09-21 11:10:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/2_🌍_Mapping_Demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2517 2022-09-21 11:10:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/3_📊_DataFrame_Demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1435 2022-09-22 08:12:10.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/xx.py
+-rwxr--r--   0 betterme   (501) staff       (20)      282 2022-09-22 06:26:24.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      251 2020-11-05 12:11:21.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/nlpzoo_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2314 2022-06-16 08:32:53.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/ocr_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2348 2020-11-13 07:17:06.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/ocr_app_.py
+-rw-r--r--   0 betterme   (501) staff       (20)      901 2022-09-29 08:58:53.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/ppocr_.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.962164 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/profile/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2021-09-05 05:37:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/profile/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      935 2021-09-05 07:52:44.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/profile/main.py
+-rw-r--r--   0 betterme   (501) staff       (20)       56 2021-09-05 06:45:32.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/profile/requirements.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      277 2021-10-12 12:40:29.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/profile/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2021-09-05 05:28:27.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/requirements.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      410 2022-10-10 09:55:45.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.963121 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2021-09-04 16:21:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2427 2023-04-05 06:05:51.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/main.py
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2021-09-05 08:18:44.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/packages.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2021-09-05 08:07:04.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/requirements.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      275 2021-09-05 03:26:24.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2021-10-12 13:35:51.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/st_pandas_profiling.py
+-rw-r--r--   0 betterme   (501) staff       (20)      393 2021-11-10 07:19:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/text_update.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2327 2020-11-12 08:20:43.000000 AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/xindao_ann_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.963686 AppZoo-2023.4.6.14.25.49/appzoo/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 AppZoo-2023.4.6.14.25.49/appzoo/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      283 2021-09-03 03:28:26.000000 AppZoo-2023.4.6.14.25.49/appzoo/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1587 2022-07-04 06:43:38.000000 AppZoo-2023.4.6.14.25.49/appzoo/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.964024 AppZoo-2023.4.6.14.25.49/appzoo/data/
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-06 06:25:49.000000 AppZoo-2023.4.6.14.25.49/appzoo/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2020-11-03 05:24:54.000000 AppZoo-2023.4.6.14.25.49/appzoo/data/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.964886 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/
+-rw-r--r--   0 betterme   (501) staff       (20)      325 2022-08-19 09:25:31.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.965243 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2022-09-16 02:16:35.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2022-09-16 03:15:15.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/main.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.965594 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/nlp_apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2022-09-16 02:16:00.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/nlp_apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      616 2022-09-16 03:29:01.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/nlp_apps/lac_cut.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.966320 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/ocr_apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2022-09-16 02:16:06.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/ocr_apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    57560 2022-09-15 03:56:47.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/ocr_apps/image.png
+-rw-r--r--   0 betterme   (501) staff       (20)      434 2023-03-27 02:02:01.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/ocr_apps/paddle_ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1657 2022-09-16 05:13:38.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1153 2022-09-09 01:08:52.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.966941 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/multi_apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      239 2022-09-08 09:57:14.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/multi_apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      256 2022-09-08 09:59:44.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/multi_apps/a.py
+-rw-r--r--   0 betterme   (501) staff       (20)      256 2022-09-08 09:59:45.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/multi_apps/b.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.968033 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2022-09-01 09:17:40.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2022-08-19 10:20:23.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base.proto
+-rw-r--r--   0 betterme   (501) staff       (20)      725 2022-08-19 10:04:26.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base_.proto
+-rw-r--r--   0 betterme   (501) staff       (20)     1818 2022-09-01 09:20:38.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base_pb2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2253 2022-09-01 09:20:39.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base_pb2_grpc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      568 2022-10-10 01:26:23.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/create_proto.py
+-rwxr--r--   0 betterme   (501) staff       (20)      285 2022-08-19 08:31:45.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/create_proto.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.968935 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/
+-rw-r--r--   0 betterme   (501) staff       (20)      254 2022-09-01 08:48:53.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2022-08-19 10:20:23.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base.proto
+-rw-r--r--   0 betterme   (501) staff       (20)      725 2022-08-19 10:04:26.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base_.proto
+-rw-r--r--   0 betterme   (501) staff       (20)     3831 2022-08-19 10:06:46.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base_pb2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2253 2022-08-22 01:08:21.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base_pb2_grpc.py
+-rwxr--r--   0 betterme   (501) staff       (20)      285 2022-08-19 08:31:45.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/create_proto.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2679 2022-09-19 01:52:27.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/service.py
+-rw-r--r--   0 betterme   (501) staff       (20)      433 2022-09-08 08:42:39.000000 AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1396 2022-06-14 06:33:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/gunicorn.conf.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.969659 AppZoo-2023.4.6.14.25.49/appzoo/jina_app/
+-rw-r--r--   0 betterme   (501) staff       (20)      239 2022-09-09 08:59:12.000000 AppZoo-2023.4.6.14.25.49/appzoo/jina_app/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      347 2023-03-07 01:58:03.000000 AppZoo-2023.4.6.14.25.49/appzoo/jina_app/c.py
+-rw-r--r--   0 betterme   (501) staff       (20)      736 2023-03-09 05:27:27.000000 AppZoo-2023.4.6.14.25.49/appzoo/jina_app/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-07 01:57:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/jina_app/s.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1004 2023-03-09 05:17:13.000000 AppZoo-2023.4.6.14.25.49/appzoo/jina_app/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1467 2022-10-28 07:17:23.000000 AppZoo-2023.4.6.14.25.49/appzoo/main.py
+-rw-r--r--   0 betterme   (501) staff       (20)      411 2022-10-27 05:47:22.000000 AppZoo-2023.4.6.14.25.49/appzoo/req.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.970096 AppZoo-2023.4.6.14.25.49/appzoo/scheduler/
+-rw-r--r--   0 betterme   (501) staff       (20)     4706 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/scheduler/Scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/scheduler/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3499 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/scheduler/__sanic.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.970243 AppZoo-2023.4.6.14.25.49/appzoo/st_app/
+-rw-r--r--   0 betterme   (501) staff       (20)      282 2022-09-22 06:29:22.000000 AppZoo-2023.4.6.14.25.49/appzoo/st_app/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.970396 AppZoo-2023.4.6.14.25.49/appzoo/static/
+-rw-r--r--   0 betterme   (501) staff       (20)      248 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/static/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.970537 AppZoo-2023.4.6.14.25.49/appzoo/static/css/
+-rw-r--r--   0 betterme   (501) staff       (20)      955 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/static/css/main.css
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.970744 AppZoo-2023.4.6.14.25.49/appzoo/static/js/
+-rw-r--r--   0 betterme   (501) staff       (20)     1551 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/static/js/main.js
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.971839 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2022-09-22 07:34:00.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      282 2022-09-22 06:29:22.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.972380 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/
+-rw-r--r--   0 betterme   (501) staff       (20)      259 2022-10-25 02:34:56.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2022-10-17 01:55:18.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.972533 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/
+-rw-r--r--   0 betterme   (501) staff       (20)     4334 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.943279 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.973316 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/
+-rw-r--r--   0 betterme   (501) staff       (20)      859 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/asset-manifest.json
+-rw-r--r--   0 betterme   (501) staff       (20)     2031 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/index.html
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/precache-manifest.91710ed8b790b4cd059933cd5b952d13.js
+-rw-r--r--   0 betterme   (501) staff       (20)     1183 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/service-worker.js
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.943411 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.977049 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/
+-rw-r--r--   0 betterme   (501) staff       (20)   328155 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js
+-rw-r--r--   0 betterme   (501) staff       (20)     1774 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.LICENSE.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  1275620 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.map
+-rw-r--r--   0 betterme   (501) staff       (20)      693 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js
+-rw-r--r--   0 betterme   (501) staff       (20)     2653 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js.map
+-rw-r--r--   0 betterme   (501) staff       (20)     1598 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 betterme   (501) staff       (20)     8317 2022-10-17 02:34:42.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0 betterme   (501) staff       (20)     1604 2022-10-31 10:10:46.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/time.html
+-rw-r--r--   0 betterme   (501) staff       (20)     1509 2023-03-26 05:08:11.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/page.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.977695 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/pics/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-03-24 07:59:23.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/pics/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)  5979276 2023-03-24 07:56:12.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/pics/夕阳.png
+-rwxr--r--   0 betterme   (501) staff       (20)      392 2022-11-29 08:59:54.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.986272 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.986605 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2022-10-19 02:58:55.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      510 2022-12-07 06:48:02.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      582 2022-09-21 11:10:09.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   144311 2022-12-07 08:42:31.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/a.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.986915 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)      306 2022-12-07 08:42:21.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/pages/0__0.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2001 2022-12-07 07:04:25.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/pages/分词&实体识别.py
+-rwxr--r--   0 betterme   (501) staff       (20)      235 2022-10-17 01:32:27.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     1241 2022-12-07 05:53:46.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/👋.py
+-rw-r--r--   0 betterme   (501) staff       (20)      229 2022-09-23 00:56:37.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6040 2023-04-06 06:05:28.000000 AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.988666 AppZoo-2023.4.6.14.25.49/appzoo/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      251 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2022-10-24 02:35:03.000000 AppZoo-2023.4.6.14.25.49/appzoo/templates/css.py
+-rw-r--r--   0 betterme   (501) staff       (20)      160 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/templates/example_template.html
+-rw-r--r--   0 betterme   (501) staff       (20)      785 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/templates/index.html
+-rw-r--r--   0 betterme   (501) staff       (20)     1893 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/templates/meeting.html
+-rw-r--r--   0 betterme   (501) staff       (20)     1635 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/templates/upload.html
+-rw-r--r--   0 betterme   (501) staff       (20)      924 2023-04-06 06:25:25.000000 AppZoo-2023.4.6.14.25.49/appzoo/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.990753 AppZoo-2023.4.6.14.25.49/appzoo/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      954 2021-10-12 12:33:57.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/Templates.py
+-rw-r--r--   0 betterme   (501) staff       (20)      246 2022-09-23 07:55:19.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1465 2022-09-29 10:19:15.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/handlers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1143 2020-11-12 06:17:29.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/image_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.991121 AppZoo-2023.4.6.14.25.49/appzoo/utils/log/
+-rw-r--r--   0 betterme   (501) staff       (20)      504 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/log/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1661 2020-11-05 11:48:55.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/log/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1098 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/make_scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1604 2022-09-29 10:13:19.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/melog.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      414 2022-06-28 08:49:53.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      727 2022-09-29 10:43:51.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/settings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1397 2022-06-28 09:21:25.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/shap_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)      911 2022-09-23 02:43:41.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/st_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1581 2022-06-24 07:10:14.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/streamlit_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1241 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/upload.py
+-rw-r--r--   0 betterme   (501) staff       (20)      326 2022-06-28 08:44:49.000000 AppZoo-2023.4.6.14.25.49/appzoo/utils/x.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.991810 AppZoo-2023.4.6.14.25.49/appzoo/webs/
+-rw-r--r--   0 betterme   (501) staff       (20)      248 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/webs/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      605 2020-11-05 11:45:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/webs/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/appzoo/webs/jinja_example.py
+-rw-r--r--   0 betterme   (501) staff       (20)      886 2020-11-05 11:45:17.000000 AppZoo-2023.4.6.14.25.49/appzoo/webs/meeting.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-06 06:25:49.991969 AppZoo-2023.4.6.14.25.49/configs/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2020-11-05 11:43:58.000000 AppZoo-2023.4.6.14.25.49/configs/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-06 06:25:49.992572 AppZoo-2023.4.6.14.25.49/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2022 2022-10-27 02:44:15.000000 AppZoo-2023.4.6.14.25.49/setup.py
```

### Comparing `AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/PKG-INFO` & `AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppZoo
-Version: 2023.4.25.19.8.56
+Version: 2023.4.6.14.25.49
 Summary: description
 Home-page: https://github.com/yuanjie-ai/AppZoo
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `AppZoo-2023.4.25.19.8.56/AppZoo.egg-info/SOURCES.txt` & `AppZoo-2023.4.6.14.25.49/AppZoo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -134,51 +134,44 @@
 appzoo/grpc_app/protos_/base_.proto
 appzoo/grpc_app/protos_/base_pb2.py
 appzoo/grpc_app/protos_/base_pb2_grpc.py
 appzoo/grpc_app/protos_/create_proto.sh
 appzoo/jina_app/__init__.py
 appzoo/jina_app/c.py
 appzoo/jina_app/client.py
-appzoo/jina_app/data.txt
-appzoo/jina_app/demo1.py
 appzoo/jina_app/s.py
 appzoo/jina_app/server.py
-appzoo/jina_app/ss.py
 appzoo/scheduler/Scheduler.py
 appzoo/scheduler/__init__.py
 appzoo/scheduler/__sanic.py
 appzoo/st_app/__init__.py
 appzoo/static/__init__.py
 appzoo/static/css/main.css
 appzoo/static/js/main.js
 appzoo/streamlit_app/README.md
 appzoo/streamlit_app/__init__.py
-appzoo/streamlit_app/backend.py
-appzoo/streamlit_app/init.css
-appzoo/streamlit_app/init.html
 appzoo/streamlit_app/page.py
 appzoo/streamlit_app/run.sh
 appzoo/streamlit_app/test.py
 appzoo/streamlit_app/utils.py
-appzoo/streamlit_app/components/lda/lda.py
-appzoo/streamlit_app/components_/README.md
-appzoo/streamlit_app/components_/__init__.py
-appzoo/streamlit_app/components_/time.html
-appzoo/streamlit_app/components_/streamlit_autorefresh/__init__.py
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/asset-manifest.json
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/index.html
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/precache-manifest.91710ed8b790b4cd059933cd5b952d13.js
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/service-worker.js
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.LICENSE.txt
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.map
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js.map
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js
-appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js.map
+appzoo/streamlit_app/components/README.md
+appzoo/streamlit_app/components/__init__.py
+appzoo/streamlit_app/components/time.html
+appzoo/streamlit_app/components/streamlit_autorefresh/__init__.py
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/asset-manifest.json
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/index.html
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/precache-manifest.91710ed8b790b4cd059933cd5b952d13.js
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/service-worker.js
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.LICENSE.txt
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.map
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js.map
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js
+appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js.map
 appzoo/streamlit_app/pics/__init__.py
 appzoo/streamlit_app/pics/夕阳.png
 appzoo/streamlit_app/templates/__init__.py
 appzoo/streamlit_app/templates/a.png
 appzoo/streamlit_app/templates/run.sh
 appzoo/streamlit_app/templates/👋.py
 appzoo/streamlit_app/templates/.streamlit/_config.toml
```

### Comparing `AppZoo-2023.4.25.19.8.56/LICENSE` & `AppZoo-2023.4.6.14.25.49/LICENSE`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/PKG-INFO` & `AppZoo-2023.4.6.14.25.49/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppZoo
-Version: 2023.4.25.19.8.56
+Version: 2023.4.6.14.25.49
 Summary: description
 Home-page: https://github.com/yuanjie-ai/AppZoo
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `AppZoo-2023.4.25.19.8.56/README.md` & `AppZoo-2023.4.6.14.25.49/README.md`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/README_.md` & `AppZoo-2023.4.6.14.25.49/README_.md`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/app_run.py` & `AppZoo-2023.4.6.14.25.49/appzoo/app_run.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/ann_search_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/ann_search_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/common_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/common_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/feishu_bot_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/feishu_bot_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/gen_synonyms.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/gen_synonyms.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/image.png` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/image.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/lite_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/lite_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/mongo_cache.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/mongo_item.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/mongo_item.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/nh_choice_model.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/nh_choice_model.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/ocr_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/ocr_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/ocr_app_.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/ocr_app_.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/raw_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/raw_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/simbert_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/simbert_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/test.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/test.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/user_ann.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/user_ann.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/wecom_callback.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/wecom_callback.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/wecom_callback_.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/wecom_callback_.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_fastapi/wecom_callback_fastapi.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_fastapi/wecom_callback_fastapi.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/2_.png` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/2_.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/0.png` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/0.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/1.png` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/1.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gradio/flagged/name/2.png` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gradio/flagged/name/2.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_gui/gooey_gui.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_gui/gooey_gui.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_pywebio/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_pywebio/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/RpcApp.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/RpcApp.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_rpc/server.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_rpc/server.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/demo_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/demo_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/display_data.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/display_data.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/example.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/example.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/field_translation/main.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/field_translation/main.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/__init__.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/__init__.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/home.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/home.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/0__Demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/0__Demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/0_📹_Animation_Demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/0_📹_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/1_📈_Plotting_Demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/1_📈_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/2_🌍_Mapping_Demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/2_🌍_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/3_📊_DataFrame_Demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/3_📊_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/home/pages/xx.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/home/pages/xx.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/ocr_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/ocr_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/ocr_app_.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/ocr_app_.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/ppocr_.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/ppocr_.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/profile/main.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/profile/main.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/simbert/main.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/simbert/main.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/apps_streamlit/xindao_ann_demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/apps_streamlit/xindao_ann_demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/clis/cli.py` & `AppZoo-2023.4.6.14.25.49/appzoo/clis/cli.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/nlp_apps/lac_cut.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/nlp_apps/lac_cut.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/apps/ocr_apps/image.png` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/apps/ocr_apps/image.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/client.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/client.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base.proto` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base.proto`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base_.proto` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base_.proto`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base_pb2.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base_pb2.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/base_pb2_grpc.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/base_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos/create_proto.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos/create_proto.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base.proto` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base.proto`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base_.proto` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base_.proto`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base_pb2.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base_pb2.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/protos_/base_pb2_grpc.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/protos_/base_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/grpc_app/service.py` & `AppZoo-2023.4.6.14.25.49/appzoo/grpc_app/service.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/gunicorn.conf.py` & `AppZoo-2023.4.6.14.25.49/appzoo/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/jina_app/client.py` & `AppZoo-2023.4.6.14.25.49/appzoo/jina_app/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 
 
 
 from jina import Client, Document, DocumentArray
 
-# c = Client(host='grpc://0.0.0.0:8501')
-c = Client(host='http://0.0.0.0:8501')
+c = Client(host='grpc://0.0.0.0:9955')
 
+# _ = c.post('/cut', Document()).texts
+# print(_)
 
-print(c.post('/cut', DocumentArray(Document(text='我在南京'))).texts)
+print(c.post('/cut', Document(text='我在南京')).texts)
 
 # r = c.post(
 #     '/',
 #     inputs=DocumentArray([
 #         Document(text='如何更换花呗绑定银行卡'),
 #         Document(text='花呗更改绑定银行卡')
 #     ])
@@ -29,8 +30,8 @@
 #
 # {
 #     "data": [
 #         {
 #             "text": "我在南京"
 #         }
 #     ]
-# }
+# }
```

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/main.py` & `AppZoo-2023.4.6.14.25.49/appzoo/main.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/scheduler/Scheduler.py` & `AppZoo-2023.4.6.14.25.49/appzoo/scheduler/Scheduler.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/scheduler/__sanic.py` & `AppZoo-2023.4.6.14.25.49/appzoo/scheduler/__sanic.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/static/css/main.css` & `AppZoo-2023.4.6.14.25.49/appzoo/static/css/main.css`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/static/js/main.js` & `AppZoo-2023.4.6.14.25.49/appzoo/static/js/main.js`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/__init__.py` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/__init__.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/asset-manifest.json` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/index.html` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/precache-manifest.91710ed8b790b4cd059933cd5b952d13.js` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/precache-manifest.91710ed8b790b4cd059933cd5b952d13.js`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/service-worker.js` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.LICENSE.txt` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.map` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/2.a187b8c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js.map` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/main.6f4c74db.chunk.js.map`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/streamlit_autorefresh/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/components_/time.html` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/components/time.html`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/page.py` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/page.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/pics/夕阳.png` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/pics/夕阳.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/.streamlit/_config.toml` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/.streamlit/_config.toml`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/__init__.py` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/a.png` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/a.png`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/pages/分词&实体识别.py` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/pages/分词&实体识别.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/templates/👋.py` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/templates/👋.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/streamlit_app/utils.py` & `AppZoo-2023.4.6.14.25.49/appzoo/streamlit_app/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -132,19 +132,14 @@
 
 
 def display_pdf(base64_pdf, width='100%', height=1000):
     _ = f"""<embed src="data:application/pdf;base64,{base64_pdf}" width="{width}" height="{height}" type="application/pdf">"""
     st.markdown(_, unsafe_allow_html=True)
 
 
-def display_pdf4file(file, width='100%', height=500):  # 上传PDF文件
-    base64_pdf = base64.b64encode(file.read()).decode('utf-8')
-    display_pdf(base64_pdf, width, height)
-
-
 def display_html(text='会飞的文字'):  # html("""<marquee bgcolor="#00ccff" behavior="alternate">这是一个滚动条</marquee>""")
     _ = f"""
         <marquee direction="down" width="100%" height="100%" behavior="alternate" style="border:solid"  bgcolor="#00FF00">
 
           <marquee behavior="alternate">
 
             {text}
@@ -158,83 +153,54 @@
 
 def reply4input(
         input,
         history=None,
         reply_func=lambda input: f'{input}的答案',
         max_turns=3,
         container=None,
-        previous_messages=None,
-        user_avatar_style="adventurer",
-        bot_avatar_style="Big Smile",
-        seed=42,
+        user_avatar_style="big-smile",
+        bot_avatar_style="bottts",
 ):
-    """https://www.dicebear.com/styles/big-smile
+    """
         container = st.container()  # 占位符
         text = st.text_area(label="用户输入", height=100, placeholder="请在这儿输入您的问题")
 
         if st.button("发送", key="predict"):
             with st.spinner("AI正在思考，请稍等........"):
                 history = st.session_state.get('state')
                 st.session_state["state"] = reply4input(text, history, container=container)
                 print(st.session_state['state'])
     """
     from streamlit_chat import message
-    user_message = partial(message, avatar_style=user_avatar_style.strip().replace(' ', '-').lower(), is_user=True,
-                           seed=seed)
-    bot_message = partial(message, avatar_style=bot_avatar_style.strip().replace(' ', '-').lower(), is_user=False,
-                          seed=seed)
+    user_message = partial(message, avatar_style=user_avatar_style, is_user=True)
+    bot_message = partial(message, avatar_style=bot_avatar_style, is_user=False)
 
     if history is None:
         history = []  # [(input/query, response)]
 
     if container is None:
         container = st.container()
 
     with container:
-        if previous_messages:
-            for msg in previous_messages:
-                bot_message(msg)  # display all the previous message
-
-        if max_turns > 1 and len(history) > 0:  # 展示历史
+        if len(history) > 0:  # 展示历史
             for i, (query, response) in enumerate(history[-max_turns + 1:]):
                 user_message(query, key=str(i) + "_user")
                 bot_message(response, key=str(i))
 
         user_message(input, key=str(len(history)) + "_user")
         # st.write("AI正在回复:")
         with st.empty():
             response = reply_func(input)
-            if isinstance(response, types.GeneratorType):
-                for _response in response:
-                    bot_message(_response)
-                response = _response
-            else:
-                bot_message(response)
+            bot_message(response)
 
     history.append((input, response))
     return history
 
 
-def set_popupwindow(title='这是一个弹窗', text='### 这是一个弹窗内容', padding=20, max_width=None):  # todo: 模仿写插件
+def set_popupwindow(title='这是一个弹窗', text='### 这是一个弹窗内容', padding=20, max_width=None): # todo: 模仿写插件
     from streamlit_modal import Modal
     modal = Modal(title, title, padding, max_width)
     if st.button("一键预测"):
         modal.open()
     if modal.is_open():
         with modal.container():
             pass
-
-
-def set_button():
-    css = """<style>
-     .stDownloadButton>button {
-         background-color: #0099ff;
-        color:#ffffff;
-    }
-    
-    .stDownloadButton>button:hover {
-       background-color: #00ff00;
-        color:#ff0000;
-       }
-    </style>
-    """
-    html(css)  # st.markdown
```

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/templates/css.py` & `AppZoo-2023.4.6.14.25.49/appzoo/templates/css.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/templates/index.html` & `AppZoo-2023.4.6.14.25.49/appzoo/templates/index.html`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/templates/meeting.html` & `AppZoo-2023.4.6.14.25.49/appzoo/templates/meeting.html`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/templates/upload.html` & `AppZoo-2023.4.6.14.25.49/appzoo/templates/upload.html`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/test.py` & `AppZoo-2023.4.6.14.25.49/appzoo/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,8 +41,12 @@
 app.add_route_plus(create_task)
 app.add_route_plus(get_task_result)
 
 
 if __name__ == '__main__':
 
     # app.run()
-    pass
+    from paddlenlp import Taskflow
+
+    ner = Taskflow('ner', entity_only=True)
+
+    disk_cache(ner)
```

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/Templates.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/Templates.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/handlers.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/image_utils.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/log/demo.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/log/demo.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/make_scheduler.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/make_scheduler.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/melog.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/melog.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/settings.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/settings.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/shap_app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/shap_app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/st_utils.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/st_utils.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/streamlit_utils.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/utils/upload.py` & `AppZoo-2023.4.6.14.25.49/appzoo/utils/upload.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/webs/app.py` & `AppZoo-2023.4.6.14.25.49/appzoo/webs/app.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/webs/jinja_example.py` & `AppZoo-2023.4.6.14.25.49/appzoo/webs/jinja_example.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/appzoo/webs/meeting.py` & `AppZoo-2023.4.6.14.25.49/appzoo/webs/meeting.py`

 * *Files identical despite different names*

### Comparing `AppZoo-2023.4.25.19.8.56/setup.py` & `AppZoo-2023.4.6.14.25.49/setup.py`

 * *Files identical despite different names*

