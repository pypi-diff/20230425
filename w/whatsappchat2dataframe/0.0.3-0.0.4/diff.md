# Comparing `tmp/whatsappchat2dataframe-0.0.3.tar.gz` & `tmp/whatsappchat2dataframe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsappchat2dataframe-0.0.3.tar", last modified: Thu Apr 20 20:57:37 2023, max compression
+gzip compressed data, was "whatsappchat2dataframe-0.0.4.tar", last modified: Tue Apr 25 10:38:32 2023, max compression
```

## Comparing `whatsappchat2dataframe-0.0.3.tar` & `whatsappchat2dataframe-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:57:37.668117 whatsappchat2dataframe-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-04-20 19:12:16.000000 whatsappchat2dataframe-0.0.3/LICENCE
--rw-rw-rw-   0        0        0     1074 2023-04-20 20:57:37.668117 whatsappchat2dataframe-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-04-20 20:55:19.000000 whatsappchat2dataframe-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 20:57:37.668117 whatsappchat2dataframe-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-20 20:55:58.000000 whatsappchat2dataframe-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:57:37.650116 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/
--rw-rw-rw-   0        0        0       59 2023-04-20 12:54:20.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/__init__.py
--rw-rw-rw-   0        0        0     2002 2023-04-20 19:43:39.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/chat2dataframe.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:57:37.667123 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/
--rw-rw-rw-   0        0        0     1074 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-20 20:57:37.000000 whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:38:32.846175 whatsappchat2dataframe-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-20 19:12:16.000000 whatsappchat2dataframe-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0     1074 2023-04-25 10:38:32.846175 whatsappchat2dataframe-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-04-20 20:55:19.000000 whatsappchat2dataframe-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:38:32.846175 whatsappchat2dataframe-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-25 10:38:18.000000 whatsappchat2dataframe-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:38:32.835175 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe/
+-rw-rw-rw-   0        0        0       59 2023-04-20 12:54:20.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-25 10:36:11.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe/chat2dataframe.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:38:32.845175 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/
+-rw-rw-rw-   0        0        0     1074 2023-04-25 10:38:32.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-04-25 10:38:32.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:38:32.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 10:38:32.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-25 10:38:32.000000 whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/top_level.txt
```

### Comparing `whatsappchat2dataframe-0.0.3/LICENCE` & `whatsappchat2dataframe-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `whatsappchat2dataframe-0.0.3/PKG-INFO` & `whatsappchat2dataframe-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsappchat2dataframe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converts a Whatsapp chat (.txt file) into a pandas DataFrame
 Author: Kiran Busch
 Author-email: <kiranbusch@t-online.de>
 Keywords: python,whatsapp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whatsappchat2dataframe-0.0.3/setup.py` & `whatsappchat2dataframe-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Converts a Whatsapp chat (.txt file) into a pandas DataFrame'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="whatsappchat2dataframe",
     version=VERSION,
```

### Comparing `whatsappchat2dataframe-0.0.3/whatsappchat2dataframe/chat2dataframe.py` & `whatsappchat2dataframe-0.0.4/whatsappchat2dataframe/chat2dataframe.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         Args:
             path_to_filename (str): path to file e.g. data/chat.txt
 
         Returns:
             pd.DataFrame: return a pandas DataFrame of the .txt file
         """
         self.DATE_TIME = re.compile(r"([\[]).*?([\]])")
+        self.DATE_TIME = re.compile(r"[\[]*[0-9]+[\./][0-9]+[\./][0-9]+..[0-9]+:[0-9]+[:]*([0-9]+)*[\]]*[-]*")
         self.AUTHOR = re.compile(r"((( [a-zA-ZöäüÖÄÜ]+)+):)")
         self.LTR = chr(8206)
         try:
             with open(path_to_filename, 'r') as file:
                 self.data = file.read().replace('\n', '')
         except Exception as e:
             print(f"Could not process {path_to_filename}, because the following error occured: {type(e).__name__}: {str(e)}")
@@ -35,18 +36,26 @@
         df['numMessage']=1
         return df
 
     def __to_pd_row(self, s):
         match = self.DATE_TIME.match(s)
         if match:
             g = match.group(0)
-            date = g[1:9]
-            time = g[11:-1]
+            date_time = g.replace('[','').replace(']','').replace(' ','').split(',')
             author = re.search(self.AUTHOR, s).group(0)[1:-1]
             message = s.split(': ')[1]
-            return pd.to_datetime(f'{date}-{time}', format="%d.%m.%y-%H:%M:%S"), author, message.replace("\n", "")
+            return self.__try_parsing_date(date_time), author, message.replace("\n", "")
         
     def __chat2df(self,data):
         start_positions_date = [m.start() for m in re.finditer(self.DATE_TIME, data)]
         for start,end in tqdm(list(zip(start_positions_date[:-1],start_positions_date[1:])), desc='Read messages'):
             subdata = data[start:end]
-            yield self.__to_pd_row(subdata.replace(self.LTR, ""))
+            if len(self.AUTHOR.findall(subdata))>0:
+                yield self.__to_pd_row(subdata.replace(self.LTR, ""))
+    
+    def __try_parsing_date(self,date_time):
+        for fmt in ("%d.%m.%y-%H:%M:%S", "%Y/%m/%d-%H:%M:%S", "%d/%m/%y-%H:%M", "%d.%m.%y-%H:%M"):
+            try:
+                return pd.to_datetime(f'{date_time[0]}-{date_time[1]}', format=fmt)
+            except ValueError:
+                pass
+        raise ValueError(f'no valid date format found for "{str(date_time[0])}-{str(date_time[1])}"')
```

### Comparing `whatsappchat2dataframe-0.0.3/whatsappchat2dataframe.egg-info/PKG-INFO` & `whatsappchat2dataframe-0.0.4/whatsappchat2dataframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsappchat2dataframe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converts a Whatsapp chat (.txt file) into a pandas DataFrame
 Author: Kiran Busch
 Author-email: <kiranbusch@t-online.de>
 Keywords: python,whatsapp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

