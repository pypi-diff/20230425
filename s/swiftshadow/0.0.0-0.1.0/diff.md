# Comparing `tmp/swiftshadow-0.0.0.tar.gz` & `tmp/swiftshadow-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.0.0.tar", last modified: Fri Apr 14 10:23:44 2023, max compression
+gzip compressed data, was "swiftshadow-0.1.0.tar", last modified: Tue Apr 25 07:08:06 2023, max compression
```

## Comparing `swiftshadow-0.0.0.tar` & `swiftshadow-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:23:44.023027 swiftshadow-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 10:23:32.000000 swiftshadow-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 10:23:44.023027 swiftshadow-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 10:23:32.000000 swiftshadow-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:23:44.023027 swiftshadow-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-14 10:23:32.000000 swiftshadow-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:23:44.023027 swiftshadow-0.0.0/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:23:32.000000 swiftshadow-0.0.0/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-14 10:23:32.000000 swiftshadow-0.0.0/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:23:44.023027 swiftshadow-0.0.0/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 10:23:44.000000 swiftshadow-0.0.0/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 10:23:44.000000 swiftshadow-0.0.0/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:23:44.000000 swiftshadow-0.0.0/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 10:23:44.000000 swiftshadow-0.0.0/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 10:23:44.000000 swiftshadow-0.0.0/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.0.0/LICENSE` & `swiftshadow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.0.0/setup.py` & `swiftshadow-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Install packages as defined in this file into the Python environment."""
 
 from setuptools import setup, find_packages
 
 # The version of this tool is based on the following steps:
 
 # https://packaging.python.org/guides/single-sourcing-package-version/
+from pathlib import Path
 
+this_directory = Path(__file__).parent
+
+long_description = (this_directory / "README.md").read_text()
 VERSION = {}
 
 with open("./swiftshadow/__init__.py") as fp:
     # pylint: disable=W0122
 
     exec(fp.read(), VERSION)
 
 setup(
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
-    url="https://github.com/Chicken1Geek/swiftshadow",
+    url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
-    long_description="Swiftshadow is a proxy rotator that sources proxies for free and provides elegant pythonic API to manage proxies. Build for speed and performance in mind.",
-    version=VERSION.get("__version__", "0.0.0"),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    version=VERSION.get("__version__", "0.1.0"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.0.0/swiftshadow/swiftshadow.py` & `swiftshadow-0.1.0/swiftshadow/swiftshadow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,137 @@
 from requests import get
 from random import choice
 from datetime import datetime, timezone, timedelta
 from pickle import dump, load
+from helpers import log
+from providers import Proxyscrape, Scrapingant
 
 
 class Proxy:
-    def __init__(self, country=None, protocol="http", maxProxies=10, autoRotate=False):
-        self.country = country
+    def __init__(
+        self,
+        countries: list = [],
+        protocol: str = "http",
+        maxProxies: int = 10,
+        autoRotate: bool = False,
+        cachePeriod: int = 10,
+    ):
+        """
+        The one class for everything.
+
+        Proxy class contains all necessary methods required to use swiftshadow.
+
+        Args:
+                countries: ISO 3166-2 Two letter country codes to filter proxies.
+                protocol: HTTP/HTTPS protocol to filter proxies.
+                maxProxies: Maximum number of proxies to store and rotate from.
+                autoRotate: Rotates proxy when `Proxy.proxy()` function is called.
+                cachePeriod: Time to cache proxies in minutes.
+
+        Returns:
+                proxyClass (swiftshadow.Proxy): `swiftshadow.Proxy` class instance
+
+        Examples:
+                Simplest way to get a proxy
+                >>> from swiftshadow import Proxy
+                >>> swift = Proxy()
+                >>> print(swift.proxy())
+                {'http':'192.0.0.1:8080'}
+        Note:
+                Proxies are sourced from **Proxyscrape** and **Scrapingant** websites which are freely available and validated locally.
+        """
+        self.countries = [i.upper() for i in countries]
         self.protocol = protocol
         self.maxProxies = maxProxies
         self.autoRotate = autoRotate
-        self.update()
+        self.cachePeriod = cachePeriod
+        self.updateProxyList()
 
     def checkIp(self, ip, cc, protocol):
         if (ip[1] == cc or cc == None) and ip[2] == protocol:
             proxy = {ip[2]: ip[0]}
             try:
-                oip = get(f"{protocol}://ipinfo.io/ip", proxies=proxy, timeout=5).text
+                oip = get(f"{protocol}://ipinfo.io/ip", proxies=proxy).text
             except:
                 return False
             if oip.count(".") == 3 and oip != self.mip:
                 return True
             else:
                 return False
         else:
             return False
 
-    def checkCache(self, latestTimeString, cache=datetime.now(timezone.utc)):
-        latest = datetime.strptime(latestTimeString + " UTC", "%Y-%m-%d %H:%M:%S %Z")
-        latest = latest.replace(tzinfo=timezone.utc)
-        expiry = latest + timedelta(minutes=10)
+    def checkCache(self, latest, cache=datetime.now(timezone.utc)):
+        expiry = latest + timedelta(minutes=self.cachePeriod)
         live = cache - latest
         dead = expiry - cache
-        if live.seconds / 60 < 10.0 and dead.seconds / 60 < 10.0:
+        limit = float(self.cachePeriod)
+        if live.seconds / 60 < limit and dead.seconds / 60 < limit:
             cacheValid = True
         else:
             cacheValid = False
         return cacheValid
 
-    def update(self):
-        raw = get("https://free-proxy-list.net/").text
+    def updateProxyList(self):
         try:
             with open(".swiftshadow.dat", "rb") as file:
                 data = load(file)
-                cacheState = self.checkCache(
-                    raw.split("UTC")[0].split("Updated at")[-1].strip(), data[0]
-                )
+                self.latest = data[0]
+                cacheState = self.checkCache(self.latest)
             if cacheState:
-                print("[ swiftshadow ] Loaded proxies from cache")
+                log(
+                    "info",
+                    f"{datetime.now(timezone.utc).time()} Loaded proxies from cache",
+                )
                 self.proxies = data[1]
                 self.current = self.proxies[0]
                 return
             else:
-                print("[ swiftshadow ] Cache expired. Updating cache...")
+                log(
+                    "info",
+                    f"{datetime.now(timezone.utc).time()} Cache expired. Updating cache...",
+                )
         except FileNotFoundError:
-            print("[ swiftshadow ] No cache found. Creating cache... ")
-        self.mip = get("https://ipinfo.io/ip").text
-        raw = [
-            i.split("<td>")
-            for i in raw.split("<tbody>")[1].split("</tbody>")[0].split("</tr><tr>")
-        ]
-        raw = [
-            [
-                i[1].rstrip("</td>"),
-                i[2].rstrip("</td>"),
-                i[3].split("<", 1)[0],
-                i[-1].split("hx", 1)[1][2],
-            ]
-            for i in raw
-        ]
-        final = [
-            [i[0] + ":" + i[1], i[2], "https" if i[3] == "y" else "http"] for i in raw
-        ]
+            log("error", "No cache found. Cache will be created after update")
+
         self.proxies = []
-        for i in final:
-            if self.checkIp(i, self.country, self.protocol):
-                if len(self.proxies) == self.maxProxies:
-                    break
-                self.proxies.append({i[2]: i[0]})
+        self.proxies.extend(Proxyscrape(self.maxProxies, self.countries, self.protocol))
+        if len(self.proxies) != self.maxProxies:
+            self.proxies.extend(
+                Scrapingant(self.maxProxies, self.countries, self.protocol)
+            )
         if len(self.proxies) == 0:
-            print(
-                "[ swiftshadow ] No proxies found for current settings. To prevent runtime error updating the proxy list again."
+            log(
+                "warn",
+                "No proxies found for current settings. To prevent runtime error updating the proxy list again.",
             )
             self.update()
         with open(".swiftshadow.dat", "wb") as file:
             dump([datetime.now(timezone.utc), self.proxies], file)
-
         self.current = self.proxies[0]
 
     def rotate(self):
+        """
+        Rotate the current proxy.
+
+        Sets the current proxy to a random one from available proxies and also validates cache.
+
+        Note:
+                Function only for manual rotation. If `autoRotate` is set to `True` then no need to call this function.
+        """
+        if not self.checkCache(self.latest):
+            self.update()
         self.current = choice(self.proxies)
 
     def proxy(self):
+        """
+        Returns a proxy dict.
+
+        Returns:
+                proxyDict (dict):A proxy dict of format `{protocol:address}`
+        """
+        if not self.checkCache(self.latest):
+            self.update()
         if self.autoRotate == True:
             return choice(self.proxies)
         else:
             return self.current
-
-
-# a = Proxy(country='IN')
-# print(a.proxies)
```

