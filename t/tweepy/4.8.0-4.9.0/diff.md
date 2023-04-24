# Comparing `tmp/tweepy-4.8.0.tar.gz` & `tmp/tweepy-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweepy-4.8.0.tar", last modified: Thu Mar 24 21:08:19 2022, max compression
+gzip compressed data, was "tweepy-4.9.0.tar", last modified: Thu May  5 14:24:50 2022, max compression
```

## Comparing `tweepy-4.8.0.tar` & `tweepy-4.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 21:08:19.946248 tweepy-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-03-24 21:08:08.000000 tweepy-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-24 21:08:08.000000 tweepy-4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-03-24 21:08:19.946248 tweepy-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-03-24 21:08:08.000000 tweepy-4.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-03-24 21:08:08.000000 tweepy-4.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-24 21:08:19.946248 tweepy-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-03-24 21:08:08.000000 tweepy-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 21:08:19.942248 tweepy-4.8.0/tweepy/
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   137623 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 21:08:19.946248 tweepy-4.8.0/tweepy/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17061 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/asynchronous/streaming.py
--rw-r--r--   0 runner    (1001) docker     (121)     7710 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    12778 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)   133736 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/media.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    13778 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/place.py
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/poll.py
--rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/space.py
--rw-r--r--   0 runner    (1001) docker     (121)    35574 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/streaming.py
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/tweet.py
--rw-r--r--   0 runner    (1001) docker     (121)     4564 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/user.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-03-24 21:08:08.000000 tweepy-4.8.0/tweepy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 21:08:19.946248 tweepy-4.8.0/tweepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-03-24 21:08:19.000000 tweepy-4.8.0/tweepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-03-24 21:08:19.000000 tweepy-4.8.0/tweepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 21:08:19.000000 tweepy-4.8.0/tweepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-03-24 21:08:19.000000 tweepy-4.8.0/tweepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-24 21:08:19.000000 tweepy-4.8.0/tweepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 21:08:19.000000 tweepy-4.8.0/tweepy.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:24:50.325308 tweepy-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-05-05 14:24:43.000000 tweepy-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-05 14:24:43.000000 tweepy-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-05-05 14:24:50.325308 tweepy-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-05-05 14:24:43.000000 tweepy-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-05 14:24:43.000000 tweepy-4.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-05-05 14:24:50.325308 tweepy-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-05-05 14:24:43.000000 tweepy-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:24:50.325308 tweepy-4.9.0/tweepy/
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   139632 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:24:50.325308 tweepy-4.9.0/tweepy/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17061 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/asynchronous/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7710 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12778 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)   133736 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/media.py
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13778 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/place.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/poll.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5381 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/space.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36912 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/tweet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4564 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-05-05 14:24:43.000000 tweepy-4.9.0/tweepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:24:50.325308 tweepy-4.9.0/tweepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-05-05 14:24:50.000000 tweepy-4.9.0/tweepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-05-05 14:24:50.000000 tweepy-4.9.0/tweepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 14:24:50.000000 tweepy-4.9.0/tweepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-05-05 14:24:50.000000 tweepy-4.9.0/tweepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-05 14:24:50.000000 tweepy-4.9.0/tweepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 14:24:50.000000 tweepy-4.9.0/tweepy.egg-info/zip-safe
```

### Comparing `tweepy-4.8.0/LICENSE` & `tweepy-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/PKG-INFO` & `tweepy-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweepy
-Version: 4.8.0
+Version: 4.9.0
 Summary: Twitter library for Python
 Home-page: https://www.tweepy.org/
 Author: Joshua Roesslein
 Author-email: tweepy@googlegroups.com
 License: MIT
 Download-URL: https://pypi.org/project/tweepy/
 Project-URL: Documentation, https://tweepy.readthedocs.io
```

### Comparing `tweepy-4.8.0/README.md` & `tweepy-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/setup.py` & `tweepy-4.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,14 @@
     version = match.group(1)
 else:
     raise RuntimeError(f"Unable to find version string in {VERSION_FILE}.")
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
-tests_require = [
-    "vcrpy>=1.10.3",
-]
-
 setup(
     name="tweepy",
     version=version,
     description="Twitter library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
@@ -38,23 +34,23 @@
     download_url="https://pypi.org/project/tweepy/",
     packages=find_packages(),
     install_requires=[
         "oauthlib>=3.2.0,<4",
         "requests>=2.27.0,<3",
         "requests-oauthlib>=1.2.0,<2",
     ],
-    tests_require=tests_require,
     extras_require={
         "async": ["aiohttp>=3.7.3,<4"],
         "dev": [
+            "coverage>=4.4.2",
             "coveralls>=2.1.0",
-            "tox>=3.14.0",
+            "tox>=3.21.0",
          ],
         "socks": ["requests[socks]>=2.27.0,<3"],
-        "test": tests_require,
+        "test": ["vcrpy>=1.10.3"],
     },
     test_suite="tests",
     keywords="twitter library",
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Software Development :: Libraries",
```

### Comparing `tweepy-4.8.0/tweepy/__init__.py` & `tweepy-4.9.0/tweepy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Tweepy
 # Copyright 2009-2022 Joshua Roesslein
 # See LICENSE for details.
 
 """
 Tweepy Twitter API library
 """
-__version__ = '4.8.0'
+__version__ = '4.9.0'
 __author__ = 'Joshua Roesslein'
 __license__ = 'MIT'
 
 from tweepy.api import API
 from tweepy.auth import (
     AppAuthHandler, OAuthHandler, OAuth1UserHandler, OAuth2AppHandler,
     OAuth2BearerHandler, OAuth2UserHandler
```

### Comparing `tweepy-4.8.0/tweepy/api.py` & `tweepy-4.9.0/tweepy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3391,14 +3391,68 @@
         if ctas is not None:
             message_data['ctas'] = ctas
         return self.request(
             'POST', 'direct_messages/events/new',
             json_payload=json_payload, **kwargs
         )
 
+    # Typing indicator and read receipts
+
+    def indicate_direct_message_typing(self, recipient_id, **kwargs):
+        """indicate_direct_message_typing(recipient_id)
+
+        Displays a visual typing indicator in the recipient’s Direct Message
+        conversation view with the sender. Each request triggers a typing
+        indicator animation with a duration of ~3 seconds.
+
+        .. versionadded:: 4.9
+
+        Parameters
+        ----------
+        recipient_id
+            The user ID of the user to receive the typing indicator.
+
+        References
+        ----------
+        https://developer.twitter.com/en/docs/twitter-api/v1/direct-messages/typing-indicator-and-read-receipts/api-reference/new-typing-indicator
+        """
+        return self.request(
+            'POST', 'direct_messages/indicate_typing', endpoint_parameters=(
+                'recipient_id'
+            ), recipient_id=recipient_id, **kwargs
+        )
+
+    def mark_direct_message_read(self, last_read_event_id, recipient_id,
+                                 **kwargs):
+        """mark_direct_message_read(last_read_event_id, recipient_id)
+
+        Marks a message as read in the recipient’s Direct Message conversation
+        view with the sender.
+
+        .. versionadded:: 4.9
+
+        Parameters
+        ----------
+        last_read_event_id
+            The message ID of the most recent message to be marked read. All
+            messages before it will be marked read as well.
+        recipient_id
+            The user ID of the user the message is from.
+
+        References
+        ----------
+        https://developer.twitter.com/en/docs/twitter-api/v1/direct-messages/typing-indicator-and-read-receipts/api-reference/new-read-receipt
+        """
+        return self.request(
+            'POST', 'direct_messages/mark_read', endpoint_parameters=(
+                'last_read_event_id', 'recipient_id'
+            ), last_read_event_id=last_read_event_id,
+            recipient_id=recipient_id, **kwargs
+        )
+
     # Upload media
 
     @payload('media')
     def get_media_upload_status(self, media_id, **kwargs):
         """get_media_upload_status(media_id)
 
         Check on the progress of a chunked media upload. If the upload has
```

### Comparing `tweepy-4.8.0/tweepy/asynchronous/streaming.py` & `tweepy-4.9.0/tweepy/asynchronous/streaming.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/auth.py` & `tweepy-4.9.0/tweepy/auth.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/cache.py` & `tweepy-4.9.0/tweepy/cache.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/client.py` & `tweepy-4.9.0/tweepy/client.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/cursor.py` & `tweepy-4.9.0/tweepy/cursor.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/errors.py` & `tweepy-4.9.0/tweepy/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,28 +41,44 @@
 
         try:
             response_json = response.json()
         except requests.JSONDecodeError:
             super().__init__(f"{response.status_code} {response.reason}")
         else:
             errors = response_json.get("errors", [])
+
             # Use := when support for Python 3.7 is dropped
             if "error" in response_json:
                 errors.append(response_json["error"])
+
             error_text = ""
+
             for error in errors:
                 self.api_errors.append(error)
+
+                if isinstance(error, str):
+                    self.api_messages.append(error)
+                    error_text += '\n' + error
+                    continue
+
                 if "code" in error:
                     self.api_codes.append(error["code"])
                 if "message" in error:
                     self.api_messages.append(error["message"])
+
                 if "code" in error and "message" in error:
                     error_text += f"\n{error['code']} - {error['message']}"
                 elif "message" in error:
                     error_text += '\n' + error["message"]
+
+            # Use := when support for Python 3.7 is dropped
+            if not error_text and "detail" in response_json:
+                self.api_messages.append(response_json["detail"])
+                error_text = '\n' + response_json["detail"]
+
             super().__init__(
                 f"{response.status_code} {response.reason}{error_text}"
             )
 
 
 class BadRequest(HTTPException):
     """BadRequest()
```

### Comparing `tweepy-4.8.0/tweepy/list.py` & `tweepy-4.9.0/tweepy/list.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/media.py` & `tweepy-4.9.0/tweepy/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     ----------
     data : dict
         The JSON data representing the media.
     media_key : str
         Unique identifier of the expanded media content.
     type : str
         Type of content (animated_gif, photo, video).
+    url : str | None
+        A direct URL to the media file on Twitter.
     duration_ms : int | None
         Available when type is video. Duration in milliseconds of the video.
     height : int | None
         Height of this content in pixels.
     non_public_metrics : dict | None
         Non-public engagement metrics for the media content at the time of the
         request. 
@@ -53,46 +55,43 @@
         Public engagement metrics for the media content at the time of the
         request.
     width : int | None
         Width of this content in pixels.
     alt_text : str | None
         A description of an image to enable and support accessibility. Can be
         up to 1000 characters long. Alt text can only be added to images at the
-        moment. 
-    url : str | None
+        moment.
 
     References
     ----------
     https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/media
     """
 
     __slots__ = (
-        "data", "media_key", "type", "duration_ms", "height",
+        "data", "media_key", "url", "type", "duration_ms", "height",
         "non_public_metrics", "organic_metrics", "preview_image_url",
-        "promoted_metrics", "public_metrics", "width", "alt_text", "url"
+        "promoted_metrics", "public_metrics", "width", "alt_text",
     )
 
     def __init__(self, data):
         self.data = data
         self.media_key = data["media_key"]
         self.type = data["type"]
 
+        self.url = data.get("url")
         self.duration_ms = data.get("duration_ms")
         self.height = data.get("height")
         self.non_public_metrics = data.get("non_public_metrics")
         self.organic_metrics = data.get("organic_metrics")
         self.preview_image_url = data.get("preview_image_url")
         self.promoted_metrics = data.get("promoted_metrics")
         self.public_metrics = data.get("public_metrics")
         self.width = data.get("width")
         self.alt_text = data.get("alt_text")
 
-        # https://twittercommunity.com/t/documentation-for-media-object-missing-url-field/163062
-        self.url = data.get("url")
-
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.media_key == other.media_key
 
         return NotImplemented
 
     def __hash__(self):
```

### Comparing `tweepy-4.8.0/tweepy/mixins.py` & `tweepy-4.9.0/tweepy/mixins.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/models.py` & `tweepy-4.9.0/tweepy/models.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/pagination.py` & `tweepy-4.9.0/tweepy/pagination.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/parsers.py` & `tweepy-4.9.0/tweepy/parsers.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/place.py` & `tweepy-4.9.0/tweepy/place.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/poll.py` & `tweepy-4.9.0/tweepy/poll.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/space.py` & `tweepy-4.9.0/tweepy/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,27 @@
     is_ticketed : bool | None
         Indicates is this is a ticketed Space.
     invited_user_ids : list
         The list of user IDs that were invited to join as speakers. Usually,
         users in this list are invited to speak via the Invite user option.
     participant_count : int | None
         The current number of users in the Space, including Hosts and Speakers.
+    subscriber_count : int | None
+        The number of people who set a reminder to a Space.
     scheduled_start : datetime.datetime | None
         Indicates the start time of a scheduled Space, as set by the creator of
         the Space. This field is returned only if the Space has been scheduled;
         in other words, if the field is returned, it means the Space is a
         scheduled Space.
     speaker_ids : list
         The list of users who were speaking at any point during the Space. This
         list contains all the users in ``invited_user_ids`` in addition to any
         user who requested to speak and was allowed via the Add speaker option.
     started_at : datetime.datetime | None
         Indicates the actual start time of a Space.
-    subscriber_count : int | None
     title : str | None
         The title of the Space as specified by the creator.
     topic_ids : list
         A list of IDs of the topics selected by the creator of the Space.
     updated_at : datetime.datetime | None
         Specifies the date and time of the last update to any of the Space's
         metadata, such as its title or scheduled time.
@@ -82,15 +83,15 @@
 
     .. _Spaces lookup endpoints: https://developer.twitter.com/en/docs/twitter-api/spaces/lookup/introduction
     """
 
     __slots__ = (
         "data", "id", "state", "created_at", "ended_at", "host_ids", "lang",
         "is_ticketed", "invited_user_ids", "participant_count",
-        "scheduled_start", "speaker_ids", "started_at", "subscriber_count",
+        "subscriber_count", "scheduled_start", "speaker_ids", "started_at",
         "title", "topic_ids", "updated_at"
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data["id"]
         self.state = data["state"]
@@ -104,28 +105,26 @@
             self.ended_at = parse_datetime(self.ended_at)
 
         self.host_ids = data.get("host_ids", [])
         self.lang = data.get("lang")
         self.is_ticketed = data.get("is_ticketed")
         self.invited_user_ids = data.get("invited_user_ids", [])
         self.participant_count = data.get("participant_count")
+        self.subscriber_count = data.get("subscriber_count")
 
         self.scheduled_start = data.get("scheduled_start")
         if self.scheduled_start is not None:
             self.scheduled_start = parse_datetime(self.scheduled_start)
 
         self.speaker_ids = data.get("speaker_ids", [])
 
         self.started_at = data.get("started_at")
         if self.started_at is not None:
             self.started_at = parse_datetime(self.started_at)
 
-        # https://twittercommunity.com/t/missing-documentation-for-new-space-object-subscriber-count-field-on-space-object-page/166943
-        self.subscriber_count = data.get("subscriber_count")
-
         self.title = data.get("title")
 
         self.topic_ids = data.get("topic_ids", [])
 
         self.updated_at = data.get("updated_at")
         if self.updated_at is not None:
             self.updated_at = parse_datetime(self.updated_at)
```

### Comparing `tweepy-4.8.0/tweepy/streaming.py` & `tweepy-4.9.0/tweepy/streaming.py`

 * *Files 3% similar despite different names*

```diff
@@ -261,14 +261,21 @@
         super()._connect(method, url, auth=auth, **kwargs)
 
     def filter(self, *, follow=None, track=None, locations=None,
                filter_level=None, languages=None, stall_warnings=False,
                threaded=False):
         """Filter realtime Tweets
 
+        .. deprecated:: 4.9
+            `The delivery of compliance messages through the Twitter API v1.1
+            endpoint this method uses has been deprecated, and they will stop
+            being delivered beginning October 29, 2022.`_ Twitter API v2 can be
+            used instead with :meth:`StreamingClient.filter` and/or
+            :class:`Client` :ref:`batch compliance <Batch compliance>` methods.
+
         Parameters
         ----------
         follow : list[int | str] | None
             User IDs, indicating the users to return statuses for in the stream
         track : list[str] | None
             Keywords to track
         locations : list[float] | None
@@ -306,14 +313,17 @@
 
         References
         ----------
         https://developer.twitter.com/en/docs/twitter-api/v1/tweets/filter-realtime/api-reference/post-statuses-filter
 
         .. _BCP 47: https://tools.ietf.org/html/bcp47
         .. _advanced search: https://twitter.com/search-advanced
+        .. _The delivery of compliance messages through the Twitter API v1.1
+            endpoint this method uses has been deprecated, and they will stop
+            being delivered beginning October 29, 2022.: https://twittercommunity.com/t/deprecation-announcement-removing-compliance-messages-from-statuses-filter-and-retiring-statuses-sample-from-the-twitter-api-v1-1/170500
         """
         if self.running:
             raise TweepyException("Stream is already connected")
 
         method = "POST"
         endpoint = "statuses/filter"
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
@@ -341,14 +351,19 @@
                                           body=body)
         else:
             self._connect(method, endpoint, headers=headers, body=body)
 
     def sample(self, *, languages=None, stall_warnings=False, threaded=False):
         """Sample realtime Tweets
 
+        .. deprecated:: 4.9
+            `The Twitter API v1.1 endpoint this method uses is now deprecated
+            and will be retired on October 29, 2022.`_ Twitter API v2 can be
+            used instead with :meth:`StreamingClient.sample`.
+
         Parameters
         ----------
         languages : list[str] | None
             Setting this parameter to a comma-separated list of `BCP 47`_
             language identifiers corresponding to any of the languages listed
             on Twitter’s `advanced search`_ page will only return Tweets that
             have been detected as being written in the specified languages. For
@@ -366,14 +381,16 @@
 
         References
         ----------
         https://developer.twitter.com/en/docs/twitter-api/v1/tweets/sample-realtime/api-reference/get-statuses-sample
 
         .. _BCP 47: https://tools.ietf.org/html/bcp47
         .. _advanced search: https://twitter.com/search-advanced
+        .. _The Twitter API v1.1 endpoint this method uses is now deprecated
+            and will be retired on October 29, 2022.: https://twittercommunity.com/t/deprecation-announcement-removing-compliance-messages-from-statuses-filter-and-retiring-statuses-sample-from-the-twitter-api-v1-1/170500
         """
         if self.running:
             raise TweepyException("Stream is already connected")
 
         method = "GET"
         endpoint = "statuses/sample"
```

### Comparing `tweepy-4.8.0/tweepy/tweet.py` & `tweepy-4.9.0/tweepy/tweet.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy/user.py` & `tweepy-4.9.0/tweepy/user.py`

 * *Files identical despite different names*

### Comparing `tweepy-4.8.0/tweepy.egg-info/PKG-INFO` & `tweepy-4.9.0/tweepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweepy
-Version: 4.8.0
+Version: 4.9.0
 Summary: Twitter library for Python
 Home-page: https://www.tweepy.org/
 Author: Joshua Roesslein
 Author-email: tweepy@googlegroups.com
 License: MIT
 Download-URL: https://pypi.org/project/tweepy/
 Project-URL: Documentation, https://tweepy.readthedocs.io
```

### Comparing `tweepy-4.8.0/tweepy.egg-info/SOURCES.txt` & `tweepy-4.9.0/tweepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

