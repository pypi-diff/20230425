# Comparing `tmp/operbot-170.tar.gz` & `tmp/operbot-171.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operbot-170.tar", last modified: Mon Apr 17 15:53:45 2023, max compression
+gzip compressed data, was "operbot-171.tar", last modified: Tue Apr 25 08:59:08 2023, max compression
```

## Comparing `operbot-170.tar` & `operbot-171.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-17 15:53:45.140474 operbot-170/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-13 20:09:14.000000 operbot-170/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.136474 operbot-170/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2680 2023-04-17 15:49:49.000000 operbot-170/bin/operbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)      950 2023-04-13 20:18:15.000000 operbot-170/bin/operbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-13 20:44:02.000000 operbot-170/bin/operbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-13 20:17:12.000000 operbot-170/bin/operbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.136474 operbot-170/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-13 20:41:39.000000 operbot-170/files/operbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.136474 operbot-170/operbot/
--rw-r--r--   0 bart      (1000) bart      (1001)       91 2023-04-13 20:37:44.000000 operbot-170/operbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-13 20:14:50.000000 operbot-170/operbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-16 22:43:23.000000 operbot-170/operbot/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1713 2023-04-17 15:52:54.000000 operbot-170/operbot/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/operbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 20:14:58.000000 operbot-170/operbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-13 20:14:58.000000 operbot-170/operbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-13 20:22:31.000000 operbot-170/operbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-13 20:22:44.000000 operbot-170/operbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1130 2023-04-13 20:23:05.000000 operbot-170/operbot/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17293 2023-04-17 15:50:03.000000 operbot-170/operbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      894 2023-04-13 20:23:30.000000 operbot-170/operbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7720 2023-04-13 20:24:16.000000 operbot-170/operbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-13 20:24:29.000000 operbot-170/operbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)      997 2023-04-13 20:24:42.000000 operbot-170/operbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-16 21:53:04.000000 operbot-170/operbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-13 20:25:19.000000 operbot-170/operbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2632 2023-04-13 20:25:32.000000 operbot-170/operbot/modules/usr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-17 14:44:06.000000 operbot-170/operbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3462 2023-04-17 14:05:02.000000 operbot-170/operbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-14 16:23:57.000000 operbot-170/operbot/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-16 21:54:33.000000 operbot-170/operbot/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-13 20:14:50.000000 operbot-170/operbot/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/operbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      801 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-17 15:53:45.000000 operbot-170/operbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-17 15:53:45.140474 operbot-170/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-17 12:23:48.000000 operbot-170/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-17 15:53:45.140474 operbot-170/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-13 20:09:14.000000 operbot-170/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-13 20:09:14.000000 operbot-170/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-13 20:09:14.000000 operbot-170/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-13 20:09:14.000000 operbot-170/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-13 20:09:14.000000 operbot-170/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 08:59:08.897756 operbot-171/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-25 07:12:36.000000 operbot-171/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2846 2023-04-25 07:12:36.000000 operbot-171/bin/operbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      948 2023-04-25 07:12:36.000000 operbot-171/bin/operbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-25 07:12:36.000000 operbot-171/bin/operbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-25 07:12:36.000000 operbot-171/bin/operbotd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-25 07:12:36.000000 operbot-171/files/operbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/operbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)      147 2023-04-25 08:55:43.000000 operbot-171/operbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2834 2023-04-25 08:58:33.000000 operbot-171/operbot/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-25 07:15:29.000000 operbot-171/operbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-25 07:15:29.000000 operbot-171/operbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-04-25 07:15:29.000000 operbot-171/operbot/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/operbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17599 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      918 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7792 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1022 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2657 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-25 07:15:29.000000 operbot-171/operbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4661 2023-04-25 07:15:29.000000 operbot-171/operbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      211 2023-04-25 07:19:01.000000 operbot-171/operbot/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-25 07:15:29.000000 operbot-171/operbot/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-25 07:15:29.000000 operbot-171/operbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-25 07:15:29.000000 operbot-171/operbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/operbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      817 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-25 08:59:08.897756 operbot-171/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-25 07:12:36.000000 operbot-171/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-25 07:12:36.000000 operbot-171/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-25 07:12:36.000000 operbot-171/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-25 07:12:36.000000 operbot-171/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-25 07:12:36.000000 operbot-171/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-25 07:12:36.000000 operbot-171/test/test_storage.py
```

### Comparing `operbot-170/PKG-INFO` & `operbot-171/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 170
+Version: 171
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-170/README.rst` & `operbot-171/README.rst`

 * *Files identical despite different names*

### Comparing `operbot-170/bin/operbot` & `operbot-171/bin/operbot`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,C0413,W0212,E0611,E0401,I1101
 
 
-'operator bot'
+'object programming bot'
 
 
 import os
+import readline
 import sys
 import termios
 import time
 import traceback
 
 
 sys.path.insert(0, os.getcwd())
 
 
 import operbot.modules
 
 
 from operbot.handler import Client, Error, command, parse
 from operbot.loggers import Logging
+from operbot.objects import update
 from operbot.persist import Persist
+from operbot.runtime import Cfg
 from operbot.scanner import importer, scandir, scanpkg, starter
 from operbot.threads import launch
 
 
-MOD = "cmd,err,irc,log,rss,sts,thr"
-NAME = "operbot"
+readline.redisplay()
 
 
-date = time.ctime(time.time()).replace('  ', ' ')
+MOD = ",cmd,err,irc,log,rss,sts,tdo,thr"
+
+
+Persist.workdir = os.path.expanduser("~/.%s" % Cfg.name)
 
 
-Persist.workdir = os.path.expanduser("~/.%s" % NAME)
+date = time.ctime(time.time()).replace('  ', ' ')
 
 
 def cprint(txt):
-    print(txt)
-    sys.stdout.flush()
+    if "v" in Cfg.opts:
+        print(txt)
+        sys.stdout.flush()
 
 
-Logging.debug = cprint
+Logging.raw = cprint
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
@@ -103,29 +109,31 @@
             termios.tcsetattr(fds, termios.TCSADRAIN, old)
         waiter()
 
 
 def main():
     dowait = False
     cfg = parse(' '.join(sys.argv[1:]))
+    update(Cfg, cfg)
+    mod = Cfg.sets.mod
     if os.path.exists("modules"):
-        scandir("modules", importer, cfg.mod or MOD)
-    scanpkg(operbot.modules, importer, cfg.mod or MOD)
+        scandir("modules", importer, mod + MOD)
+    scanpkg(operbot.modules, importer, mod + MOD)
     if cfg.txt:
         cli = CLI()
         command(cli, cfg.otxt)
     elif 'd' in cfg.opts:
         daemon()
         dowait = True
     elif 'c' in cfg.opts:
-        print(f'{NAME.upper()} started {date}')
+        print(f'{Cfg.name.upper()} started {date}')
         dowait = True
     if dowait:
-        scanpkg(operbot.modules, starter, cfg.mod or MOD)
-        scandir("modules", starter, cfg.mod or MOD)
+        scanpkg(operbot.modules, starter, mod + MOD)
+        scandir("modules", starter, mod + MOD)
         if "c" in cfg.opts:
             csl = Console()
             launch(csl.loop)
         while 1:
             time.sleep(1.0)
             waiter()
```

### Comparing `operbot-170/bin/operbotcmd` & `operbot-171/bin/operbotcmd`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,C0413,W0212,E0611,E0401
+# pylint: disable=C0115,C0116,C0413,W0212,E0611,E0401,R0201
 
 
 'operator bot'
 
 
 import os
 import sys
@@ -13,29 +13,30 @@
 
 sys.path.insert(0, os.getcwd())
 
 
 import operbot.modules
 
 
-from operbot.handler import Client, Error
-from operbot.handler import command, parse
-from operbot.persist import Persist
-from operbot.scanner import scanpkg, importer
+from opb.handler import Client, Error
+from opb.handler import command, parse
+from opb.persist import Persist
+from opb.scanner import scanpkg, importer
 
 
-Persist.workdir = "/var/lib/operbot/"
+Persist.workdir = "/var/lib/opb/"
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
-    def raw(self, txt):
+    @staticmethod
+    def raw(txt):
         print(txt)
         sys.stdout.flush()
 
 
 def waiter():
     got = []
     for ex in Error.errors:
```

### Comparing `operbot-170/bin/operbotd` & `operbot-171/bin/operbotd`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/clocked.py` & `operbot-171/operbot/clocked.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/handler.py` & `operbot-171/operbot/handler.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/modules/irc.py` & `operbot-171/operbot/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import threading
 import _thread
 
 
 from ..handler import Client, Command, Error, Event, Listens
 from ..loggers import Logging
 from ..objects import Default, Object, edit, keys, prt
-from ..persist import last, write
+from ..persist import Class, last, write
+from ..runtime import Cfg
 from ..threads import launch
 
 
 from .usr import Users
 
 
 def __dir__():
@@ -35,40 +36,43 @@
             'cfg',
             'mre',
             'pwd',
             'start'
            )
 
 
-NAME = "operbot"
-
-
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
-    #irc.joined.wait()
+    if "v" in Cfg.opts:
+        Logging.debug(prt(
+                          irc.cfg,
+                          ",".join(keys(irc.cfg)),
+                          skip='control,password,realname,sleep,username')
+                         )
+        irc.joined.wait()
     return irc
 
 
 class Config(Default):
 
-    channel = '#%s' % NAME
+    channel = '#%s' % Cfg.name
     control = '!'
-    nick = NAME
+    nick = Cfg.name
     password = ''
     port = 6667
-    realname = NAME
+    realname = Cfg.name
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = NAME
+    username = Cfg.name
     users = False
 
     def __init__(self):
         Default.__init__(self)
         self.control = Config.control
         self.channel = Config.channel
         self.nick = Config.nick
@@ -79,14 +83,17 @@
         self.server = Config.server
         self.servermodes = Config.servermodes
         self.sleep = Config.sleep
         self.username = Config.username
         self.users = Config.users
 
 
+Class.add(Config)
+
+
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = True
         self.fix_sentence_endings = True
@@ -258,27 +265,28 @@
             os.set_inheritable(self.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.connected.set()
             return True
         return False
 
+
     def direct(self, txt):
         Logging.debug(txt)
         self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as ex:
-            Logging.debug(str(ex))
+            Error.errors.append(ex)
 
     def docommand(self, evt):
         evt.orig = repr(self)
         Command.handle(evt)
 
     def doconnect(self, server, nck, port=6667):
         while 1:
@@ -361,18 +369,18 @@
                 break
 
     def logon(self, server, nck):
         self.connected.wait()
         self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username or NAME,
+                 'USER %s %s %s :%s' % (self.cfg.username or Cfg.name,
                  server,
                  server,
-                 self.cfg.realname or NAME)
+                 self.cfg.realname or Cfg.name)
                 )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
@@ -539,15 +547,15 @@
         self.connected.clear()
         self.joined.clear()
         launch(Client.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
-               self.cfg.nick or NAME,
+               self.cfg.nick or Cfg.name,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
         Logging.debug("stopping")
```

### Comparing `operbot-170/operbot/modules/log.py` & `operbot-171/operbot/modules/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 'log'
 
 
 import time
 
 
 from ..clocked import elapsed
-from ..persist import find, fntime, write
+from ..persist import Class, find, fntime, write
 from ..objects import Object
 
 
 def __dir__():
     return (
             'Log',
             'log',
@@ -23,14 +23,17 @@
 class Log(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
+Class.add(Log)
+
+
 def log(event):
     if not event.rest:
         nmr = 0
         for obj in find('log'):
             event.reply('%s %s %s' % (
                                       nmr,
                                       obj.txt,
```

### Comparing `operbot-170/operbot/modules/rss.py` & `operbot-171/operbot/modules/rss.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
 from ..clocked import Repeater, elapsed
 from ..handler import Listens, spl
 from ..objects import Object, prt, update
-from ..persist import find, fntime, last, write
+from ..persist import Class, find, fntime, last, write
+from ..runtime import Cfg
 from ..threads import launch, threaded
 
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
@@ -62,21 +63,27 @@
     def __init__(self):
         super().__init__()
         self.display_list = 'title,link,author'
         self.name = ''
         self.rss = ''
 
 
+Class.add(Rss)
+
+
 class Seen(Object):
 
     def __init__(self):
         super().__init__()
         self.urls = []
 
 
+Class.add(Seen)
+
+
 class Fetcher(Object):
 
     dosave = False
     seen = Seen()
 
     def __init__(self):
         super().__init__()
@@ -182,15 +189,15 @@
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
 def getfeed(url, item):
-    if DEBUG:
+    if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
     if not result:
         return [Object(), Object()]
```

### Comparing `operbot-170/operbot/modules/tdo.py` & `operbot-171/operbot/modules/tdo.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 
 import time
 
 
 from ..clocked import elapsed
 from ..objects import Object
-from ..persist import find, fntime, write
+from ..persist import Class, find, fntime, write
 
 
 class Todo(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
+Class.add(Todo)
+
+
 def dne(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
     for obj in find('todo', selector):
         obj.__deleted__ = True
         write(obj)
```

### Comparing `operbot-170/operbot/modules/thr.py` & `operbot-171/operbot/modules/thr.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/modules/usr.py` & `operbot-171/operbot/modules/usr.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 import time
 
 
 from ..clocked import elapsed
 from ..objects import Object, update
-from ..persist import find, fntime, write
+from ..persist import Class, find, fntime, write
 
 
 def __dir__():
     return (
             'NoUser',
             'Users',
             'User',
@@ -81,14 +81,17 @@
         Object.__init__(self)
         self.user = ''
         self.perms = []
         if val:
             update(self, val)
 
 
+Class.add(User)
+
+
 def dlt(event):
     if not event.args:
         event.reply('dlt <username>')
         return
     selector = {'user': event.args[0]}
     for obj in find('user', selector):
         obj.__deleted__ = True
```

### Comparing `operbot-170/operbot/objects.py` & `operbot-171/operbot/objects.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/persist.py` & `operbot-171/operbot/persist.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import json
 import os
 import pathlib
 import time
 import _thread
 
 
-from .objects import Object, ObjectDecoder, ObjectEncoder
+from .objects import Default, Object, ObjectDecoder, ObjectEncoder
 from .objects import kind, search, update
 
 
 def __dir__():
     return (
             'Persist',
             'cdir',
@@ -30,14 +30,43 @@
 
 __all__ = __dir__()
 
 
 disklock = _thread.allocate_lock()
 
 
+class NoClassError(Exception):
+
+    "class is not registered"
+
+
+class Class:
+
+    cls = Default()
+
+    @staticmethod
+    def add(clz):
+        setattr(Class.cls, "%s.%s" % (clz.__module__, clz.__name__), clz)
+
+    @staticmethod
+    def get(cmd):
+        return getattr(Class.cls, cmd, None)
+
+    @staticmethod
+    def match(mtc):
+        mtc = mtc.lower()
+        for clz in Class.cls:
+            if mtc == clz.split(".")[-1].lower():
+                yield clz
+
+    @staticmethod
+    def remove(cmd):
+        del Class.cls[cmd]
+
+
 class Persist(Object):
 
     workdir = ""
 
     @staticmethod
     def logdir():
         return os.path.join(Persist.workdir, "logs")
@@ -55,35 +84,39 @@
     return json.dump(*args, **kw)
 
 
 def files() -> []:
     return os.listdir(os.path.join(Persist.workdir, "store"))
 
 
-def fns(match) -> []:
+def fns(mtc) -> []:
     assert Persist.workdir
     dname = ''
-    lst = match.lower().split(".")[-1]
+    lst = mtc.lower().split(".")[-1]
     for rootdir, dirs, _files in os.walk(Persist.workdir, topdown=False):
         if dirs:
             dname = sorted(dirs)[-1]
             if dname.count('-') == 2:
                 ddd = os.path.join(rootdir, dname)
                 fls = sorted(os.listdir(ddd))
                 if fls:
                     path2 = os.path.join(ddd, fls[-1])
                     spl = strip(path2).split(os.sep)[0]
                     if lst in spl.lower().split(".")[-1]:
                         yield strip(path2)
 
 
 def hook(otp) -> Object:
-    obj = Object()
-    read(obj, otp)
-    return obj
+    clz = fnclass(otp)
+    cls = Class.get(clz)
+    if cls:
+        obj = cls()
+        read(obj, otp)
+        return obj
+    raise NoClassError(clz)
 
 
 def load(fpt, *args, **kw) -> Object:
     return json.load(fpt, *args, cls=ObjectDecoder, **kw)
 
 
 def path(pth) -> str:
@@ -93,14 +126,15 @@
 def read(obj, pth) -> None:
     pth = path(pth)
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
+    return obj.__oid__
 
 
 def setwd(pth) -> None:
     Persist.workdir = pth
 
 
 def strip(pth) -> str:
@@ -117,18 +151,18 @@
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
 
 
-def find(match, selector=None) -> []:
+def find(mtc, selector=None) -> []:
     if selector is None:
         selector = {}
-    for fnm in fns(match):
+    for fnm in fns(mtc):
         obj = hook(fnm)
         if '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
         yield obj
 
@@ -143,14 +177,38 @@
     if result:
         inp = result[-1]
         update(obj, inp)
         obj.__oid__ = inp.__oid__
     return obj.__oid__
 
 
+def match(mtc, selector=None) -> []:
+    if selector is None:
+        selector = {}
+    for tpe in Class.match(mtc):
+        print(tpe)
+        for fnm in fns(tpe):
+            obj = hook(fnm)
+            if '__deleted__' in obj:
+                continue
+            if selector and not search(obj, selector):
+                continue
+            yield obj
+
+
+def fnclass(pth):
+    try:
+        *_rest, mpth = pth.split("store")
+        splitted = mpth.split(os.sep)
+        return splitted[0]
+    except ValueError:
+        pass
+    return None
+
+
 def fntime(daystr):
     daystr = daystr.replace('_', ':')
     datestr = ' '.join(daystr.split(os.sep)[-2:])
     if '.' in datestr:
         datestr, rest = datestr.rsplit('.', 1)
     else:
         rest = ''
```

### Comparing `operbot-170/operbot/scanner.py` & `operbot-171/operbot/scanner.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/threads.py` & `operbot-171/operbot/threads.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot/utility.py` & `operbot-171/operbot/utility.py`

 * *Files identical despite different names*

### Comparing `operbot-170/operbot.egg-info/PKG-INFO` & `operbot-171/operbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 170
+Version: 171
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-170/operbot.egg-info/SOURCES.txt` & `operbot-171/operbot.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 setup.py
 bin/operbot
 bin/operbotcmd
 bin/operbotctl
 bin/operbotd
 files/operbot.service
 operbot/__init__.py
+operbot/__main__.py
 operbot/clocked.py
 operbot/handler.py
 operbot/loggers.py
 operbot/objects.py
 operbot/persist.py
+operbot/runtime.py
 operbot/scanner.py
 operbot/threads.py
 operbot/utility.py
 operbot.egg-info/PKG-INFO
 operbot.egg-info/SOURCES.txt
 operbot.egg-info/dependency_links.txt
 operbot.egg-info/top_level.txt
 operbot/modules/__init__.py
 operbot/modules/cmd.py
 operbot/modules/err.py
 operbot/modules/flt.py
-operbot/modules/fnd.py
 operbot/modules/irc.py
 operbot/modules/log.py
 operbot/modules/rss.py
 operbot/modules/sts.py
 operbot/modules/tdo.py
 operbot/modules/thr.py
 operbot/modules/upt.py
```

### Comparing `operbot-170/setup.py` & `operbot-171/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="operbot",
-    version="170",
+    version="171",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/operbot",
     description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `operbot-170/test/test_decoder.py` & `operbot-171/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `operbot-170/test/test_inherit.py` & `operbot-171/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `operbot-170/test/test_objects.py` & `operbot-171/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `operbot-170/test/test_storage.py` & `operbot-171/test/test_storage.py`

 * *Files identical despite different names*

