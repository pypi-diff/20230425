# Comparing `tmp/schoolware_api-0.2.0.tar.gz` & `tmp/schoolware_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-0.2.0.tar", last modified: Sat Mar 11 08:41:39 2023, max compression
+gzip compressed data, was "schoolware_api-1.0.0.tar", last modified: Tue Apr 25 10:16:21 2023, max compression
```

## Comparing `schoolware_api-0.2.0.tar` & `schoolware_api-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mb        (1000) mb        (1000)        0 2023-03-11 08:41:39.035739 schoolware_api-0.2.0/
--rw-rw-r--   0 mb        (1000) mb        (1000)     1813 2023-03-11 08:41:39.035739 schoolware_api-0.2.0/PKG-INFO
--rw-rw-r--   0 mb        (1000) mb        (1000)     1299 2023-03-11 08:31:32.000000 schoolware_api-0.2.0/README.md
--rw-rw-r--   0 mb        (1000) mb        (1000)      679 2023-03-11 08:26:59.000000 schoolware_api-0.2.0/pyproject.toml
-drwxrwxr-x   0 mb        (1000) mb        (1000)        0 2023-03-11 08:41:39.035739 schoolware_api-0.2.0/schoolware_api/
--rw-rw-r--   0 mb        (1000) mb        (1000)        0 2023-03-02 10:22:23.000000 schoolware_api-0.2.0/schoolware_api/__init__.py
--rw-rw-r--   0 mb        (1000) mb        (1000)    12195 2023-03-11 08:26:17.000000 schoolware_api-0.2.0/schoolware_api/schoolware_api.py
-drwxrwxr-x   0 mb        (1000) mb        (1000)        0 2023-03-11 08:41:39.035739 schoolware_api-0.2.0/schoolware_api.egg-info/
--rw-rw-r--   0 mb        (1000) mb        (1000)     1813 2023-03-11 08:41:39.000000 schoolware_api-0.2.0/schoolware_api.egg-info/PKG-INFO
--rw-rw-r--   0 mb        (1000) mb        (1000)      282 2023-03-11 08:41:39.000000 schoolware_api-0.2.0/schoolware_api.egg-info/SOURCES.txt
--rw-rw-r--   0 mb        (1000) mb        (1000)        1 2023-03-11 08:41:39.000000 schoolware_api-0.2.0/schoolware_api.egg-info/dependency_links.txt
--rw-rw-r--   0 mb        (1000) mb        (1000)       36 2023-03-11 08:41:39.000000 schoolware_api-0.2.0/schoolware_api.egg-info/requires.txt
--rw-rw-r--   0 mb        (1000) mb        (1000)       15 2023-03-11 08:41:39.000000 schoolware_api-0.2.0/schoolware_api.egg-info/top_level.txt
--rw-rw-r--   0 mb        (1000) mb        (1000)       38 2023-03-11 08:41:39.035739 schoolware_api-0.2.0/setup.cfg
--rw-rw-r--   0 mb        (1000) mb        (1000)      370 2023-03-11 08:27:07.000000 schoolware_api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:16:21.935533 schoolware_api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-25 10:16:21.935533 schoolware_api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-25 10:16:10.000000 schoolware_api-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-25 10:16:10.000000 schoolware_api-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:16:21.935533 schoolware_api-1.0.0/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:16:10.000000 schoolware_api-1.0.0/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-25 10:16:10.000000 schoolware_api-1.0.0/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:16:21.935533 schoolware_api-1.0.0/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-25 10:16:21.000000 schoolware_api-1.0.0/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-25 10:16:21.000000 schoolware_api-1.0.0/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:16:21.000000 schoolware_api-1.0.0/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 10:16:21.000000 schoolware_api-1.0.0/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 10:16:21.000000 schoolware_api-1.0.0/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:16:21.935533 schoolware_api-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 10:16:10.000000 schoolware_api-1.0.0/setup.py
```

### Comparing `schoolware_api-0.2.0/PKG-INFO` & `schoolware_api-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 0.2.0
+Version: 1.0.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Schoolware-api
-A api for schoolware written in python
+An api for schoolware written in python
 
-# capabilities
+## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
 
-# config
-domain: domain name of schoolware
-user: school microsaft email
-password: school microsaft password
-bg: background procces to keep token valid
-bot_token: telegram bot token to enable telegram bot
-chat_id: id to send messages to
-
-# install
-* ```pip3 install schoolware-api```
-* ```playwright install &&  playwright install-deps```
+## Config
+| Key | Description |
+| --- | --- |
+| domain | domain name of schoolware
+| user | school microsoft email
+| password | school microsoft password
+| bg | background procces to keep token valid
+| bot_token | telegram bot token to enable telegram bot
+| chat_id | id to send messages to
+| verbose | show a lot more info
+
+## Install
+* `pip3 install schoolware_api termcolor --upgrade `
+* `playwright install &&  playwright install-deps`
 
-# simple example
+## optional
+* `pip3 install python-telegram-bot`
 
-```
+## Simple example
+
+```python
 from schoolware_api import schoolware_api
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
 
 schoolware = schoolware_api.schoolware(config)
 
 print(schoolware.todo())  # Returns all todo items
 print(schoolware.punten()) # Returns all scores this schoolyear
 print(schoolware.agenda()) # Returns agenda points today
 print(schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
-# complete example
-```
+## Complete example
+```python
 from schoolware_api import schoolware_api
-{"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
+config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
 schoolware = schoolware_api.schoolware(config)
 
-same as other
+# same as other
 ```
```

### Comparing `schoolware_api-0.2.0/README.md` & `schoolware_api-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 
 # Schoolware-api
-A api for schoolware written in python
+An api for schoolware written in python
 
-# capabilities
+## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
 
-# config
-domain: domain name of schoolware
-user: school microsaft email
-password: school microsaft password
-bg: background procces to keep token valid
-bot_token: telegram bot token to enable telegram bot
-chat_id: id to send messages to
-
-# install
-* ```pip3 install schoolware-api```
-* ```playwright install &&  playwright install-deps```
+## Config
+| Key | Description |
+| --- | --- |
+| domain | domain name of schoolware
+| user | school microsoft email
+| password | school microsoft password
+| bg | background procces to keep token valid
+| bot_token | telegram bot token to enable telegram bot
+| chat_id | id to send messages to
+| verbose | show a lot more info
+
+## Install
+* `pip3 install schoolware_api termcolor --upgrade `
+* `playwright install &&  playwright install-deps`
 
-# simple example
+## optional
+* `pip3 install python-telegram-bot`
 
-```
+## Simple example
+
+```python
 from schoolware_api import schoolware_api
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
 
 schoolware = schoolware_api.schoolware(config)
 
 print(schoolware.todo())  # Returns all todo items
 print(schoolware.punten()) # Returns all scores this schoolyear
 print(schoolware.agenda()) # Returns agenda points today
 print(schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
-# complete example
-```
+## Complete example
+```python
 from schoolware_api import schoolware_api
-{"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
+config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
 schoolware = schoolware_api.schoolware(config)
 
-same as other
-```
+# same as other
+```
```

### Comparing `schoolware_api-0.2.0/pyproject.toml` & `schoolware_api-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "0.2.0"
+version = "1.0.0"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-0.2.0/schoolware_api/schoolware_api.py` & `schoolware_api-1.0.0/schoolware_api/schoolware_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,19 +46,15 @@
             print("getting startup token")
         self.check_if_valid()
         self.num_points = len(self.punten())
         
 #Token&cookie stuff
     def get_new_token(self):
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            start_time = time.time()
-            print(colored("• Starting get token", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_print(self,"get_token")
         ##########VERBOSE##########
 
         with sync_playwright() as p:
             browser = p.chromium.launch()
             context = browser.new_context(user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0")
             page = context.new_page()
             page.goto(f"https://{self.domain}/webleerling/start.html#!fn=llagenda")
@@ -69,56 +65,44 @@
             page.get_by_text("Sign In").click()
             page.wait_for_load_state()
             if(context.cookies()[0]["name"] == "FPWebSession"):
                 self.token = context.cookies()[0]["value"]
                 self.cookie = dict(FPWebSession=self.token)
             browser.close()
             ##########VERBOSE##########
-            if(self.verbose):
-                print(colored("#"*50, "grey"))
-                end_time = time.time()
-                print(colored(f"• Done getting token time:{end_time - start_time}", "green"))
-                print(colored("#"*50, "grey"))
+            verbose_end(self,"get_token")
             ##########VERBOSE##########
             return self.token
     
     def check_if_valid(self):
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            start_time = time.time()
-            print(colored(f"• Starting check token", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_print(self,"check_token")
         ##########VERBOSE##########
 
         r = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/myschoolwareaccount", cookies=self.cookie)
 
-        ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            end_time = time.time()
-            print(colored(f"• Done checking token time:{end_time - start_time}", "green"))
-            print(colored("#"*50, "grey"))
-        ##########VERBOSE##########
+
         if (r.status_code != 200):
             if(r.status_code == 401):
+                ##########VERBOSE##########
+                verbose_end(self,"check_token invalid")
+                ##########VERBOSE##########
                 self.get_new_token()
             else:
                 raise "error with token"
         else:
+            ##########VERBOSE##########
+            verbose_end(self,"check_token")
+            ##########VERBOSE##########
             return True
 
 #todo
     def todo(self):
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            start_time = time.time()
-            print(colored("• Starting todo", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_print(self,"todo")
         ##########VERBOSE##########
 
         self.check_if_valid()
         task_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/AgendaPunt/?_dc=1665240724814&MinVan={date.today()}T00:00:00&IsTaakOfToets=true", cookies=self.cookie).json()["data"]
         self.todo_list = []
 
         for taak in task_data:
@@ -129,39 +113,34 @@
             elif(taak["TypePunt"] == 101):
                 soort="hertoets"
 
             vak= taak["VakNaam"]
             titel= taak["Titel"]
             onderwerp= taak["Commentaar"]
             eind_time = taak["Tot"].split(' ')[0]
+            dt = datetime.strptime(taak["Tot"].split(' ')[0], '%Y-%m-%d')
+            day = dt.strftime('%A')
 
             self.todo_list.append({
                 "soort": soort,
                 "vak": vak,
                 "titel": titel,
                 "onderwerp": onderwerp,
-                "eind_time": eind_time
+                "eind_time": eind_time,
+                "day": day
             })
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            end_time = time.time()
-            print(colored(f"• Done todo time:{end_time - start_time}", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_end(self,"todo")
         ##########VERBOSE##########
         return self.todo_list
 
 #punten
     def punten(self):
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            start_time = time.time()
-            print(colored("• Starting punten", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_print(self,"punten")
         ##########VERBOSE##########
         self.check_if_valid()
         punten_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/PuntenbladGridLeerling?&Leerling=15201&?BeoordelingMomentVan=1990-09-01+00:00:00", cookies=self.cookie).json()["data"]
         self.scores = []
         for vak in punten_data:
 
             for punt in vak["Beoordelingen"]:
@@ -172,48 +151,43 @@
                 try:
                     behaalde_score = float(punt["BeoordelingWaarde"]["NumeriekAsString"])
                 except:
                     behaalde_score = "n/a"
                 publicatie_datum = punt["BeoordelingMomentPublicatieDatum"]
                 datum = punt["BeoordelingMomentDatum"]
                 titel = punt["BeoordelingMomentOmschrijving"]
+                dt = datetime.strptime(punt["BeoordelingMomentDatum"].split(' ')[0], '%Y-%m-%d')
+                day = dt.strftime('%A')
                 if(punt["BeoordelingMomentType_"] == "bmtToets"):
                     soort = "toets"
                 else:
                     soort = "taak"
 
                 self.scores.append({
                     "soort": soort,
                     "vak": vak,
                     "titel": titel,
                     "DW": DW,
                     "tot_sc": totale_score,
                     "gew_sc": gewenste_score,
                     "score": behaalde_score,
                     "datum": datum,
-                    "pub_datum": publicatie_datum
+                    "pub_datum": publicatie_datum,
+                    "day": day
                 })
         self.scores.sort(key=lambda x: datetime.strptime(x['datum'], '%Y-%m-%d %H:%M:%S'), reverse=True)
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            end_time = time.time()
-            print(colored(f"• Done punten time:{end_time - start_time}", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_end(self,"punten")
         ##########VERBOSE##########
         return self.scores
 
 #agenda
     def agenda(self, datum=""):
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            start_time = time.time()
-            print(colored("• Starting agenda", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_print(self,"_agenda")
         ##########VERBOSE##########
         self.check_if_valid()
         #begin en einde week
         day = str(date.today())
         dt = datetime.strptime(day, '%Y-%m-%d')
         start = (dt - timedelta(days=dt.weekday())).strftime('%Y-%m-%d')
         if(self.verbose):
@@ -224,36 +198,26 @@
         ####
         agenda_data = requests.get(f"https://kov.schoolware.be/webleerling/bin/server.fcgi/REST/AgendaPunt/?_MaxVan={end}&MinTot={start}", cookies=self.cookie).json()["data"]
         self.rooster = []
         for agenda in agenda_data:
             if(agenda["TypePunt"]==1 or agenda["TypePunt"]==2):
                 self.rooster.append(agenda)
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            end_time = time.time()
-            print(colored(f"• Done agenda time:{end_time - start_time}", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_end(self,"agenda")
         ##########VERBOSE##########
         return self.filter_rooster(self.rooster, datum)
 
     def filter_rooster(self, rooster, datum=""):
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            start_time = time.time()
-            print(colored("• Starting filter_agenda", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_print(self,"filter_agenda")
         ##########VERBOSE##########
         today = []
         if(datum == ""):
             datum = datetime.today()
-
         datum = str(datum).split(' ')[0]
-
         for agenda in rooster:
             if(str(agenda['Van'].split(' ')[0]) == datum):
                 vak = agenda['VakNaam']
                 lokaal = agenda['LokaalCode']
                 titel = agenda['Titel']
                 uur = agenda['Van'].split(' ')[1]
 
@@ -279,34 +243,32 @@
                         agenda["skip"] = True
                     elif(today[index+1]["vak"] == today[index+1]["titel"]):
                         today[index+1]["skip"] = True
                         today_filterd.append(agenda)
                 else:
                     today_filterd.append(agenda)
         ##########VERBOSE##########
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            end_time = time.time()
-            print(colored(f"• Done filter-agenda time:{end_time - start_time}", "green"))
-            print(colored("#"*50, "grey"))
+        verbose_end(self,"filter-agenda")
         ##########VERBOSE##########
 
         return today_filterd
-            
+
+##########OTHER##########
+
 #bg procces
 def bg(self):
     from time import sleep
     if(self.verbose):
         print(colored("background procces started","blue"))
     while True:
         sleep(5*60)
         if(self.verbose):
             print(colored("background task: checking token","blue"))
         self.check_if_valid()
-
+#telegram bot
 def telegram_def(self):
     import telegram
     from time import sleep
     import asyncio
     if(self.verbose):
         self.bot = telegram.Bot(self.config["bot_token"])
     print(colored("telegram started","blue"))
@@ -317,11 +279,25 @@
         num_now = len(self.punten())
         if(self.num_points < num_now):
             diff = num_now - self.num_points
             self.num_points = num_now
             
             asyncio.run(telegram_send_msg(self, diff))
 
-
 async def telegram_send_msg(self, diff):
     async with self.bot:
-        await self.bot.send_message(text=f'{diff} New point(s)', chat_id=self.config["chat_id"])
+        await self.bot.send_message(text=f'{diff} New point(s)', chat_id=self.config["chat_id"])
+
+##########VERBOSE##########
+def verbose_print(self,message):
+    if(self.verbose):
+        print(colored("#"*50, "grey"))
+        self.start_time = time.time()
+        print(colored(f"• starting {message}", "green"))
+        print(colored("#"*50, "grey"))
+def verbose_end(self,message):
+    if(self.verbose):
+        print(colored("#"*50, "grey"))
+        end_time = time.time()
+        print(colored(f"• Done {message} time:{end_time - self.start_time}", "green"))
+        print(colored("#"*50, "grey"))
+##########VERBOSE##########
```

### Comparing `schoolware_api-0.2.0/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.0.0/schoolware_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 0.2.0
+Version: 1.0.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # Schoolware-api
-A api for schoolware written in python
+An api for schoolware written in python
 
-# capabilities
+## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
 
-# config
-domain: domain name of schoolware
-user: school microsaft email
-password: school microsaft password
-bg: background procces to keep token valid
-bot_token: telegram bot token to enable telegram bot
-chat_id: id to send messages to
-
-# install
-* ```pip3 install schoolware-api```
-* ```playwright install &&  playwright install-deps```
+## Config
+| Key | Description |
+| --- | --- |
+| domain | domain name of schoolware
+| user | school microsoft email
+| password | school microsoft password
+| bg | background procces to keep token valid
+| bot_token | telegram bot token to enable telegram bot
+| chat_id | id to send messages to
+| verbose | show a lot more info
+
+## Install
+* `pip3 install schoolware_api termcolor --upgrade `
+* `playwright install &&  playwright install-deps`
 
-# simple example
+## optional
+* `pip3 install python-telegram-bot`
 
-```
+## Simple example
+
+```python
 from schoolware_api import schoolware_api
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
 
 schoolware = schoolware_api.schoolware(config)
 
 print(schoolware.todo())  # Returns all todo items
 print(schoolware.punten()) # Returns all scores this schoolyear
 print(schoolware.agenda()) # Returns agenda points today
 print(schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
-# complete example
-```
+## Complete example
+```python
 from schoolware_api import schoolware_api
-{"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
+config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
 schoolware = schoolware_api.schoolware(config)
 
-same as other
+# same as other
 ```
```

