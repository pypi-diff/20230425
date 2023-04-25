# Comparing `tmp/pypac-0.8.1-py2.py3-none-any.whl.zip` & `tmp/pypac-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 24800 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      883 b- defN 18-Mar-02 04:05 pypac/__init__.py
--rw-rw-rw-  2.0 fat    14213 b- defN 18-Mar-01 04:59 pypac/api.py
+Zip file size: 26792 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      883 b- defN 18-Jun-03 02:18 pypac/__init__.py
+-rw-rw-rw-  2.0 fat    15141 b- defN 18-Jun-03 02:13 pypac/api.py
+-rw-rw-rw-  2.0 fat     3556 b- defN 18-Jun-03 02:13 pypac/os_settings.py
 -rw-rw-rw-  2.0 fat     5791 b- defN 18-Mar-02 03:57 pypac/parser.py
 -rw-rw-rw-  2.0 fat    12607 b- defN 18-Mar-02 03:57 pypac/parser_functions.py
 -rw-rw-rw-  2.0 fat     5435 b- defN 18-Feb-21 07:04 pypac/resolver.py
 -rw-rw-rw-  2.0 fat     2191 b- defN 18-Feb-28 07:51 pypac/windows.py
 -rw-rw-rw-  2.0 fat     2324 b- defN 17-Apr-04 06:41 pypac/wpad.py
--rw-rw-rw-  2.0 fat     4686 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat    10351 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1372 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        6 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      116 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     5863 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1096 b- defN 18-Mar-02 04:05 pypac-0.8.1.dist-info/RECORD
-14 files, 66934 bytes uncompressed, 23034 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     5066 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat    10351 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1483 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        6 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      116 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     6331 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1174 b- defN 18-Jun-03 02:33 pypac-0.9.0.dist-info/RECORD
+15 files, 72455 bytes uncompressed, 24910 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: pypac/__init__.py
 Comment: 
 
 Filename: pypac/api.py
 Comment: 
 
+Filename: pypac/os_settings.py
+Comment: 
+
 Filename: pypac/parser.py
 Comment: 
 
 Filename: pypac/parser_functions.py
 Comment: 
 
 Filename: pypac/resolver.py
@@ -15,29 +18,29 @@
 
 Filename: pypac/windows.py
 Comment: 
 
 Filename: pypac/wpad.py
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/DESCRIPTION.rst
+Filename: pypac-0.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/LICENSE.txt
+Filename: pypac-0.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/metadata.json
+Filename: pypac-0.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/top_level.txt
+Filename: pypac-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/WHEEL
+Filename: pypac-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/METADATA
+Filename: pypac-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pypac-0.8.1.dist-info/RECORD
+Filename: pypac-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pypac/__init__.py

```diff
@@ -16,13 +16,13 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from pypac.api import get_pac, collect_pac_urls, download_pac, PACSession, pac_context_for_url
 
 
-__version__ = '0.8.1'
+__version__ = '0.9.0'
 
 
 __all__ = [
     'get_pac', 'collect_pac_urls', 'download_pac', 'PACSession', 'pac_context_for_url'
 ]
```

## pypac/api.py

```diff
@@ -5,28 +5,29 @@
 from contextlib import contextmanager
 
 import requests
 from requests.exceptions import ProxyError, ConnectTimeout
 
 from pypac.parser import PACFile, ARBITRARY_HIGH_RECURSION_LIMIT
 from pypac.resolver import ProxyResolver, ProxyConfigExhaustedError
-from pypac.windows import autoconfig_url_from_registry, ON_WINDOWS, file_url_to_local_path
+from pypac.os_settings import autoconfig_url_from_registry, autoconfig_url_from_preferences, \
+    ON_WINDOWS, ON_DARWIN, file_url_to_local_path
 from pypac.wpad import proxy_urls_from_dns
 
 
-def get_pac(url=None, js=None, from_registry=True, from_dns=True, timeout=2, allowed_content_types=None, **kwargs):
+def get_pac(url=None, js=None, from_os_settings=True, from_dns=True, timeout=2, allowed_content_types=None, **kwargs):
     """
     Convenience function for finding and getting a parsed PAC file (if any) that's ready to use.
 
     :param str url: Download PAC from a URL.
-        If provided, `from_registry` and `from_dns` are ignored.
+        If provided, `from_os_settings` and `from_dns` are ignored.
     :param str js: Parse the given string as a PAC file.
-        If provided, `from_registry` and `from_dns` are ignored.
-    :param bool from_registry: Look for a PAC URL or filesystem path from the Windows Registry, and use it if present.
-        Doesn't do anything on non-Windows platforms.
+        If provided, `from_os_settings` and `from_dns` are ignored.
+    :param bool from_os_settings: Look for a PAC URL or filesystem path from the OS settings, and use it if present.
+        Doesn't do anything on non-Windows or non-macOS/OSX platforms.
     :param bool from_dns: Look for a PAC file using the WPAD protocol.
     :param timeout: Time to wait for host resolution and response for each URL.
     :param allowed_content_types: If the response has a ``Content-Type`` header,
         then consider the response to be a PAC file only if the header is one of these values.
         If not specified, the allowed types are
         ``application/x-ns-proxy-autoconfig`` and ``application/x-javascript-config``.
     :return: The first valid parsed PAC file according to the criteria, or `None` if nothing was found.
@@ -37,44 +38,70 @@
         downloaded_pac = download_pac([url], timeout=timeout, allowed_content_types=allowed_content_types)
         if not downloaded_pac:
             return
         return PACFile(downloaded_pac, **kwargs)
     if js:
         return PACFile(js, **kwargs)
 
-    if from_registry and ON_WINDOWS:
-        path = autoconfig_url_from_registry()
+    # Deprecated in 0.8.2
+    from_registry = kwargs.get('from_registry')
+    if from_registry is not None:
+        import warnings
+        warnings.warn('from_registry is deprecated, use from_os_settings instead.')
+        from_os_settings = from_registry
+
+    if from_os_settings:
+        if ON_WINDOWS:
+            path = autoconfig_url_from_registry()
+        elif ON_DARWIN:
+            path = autoconfig_url_from_preferences()
+        else:
+            path = None
+
         if path and path.lower().startswith('file://'):
             path = file_url_to_local_path(path)
 
         if path and os.path.isfile(path):
             with open(path) as f:
                 return PACFile(f.read(), **kwargs)
 
-    pac_candidate_urls = collect_pac_urls(from_registry=True, from_dns=from_dns)
+    pac_candidate_urls = collect_pac_urls(from_os_settings=True, from_dns=from_dns)
     downloaded_pac = download_pac(pac_candidate_urls, timeout=timeout, allowed_content_types=allowed_content_types)
     if not downloaded_pac:
         return
     return PACFile(downloaded_pac, **kwargs)
 
 
-def collect_pac_urls(from_registry=True, from_dns=True):
+def collect_pac_urls(from_os_settings=True, from_dns=True, **kwargs):
     """
     Get all the URLs that potentially yield a PAC file.
 
-    :param bool from_registry: Look for a PAC URL from the Windows Registry.
+    :param bool from_os_settings: Look for a PAC URL from the OS settings.
         If a value is found and is a URL, it comes first in the returned list.
-        Doesn't do anything on non-Windows platforms.
+        Doesn't do anything on non-Windows or non-macOS/OSX platforms.
     :param bool from_dns: Assemble a list of PAC URL candidates using the WPAD protocol.
     :return: A list of URLs that should be tried in order.
     :rtype: list[str]
     """
+    # Deprecated in 0.8.2
+    from_registry = kwargs.get('from_registry')
+    if from_registry is not None:
+        import warnings
+        warnings.warn('from_registry is deprecated, use from_os_settings instead.')
+        from_os_settings = from_registry
+
     pac_urls = []
-    if from_registry and ON_WINDOWS:
-        url_or_path = autoconfig_url_from_registry()
+    if from_os_settings:
+        if ON_WINDOWS:
+            url_or_path = autoconfig_url_from_registry()
+        elif ON_DARWIN:
+            url_or_path = autoconfig_url_from_preferences()
+        else:
+            url_or_path = None
+
         if url_or_path and (url_or_path.lower().startswith('http://') or url_or_path.lower().startswith('https://')):
             pac_urls.append(url_or_path)
     if from_dns:
         pac_urls.extend(proxy_urls_from_dns())
     return pac_urls
```

## Comparing `pypac-0.8.1.dist-info/DESCRIPTION.rst` & `pypac-0.9.0.dist-info/DESCRIPTION.rst`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     >>> session.get('http://example.org')
     ...
 
 If a PAC file isn't found, then ``PACSession`` acts exactly like a regular ``Session``.
 
 PyPAC can find PAC files according to the DNS portion of the `Web Proxy Auto-Discovery (WPAD)`_ protocol.
 On Windows, PyPAC can also obtain the PAC file URL from the Internet Options dialog, via the registry.
+On macOS, PyPAC can obtain the PAC file URL from System Preferences.
 
 .. _Web Proxy Auto-Discovery (WPAD): https://en.wikipedia.org/wiki/Web_Proxy_Autodiscovery_Protocol
 
 If you're looking to add *basic* PAC functionality to a library that you're using,
 try the ``pac_context_for_url()`` context manager:
 
 .. code-block:: python
@@ -54,15 +55,15 @@
 that honours proxy environment variables.
 
 
 Features
 --------
 
 * The same Requests API that you already know and love
-* Honour PAC setting from Windows Internet Options
+* Honour PAC setting from Windows Internet Options and macOS System Preferences
 * Follow DNS Web Proxy Auto-Discovery protocol
 * Proxy authentication pass-through
 * Proxy failover and load balancing
 * Generic components for adding PAC support to other code
 
 PyPAC supports Python 2.7 and 3.4+.
 
@@ -77,14 +78,22 @@
 
 Documentation
 -------------
 
 PyPAC's documentation is available at http://pypac.readthedocs.io/.
 
 
+0.9.0 (2018-06-02)
+------------------
+
+- Add macOS support for PAC in System Preferences (#23). Thanks @LKleinNux.
+- The `from_registry` argument on `pypac.get_pac()` and `pypac.collect_pac_urls()`
+  is now deprecated and will be removed in 1.0.0. Use `from_os_settings` instead.
+
+
 0.8.1 (2018-03-01)
 ------------------
 
 - Defer Js2Py import until it's needed. It uses a lot of memory.
   See #20 for details.
```

## Comparing `pypac-0.8.1.dist-info/LICENSE.txt` & `pypac-0.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pypac-0.8.1.dist-info/metadata.json` & `pypac-0.9.0.dist-info/metadata.json`

 * *Files 8% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'run_requires'": '{insert: [(2, OrderedDict([(\'environment\', \'sys_platform == "darwin"\'), '*

 * *                   "('requires', ['pyobjc-framework-SystemConfiguration (>=3.2.1)'])]))]}",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -57,20 +57,26 @@
             ]
         },
         {
             "extra": "socks",
             "requires": [
                 "requests[socks] (>=2.10.0)"
             ]
+        },
+        {
+            "environment": "sys_platform == \"darwin\"",
+            "requires": [
+                "pyobjc-framework-SystemConfiguration (>=3.2.1)"
+            ]
         }
     ],
     "summary": "Proxy auto-config and auto-discovery for Python.",
     "test_requires": [
         {
             "requires": [
                 "mock",
                 "pytest"
             ]
         }
     ],
-    "version": "0.8.1"
+    "version": "0.9.0"
 }
```

## Comparing `pypac-0.8.1.dist-info/METADATA` & `pypac-0.9.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: pypac
-Version: 0.8.1
+Version: 0.9.0
 Summary: Proxy auto-config and auto-discovery for Python.
 Home-page: https://github.com/carsonyl/pypac
 Author: Carson Lam
 Author-email: carsonyylam@gmail.com
 License: Apache 2.0
 Description-Content-Type: UNKNOWN
 Keywords: pypac pac proxy autoconfig requests
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
 Requires-Dist: requests (<3.0.0,>=2.0.0)
 Requires-Dist: tld (<1.0.0,>=0.7.3)
 Requires-Dist: js2py (>=0.43)
+Requires-Dist: pyobjc-framework-SystemConfiguration (>=3.2.1); sys_platform == "darwin"
 Provides-Extra: socks
 Requires-Dist: requests[socks] (>=2.10.0); extra == 'socks'
 
 PyPAC: Proxy auto-config for Python
 ===================================
 
 .. image:: https://img.shields.io/pypi/v/pypac.svg?maxAge=2592000
@@ -61,14 +62,15 @@
     >>> session.get('http://example.org')
     ...
 
 If a PAC file isn't found, then ``PACSession`` acts exactly like a regular ``Session``.
 
 PyPAC can find PAC files according to the DNS portion of the `Web Proxy Auto-Discovery (WPAD)`_ protocol.
 On Windows, PyPAC can also obtain the PAC file URL from the Internet Options dialog, via the registry.
+On macOS, PyPAC can obtain the PAC file URL from System Preferences.
 
 .. _Web Proxy Auto-Discovery (WPAD): https://en.wikipedia.org/wiki/Web_Proxy_Autodiscovery_Protocol
 
 If you're looking to add *basic* PAC functionality to a library that you're using,
 try the ``pac_context_for_url()`` context manager:
 
 .. code-block:: python
@@ -85,15 +87,15 @@
 that honours proxy environment variables.
 
 
 Features
 --------
 
 * The same Requests API that you already know and love
-* Honour PAC setting from Windows Internet Options
+* Honour PAC setting from Windows Internet Options and macOS System Preferences
 * Follow DNS Web Proxy Auto-Discovery protocol
 * Proxy authentication pass-through
 * Proxy failover and load balancing
 * Generic components for adding PAC support to other code
 
 PyPAC supports Python 2.7 and 3.4+.
 
@@ -108,14 +110,22 @@
 
 Documentation
 -------------
 
 PyPAC's documentation is available at http://pypac.readthedocs.io/.
 
 
+0.9.0 (2018-06-02)
+------------------
+
+- Add macOS support for PAC in System Preferences (#23). Thanks @LKleinNux.
+- The `from_registry` argument on `pypac.get_pac()` and `pypac.collect_pac_urls()`
+  is now deprecated and will be removed in 1.0.0. Use `from_os_settings` instead.
+
+
 0.8.1 (2018-03-01)
 ------------------
 
 - Defer Js2Py import until it's needed. It uses a lot of memory.
   See #20 for details.
```

