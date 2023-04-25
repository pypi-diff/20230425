# Comparing `tmp/xyz_util-0.7.5-py3-none-any.whl.zip` & `tmp/xyz_util-0.7.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 50979 bytes, number of entries: 25
+Zip file size: 51026 bytes, number of entries: 25
 -rw-r--r--  2.0 unx       88 b- defN 20-Jan-17 14:46 xyz_util/__init__.py
--rw-r--r--  2.0 unx      665 b- defN 22-Apr-11 04:56 xyz_util/cmdutils.py
+-rw-r--r--  2.0 unx      732 b- defN 23-Apr-25 02:25 xyz_util/cmdutils.py
 -rw-r--r--  2.0 unx     9639 b- defN 23-Jan-12 06:48 xyz_util/crawlutils.py
 -rw-r--r--  2.0 unx      903 b- defN 18-Oct-15 06:43 xyz_util/cryptutils.py
 -rw-r--r--  2.0 unx    15883 b- defN 23-Jan-20 15:50 xyz_util/datautils.py
 -rw-r--r--  2.0 unx     6400 b- defN 21-Aug-09 10:21 xyz_util/dateutils.py
 -rw-r--r--  2.0 unx    13185 b- defN 21-Jul-04 23:24 xyz_util/dbutils.py
 -rw-r--r--  2.0 unx    17205 b- defN 21-Jul-26 09:02 xyz_util/excelutils.py
 -rw-r--r--  2.0 unx     2667 b- defN 21-Jul-04 23:24 xyz_util/formutils.py
 -rw-r--r--  2.0 unx     4613 b- defN 21-Dec-19 01:47 xyz_util/importutils.py
--rw-r--r--  2.0 unx     2843 b- defN 23-Apr-03 12:29 xyz_util/mediautils.py
+-rw-r--r--  2.0 unx     2862 b- defN 23-Apr-21 07:44 xyz_util/mediautils.py
 -rw-r--r--  2.0 unx    13998 b- defN 22-Aug-03 00:02 xyz_util/modelutils.py
 -rw-r--r--  2.0 unx    16893 b- defN 23-Mar-23 07:06 xyz_util/mongoutils.py
 -rw-r--r--  2.0 unx    14661 b- defN 21-Jul-13 11:57 xyz_util/pandasutils.py
 -rw-r--r--  2.0 unx      507 b- defN 21-Jun-01 00:29 xyz_util/pdfutils.py
 -rw-r--r--  2.0 unx    15349 b- defN 22-Jul-04 08:21 xyz_util/statutils.py
 -rw-r--r--  2.0 unx     1997 b- defN 23-Mar-06 16:57 xyz_util/textutils.py
 -rw-r--r--  2.0 unx     1675 b- defN 20-Aug-01 15:19 xyz_util/transferutils.py
 -rw-r--r--  2.0 unx     5316 b- defN 21-Jun-05 23:16 xyz_util/validators.py
 -rw-r--r--  2.0 unx     7815 b- defN 21-May-26 06:42 xyz_util/views.py
 -rw-r--r--  2.0 unx     3956 b- defN 21-Jul-04 23:24 xyz_util/widgetutils.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Apr-04 02:35 xyz_util-0.7.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 02:35 xyz_util-0.7.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-04 02:35 xyz_util-0.7.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1949 b- defN 23-Apr-04 02:35 xyz_util-0.7.5.dist-info/RECORD
-25 files, 159364 bytes uncompressed, 47895 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx     1056 b- defN 23-Apr-25 02:47 xyz_util-0.7.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 02:47 xyz_util-0.7.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-25 02:47 xyz_util-0.7.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1949 b- defN 23-Apr-25 02:47 xyz_util-0.7.6.dist-info/RECORD
+25 files, 159450 bytes uncompressed, 47942 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: xyz_util/views.py
 Comment: 
 
 Filename: xyz_util/widgetutils.py
 Comment: 
 
-Filename: xyz_util-0.7.5.dist-info/METADATA
+Filename: xyz_util-0.7.6.dist-info/METADATA
 Comment: 
 
-Filename: xyz_util-0.7.5.dist-info/WHEEL
+Filename: xyz_util-0.7.6.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_util-0.7.5.dist-info/top_level.txt
+Filename: xyz_util-0.7.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_util-0.7.5.dist-info/RECORD
+Filename: xyz_util-0.7.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_util/cmdutils.py

```diff
@@ -15,7 +15,10 @@
     else:
         if without_output:
             DEVNULL = open(os.devnull, 'wb')
             subprocess.Popen(cmd, stdout=DEVNULL, stderr=DEVNULL)
         else:
             p = subprocess.Popen(cmd, stdout=subprocess.PIPE)
             return p.stdout.read()
+
+def get_files(path):
+    return cmd_call(f'ls {path}').split('\n')
```

## xyz_util/mediautils.py

```diff
@@ -52,15 +52,15 @@
 
     def video_set_audio(self, video_path, audio_path, save_path, **kwargs):
         return self.execute('-i', video_path, '-i', audio_path, '-map', '0:v', '-map', '1:a', '-c:v', 'copy', save_path,
                             **kwargs)
 
     def images_to_video(self, images_path, video_path, fps=5, **kwargs):
         return self.execute('-r', f'{fps}', '-i', images_path, '-pix_fmt', 'yuv420p', '-vf',
-                            "pad=ceil(iw/2)*2:ceil(ih/2)*2", video_path, **kwargs)
+                            "pad=ceil(iw/2)*2:ceil(ih/2)*2", '-c:v', 'libx265', video_path, **kwargs)
 
     def video_concat(self, videos, output, **kwargs):
         inputs = []
         streams = ''
         n = len(videos)
         for i, v in enumerate(videos):
             streams += f'[{i}:0][{i}:1]'
```

## Comparing `xyz_util-0.7.5.dist-info/METADATA` & `xyz_util-0.7.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-util
-Version: 0.7.5
+Version: 0.7.6
 Summary: common utils
 Home-page: https://github.com/szuprefix/py-xyz-util
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_util-0.7.5.dist-info/RECORD` & `xyz_util-0.7.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 xyz_util/__init__.py,sha256=WEJvfVJ_HXMJKRpMfXP0srWexMdmSlu_Nq5AIb9Ciio,88
-xyz_util/cmdutils.py,sha256=ijHv3riYdAWwPevj_jqS5PW0B88J0Xp6DSSvbVbV6sk,665
+xyz_util/cmdutils.py,sha256=6BKHJzt0eT4kd2Dym5a-q0iUTXIXicTXab5_Cz4bfJI,732
 xyz_util/crawlutils.py,sha256=a0fP1DzAuzux9p-QcIftS-ZnaGfA87aTtgxhtErMr5U,9639
 xyz_util/cryptutils.py,sha256=UVNZlZ-7d-X7rWjUxMPv8EpvtXIyI6YKPZNgb6MCx_Q,903
 xyz_util/datautils.py,sha256=sW0N9-sj26pwmG6bnsia9Lnny3P1KWvyUaup2982PUg,15883
 xyz_util/dateutils.py,sha256=doPQh86iJNIWhA1EsZy1ar3Vgw3RSFAxUkTgPX_RU3s,6400
 xyz_util/dbutils.py,sha256=Wj4Bf7tJg2UzwTP5-p4rCACXTaIvH5J6milAOpAGHUk,13185
 xyz_util/excelutils.py,sha256=FuK1RnGPG1XFRNDyYbKPK7urc9tvgNXFtR9-NLlamkE,17205
 xyz_util/formutils.py,sha256=bM5pEShw-gmUm5RMVyQ9xPO7RAHZ4TNTwaFXlzebvmU,2667
 xyz_util/importutils.py,sha256=9EQaTCRYVzWAo9SHpffFV1XqFND9MU0e63KMJPmx1bI,4613
-xyz_util/mediautils.py,sha256=Jk8E4oLnK2SeG68OzmsPlU7vz9Sz60M-ZN7g6aBk9kU,2843
+xyz_util/mediautils.py,sha256=LxrlY0XAqo3oImrKm87S7SriORUGTbedM7v2pNIK3sQ,2862
 xyz_util/modelutils.py,sha256=wuwMbTCL3RIjPOlbpuxC55dqfET5SsitV_gu0tRHwHk,13998
 xyz_util/mongoutils.py,sha256=vilihwLZ7g6n89a02nOhXvcIxu8UTTzdf4t3qywZWDM,16893
 xyz_util/pandasutils.py,sha256=gOuey7Vf6E62WFYVM4T2EwER9WQ_4Tmk4Ays0h6bCTQ,14661
 xyz_util/pdfutils.py,sha256=EFWIB4j74NHaCmGuVTZGSRbvoB-spl0Vj1_BKFjZl2I,507
 xyz_util/statutils.py,sha256=pl1Dn4rIPYfaZnSEkmPbfY5Z_tItKpeqor01tfPkE6Y,15349
 xyz_util/textutils.py,sha256=AYJm8SQrq-CxyLA4G9bzJyiFFcNW57NckRU0X2CItLI,1997
 xyz_util/transferutils.py,sha256=76VLi9Fjt3whO42oDvBJ0R2_CFzCkxeVxcfIB7VWtrc,1675
 xyz_util/validators.py,sha256=8qulZP-yPyal_GJWzmQzkm8yCHiMuGJ_hVPmK8bW-Ww,5316
 xyz_util/views.py,sha256=X2_JtrTLmg_nzaAHRKuh4umUtgmFsnVvcFFNRtlUfOo,7815
 xyz_util/widgetutils.py,sha256=uTZenfxd0zXpRx40lgS86kU0BKccYyg_Sh3XdmUVg7Q,3956
-xyz_util-0.7.5.dist-info/METADATA,sha256=HSCy3XmHl42a9G8dposoGtRefnzlufkgrk4NQIcAUb4,1056
-xyz_util-0.7.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_util-0.7.5.dist-info/top_level.txt,sha256=0uGpvx0NID3M2oMuWv7LYVDnUpUIIOwIWp8Br1tItgM,9
-xyz_util-0.7.5.dist-info/RECORD,,
+xyz_util-0.7.6.dist-info/METADATA,sha256=PjWTyUJqhiEZdMxbKsfclzbt_ydM_YO2wUt5Q13XaQA,1056
+xyz_util-0.7.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_util-0.7.6.dist-info/top_level.txt,sha256=0uGpvx0NID3M2oMuWv7LYVDnUpUIIOwIWp8Br1tItgM,9
+xyz_util-0.7.6.dist-info/RECORD,,
```

